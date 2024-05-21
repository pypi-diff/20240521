# Comparing `tmp/ellis_django_views-0.1.tar.gz` & `tmp/ellis_django_views-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellis_django_views-0.1.tar", last modified: Tue May 21 07:06:49 2024, max compression
+gzip compressed data, was "ellis_django_views-0.15.tar", last modified: Tue May 21 10:58:10 2024, max compression
```

## Comparing `ellis_django_views-0.1.tar` & `ellis_django_views-0.15.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 07:06:49.585613 ellis_django_views-0.1/
--rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.1/LICENSE
--rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 06:59:28.000000 ellis_django_views-0.1/MANIFEST.in
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1074 2024-05-21 07:06:49.585246 ellis_django_views-0.1/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)      610 2024-05-21 06:55:57.000000 ellis_django_views-0.1/README.md
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 07:06:49.581331 ellis_django_views-0.1/ellis_django_views/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 06:48:41.000000 ellis_django_views-0.1/ellis_django_views/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)       63 2024-05-21 06:48:41.000000 ellis_django_views-0.1/ellis_django_views/admin.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 06:48:41.000000 ellis_django_views-0.1/ellis_django_views/apps.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 07:06:49.584842 ellis_django_views-0.1/ellis_django_views/migrations/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 06:48:41.000000 ellis_django_views-0.1/ellis_django_views/migrations/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      663 2024-05-21 06:55:01.000000 ellis_django_views-0.1/ellis_django_views/models.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      239 2024-05-21 06:55:02.000000 ellis_django_views-0.1/ellis_django_views/serializers.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)    17427 2024-05-21 06:55:05.000000 ellis_django_views-0.1/ellis_django_views/test_views.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      540 2024-05-21 06:55:06.000000 ellis_django_views-0.1/ellis_django_views/urls.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      980 2024-05-21 06:54:37.000000 ellis_django_views-0.1/ellis_django_views/views.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 06:55:07.000000 ellis_django_views-0.1/ellis_django_views/views_abstract.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 06:55:08.000000 ellis_django_views-0.1/ellis_django_views/views_implementation.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 07:06:49.584319 ellis_django_views-0.1/ellis_django_views.egg-info/
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1074 2024-05-21 07:06:49.000000 ellis_django_views-0.1/ellis_django_views.egg-info/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)      606 2024-05-21 07:06:49.000000 ellis_django_views-0.1/ellis_django_views.egg-info/SOURCES.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 07:06:49.000000 ellis_django_views-0.1/ellis_django_views.egg-info/dependency_links.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 07:06:49.000000 ellis_django_views-0.1/ellis_django_views.egg-info/requires.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 07:06:49.000000 ellis_django_views-0.1/ellis_django_views.egg-info/top_level.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 07:06:49.585726 ellis_django_views-0.1/setup.cfg
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1397 2024-05-21 07:06:42.000000 ellis_django_views-0.1/setup.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.643673 ellis_django_views-0.15/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.15/LICENSE
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 06:59:28.000000 ellis_django_views-0.15/MANIFEST.in
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1075 2024-05-21 10:58:10.643351 ellis_django_views-0.15/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      610 2024-05-21 06:55:57.000000 ellis_django_views-0.15/README.md
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.574254 ellis_django_views-0.15/ellis_django_views/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.15/ellis_django_views/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.15/ellis_django_views/apps.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.593935 ellis_django_views-0.15/ellis_django_views/migrations/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.15/ellis_django_views/migrations/0001_initial.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.15/ellis_django_views/migrations/__init__.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.625062 ellis_django_views-0.15/ellis_django_views/tests/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.15/ellis_django_views/tests/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.15/ellis_django_views/tests/models.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.15/ellis_django_views/tests/serializers.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.15/ellis_django_views/tests/test_views.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.15/ellis_django_views/tests/urls.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.15/ellis_django_views/tests/views.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.642796 ellis_django_views-0.15/ellis_django_views/utils/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.15/ellis_django_views/utils/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.15/ellis_django_views/utils/error_messages.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.15/ellis_django_views/utils/request_params.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.15/ellis_django_views/utils/url_names.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.15/ellis_django_views/utils/url_paths.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.15/ellis_django_views/views_abstract.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.15/ellis_django_views/views_implementation.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.588642 ellis_django_views-0.15/ellis_django_views.egg-info/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1075 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/SOURCES.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/dependency_links.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/requires.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/top_level.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 10:58:10.643771 ellis_django_views-0.15/setup.cfg
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1521 2024-05-21 10:57:51.000000 ellis_django_views-0.15/setup.py
```

### Comparing `ellis_django_views-0.1/LICENSE` & `ellis_django_views-0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1/PKG-INFO` & `ellis_django_views-0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis_django_views
-Version: 0.1
+Version: 0.15
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `ellis_django_views-0.1/README.md` & `ellis_django_views-0.15/README.md`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1/ellis_django_views/test_views.py` & `ellis_django_views-0.15/ellis_django_views/tests/test_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from rest_framework import status
 from django.test import TestCase, Client
 from django.core.files.uploadedfile import SimpleUploadedFile
 from ellis_django_views.utils import url_paths, request_params, error_messages
-from ellis_django_views.models import TestImageModel
+from ellis_django_views.tests.models import TestImageModel
 from PIL import Image as PilImage
 import tempfile
 import os, shutil
 
 class ViewsImplTests(TestCase):
     def setUp(self):
         self.client = Client()
@@ -35,15 +35,15 @@
     def test_image_POST_missing_auth_token(self):
         # Test case to check handling of missing authorization token in POST request
         # Simulates sending a POST request without an authorization token
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing auth token
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
-        response = self.client.post(path=f'/{self.urls.IMAGE_POST}',
+        response = self.client.post(path=f'/{self.urls.TEST_POST}',
                                     data=request)
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
         self.assertEqual(
             response.json()[error_messages.ERROR],
             f'{error_messages.MISSING_HEADER_PARAMETER}{request_params.AUTH_TOKEN}')
 
 
@@ -53,22 +53,22 @@
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing auth token
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         image = TestImageModel.objects.get(pk=pk)
         request = {request_params.PK : pk}
         headers = {}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_GET}', data=request, **headers)
+            path=f'/{self.urls.TEST_GET}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_400_BAD_REQUEST)
         self.assertEqual(
             response.json()[error_messages.ERROR],
             f'{error_messages.MISSING_HEADER_PARAMETER}{request_params.AUTH_TOKEN}')
         image.delete()
         shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
@@ -79,25 +79,25 @@
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing auth token
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         uploaded_file =  self.upload_image(self.test_image)
         request = {request_params.PK : pk,
                    request_params.IMAGE : uploaded_file}
         image = TestImageModel.objects.get(pk=pk)
         headers = {}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_PUT}', data=request, **headers)
+            path=f'/{self.urls.TEST_PUT}', data=request, **headers)
         self.assertEqual(response.status_code,status.HTTP_400_BAD_REQUEST)
         self.assertEqual(
             response.json()[error_messages.ERROR],
             f'{error_messages.MISSING_HEADER_PARAMETER}{request_params.AUTH_TOKEN}')
         image.delete()
         shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
 
@@ -107,22 +107,22 @@
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing auth token
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         request = {request_params.PK : pk}
         headers = {}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_DELETE}', data=request, **headers)
+            path=f'/{self.urls.TEST_DELETE}', data=request, **headers)
         self.assertEqual(response.status_code,status.HTTP_400_BAD_REQUEST)
         self.assertEqual(
             response.json()[error_messages.ERROR],
             f'{error_messages.MISSING_HEADER_PARAMETER}{request_params.AUTH_TOKEN}')
         images = TestImageModel.objects.all()
         self.assertEqual(len(images), 1)
         image = TestImageModel.objects.get(pk=pk)
@@ -133,15 +133,15 @@
         # Test case to check handling of missing image file in POST request
         # Simulates sending a POST request without an image file
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing image file
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}',
+            path=f'/{self.urls.TEST_POST}',
             content_type=request_params.CONTENT_TYPE, data={}, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_400_BAD_REQUEST)
         self.assertEqual(response.json()[error_messages.ERROR],
                          {request_params.IMAGE:
                           [error_messages.FILE_NOT_SUBMITTED]})
         images = TestImageModel.objects.all()
@@ -153,21 +153,21 @@
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing image file
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         request = {request_params.PK : pk}
         image = TestImageModel.objects.get(pk=pk)
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_PUT}', data=request, **headers)
+            path=f'/{self.urls.TEST_PUT}', data=request, **headers)
         self.assertEqual(
             response.status_code, status.HTTP_400_BAD_REQUEST)
         self.assertEqual(
             response.json()[error_messages.ERROR],
             {request_params.IMAGE:[error_messages.FILE_NOT_SUBMITTED]})
         image = TestImageModel.objects.get(pk=pk)
         image.delete()
@@ -179,21 +179,21 @@
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing primary key
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         image = TestImageModel.objects.get(pk=pk)
         request = {}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_GET}', data=request, **headers)
+            path=f'/{self.urls.TEST_GET}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_400_BAD_REQUEST)
         self.assertEqual(response.json()[error_messages.ERROR],
                          f'{error_messages.MISSING_PARAMETER}pk')
         image.delete()
         shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
 
@@ -203,23 +203,23 @@
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing primary key
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         image = TestImageModel.objects.get(pk=pk)
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_PUT}', data=request, **headers)
+            path=f'/{self.urls.TEST_PUT}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_400_BAD_REQUEST)
         self.assertEqual(response.json()[error_messages.ERROR],
                          f'{error_messages.MISSING_PARAMETER}pk')
         image = TestImageModel.objects.get(pk=pk)
         image.delete()
         shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
@@ -230,20 +230,20 @@
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing primary key
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         request = {}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_DELETE}', data=request, **headers)
+            path=f'/{self.urls.TEST_DELETE}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_400_BAD_REQUEST)
         self.assertEqual(response.json()[error_messages.ERROR],
                          f'{error_messages.MISSING_PARAMETER}pk')
         images = TestImageModel.objects.all()
         self.assertEqual(len(images), 1)
         shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
@@ -254,15 +254,15 @@
         # Asserts that the response returns a 200 OK status
         # and the image is created successfully in the database
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request,**headers)
+            path=f'/{self.urls.TEST_POST}', data=request,**headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         image = TestImageModel.objects.get(pk=pk)
         self.assertEqual(image.image.url,
                          response.json()[request_params.IMAGE])
         image.delete()
@@ -274,21 +274,21 @@
         # Asserts that the response returns a 200 OK status
         # and the requested image is returned successfully
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         image = TestImageModel.objects.get(pk=pk)
         request = {request_params.PK : pk}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_GET}', data=request, **headers)
+            path=f'/{self.urls.TEST_GET}', data=request, **headers)
         self.assertEqual(image.image.url,
                          response.json()[request_params.IMAGE])
         image.delete()
         shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
 
     def test_image_UPDATE_correct(self):
         # Test case to check correct updating of an image
@@ -296,24 +296,24 @@
         # Asserts that the response returns a 200 OK status
         # and the image is updated successfully in the database
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         uploaded_file = self.upload_image(self.test_updated_image)
         request = {request_params.PK : pk,
                    request_params.IMAGE : uploaded_file}
         image = TestImageModel.objects.get(pk=pk)
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_PUT}', data=request, **headers)
+            path=f'/{self.urls.TEST_PUT}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         image = TestImageModel.objects.get(pk=pk)
         self.assertEqual(image.image.name,
                          f'{url_paths.IMAGES}{pk}/{self.test_updated_image}')
         image.delete()
         shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
@@ -324,19 +324,19 @@
         # Asserts that the response returns a 200 OK status
         # and the image is deleted successfully from the database
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_POST}', data=request, **headers)
+            path=f'/{self.urls.TEST_POST}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         request = {request_params.PK : pk}
         response = self.client.post(
-            path=f'/{self.urls.IMAGE_DELETE}', data=request, **headers)
+            path=f'/{self.urls.TEST_DELETE}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         images = TestImageModel.objects.all()
         self.assertEqual(len(images), 0)
         shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
```

### Comparing `ellis_django_views-0.1/ellis_django_views/views_abstract.py` & `ellis_django_views-0.15/ellis_django_views/views_abstract.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1/ellis_django_views/views_implementation.py` & `ellis_django_views-0.15/ellis_django_views/views_implementation.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1/ellis_django_views.egg-info/PKG-INFO` & `ellis_django_views-0.15/ellis_django_views.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis-django-views
-Version: 0.1
+Version: 0.15
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `ellis_django_views-0.1/ellis_django_views.egg-info/SOURCES.txt` & `ellis_django_views-0.15/ellis_django_views.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 ellis_django_views/__init__.py
-ellis_django_views/admin.py
 ellis_django_views/apps.py
-ellis_django_views/models.py
-ellis_django_views/serializers.py
-ellis_django_views/test_views.py
-ellis_django_views/urls.py
-ellis_django_views/views.py
 ellis_django_views/views_abstract.py
 ellis_django_views/views_implementation.py
 ellis_django_views.egg-info/PKG-INFO
 ellis_django_views.egg-info/SOURCES.txt
 ellis_django_views.egg-info/dependency_links.txt
 ellis_django_views.egg-info/requires.txt
 ellis_django_views.egg-info/top_level.txt
-ellis_django_views/migrations/__init__.py
+ellis_django_views/migrations/0001_initial.py
+ellis_django_views/migrations/__init__.py
+ellis_django_views/tests/__init__.py
+ellis_django_views/tests/models.py
+ellis_django_views/tests/serializers.py
+ellis_django_views/tests/test_views.py
+ellis_django_views/tests/urls.py
+ellis_django_views/tests/views.py
+ellis_django_views/utils/__init__.py
+ellis_django_views/utils/error_messages.py
+ellis_django_views/utils/request_params.py
+ellis_django_views/utils/url_names.py
+ellis_django_views/utils/url_paths.py
```

### Comparing `ellis_django_views-0.1/setup.py` & `ellis_django_views-0.15/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     include_package_data=True,
     name='ellis_django_views',
-    version='0.1',
+    version='0.15',
     packages=find_packages(),
     description='Generic views for Model View Serializer (MVS) pattern',
     author='Carl Victor Ellis',
     author_email='carl.ellis@hotmail.com.au',
     license='GNU',
     url='https://carlellis.io',
     long_description='Ellis views are generic views for Create, Request, Update and Delete views, simply define serializer_model, model and is_authorised methods.',
@@ -30,8 +30,15 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
+    tests_require=[
+        'pytest',
+        'pytest-django',
+    ],
+    setup_requires=[
+        'pytest-runner',
+    ],
 )
```

