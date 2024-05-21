# Comparing `tmp/dinamis-sdk-0.1.7.tar.gz` & `tmp/dinamis_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinamis-sdk-0.1.7.tar", last modified: Fri Apr 12 09:11:51 2024, max compression
+gzip compressed data, was "dinamis_sdk-0.1.8.tar", last modified: Tue May 21 18:17:20 2024, max compression
```

## Comparing `dinamis-sdk-0.1.7.tar` & `dinamis_sdk-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:11:51.870760 dinamis-sdk-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)    11340 2024-04-12 08:33:33.000000 dinamis-sdk-0.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      391 2024-04-12 09:11:51.870760 dinamis-sdk-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-04-12 08:36:51.000000 dinamis-sdk-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:11:51.862760 dinamis-sdk-0.1.7/dinamis_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-12 08:33:33.000000 dinamis-sdk-0.1.7/dinamis_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8848 2024-04-12 09:11:36.000000 dinamis-sdk-0.1.7/dinamis_sdk/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:11:51.870760 dinamis-sdk-0.1.7/dinamis_sdk/examples/
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-12 08:33:33.000000 dinamis-sdk-0.1.7/dinamis_sdk/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2024-04-12 08:33:33.000000 dinamis-sdk-0.1.7/dinamis_sdk/examples/pyotb_ndvi_loss.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-12 08:33:33.000000 dinamis-sdk-0.1.7/dinamis_sdk/examples/pyotb_toa_mosaic.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2024-04-12 08:33:33.000000 dinamis-sdk-0.1.7/dinamis_sdk/examples/rio_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    17394 2024-04-12 08:33:33.000000 dinamis-sdk-0.1.7/dinamis_sdk/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-04-12 08:36:51.000000 dinamis-sdk-0.1.7/dinamis_sdk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:11:51.870760 dinamis-sdk-0.1.7/dinamis_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      391 2024-04-12 09:11:51.000000 dinamis-sdk-0.1.7/dinamis_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2024-04-12 09:11:51.000000 dinamis-sdk-0.1.7/dinamis_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 09:11:51.000000 dinamis-sdk-0.1.7/dinamis_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 09:11:51.000000 dinamis-sdk-0.1.7/dinamis_sdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       80 2024-04-12 09:11:51.000000 dinamis-sdk-0.1.7/dinamis_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-12 09:11:51.000000 dinamis-sdk-0.1.7/dinamis_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 09:11:51.870760 dinamis-sdk-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      496 2024-04-12 09:11:36.000000 dinamis-sdk-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:11:51.870760 dinamis-sdk-0.1.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)      408 2024-04-12 08:33:33.000000 dinamis-sdk-0.1.7/tests/test_spot-6-7-drs.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-12 08:33:33.000000 dinamis-sdk-0.1.7/tests/test_super-s2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.313818 dinamis_sdk-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-21 18:17:20.313818 dinamis_sdk-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.305818 dinamis_sdk-0.1.8/dinamis_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      284 2024-05-21 18:04:01.000000 dinamis_sdk-0.1.8/dinamis_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8903 2024-05-21 18:09:08.000000 dinamis_sdk-0.1.8/dinamis_sdk/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.309818 dinamis_sdk-0.1.8/dinamis_sdk/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/examples/pyotb_ndvi_loss.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/examples/pyotb_toa_mosaic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/examples/rio_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    17399 2024-05-21 18:04:02.000000 dinamis_sdk-0.1.8/dinamis_sdk/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.309818 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 18:17:20.313818 dinamis_sdk-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.309818 dinamis_sdk-0.1.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-21 18:09:08.000000 dinamis_sdk-0.1.8/tests/test_spot-6-7-drs.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-21 18:09:08.000000 dinamis_sdk-0.1.8/tests/test_super-s2.py
```

### Comparing `dinamis-sdk-0.1.7/LICENSE` & `dinamis_sdk-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.7/README.md` & `dinamis_sdk-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.7/dinamis_sdk/auth.py` & `dinamis_sdk-0.1.8/dinamis_sdk/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import os
 import time
 from abc import abstractmethod
 from typing import Dict
 import requests
 from pydantic import BaseModel, Field  # pylint: disable = no-name-in-module
 import qrcode
-from .utils import log, JWT_FILE, TOKEN_ENDPOINT, AUTH_BASE_URL, TOKEN_SERVER
 import urllib3
+from .utils import log, JWT_FILE, TOKEN_ENDPOINT, AUTH_BASE_URL, TOKEN_SERVER
 
 
 class JWT(BaseModel):  # pylint: disable = R0903
     """JWT model."""
 
     access_token: str = Field(alias="access_token")
     expires_in: int = Field(alias="expires_in")
@@ -246,14 +246,15 @@
 
         self.refresh_if_needed()
 
         return self.jwt.access_token
 
 
 class TokenServer:
+    """Token server."""
     def __init__(self, endpoint: str, total_retry=5, backoff_factor=0.8):
         self.endpoint = endpoint
         self.session = requests.Session()
         retry = urllib3.util.retry.Retry(
             total=total_retry,
             backoff_factor=backoff_factor,
             status_forcelist=[404, 429, 500, 502, 503, 504],
@@ -267,14 +268,15 @@
         return self.session.get(self.endpoint, timeout=10).json()
 
 
 session = TokenServer(TOKEN_SERVER) if TOKEN_SERVER else OAuth2Session()
 
 
 def _get_access_token():
+    """Get an access token."""
     return session.get_access_token()
 
 
 get_access_token = _get_access_token
 
 
 def set_access_token_fn(func):
```

### Comparing `dinamis-sdk-0.1.7/dinamis_sdk/examples/pyotb_ndvi_loss.py` & `dinamis_sdk-0.1.8/dinamis_sdk/examples/pyotb_ndvi_loss.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.7/dinamis_sdk/examples/pyotb_toa_mosaic.py` & `dinamis_sdk-0.1.8/dinamis_sdk/examples/pyotb_toa_mosaic.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.7/dinamis_sdk/examples/rio_metadata.py` & `dinamis_sdk-0.1.8/dinamis_sdk/examples/rio_metadata.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.7/dinamis_sdk/s3.py` & `dinamis_sdk-0.1.8/dinamis_sdk/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     """
     if is_vrt_string(url):
         return sign_vrt_string(url)
     return sign_urls(urls=[url])[url]
 
 
-def sign_urls(urls: List[str]) -> str:
+def sign_urls(urls: List[str]) -> Dict[str, str]:
     """Sign URLs with a S3 Token.
 
     Signing URL allows read access to files in storage.
 
     Args:
         urls: List of HREF to sign
 
@@ -483,17 +483,17 @@
         n_chunks = math.ceil(n_urls / MAX_URLS)
         log.debug("Number of chunks of URLs to sign: %s", n_chunks)
         for i_chunk in range(n_chunks):
             log.debug("Processing chunk %s/%s", i_chunk + 1, n_chunks)
             chunk_start = i_chunk * MAX_URLS
             chunk_end = min(chunk_start + MAX_URLS, n_urls)
             not_signed_urls_chunk = not_signed_urls[chunk_start:chunk_end]
-            params={"urls": not_signed_urls_chunk}
+            params = {"urls": not_signed_urls_chunk}
             if SIGNED_URL_DURATION_SECONDS:
-                params.update({"duration_seconds": SIGNED_URL_DURATION_SECONDS})
+                params["duration_seconds"] = SIGNED_URL_DURATION_SECONDS
             response = session.post(
                 f"{S3_SIGNING_ENDPOINT}sign_urls",
                 params=params,
                 headers=headers,
                 timeout=10
             )
             response.raise_for_status()
```

### Comparing `dinamis-sdk-0.1.7/dinamis_sdk/utils.py` & `dinamis_sdk-0.1.8/dinamis_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.7/dinamis_sdk.egg-info/SOURCES.txt` & `dinamis_sdk-0.1.8/dinamis_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

