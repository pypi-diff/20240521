# Comparing `tmp/s3func-0.1.5.tar.gz` & `tmp/s3func-0.2.0.tar.gz`

## Comparing `s3func-0.1.5.tar` & `s3func-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/__init__.py
--rw-r--r--   0        0        0    21923 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/main.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/tests/__init__.py
--rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/tests/stns_data.blt
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/tests/test_s3func.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.1.5/.gitignore
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.1.5/LICENSE
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.1.5/README.md
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 s3func-0.2.0/s3func/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 s3func-0.2.0/s3func/b2.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 s3func-0.2.0/s3func/http_url.py
+-rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 s3func-0.2.0/s3func/s3.py
+-rw-r--r--   0        0        0    12826 2020-02-02 00:00:00.000000 s3func-0.2.0/s3func/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.2.0/s3func/tests/__init__.py
+-rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.2.0/s3func/tests/stns_data.blt
+-rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 s3func-0.2.0/s3func/tests/test_s3func.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.2.0/.gitignore
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.2.0/README.md
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.2.0/PKG-INFO
```

### Comparing `s3func-0.1.5/s3func/main.py` & `s3func-0.2.0/s3func/s3.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,50 +3,52 @@
 """
 Created on May 13 08:04:38 2024
 
 @author: mike
 """
 import io
 # import os
-from pydantic import HttpUrl
+# from pydantic import HttpUrl
 from typing import List, Union
 import boto3
 import botocore
 import copy
 # import requests
-import urllib.parse
-from urllib3.util import Retry, Timeout
+# import urllib.parse
+# from urllib3.util import Retry, Timeout
 # import datetime
 import hashlib
 # from requests import Session
 # from requests.adapters import HTTPAdapter
 import urllib3
+# import uuid
+from time import sleep
+from timeit import default_timer
+
+# from . import http_url
+# import http_url
 
 from . import utils
 # import utils
 
 #######################################################
 ### Parameters
 
-# key_patterns = {
-#     'b2': '{base_url}/{bucket}/{obj_key}',
-#     'contabo': '{base_url}:{bucket}/{obj_key}',
-#     }
-
-# multipart_size = 2**28
 
-b2_auth_url = 'https://api.backblazeb2.com/b2api/v3/b2_authorize_account'
+md5_locks = {
+    'shared': 'cfcd208495d565ef66e7dff9f98764da',
+    'exclusive': 'c4ca4238a0b923820dcc509a6f75849b'
+    }
 
-available_capabilities = [ "listKeys", "writeKeys", "deleteKeys", "listAllBucketNames", "listBuckets", "readBuckets", "writeBuckets", "deleteBuckets", "readBucketRetentions", "writeBucketRetentions", "readBucketEncryption", "writeBucketEncryption", "writeBucketNotifications", "listFiles", "readFiles", "shareFiles", "writeFiles", "deleteFiles", "readBucketNotifications", "readFileLegalHolds", "writeFileLegalHolds", "readFileRetentions", "writeFileRetentions", "bypassGovernance" ]
 
-##################################################
-### S3 Client and url session
+#######################################################
+### Main functions
 
 
-def s3_client(connection_config: utils.ConnectionConfig, max_pool_connections: int = 10, max_attempts: int = 3, retry_mode: str='adaptive', read_timeout: int=120):
+def client(connection_config: utils.ConnectionConfig, max_pool_connections: int = 10, max_attempts: int = 3, retry_mode: str='adaptive', read_timeout: int=120):
     """
     Function to establish a client connection with an S3 account. This can use the legacy connect (signature_version s3) and the current version.
 
     Parameters
     ----------
     connection_config : dict
         A dictionary of the connection info necessary to establish an S3 connection. It should contain service_name, endpoint_url, aws_access_key_id, and aws_secret_access_key.
@@ -80,126 +82,25 @@
     else:
         s3_config.update({'config': botocore.config.Config(max_pool_connections=max_pool_connections, retries={'mode': retry_mode, 'max_attempts': max_attempts}, read_timeout=read_timeout)})
         s3 = boto3.client(**s3_config)
 
     return s3
 
 
-# def url_session(max_pool_connections: int = 30, max_attempts: int=3, read_timeout: int=120):
-#     """
-#     Function to setup a requests url session for url downloads
-
-#     Parameters
-#     ----------
-#     max_pool_connections : int
-#         The number of simultaneous connections for the S3 connection.
-#     max_attempts: int
-#         The number of retries if the connection fails.
-#     read_timeout: int
-#         The read timeout in seconds.
-
-#     Returns
-#     -------
-#     Session object
-#     """
-#     s = Session()
-#     retries1 = Retry(
-#         total=max_attempts,
-#         backoff_factor=1,
-#     )
-#     s.mount('https://', TimeoutHTTPAdapter(timeout=read_timeout, max_retries=retries1, pool_connections=max_pool_connections, pool_maxsize=max_pool_connections))
-
-#     return s
-
-
-def url_session(max_pool_connections: int = 10, max_attempts: int=3, read_timeout: int=120):
-    """
-    Function to setup a urllib3 pool manager for url downloads.
-
-    Parameters
-    ----------
-    max_pool_connections : int
-        The number of simultaneous connections for the S3 connection.
-    max_attempts: int
-        The number of retries if the connection fails.
-    read_timeout: int
-        The read timeout in seconds.
-
-    Returns
-    -------
-    Pool Manager object
-    """
-    timeout = urllib3.util.Timeout(read_timeout)
-    retries = Retry(
-        total=max_attempts,
-        backoff_factor=1,
-        )
-    http = urllib3.PoolManager(num_pools=max_pool_connections, timeout=timeout, retries=retries)
-
-    return http
-
-
-
-#######################################################
-### Main functions
-
-
-# def url_to_stream(url: HttpUrl, session: requests.sessions.Session=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **url_session_kwargs):
-#     """
-#     requests version
-#     """
-#     if session is None:
-#         session = url_session(**url_session_kwargs)
-
-#     headers = build_url_headers(range_start=range_start, range_end=range_end)
-
-#     response = session.get(url, headers=headers, stream=True)
-#     stream = ResponseStream(response.iter_content(chunk_size))
-
-#     return stream
-
-
-def url_to_stream(url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **url_session_kwargs):
-    """
-
-    """
-    if session is None:
-        session = url_session(**url_session_kwargs)
-
-    headers = utils.build_url_headers(range_start=range_start, range_end=range_end)
-
-    response = session.request('get', url, headers=headers, preload_content=False)
-    resp = utils.HttpResponse(response)
-
-    return resp
-
-
-def base_url_to_stream(obj_key: str, base_url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **url_session_kwargs):
-    """
-
-    """
-    if not base_url.endswith('/'):
-        base_url += '/'
-    url = urllib.parse.urljoin(base_url, obj_key)
-    response = url_to_stream(url, session, range_start, range_end, chunk_size, **url_session_kwargs)
-
-    return response
-
-
-def get_object(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **s3_client_kwargs):
+def get_object(obj_key: str, bucket: str, s3_client: botocore.client.BaseClient = None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **s3_client_kwargs):
     """
     Function to get an object from an S3 bucket. Either s3 or connection_config must be used. This function will return a file object of the object in the S3 location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
 
     Parameters
     ----------
     obj_key : str
         The object key in the S3 bucket.
     bucket : str
         The bucket name.
-    s3 : botocore.client.BaseClient
+    s3_client : botocore.client.BaseClient
         An S3 client object created via the s3_client function.
     version_id : str
         The S3 version id associated with the object.
     range_start: int
         The byte range start for the file.
     range_end: int
         The byte range end for the file.
@@ -209,130 +110,105 @@
         kwargs to the s3_client function if the s3 parameter was not passed.
 
     Returns
     -------
     read-only file obj
     """
     ## Get the object
-    if s3 is None:
-        s3 = s3_client(**s3_client_kwargs)
+    if s3_client is None:
+        s3_client = client(**s3_client_kwargs)
 
     params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id, range_start=range_start, range_end=range_end)
 
-    s3resp = utils.S3Response(s3, 'get_object', **params)
+    s3resp = utils.S3Response(s3_client, 'get_object', **params)
 
     return s3resp
 
 
-def get_object_combo(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, session: urllib3.poolmanager.PoolManager=None, base_url: HttpUrl=None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **kwargs):
-    """
-    Combo function to get an object from an S3 bucket either using the S3 get_object function or the base_url_to_stream function. One of s3, connection_config, or base_url must be used. This function will return a file object of the object in the S3 (or url) location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
-
-    Parameters
-    ----------
-    obj_key : str
-        The object key in the S3 bucket.
-    bucket : str
-        The bucket name.
-    s3 : botocore.client.BaseClient
-        An S3 client object created via the s3_client function.
-    base_url : HttpUrl
-        The url path up to the obj_key.
-    version_id : str
-        The S3 version id associated with the object.
-    range_start: int
-        The byte range start for the file.
-    range_end: int
-        The byte range end for the file.
-    chunk_size: int
-        The amount of bytes to download as once.
-    kwargs:
-        Either the s3_client_kwargs or the url_session_kwargs depending on the input.
-
-    Returns
-    -------
-    read-only file obj
-    """
-    ## Get the object
-    if isinstance(base_url, str) and (version_id is None):
-        stream = base_url_to_stream(obj_key, base_url, session, range_start, range_end, chunk_size, **kwargs)
-
-    elif isinstance(s3, botocore.client.BaseClient):
-        stream = get_object(obj_key, bucket, s3, version_id, range_start, range_end, chunk_size, **kwargs)
-
-    else:
-        raise TypeError('One of s3, connection_config, or public_url needs to be correctly defined.')
-
-    return stream
-
-
-def url_to_headers(url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, **url_session_kwargs):
-    """
-
-    """
-    if session is None:
-        session = url_session(**url_session_kwargs)
+# def get_object_combo(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, session: urllib3.poolmanager.PoolManager=None, base_url: HttpUrl=None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **kwargs):
+#     """
+#     Combo function to get an object from an S3 bucket either using the S3 get_object function or the base_url_to_stream function. One of s3, connection_config, or base_url must be used. This function will return a file object of the object in the S3 (or url) location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
 
-    response = session.request('head', url)
-    resp = utils.HttpResponse(response)
+#     Parameters
+#     ----------
+#     obj_key : str
+#         The object key in the S3 bucket.
+#     bucket : str
+#         The bucket name.
+#     s3 : botocore.client.BaseClient
+#         An S3 client object created via the s3_client function.
+#     base_url : HttpUrl
+#         The url path up to the obj_key.
+#     version_id : str
+#         The S3 version id associated with the object.
+#     range_start: int
+#         The byte range start for the file.
+#     range_end: int
+#         The byte range end for the file.
+#     chunk_size: int
+#         The amount of bytes to download as once.
+#     kwargs:
+#         Either the s3_client_kwargs or the url_session_kwargs depending on the input.
 
-    return resp
+#     Returns
+#     -------
+#     read-only file obj
+#     """
+#     ## Get the object
+#     if isinstance(base_url, str) and (version_id is None):
+#         stream = http_url.base_url_to_stream(obj_key, base_url, session, range_start, range_end, chunk_size, **kwargs)
 
+#     elif isinstance(s3, botocore.client.BaseClient):
+#         stream = get_object(obj_key, bucket, s3, version_id, range_start, range_end, chunk_size, **kwargs)
 
-def base_url_to_headers(obj_key: str, base_url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, **url_session_kwargs):
-    """
+#     else:
+#         raise TypeError('One of s3, connection_config, or public_url needs to be correctly defined.')
 
-    """
-    if not base_url.endswith('/'):
-        base_url += '/'
-    url = urllib.parse.urljoin(base_url, obj_key)
-    response = url_to_headers(url, session, **url_session_kwargs)
-
-    return response
+#     return stream
 
 
-def head_object(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, version_id: str=None, **s3_client_kwargs):
+def head_object(obj_key: str, bucket: str, s3_client: botocore.client.BaseClient = None, version_id: str=None, **s3_client_kwargs):
     """
     Function to get an object from an S3 bucket. Either s3 or connection_config must be used. This function will return a file object of the object in the S3 location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
 
     Parameters
     ----------
     obj_key : str
         The object key in the S3 bucket.
     bucket : str
         The bucket name.
-    s3 : botocore.client.BaseClient
+    s3_client : botocore.client.BaseClient
         An S3 client object created via the s3_client function.
     version_id : str
         The S3 version id associated with the object.
     s3_client_kwargs:
         kwargs to the s3_client function if the s3 parameter was not passed.
 
     Returns
     -------
     read-only file obj
     """
     ## Get the object
-    if s3 is None:
-        s3 = s3_client(**s3_client_kwargs)
+    if s3_client is None:
+        s3_client = client(**s3_client_kwargs)
 
     params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id)
 
-    s3resp = utils.S3Response(s3, 'head_object', **params)
+    s3resp = utils.S3Response(s3_client, 'head_object', **params)
 
     return s3resp
 
 
-def put_object(s3: botocore.client.BaseClient, bucket: str, obj_key: str, obj: Union[bytes, io.BufferedIOBase], metadata: dict={}, content_type: str=None, object_legal_hold: bool=False):
+def put_object(s3_client: botocore.client.BaseClient, bucket: str, obj_key: str, obj: Union[bytes, io.BufferedIOBase], metadata: dict={}, content_type: str=None, object_legal_hold: bool=False):
     """
     Function to upload data to an S3 bucket. This function will iteratively write the input file_obj in chunks ensuring that little memory is needed writing the object.
 
     Parameters
     ----------
-    s3 : boto3.client
+    s3_client : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
     obj_key : str
         The key name for the uploaded object.
     obj : bytes, io.BytesIO, or io.BufferedIOBase
         The file object to be uploaded.
@@ -349,170 +225,158 @@
     """
     # TODO : In python version 3.11, the file_digest function can input a file object
     if isinstance(obj, (bytes, bytearray)) and ('content-md5' not in metadata):
         metadata['content-md5'] = hashlib.md5(obj).hexdigest()
     params = utils.build_s3_params(bucket, obj_key=obj_key, metadata=metadata, content_type=content_type, object_legal_hold=object_legal_hold)
     params['Body'] = obj
 
-    s3resp = utils.S3Response(s3, 'put_object', **params)
+    s3resp = utils.S3Response(s3_client, 'put_object', **params)
     s3resp.metadata.update(metadata)
 
     return s3resp
 
 
 #####################################
 ### Other S3 operations
 
 
-def list_objects(s3: botocore.client.BaseClient, bucket: str, prefix: str=None, start_after: str=None, delimiter: str=None, max_keys: int=None, continuation_token: str=None):
+def list_objects(s3_client: botocore.client.BaseClient, bucket: str, prefix: str=None, start_after: str=None, delimiter: str=None, max_keys: int=None):
     """
     Wrapper S3 function around the list_objects_v2 base function.
 
     Parameters
     ----------
-    s3 : boto3.client
+    s3_client : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
     prefix : str
         Limits the response to keys that begin with the specified prefix.
     start_after : str
         The S3 key to start after.
     delimiter : str
         A delimiter is a character you use to group keys.
-    continuation_token : str
-        ContinuationToken indicates to S3 that the list is being continued on this bucket with a token.
-    date_format : str
-        If the object key has a date in it, pass a date format string to parse and add a column called KeyDate.
+    max_keys : int
+        Sets the maximum number of keys returned in the response. By default, the action returns up to 1,000 key names. The response might contain fewer keys but will never contain more.
 
     Returns
     -------
-    dict
+    S3ListResponse
     """
     params = utils.build_s3_params(bucket, start_after=start_after, prefix=prefix, delimiter=delimiter, max_keys=max_keys)
 
-    if continuation_token is not None:
-        params['ContinuationToken'] = continuation_token
-
-    # js = []
-    while True:
-        js1 = s3.list_objects_v2(**params)
-
-        if 'Contents' in js1:
-            # js.extend(js1['Contents'])
-            for js in js1['Contents']:
-                etag = js['ETag'].strip('"')
-                js['ETag'] = etag
-                yield js
-            if 'NextContinuationToken' in js1:
-                continuation_token = js1['NextContinuationToken']
-            else:
-                break
-        else:
-            break
+    resp = utils.S3ListResponse(s3_client, 'list_objects_v2', **params)
 
-    # return js
+    return resp
 
 
-def list_object_versions(s3: botocore.client.BaseClient, bucket: str, start_after: str=None, prefix: str=None, delimiter: str=None, max_keys: int=None, delete_markers: bool=False):
+def list_object_versions(s3_client: botocore.client.BaseClient, bucket: str, prefix: str=None, start_after: str=None, delimiter: str=None, max_keys: int=None):
     """
     Wrapper S3 function around the list_object_versions base function.
 
     Parameters
     ----------
-    s3 : boto3.client
+    s3_client : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
     prefix : str
         Limits the response to keys that begin with the specified prefix.
     start_after : str
         The S3 key to start after.
     delimiter : str or None
         A delimiter is a character you use to group keys.
-    date_format : str
-        If the object key has a date in it, pass a date format string to parse and add a column called KeyDate.
+    max_keys : int
+        Sets the maximum number of keys returned in the response. By default, the action returns up to 1,000 key names. The response might contain fewer keys but will never contain more.
 
     Returns
     -------
-    dict
+    S3ListResponse
     """
     params = utils.build_s3_params(bucket, key_marker=start_after, prefix=prefix, delimiter=delimiter, max_keys=max_keys)
 
-    # js = []
-    # dm = []
-    while True:
-        js1 = s3.list_object_versions(**params)
-
-        if 'Versions' in js1:
-            # js.extend(js1['Versions'])
-            for js in js1['Versions']:
-                etag = js['ETag'].strip('"')
-                js['ETag'] = etag
-                yield js
-            # if 'DeleteMarkers' in js1:
-            #     dm.extend(js1['DeleteMarkers'])
-            if 'NextKeyMarker' in js1:
-                params['KeyMarker'] = js1['NextKeyMarker']
-            else:
-                break
-        else:
-            break
+    resp = utils.S3ListResponse(s3_client, 'list_object_versions', **params)
+
+    return resp
+
+
+def delete_object(s3_client: botocore.client.BaseClient, bucket: str, obj_key: str, version_id: str=None):
+    """
+    obj_keys must be a list of dictionaries. The dicts must have the keys named Key and VersionId derived from the list_object_versions function. This function will automatically separate the list into 1000 count list chunks (required by the delete_objects request).
+
+    Returns
+    -------
+    None
+    """
+    params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id)
+
+    s3resp = utils.S3Response(s3_client, 'delete_object', **params)
 
-    # if delete_markers:
-    #     return js, dm
-    # else:
-    #     return js
+    return s3resp
 
 
-def delete_objects(s3: botocore.client.BaseClient, bucket: str, obj_keys: List[dict]):
+def delete_objects(s3_client: botocore.client.BaseClient, bucket: str, obj_keys: List[dict]):
     """
     obj_keys must be a list of dictionaries. The dicts must have the keys named Key and VersionId derived from the list_object_versions function. This function will automatically separate the list into 1000 count list chunks (required by the delete_objects request).
 
     Returns
     -------
     None
     """
     for keys in utils.chunks(obj_keys, 1000):
-        _ = s3.delete_objects(Bucket=bucket, Delete={'Objects': keys, 'Quiet': True})
+        keys2 = []
+        for key in keys:
+            if 'key' in key:
+                key['Key'] = key.pop('key')
+            if 'Key' not in key:
+                raise ValueError('"key" must be passed in the list of dict.')
+            if 'version_id' in key:
+                key['VersionId'] = key.pop('version_id')
+            if 'VersionId' not in key:
+                raise ValueError('"version_id" must be passed in the list of dict.')
+            keys2.append(key)
+
+        _ = s3_client.delete_objects(Bucket=bucket, Delete={'Objects': keys2, 'Quiet': True})
 
 
 ########################################################
 ### S3 Locks and holds
 
 
-def get_object_legal_hold(s3: botocore.client.BaseClient, bucket: str, obj_key: str):
+def get_object_legal_hold(s3_client: botocore.client.BaseClient, bucket: str, obj_key: str, version_id: str=None):
     """
     Function to get the staus of a legal hold of an object. The user must have s3:GetObjectLegalHold or b2:readFileLegalHolds permissions for this request.
 
     Parameters
     ----------
-    s3 : boto3.client
+    s3_client : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
     obj_key : str
         The key name for the uploaded object.
 
     Returns
     -------
     S3Response
     """
-    s3resp = utils.S3Response(s3, 'get_object_legal_hold', Bucket=bucket, Key=obj_key)
+    params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id)
+
+    s3resp = utils.S3Response(s3_client, 'get_object_legal_hold', **params)
 
     return s3resp
 
 
-def put_object_legal_hold(s3: botocore.client.BaseClient, bucket: str, obj_key: str, lock: bool=False):
+def put_object_legal_hold(s3_client: botocore.client.BaseClient, bucket: str, obj_key: str, lock: bool=False, version_id: str=None):
     """
     Function to put or remove a legal hold on an object. The user must have s3:PutObjectLegalHold or b2:writeFileLegalHolds permissions for this request.
 
     Parameters
     ----------
-    s3 : boto3.client
+    s3_client : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
     obj_key : str
         The key name for the uploaded object.
     lock : bool
         Should a lock be added to the object?
@@ -522,50 +386,49 @@
     None
     """
     if lock:
         hold = {'Status': 'ON'}
     else:
         hold = {'Status': 'OFF'}
 
-    # resp = s3.put_object_legal_hold(Bucket=bucket, Key=obj_key, LegalHold=hold)
-    # if resp['ResponseMetadata']['HTTPStatusCode'] != 200:
-    #     raise urllib.error.HTTPError(resp['ResponseMetadata']['HTTPStatusCode'])
+    params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id)
+    params['LegalHold'] = hold
 
-    s3resp = utils.S3Response(s3, 'put_object_legal_hold', Bucket=bucket, Key=obj_key, LegalHold=hold)
+    s3resp = utils.S3Response(s3_client, 'put_object_legal_hold', **params)
 
     return s3resp
 
 
-def get_object_lock_configuration(s3: botocore.client.BaseClient, bucket: str):
+def get_object_lock_configuration(s3_client: botocore.client.BaseClient, bucket: str):
     """
     Function to whther a bucket is configured to have object locks. The user must have s3:GetBucketObjectLockConfiguration or b2:readBucketRetentions permissions for this request.
 
     Parameters
     ----------
-    s3 : boto3.client
+    s3_client : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
 
     Returns
     -------
     S3Reponse
     """
-    s3resp = utils.S3Response(s3, 'get_object_lock_configuration', Bucket=bucket)
+    s3resp = utils.S3Response(s3_client, 'get_object_lock_configuration', Bucket=bucket)
 
     return s3resp
 
 
-def put_object_lock_configuration(s3: botocore.client.BaseClient, bucket: str, lock: bool=False):
+def put_object_lock_configuration(s3_client: botocore.client.BaseClient, bucket: str, lock: bool=False):
     """
     Function to enable or disable object locks for a bucket. The user must have s3:PutBucketObjectLockConfiguration or b2:writeBucketRetentions permissions for this request.
 
     Parameters
     ----------
-    s3 : boto3.client
+    s3_client : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
     lock : bool
         Should a lock be enabled for the bucket?
 
     Returns
@@ -574,103 +437,208 @@
     """
     if lock:
         hold = {'ObjectLockEnabled': 'Enable'}
     else:
         hold = {'ObjectLockEnabled': 'Disable'}
 
     # resp = s3.put_object_lock_configuration(Bucket=bucket, ObjectLockConfiguration=hold)
-    s3resp = utils.S3Response(s3, 'put_object_lock_configuration', Bucket=bucket, ObjectLockConfiguration=hold)
+    s3resp = utils.S3Response(s3_client, 'put_object_lock_configuration', Bucket=bucket, ObjectLockConfiguration=hold)
 
     return s3resp
 
 
 class S3Lock:
     """
 
     """
-    def __init__(self, s3: botocore.client.BaseClient, bucket: str, obj_key: str):
+    def __init__(self, s3_client: botocore.client.BaseClient, bucket: str, obj_key: str, version_id: str=None):
         """
+        This class contains a locking mechanism by utilizing S3 objects and associated versions. It has implementations for both shared and exclusive (the default) locks. It follows the same locking API as python thread locks (https://docs.python.org/3/library/threading.html#lock-objects), but with some extra methods for managing "deadlocks". Object versioning MUST be activated in the S3 bucket for this to work. The required S3 permissions are ListObjects, WriteObjects, and DeleteObjects.
+
+        This initialized class can be used as a context manager exactly like the thread locks.
 
+        Parameters
+        ----------
+        s3_client : botocore.client.BaseClient
+            An initialised boto3/botocore Client. The user is recommended to use the client function in this package.
+        bucket : str
+            The S3 bucket
+        obj_key : str
+            The base object key that will be given a lock. The extension ".lock" will be appended to the key, so the user is welcome to reference an existing object without worry that it will be overwritten.
+        version_id : str
+            Open a previously locked object version. This will allow the user to continue a lock from a previous instance (e.g. if that instance crashed). This will raise a KeyError if the object version doesn't exist.
         """
+        obj_lock_key = obj_key + '.lock'
+        objs = self._list_object_versions(s3_client, bucket, obj_lock_key)
 
+        if isinstance(version_id, str):
+            objs = [l for l in objs if l['version_id'] == version_id]
+            if objs:
+                self._version_id = version_id
+                self._last_modified = objs[0]['last_modified']
+            else:
+                raise KeyError(f'No object version with {version_id}.')
+        else:
+            self._version_id = ''
+            self._last_modified = None
 
+        self._s3_client = s3_client
+        self._bucket = bucket
+        self._obj_lock_key = obj_lock_key
+        self._obj_key = obj_key
 
-#########################################################
-### Backblaze
 
+    @staticmethod
+    def _list_object_versions(s3_client, bucket, obj_lock_key):
+        """
 
-def get_authorization_b2(username, password, session=None, **url_session_kwargs):
-    """
+        """
+        objs = list_object_versions(s3_client, bucket, prefix=obj_lock_key)
+        if objs.status in (401, 403):
+            raise urllib3.exceptions.HTTPError(str(objs.error)[1:-1])
+
+        meta = objs.metadata
+        res = []
+        if 'versions' in meta:
+            for l in meta['versions']:
+                if l['etag'] == md5_locks['exclusive']:
+                    l['lock_type'] = 'exclusive'
+                elif l['etag'] == md5_locks['shared']:
+                    l['lock_type'] = 'shared'
+                else:
+                    raise ValueError('This lock file was created by something else...')
+                res.append(l)
 
-    """
-    if session is None:
-        session = url_session(**url_session_kwargs)
+        return res
 
-    headers = urllib3.make_headers(basic_auth=f'{username}:{password}')
 
-    response = session.request('get', b2_auth_url, headers=headers)
-    resp = utils.HttpResponse(response)
+    def other_locks(self):
+        """
+        Method to list all of the other locks that might also be on the object.
 
-    return resp
+        Returns
+        -------
+        list of dict
+        """
+        objs = self._list_object_versions(self._s3_client, self._bucket, self._obj_lock_key)
 
+        if objs:
+            return [l for l in objs if l['version_id'] != self._version_id]
+        else:
+            return []
 
-def create_app_key_b2(auth_dict: dict, capabilities: List[str], key_name: str, duration: int=None, bucket_id: str=None, prefix: str=None, session=None, **url_session_kwargs):
-    """
 
-    """
-    account_id = auth_dict['accountId']
-    api_url = auth_dict['apiInfo']['storageApi']['apiUrl']
-    auth_token = auth_dict['authorizationToken']
+    def break_other_locks(self):
+        """
+        Removes all other locks that are on the object. This is only meant to be used in deadlock circumstances.
 
-    fields = {
-        'accountId': account_id,
-        'capabilities': capabilities,
-        'keyName': key_name}
+        Returns
+        -------
+        list of dict of the removed keys/versions
+        """
+        objs = self._list_object_versions(self._s3_client, self._bucket, self._obj_lock_key)
 
-    if isinstance(duration, int):
-        fields['validDurationInSeconds'] = duration
+        obj_keys = []
+        if objs:
+            for l in objs:
+                obj_keys.append({'Key': l['key'], 'VersionId': l['version_id']})
 
-    if isinstance(bucket_id, str):
-        fields['bucketId'] = bucket_id
+            delete_objects(self._s3_client, self._bucket, obj_keys)
 
-    if isinstance(prefix, str):
-        fields['namePrefix'] = prefix
+        return obj_keys
 
-    url = urllib.parse.urljoin(api_url, '/b2api/v3/b2_create_key')
 
-    if session is None:
-        session = url_session(**url_session_kwargs)
+    def locked(self):
+        """
+        Checks to see if there's a lock on the object. 
 
-    response = session.request('post', url, json=fields, headers={'Authorization': auth_token})
-    resp = utils.HttpResponse(response)
+        Returns
+        -------
+        bool
+        """
+        objs = self._list_object_versions(self._s3_client, self._bucket, self._obj_lock_key)
+        if objs:
+            return True
+        else:
+            return False
 
-    return resp
 
+    def aquire(self, blocking=True, timeout=-1, exclusive=True):
+        """
+        Acquire a lock, blocking or non-blocking.
 
-def list_buckets_b2(auth_dict: dict, session=None, **url_session_kwargs):
-    """
+        When invoked with the blocking argument set to True (the default), block until the lock is unlocked, then set it to locked and return True.
+        
+        When invoked with the blocking argument set to False, do not block. If a call with blocking set to True would block, return False immediately; otherwise, set the lock to locked and return True.
+        
+        When invoked with the timeout argument set to a positive value, block for at most the number of seconds specified by timeout and as long as the lock cannot be acquired. A timeout argument of -1 specifies an unbounded wait. It is forbidden to specify a timeout when blocking is False.
+
+        When the exclusive argument is True (the default), an exclusive lock is made. If False, then a shared lock is made. These are equivalent to the exclusive and shared locks in the linux flock command.
+        
+        The return value is True if the lock is acquired successfully, False if not (for example if the timeout expired).
+
+        Returns
+        -------
+        bool
+        """
+        if self._last_modified is None:
+            if exclusive:
+                body = b'1'
+            else:
+                body = b'0'
+            resp = put_object(self._s3_client, self._bucket, self._obj_lock_key, body)
+            if resp.status != 200:
+                raise urllib3.exceptions.HTTPError(str(resp.error)[1:-1])
+            self._version_id = resp.metadata['version_id']
+            self._last_modified = resp.metadata['last_modified']
+
+            objs = self.other_locks()
+
+            objs2 = [l for l in objs if (l['last_modified'] < self._last_modified) and (l['lock_type'] == 'exclusive')]
+
+            if objs2:
+                start_time = default_timer()
+
+                while blocking:
+                    sleep(2)
+                    objs = self.other_locks()
+                    objs2 = [l for l in objs if (l['last_modified'] < self._last_modified) and (l['lock_type'] == 'exclusive')]
+                    if len(objs2) == 0:
+                        return True
+                    else:
+                        if timeout > 0:
+                            duration = default_timer() - start_time
+                            if duration > timeout:
+                                break
 
-    """
-    account_id = auth_dict['accountId']
-    api_url = auth_dict['apiInfo']['storageApi']['apiUrl']
-    auth_token = auth_dict['authorizationToken']
+                return False
+            else:
+                return True
+        else:
+            return True
 
-    fields = {
-        'accountId': account_id,
-        }
 
-    url = urllib.parse.urljoin(api_url, '/b2api/v3/b2_list_buckets')
+    def release(self):
+        """
+        Release the lock. It can only release the lock that was created via this instance. Returns nothing.
+        """
+        if self._last_modified is not None:
+            _ = delete_object(self._s3_client, self._bucket, self._obj_lock_key, self._version_id)
+            self._version_id = ''
+            self._last_modified = None
+
+    def __enter__(self):
+        self.aquire()
+
+    def __exit__(self, *args):
+        self.release()
+
 
-    if session is None:
-        session = url_session(**url_session_kwargs)
 
-    response = session.request('post', url, json=fields, headers={'Authorization': auth_token})
-    resp = utils.HttpResponse(response)
 
-    return resp
```

### Comparing `s3func-0.1.5/s3func/tests/stns_data.blt` & `s3func-0.2.0/s3func/tests/stns_data.blt`

 * *Files identical despite different names*

### Comparing `s3func-0.1.5/s3func/tests/test_s3func.py` & `s3func-0.2.0/s3func/tests/test_s3func.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import pytest
 import os, pathlib
 import uuid
 import io
+import sys
 try:
     import tomllib as toml
 except ImportError:
     import tomli as toml
-from s3func import *
+from s3func import s3, b2, http_url, utils
+
 
 #################################################
 ### Parameters
 
 script_path = pathlib.Path(os.path.realpath(os.path.dirname(__file__)))
+package_path = str(script_path.parent)
+
+# if package_path not in sys.path:
+#     sys.path.insert(0, package_path)
+# import s3, b2, http_url, utils # For running without a package
 
 try:
     with open(script_path.joinpath('s3_config.toml'), "rb") as f:
         conn_config = toml.load(f)['connection_config']
 except:
     conn_config = {
         'service_name': 's3',
@@ -32,15 +39,15 @@
 threads = 10
 object_lock = False
 file_name = 'stns_data.blt'
 obj_key = uuid.uuid4().hex
 base_url = 'https://b2.tethys-ts.xyz/file/' + bucket + '/'
 url = base_url +  obj_key
 
-s3 = s3_client(conn_config)
+s3_client = s3.client(conn_config)
 
 
 ################################################
 ### Pytest stuff
 
 
 @pytest.hookimpl(tryfirst=True, hookwrapper=True)
@@ -60,20 +67,20 @@
     yield
 
     if request.node.rep_call.failed:
         # Add code here to cleanup failure scenario
         print("executing test failed")
 
         obj_keys = []
-        for js in list_object_versions(s3, bucket):
+        for js in s3.list_object_versions(s3_client, bucket):
             if js['Key'] == obj_key:
                 obj_keys.append({'Key': js['Key'], 'VersionId': js['VersionId']})
 
         if obj_keys:
-            delete_objects(s3, bucket, obj_keys)
+            s3.delete_objects(s3_client, bucket, obj_keys)
 
     # elif request.node.rep_call.passed:
     #     # Add code here to cleanup success scenario
     #     print("executing test success")
 
 
 ################################################
@@ -88,177 +95,207 @@
 #         (3, 2, 5),
 #     ],
 # )
 # def test_add(a: int, b: int, result: int):
 #     assert add(a, b) == result
 
 
-def test_put_object():
+def test_s3_put_object():
     """
 
     """
     ### Upload with bytes
     with io.open(script_path.joinpath(file_name), 'rb') as f:
         obj = f.read()
 
-    resp1 = put_object(s3, bucket, obj_key, obj)
+    resp1 = s3.put_object(s3_client, bucket, obj_key, obj)
 
     meta = resp1.metadata
     if meta['status'] != 200:
         raise ValueError('Upload failed')
 
     resp1_etag = meta['etag']
 
     ## Upload with a file-obj
-    resp2 = put_object(s3, bucket, obj_key, io.open(script_path.joinpath(file_name), 'rb'))
+    resp2 = s3.put_object(s3_client, bucket, obj_key, io.open(script_path.joinpath(file_name), 'rb'))
 
     meta = resp2.metadata
     if meta['status'] != 200:
         raise ValueError('Upload failed')
 
     resp2_etag = meta['etag']
 
     assert resp1_etag == resp2_etag
 
 
-def test_list_objects():
+def test_s3_list_objects():
     """
 
     """
     count = 0
     found_key = False
-    for i, js in enumerate(list_objects(s3, bucket)):
+    resp = s3.list_objects(s3_client, bucket)
+    for i, js in enumerate(resp.metadata['contents']):
         count += 1
-        if js['Key'] == obj_key:
+        if js['key'] == obj_key:
             found_key = True
 
     assert found_key
 
 
-def test_list_object_versions():
+def test_s3_list_object_versions():
     """
 
     """
     count = 0
     found_key = False
-    for i, js in enumerate(list_object_versions(s3, bucket)):
+    resp = s3.list_object_versions(s3_client, bucket)
+    for i, js in enumerate(resp.metadata['versions']):
         count += 1
-        if js['Key'] == obj_key:
+        if js['key'] == obj_key:
             found_key = True
 
     assert found_key
 
 
-def test_get_object():
+def test_s3_get_object():
     """
 
     """
-    stream1 = get_object(obj_key, bucket, s3)
+    stream1 = s3.get_object(obj_key, bucket, s3_client)
     data1 = stream1.stream.read()
 
-    stream2 = get_object(obj_key, bucket, connection_config=conn_config)
+    stream2 = s3.get_object(obj_key, bucket, connection_config=conn_config)
     data2 = stream2.stream.read()
 
     assert data1 == data2
 
 
-def test_url_to_stream():
+def test_http_url_get_object():
     """
 
     """
-    stream1 = url_to_stream(url)
+    stream1 = http_url.get_object(url)
     data1 = stream1.stream.read()
 
-    stream2 = base_url_to_stream(obj_key, base_url)
+    new_url = http_url.join_url_obj_key(obj_key, base_url)
+
+    stream2 = http_url.get_object(new_url)
     data2 = stream2.stream.read()
 
     assert data1 == data2
 
 
-def test_head_object():
+def test_s3_head_object():
     """
 
     """
-    response = head_object(obj_key, bucket, s3)
+    response = s3.head_object(obj_key, bucket, s3_client)
 
     assert 'version_id' in response.metadata
 
 
-def test_url_to_headers():
+def test_http_url_head_object():
     """
 
     """
-    response = url_to_headers(url)
+    response = http_url.head_object(url)
 
     assert 'version_id' in response.metadata
 
 
 def test_legal_hold():
     """
 
     """
-    hold = get_object_legal_hold(s3, bucket, obj_key)
-    if hold.status != 403:
+    hold = s3.get_object_legal_hold(s3_client, bucket, obj_key)
+    if hold.status != 404:
         raise ValueError("There's a hold, but there shouldn't be.")
 
-    put_hold = put_object_legal_hold(s3, bucket, obj_key, True)
+    put_hold = s3.put_object_legal_hold(s3_client, bucket, obj_key, True)
     if put_hold.status != 200:
         raise ValueError("Creating a hold failed.")
 
-    hold = get_object_legal_hold(s3, bucket, obj_key)
+    hold = s3.get_object_legal_hold(s3_client, bucket, obj_key)
     if not hold.metadata['legal_hold']:
         raise ValueError("There isn't a hold, but there should be.")
 
-    put_hold = put_object_legal_hold(s3, bucket, obj_key, False)
+    put_hold = s3.put_object_legal_hold(s3_client, bucket, obj_key, False)
     if put_hold.status != 200:
         raise ValueError("Removing a hold failed.")
 
-    hold = get_object_legal_hold(s3, bucket, obj_key)
+    hold = s3.get_object_legal_hold(s3_client, bucket, obj_key)
     if hold.metadata['legal_hold']:
         raise ValueError("There's a hold, but there shouldn't be.")
 
-    resp2 = put_object(s3, bucket, obj_key, open(script_path.joinpath(file_name), 'rb'), object_legal_hold=True)
+    _ = s3.put_object(s3_client, bucket, obj_key, open(script_path.joinpath(file_name), 'rb'), object_legal_hold=True)
 
-    hold = get_object_legal_hold(s3, bucket, obj_key)
+    hold = s3.get_object_legal_hold(s3_client, bucket, obj_key)
     if not hold.metadata['legal_hold']:
         raise ValueError("There isn't a hold, but there should be.")
 
-    put_hold = put_object_legal_hold(s3, bucket, obj_key, False)
+    put_hold = s3.put_object_legal_hold(s3_client, bucket, obj_key, False)
     if put_hold.status != 200:
         raise ValueError("Removing a hold failed.")
 
-    hold = get_object_legal_hold(s3, bucket, obj_key)
+    hold = s3.get_object_legal_hold(s3_client, bucket, obj_key)
     if hold.metadata['legal_hold']:
         raise ValueError("There's a hold, but there shouldn't be.")
 
     assert True
 
 
 def test_delete_objects():
     """
 
     """
     obj_keys = []
-    for js in list_object_versions(s3, bucket):
-        if js['Key'] == obj_key:
-            obj_keys.append({'Key': js['Key'], 'VersionId': js['VersionId']})
+    resp = s3.list_object_versions(s3_client, bucket)
+    for js in resp.metadata['versions']:
+        if js['key'] == obj_key:
+            obj_keys.append({'key': js['key'], 'version_id': js['version_id']})
 
-    delete_objects(s3, bucket, obj_keys)
+    s3.delete_objects(s3_client, bucket, obj_keys)
 
     found_key = False
-    for i, js in enumerate(list_object_versions(s3, bucket)):
-        if js['Key'] == obj_key:
+    resp = s3.list_object_versions(s3_client, bucket)
+    for i, js in enumerate(resp.metadata['versions']):
+        if js['key'] == obj_key:
             found_key = True
 
     assert not found_key
 
 
+def test_S3Lock():
+    """
+
+    """
+    s3lock = s3.S3Lock(s3_client, bucket, obj_key)
+
+    other_locks = s3lock.other_locks()
+
+    assert isinstance(other_locks, list)
+
+    if other_locks:
+        _ = s3lock.break_other_locks()
+
+    assert not s3lock.locked()
+
+    assert s3lock.aquire()
+
+    assert s3lock.locked()
+
+    s3lock.release()
 
+    assert not s3lock.locked()
 
+    with s3lock:
+        assert s3lock.locked()
 
+    assert not s3lock.locked()
```

### Comparing `s3func-0.1.5/.gitignore` & `s3func-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `s3func-0.1.5/LICENSE` & `s3func-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s3func-0.1.5/README.md` & `s3func-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `s3func-0.1.5/pyproject.toml` & `s3func-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `s3func-0.1.5/PKG-INFO` & `s3func-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: s3func
-Version: 0.1.5
+Version: 0.2.0
 Summary: Simple functions for working with S3
 Project-URL: Documentation, https://mullenkamp.github.io/s3func/
 Project-URL: Source, https://github.com/mullenkamp/s3func
 Author-email: s3func <mullenkamp1@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: s3func Version: 0.1.5 Summary: Simple functions for
+Metadata-Version: 2.3 Name: s3func Version: 0.2.0 Summary: Simple functions for
 working with S3 Project-URL: Documentation, https://mullenkamp.github.io/
 s3func/ Project-URL: Source, https://github.com/mullenkamp/s3func Author-email:
 s3func
 gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
 3 :: Only Requires-Python: >=3.9 Requires-Dist: boto3 Requires-Dist: pydantic
 Requires-Dist: urllib3 Description-Content-Type: text/markdown # s3func
                      SSiimmppllee ffuunnccttiioonnss ffoorr wwoorrkkiinngg wwiitthh SS33
```

