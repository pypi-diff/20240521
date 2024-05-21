# Comparing `tmp/flickr_photos_api-2.3.0.tar.gz` & `tmp/flickr_photos_api-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr_photos_api-2.3.0.tar", last modified: Wed May  1 13:51:50 2024, max compression
+gzip compressed data, was "flickr_photos_api-2.3.1.tar", last modified: Tue May 21 08:21:04 2024, max compression
```

## Comparing `flickr_photos_api-2.3.0.tar` & `flickr_photos_api-2.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 13:51:50.304863 flickr_photos_api-2.3.0/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.3.0/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.3.0/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-01 13:51:50.304671 flickr_photos_api-2.3.0/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.3.0/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 14:50:54.000000 flickr_photos_api-2.3.0/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-05-01 13:51:50.304916 flickr_photos_api-2.3.0/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 13:51:50.298910 flickr_photos_api-2.3.0/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 13:51:50.300730 flickr_photos_api-2.3.0/src/flickr_photos_api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1378 2024-05-01 13:51:35.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/__init__.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 13:51:50.303039 flickr_photos_api-2.3.0/src/flickr_photos_api/api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)      640 2024-05-01 09:51:49.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/api/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5601 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/api/base.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    13443 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/api/collection_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2174 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/api/comment_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1862 2024-05-01 09:51:49.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/api/commons_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2234 2024-04-30 14:50:54.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/api/from_url_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/api/license_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    14939 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/api/single_photo_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     8514 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/api/user_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-05-01 12:03:23.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/py.typed
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 13:51:50.303554 flickr_photos_api-2.3.0/src/flickr_photos_api/types/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3016 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/types/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      767 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/types/contexts.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1063 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/types/users.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.3.0/src/flickr_photos_api/utils.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 13:51:50.304484 flickr_photos_api-2.3.0/src/flickr_photos_api.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-01 13:51:50.000000 flickr_photos_api-2.3.0/src/flickr_photos_api.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      958 2024-05-01 13:51:50.000000 flickr_photos_api-2.3.0/src/flickr_photos_api.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-05-01 13:51:50.000000 flickr_photos_api-2.3.0/src/flickr_photos_api.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-05-01 13:51:50.000000 flickr_photos_api-2.3.0/src/flickr_photos_api.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-05-01 13:51:50.000000 flickr_photos_api-2.3.0/src/flickr_photos_api.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 13:51:50.304203 flickr_photos_api-2.3.0/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     7788 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.0/tests/test_errors.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.3.0/tests/test_utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.899435 flickr_photos_api-2.3.1/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.3.1/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.3.1/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-21 08:21:04.899246 flickr_photos_api-2.3.1/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.3.1/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 14:50:54.000000 flickr_photos_api-2.3.1/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-05-21 08:21:04.899476 flickr_photos_api-2.3.1/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.891410 flickr_photos_api-2.3.1/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.892957 flickr_photos_api-2.3.1/src/flickr_photos_api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1378 2024-05-21 08:20:14.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/__init__.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.898109 flickr_photos_api-2.3.1/src/flickr_photos_api/api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      640 2024-05-01 09:51:49.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5822 2024-05-21 08:19:52.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/base.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    13443 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/collection_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2174 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/comment_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1862 2024-05-01 09:51:49.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/commons_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2234 2024-04-30 14:50:54.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/from_url_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/license_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    14939 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/single_photo_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     8514 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/user_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-05-01 12:03:23.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/py.typed
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.898514 flickr_photos_api-2.3.1/src/flickr_photos_api/types/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3016 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/types/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      767 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/types/contexts.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1063 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/types/users.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.899039 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      958 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.898757 flickr_photos_api-2.3.1/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     7788 2024-05-21 08:17:56.000000 flickr_photos_api-2.3.1/tests/test_errors.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.3.1/tests/test_utils.py
```

### Comparing `flickr_photos_api-2.3.0/LICENSE-APACHE` & `flickr_photos_api-2.3.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/LICENSE-MIT` & `flickr_photos_api-2.3.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/PKG-INFO` & `flickr_photos_api-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.3.0
+Version: 2.3.1
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.3.0/README.md` & `flickr_photos_api-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/pyproject.toml` & `flickr_photos_api-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/__init__.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     GroupContext,
     GroupInfo,
     PhotoContext,
     SinglePhotoInfo,
 )
 
 
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 
 
 __all__ = [
     "FlickrApi",
     "FlickrApiException",
     "ResourceNotFound",
     "InvalidApiKey",
```

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/api/__init__.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/api/base.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/api/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,10 +171,13 @@
 
             if errors["code"] == "100":
                 raise InvalidApiKey(message=errors["msg"])
 
             try:
                 raise exceptions[errors["code"]]
             except KeyError:
-                raise UnrecognisedFlickrApiException(errors)
+                # Note: the `from None` means we don't include the KeyError in
+                # the traceback -- this is to avoid exposing internal details
+                # of the library to external callers.
+                raise UnrecognisedFlickrApiException(errors) from None
 
         return xml
```

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/api/collection_methods.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/api/collection_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/api/comment_methods.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/api/comment_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/api/commons_methods.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/api/commons_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/api/from_url_methods.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/api/from_url_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/api/license_methods.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/api/license_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/api/single_photo_methods.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/api/single_photo_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/api/user_methods.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/api/user_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/exceptions.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/types/__init__.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/types/contexts.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/types/contexts.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/types/users.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/types/users.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api/utils.py` & `flickr_photos_api-2.3.1/src/flickr_photos_api/utils.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api.egg-info/PKG-INFO` & `flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.3.0
+Version: 2.3.1
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.3.0/src/flickr_photos_api.egg-info/SOURCES.txt` & `flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.0/tests/test_errors.py` & `flickr_photos_api-2.3.1/tests/test_errors.py`

 * *Files identical despite different names*

