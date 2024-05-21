# Comparing `tmp/paynow-1.0.6.tar.gz` & `tmp/paynow-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paynow-1.0.6.tar", last modified: Wed Jan 17 13:20:07 2024, max compression
+gzip compressed data, was "paynow-1.0.7.tar", last modified: Tue May 21 10:16:48 2024, max compression
```

## Comparing `paynow-1.0.6.tar` & `paynow-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:20:07.408964 paynow-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-17 13:20:04.000000 paynow-1.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-17 13:20:04.000000 paynow-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-01-17 13:20:07.408964 paynow-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-01-17 13:20:04.000000 paynow-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:20:07.408964 paynow-1.0.6/paynow/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-17 13:20:04.000000 paynow-1.0.6/paynow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-17 13:20:04.000000 paynow-1.0.6/paynow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-01-17 13:20:04.000000 paynow-1.0.6/paynow/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:20:07.408964 paynow-1.0.6/paynow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-01-17 13:20:07.000000 paynow-1.0.6/paynow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-17 13:20:07.000000 paynow-1.0.6/paynow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 13:20:07.000000 paynow-1.0.6/paynow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-17 13:20:07.000000 paynow-1.0.6/paynow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-17 13:20:07.000000 paynow-1.0.6/paynow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-17 13:20:07.408964 paynow-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-17 13:20:04.000000 paynow-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:16:48.900984 paynow-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-21 10:16:45.000000 paynow-1.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 10:16:45.000000 paynow-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-21 10:16:48.900984 paynow-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-21 10:16:45.000000 paynow-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:16:48.896984 paynow-1.0.7/paynow/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 10:16:45.000000 paynow-1.0.7/paynow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-21 10:16:45.000000 paynow-1.0.7/paynow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15950 2024-05-21 10:16:45.000000 paynow-1.0.7/paynow/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:16:48.900984 paynow-1.0.7/paynow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-21 10:16:48.000000 paynow-1.0.7/paynow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-21 10:16:48.000000 paynow-1.0.7/paynow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:16:48.000000 paynow-1.0.7/paynow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:16:48.000000 paynow-1.0.7/paynow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 10:16:48.000000 paynow-1.0.7/paynow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 10:16:48.900984 paynow-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-21 10:16:45.000000 paynow-1.0.7/setup.py
```

### Comparing `paynow-1.0.6/LICENSE.txt` & `paynow-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paynow-1.0.6/PKG-INFO` & `paynow-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paynow
-Version: 1.0.6
+Version: 1.0.7
 Summary: Paynow Python SDK
 Home-page: https://gitlab.com/paynow-developer-hub/Paynow-Python-SDK
 Author: WebDev Projects
 Author-email: pkg-dev@webdevworld.com
 Project-URL: Bug Reports, https://gitlab.com/paynow-developer-hub/Paynow-Python-SDK/issues
 Project-URL: Source, https://gitlab.com/paynow-developer-hub/Paynow-Python-SDK
 Keywords: paynow-api paynow-zimbabwe paynow-zimbabwe-api paynow-zimbabwe-sdk
```

### Comparing `paynow-1.0.6/README.md` & `paynow-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `paynow-1.0.6/paynow/model.py` & `paynow-1.0.7/paynow/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         if str(response_object['status']).lower() == 'error':
             return InitResponse(response_object)
 
         # Verify the hash from Paynow with the locally generated one
         if not self.__verify_hash(response_object, self.integration_key):
             raise HashMismatchException("Hashes do not match")
 
-        # Create a new InitResponse object object passing in the data from Paynow
+        # Create a new InitResponse object  passing in the data from Paynow
         return InitResponse(response_object)
 
     def __init_mobile(self, payment, phone, method):
         """Initiate a mobile transaction
 
         Args:
             payment (Payment): The payment object with details about transaction
@@ -464,15 +464,15 @@
             "authemail":  payment.auth_email,
             "phone": phone,
             "method": method,
             "status": "Message"
         }
 
         for key, value in body.items():
-            if(key == 'authemail'):
+            if key == 'authemail' or key == 'returnurl' or key == 'resulturl':
                 continue
 
             body[key] = quote_plus(str(value))  # Url encode the
 
         body['hash'] = self.__hash(body, self.integration_key)
 
         return body
```

### Comparing `paynow-1.0.6/paynow.egg-info/PKG-INFO` & `paynow-1.0.7/paynow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paynow
-Version: 1.0.6
+Version: 1.0.7
 Summary: Paynow Python SDK
 Home-page: https://gitlab.com/paynow-developer-hub/Paynow-Python-SDK
 Author: WebDev Projects
 Author-email: pkg-dev@webdevworld.com
 Project-URL: Bug Reports, https://gitlab.com/paynow-developer-hub/Paynow-Python-SDK/issues
 Project-URL: Source, https://gitlab.com/paynow-developer-hub/Paynow-Python-SDK
 Keywords: paynow-api paynow-zimbabwe paynow-zimbabwe-api paynow-zimbabwe-sdk
```

### Comparing `paynow-1.0.6/setup.py` & `paynow-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='paynow',  # Required
-    version='1.0.6',  # Required
+    version='1.0.7',  # Required
     description='Paynow Python SDK',  # Required
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://gitlab.com/paynow-developer-hub/Paynow-Python-SDK',  # Optional
     author='WebDev Projects',  # Optional
     author_email='pkg-dev@webdevworld.com',  # Optional
     classifiers=[  # Optional
```

