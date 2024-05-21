# Comparing `tmp/appmesh-1.0.7-py3-none-any.whl.zip` & `tmp/appmesh-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16391 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-20 10:22 appmesh/__init__.py
--rw-r--r--  2.0 unx    59666 b- defN 24-May-20 10:22 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-May-20 10:22 appmesh-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-20 10:22 appmesh-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-20 10:22 appmesh-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-20 10:22 appmesh-1.0.7.dist-info/RECORD
-6 files, 71018 bytes uncompressed, 15569 bytes compressed:  78.1%
+Zip file size: 16378 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-21 12:41 appmesh/__init__.py
+-rw-r--r--  2.0 unx    59572 b- defN 24-May-21 12:41 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-May-21 12:41 appmesh-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 12:41 appmesh-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-21 12:41 appmesh-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-21 12:41 appmesh-1.0.8.dist-info/RECORD
+6 files, 70924 bytes uncompressed, 15556 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-1.0.7.dist-info/METADATA
+Filename: appmesh-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-1.0.7.dist-info/WHEEL
+Filename: appmesh-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-1.0.7.dist-info/top_level.txt
+Filename: appmesh-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-1.0.7.dist-info/RECORD
+Filename: appmesh-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -1385,15 +1385,15 @@
         class ResponseMsg:
             """HTTP response message"""
 
             uuid: str = ""
             request_uri: str = ""
             http_status: int = 0
             body_msg_type: str = ""
-            body: bytes = b""
+            body: str = ""
             headers: dict = {}
 
             def desirialize(self, buf: bytes):
                 """Deserialize response message"""
                 dic = msgpack.unpackb(buf)
                 for k, v in dic.items():
                     setattr(self, k, v)
@@ -1435,15 +1435,15 @@
         resp_data = self.__recvall(int.from_bytes(self.__recvall(TCP_MESSAGE_HEADER_LENGTH), "big", signed=False))
         if resp_data is None or len(resp_data) == 0:
             self.__close_socket()
             raise Exception("socket connection broken")
         appmesh_resp = ResponseMsg().desirialize(resp_data)
         http_resp = requests.Response()
         http_resp.status_code = appmesh_resp.http_status
-        http_resp._content = appmesh_resp.body if "application/octet-stream" in appmesh_resp.body_msg_type.lower() else appmesh_resp.body.encode("utf8")
+        http_resp._content = appmesh_resp.body.encode("utf8")
         http_resp.headers = appmesh_resp.headers
         http_resp.encoding = MESSAGE_ENCODING_UTF8
         if appmesh_resp.body_msg_type:
             http_resp.headers["Content-Type"] = appmesh_resp.body_msg_type
         return http_resp
 
     ########################################
```

## Comparing `appmesh-1.0.7.dist-info/METADATA` & `appmesh-1.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 1.0.7
+Version: 1.0.8
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 1.0.7 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 1.0.8 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```

