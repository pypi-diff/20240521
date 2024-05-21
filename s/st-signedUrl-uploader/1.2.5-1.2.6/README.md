# Comparing `tmp/st_signedurl_uploader-1.2.5.tar.gz` & `tmp/st_signedurl_uploader-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_signedurl_uploader-1.2.5.tar", last modified: Fri May 17 07:51:01 2024, max compression
+gzip compressed data, was "st_signedurl_uploader-1.2.6.tar", last modified: Tue May 21 07:37:40 2024, max compression
```

## Comparing `st_signedurl_uploader-1.2.5.tar` & `st_signedurl_uploader-1.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-17 07:51:01.565950 st_signedurl_uploader-1.2.5/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.2.5/LICENSE
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-13 09:49:00.000000 st_signedurl_uploader-1.2.5/MANIFEST.in
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5156 2024-05-17 07:51:01.565650 st_signedurl_uploader-1.2.5/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4486 2024-05-16 07:58:26.000000 st_signedurl_uploader-1.2.5/README.md
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-17 07:51:01.566019 st_signedurl_uploader-1.2.5/setup.cfg
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      927 2024-05-17 07:27:08.000000 st_signedurl_uploader-1.2.5/setup.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-17 07:51:01.560325 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2620 2024-05-17 07:50:18.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/__init__.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-17 07:51:01.558824 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-17 07:51:01.562228 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/asset-manifest.json
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-17 07:47:23.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/bootstrap.min.css
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/index.html
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-17 07:51:01.559048 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/static/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-17 07:51:01.563283 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/static/js/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   326712 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js.LICENSE.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1249789 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js.map
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-17 07:51:01.564916 st_signedurl_uploader-1.2.5/st_signedUrl_uploader.egg-info/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5156 2024-05-17 07:51:01.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader.egg-info/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-17 07:51:01.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-17 07:51:01.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-17 07:51:01.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader.egg-info/requires.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-17 07:51:01.000000 st_signedurl_uploader-1.2.5/st_signedUrl_uploader.egg-info/top_level.txt
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-21 07:37:40.785873 st_signedurl_uploader-1.2.6/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.2.6/LICENSE
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-13 09:49:00.000000 st_signedurl_uploader-1.2.6/MANIFEST.in
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5163 2024-05-21 07:37:40.785557 st_signedurl_uploader-1.2.6/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4493 2024-05-21 07:28:48.000000 st_signedurl_uploader-1.2.6/README.md
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-21 07:37:40.785946 st_signedurl_uploader-1.2.6/setup.cfg
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      927 2024-05-21 07:37:23.000000 st_signedurl_uploader-1.2.6/setup.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-21 07:37:40.776997 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2620 2024-05-17 07:50:18.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/__init__.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-21 07:37:40.775286 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-21 07:37:40.779556 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/asset-manifest.json
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-17 07:47:23.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/bootstrap.min.css
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/index.html
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-21 07:37:40.775488 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/static/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-21 07:37:40.781787 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/static/js/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   326712 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js.LICENSE.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1249789 2024-05-17 07:47:26.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js.map
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-21 07:37:40.784730 st_signedurl_uploader-1.2.6/st_signedUrl_uploader.egg-info/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5163 2024-05-21 07:37:40.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-21 07:37:40.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-21 07:37:40.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-21 07:37:40.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader.egg-info/requires.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-21 07:37:40.000000 st_signedurl_uploader-1.2.6/st_signedUrl_uploader.egg-info/top_level.txt
```

### Comparing `st_signedurl_uploader-1.2.5/LICENSE` & `st_signedurl_uploader-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.5/PKG-INFO` & `st_signedurl_uploader-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-signedUrl-uploader
-Version: 1.2.5
+Version: 1.2.6
 Summary: Streamlit component that allows you to upload files to Google Cloud Storage via signed url
 Home-page: 
 Author: Meryam Assermouh
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -82,15 +82,15 @@
 #### Requirements :
   
 - **Google Cloud Storage Bucket:** Set up a bucket to store uploaded files.
 - **CORS Configuration:** Set your bucket's CORS settings using:
 ```
 gcloud storage buckets update gs://BUCKET_NAME --cors-file=CORS_CONFIG_FILE
 ```
-Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
+Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/assets/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
 
 ### Implementation : 
 - Create a service account and give it the role `roles/iam.serviceAccountTokenCreator`
 - **Install Cloud Storage library:** 
 ```
 pip install google-cloud-storage
 ```
```

### Comparing `st_signedurl_uploader-1.2.5/README.md` & `st_signedurl_uploader-1.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 #### Requirements :
   
 - **Google Cloud Storage Bucket:** Set up a bucket to store uploaded files.
 - **CORS Configuration:** Set your bucket's CORS settings using:
 ```
 gcloud storage buckets update gs://BUCKET_NAME --cors-file=CORS_CONFIG_FILE
 ```
-Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
+Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/assets/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
 
 ### Implementation : 
 - Create a service account and give it the role `roles/iam.serviceAccountTokenCreator`
 - **Install Cloud Storage library:** 
 ```
 pip install google-cloud-storage
 ```
```

### Comparing `st_signedurl_uploader-1.2.5/setup.py` & `st_signedurl_uploader-1.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-signedUrl-uploader",
-    version="1.2.5",
+    version="1.2.6",
     author="Meryam Assermouh",
     author_email="",
     description="Streamlit component that allows you to upload files to Google Cloud Storage via signed url",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_signedurl_uploader-1.2.5/st_signedUrl_uploader/__init__.py` & `st_signedurl_uploader-1.2.6/st_signedUrl_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/bootstrap.min.css` & `st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js` & `st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js.LICENSE.txt` & `st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.5/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js.map` & `st_signedurl_uploader-1.2.6/st_signedUrl_uploader/frontend/build/static/js/main.88223560.js.map`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.5/st_signedUrl_uploader.egg-info/PKG-INFO` & `st_signedurl_uploader-1.2.6/st_signedUrl_uploader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-signedUrl-uploader
-Version: 1.2.5
+Version: 1.2.6
 Summary: Streamlit component that allows you to upload files to Google Cloud Storage via signed url
 Home-page: 
 Author: Meryam Assermouh
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -82,15 +82,15 @@
 #### Requirements :
   
 - **Google Cloud Storage Bucket:** Set up a bucket to store uploaded files.
 - **CORS Configuration:** Set your bucket's CORS settings using:
 ```
 gcloud storage buckets update gs://BUCKET_NAME --cors-file=CORS_CONFIG_FILE
 ```
-Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
+Example CORS configuration file can be found in [CORS.json](https://github.com/Meryam-A/signed-url-uploader/blob/main/assets/CORS.json) or create your own based on [Google Cloud Documentation](https://cloud.google.com/storage/docs/cross-origin)
 
 ### Implementation : 
 - Create a service account and give it the role `roles/iam.serviceAccountTokenCreator`
 - **Install Cloud Storage library:** 
 ```
 pip install google-cloud-storage
 ```
```

### Comparing `st_signedurl_uploader-1.2.5/st_signedUrl_uploader.egg-info/SOURCES.txt` & `st_signedurl_uploader-1.2.6/st_signedUrl_uploader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

