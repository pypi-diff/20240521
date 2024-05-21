# Comparing `tmp/sentrifyai-0.1.5.tar.gz` & `tmp/sentrifyai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentrifyai-0.1.5.tar", last modified: Mon May 20 20:40:07 2024, max compression
+gzip compressed data, was "sentrifyai-0.1.6.tar", last modified: Tue May 21 20:47:50 2024, max compression
```

## Comparing `sentrifyai-0.1.5.tar` & `sentrifyai-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/
--rw-r--r--   0 runner    (1000) runner    (1000)     1056 2024-05-20 20:23:25.000000 sentrifyai-0.1.5/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      811 2024-05-20 20:39:14.000000 sentrifyai-0.1.5/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/sentrifyai/
--rw-r--r--   0 runner    (1000) runner    (1000)      169 2024-05-20 20:30:02.000000 sentrifyai-0.1.5/sentrifyai/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1691 2024-05-20 20:23:52.000000 sentrifyai-0.1.5/sentrifyai/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-05-20 20:23:52.000000 sentrifyai-0.1.5/sentrifyai/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)      322 2024-05-20 20:23:52.000000 sentrifyai-0.1.5/sentrifyai/exceptions.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/sentrifyai.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      325 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      676 2024-05-20 20:39:54.000000 sentrifyai-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 20:47:50.653164 sentrifyai-0.1.6/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1056 2024-05-21 20:43:58.000000 sentrifyai-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1265 2024-05-21 20:47:50.653164 sentrifyai-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      811 2024-05-21 20:43:58.000000 sentrifyai-0.1.6/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      360 2024-05-21 20:45:04.000000 sentrifyai-0.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 20:47:50.653164 sentrifyai-0.1.6/sentrifyai/
+-rw-r--r--   0 runner    (1000) runner    (1000)      207 2024-05-21 20:46:45.000000 sentrifyai-0.1.6/sentrifyai/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2650 2024-05-21 20:44:37.000000 sentrifyai-0.1.6/sentrifyai/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-05-21 20:43:58.000000 sentrifyai-0.1.6/sentrifyai/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      322 2024-05-21 20:43:58.000000 sentrifyai-0.1.6/sentrifyai/exceptions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 20:47:50.653164 sentrifyai-0.1.6/sentrifyai.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1265 2024-05-21 20:47:50.000000 sentrifyai-0.1.6/sentrifyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-05-21 20:47:50.000000 sentrifyai-0.1.6/sentrifyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-21 20:47:50.000000 sentrifyai-0.1.6/sentrifyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-21 20:47:50.000000 sentrifyai-0.1.6/sentrifyai.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-05-21 20:47:50.000000 sentrifyai-0.1.6/sentrifyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-21 20:47:50.000000 sentrifyai-0.1.6/sentrifyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-21 20:47:50.653164 sentrifyai-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      676 2024-05-21 20:45:17.000000 sentrifyai-0.1.6/setup.py
```

### Comparing `sentrifyai-0.1.5/LICENSE` & `sentrifyai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sentrifyai-0.1.5/PKG-INFO` & `sentrifyai-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: sentrifyai
-Version: 0.1.5
+Version: 0.1.6
 Summary: SentrifyAI API client
 Home-page: https://github.com/sentrifybot/sentrifyai-python
 Author: SentrifyAI
 Author-email: admin@sentrify.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # SentrifyAI Python Package
 
 SentrifyAI is a Python package that provides a client for interacting with the SentrifyAI API.
 
 ## Installation
 
@@ -46,8 +45,7 @@
 ## Documentation
 
 For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/sentrifybot/sentrifyai-python).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
```

### Comparing `sentrifyai-0.1.5/README.md` & `sentrifyai-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sentrifyai-0.1.5/sentrifyai/api.py` & `sentrifyai-0.1.6/sentrifyai/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import requests
 from .config import BASE_URL
 from .exceptions import ModelNotFoundError, APIRequestError
 
-class SentrifyAI:
+def list_models(self):
+  try:
+      # Send a GET request to retrieve the list of models
+      response = requests.get(f'{BASE_URL}models')
+      response.raise_for_status()  # Raise an error for non-200 status codes
+      return response.json()['models']  # Extract and return the list of models
+  except requests.exceptions.RequestException as e:
+      # Handle any request-related exceptions
+      raise APIRequestError(f'Request exception occurred: {e}')
+
+class Moderation:
     def __init__(self):
         pass
 
-    def list_models(self):
-        try:
-            # Send a GET request to retrieve the list of models
-            response = requests.get(f'{BASE_URL}models')
-            response.raise_for_status()  # Raise an error for non-200 status codes
-            return response.json()['models']  # Extract and return the list of models
-        except requests.exceptions.RequestException as e:
-            # Handle any request-related exceptions
-            raise APIRequestError(f'Request exception occurred: {e}')
-
-    def classify_message(self, model_slug, message):
+    def classify(self, model_slug, message):
         try:
             # Prepare parameters for the request
             params = {
                 'model': model_slug,
                 'message': message
             }
             # Send a GET request to classify the message
@@ -32,7 +32,33 @@
             if response.status_code == 404:
                 raise ModelNotFoundError(f'Model {model_slug} not found.')
             else:
                 raise APIRequestError(f'HTTP error occurred: {e}')
         except requests.exceptions.RequestException as e:
             # Handle any other request-related exceptions
             raise APIRequestError(f'Request exception occurred: {e}')
+
+
+class Emotions:
+  def __init__(self):
+      pass
+
+  def emotion(self, model_slug, message):
+      try:
+          # Prepare parameters for the request
+          params = {
+              'model': model_slug,
+              'message': message
+          }
+          # Send a GET request to classify the message
+          response = requests.get(f'{BASE_URL}emotions', params=params)
+          response.raise_for_status()  # Raise an error for non-200 status codes
+          return response.json()  # Return the classification result
+      except requests.exceptions.HTTPError as e:
+          # Handle HTTP errors, including 404 (Model not found)
+          if response.status_code == 404:
+              raise ModelNotFoundError(f'Model {model_slug} not found.')
+          else:
+              raise APIRequestError(f'HTTP error occurred: {e}')
+      except requests.exceptions.RequestException as e:
+          # Handle any other request-related exceptions
+          raise APIRequestError(f'Request exception occurred: {e}')
```

### Comparing `sentrifyai-0.1.5/sentrifyai.egg-info/PKG-INFO` & `sentrifyai-0.1.6/sentrifyai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: sentrifyai
-Version: 0.1.5
+Version: 0.1.6
 Summary: SentrifyAI API client
 Home-page: https://github.com/sentrifybot/sentrifyai-python
 Author: SentrifyAI
 Author-email: admin@sentrify.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # SentrifyAI Python Package
 
 SentrifyAI is a Python package that provides a client for interacting with the SentrifyAI API.
 
 ## Installation
 
@@ -46,8 +45,7 @@
 ## Documentation
 
 For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/sentrifybot/sentrifyai-python).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
```

### Comparing `sentrifyai-0.1.5/setup.py` & `sentrifyai-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sentrifyai',
-    version='0.1.5',
+    version='0.1.6',
     description='SentrifyAI API client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SentrifyAI',
     author_email='admin@sentrify.org',
     url='https://github.com/sentrifybot/sentrifyai-python',
     packages=find_packages(),
```

