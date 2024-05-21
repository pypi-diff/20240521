# Comparing `tmp/dataverse-sdk-1.1.0.tar.gz` & `tmp/dataverse_sdk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse-sdk-1.1.0.tar", last modified: Thu Jan 18 02:56:53 2024, max compression
+gzip compressed data, was "dataverse_sdk-1.2.1.tar", last modified: Tue May 21 02:04:17 2024, max compression
```

## Comparing `dataverse-sdk-1.1.0.tar` & `dataverse_sdk-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-01-18 02:56:53.216733 dataverse-sdk-1.1.0/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    13961 2024-01-18 02:56:53.216533 dataverse-sdk-1.1.0/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    13668 2024-01-18 02:49:01.000000 dataverse-sdk-1.1.0/README.md
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-01-18 02:56:53.213709 dataverse-sdk-1.1.0/dataverse_sdk/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-12-21 03:02:11.000000 dataverse-sdk-1.1.0/dataverse_sdk/__init__.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-01-18 02:56:53.214710 dataverse-sdk-1.1.0/dataverse_sdk/apis/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse-sdk-1.1.0/dataverse_sdk/apis/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10998 2024-01-16 06:44:42.000000 dataverse-sdk-1.1.0/dataverse_sdk/apis/backend.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    33609 2024-01-18 02:49:01.000000 dataverse-sdk-1.1.0/dataverse_sdk/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1872 2024-01-18 02:49:01.000000 dataverse-sdk-1.1.0/dataverse_sdk/connections.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      761 2024-01-16 06:44:42.000000 dataverse-sdk-1.1.0/dataverse_sdk/constants.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-01-18 02:56:53.215100 dataverse-sdk-1.1.0/dataverse_sdk/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse-sdk-1.1.0/dataverse_sdk/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-12-21 03:02:11.000000 dataverse-sdk-1.1.0/dataverse_sdk/exceptions/client.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-01-18 02:56:53.215875 dataverse-sdk-1.1.0/dataverse_sdk/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse-sdk-1.1.0/dataverse_sdk/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     3120 2023-12-21 03:02:11.000000 dataverse-sdk-1.1.0/dataverse_sdk/schemas/api.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    12556 2024-01-18 02:49:01.000000 dataverse-sdk-1.1.0/dataverse_sdk/schemas/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1184 2024-01-18 02:49:01.000000 dataverse-sdk-1.1.0/dataverse_sdk/schemas/common.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-01-18 02:56:53.216131 dataverse-sdk-1.1.0/dataverse_sdk/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse-sdk-1.1.0/dataverse_sdk/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      657 2023-12-21 03:02:11.000000 dataverse-sdk-1.1.0/dataverse_sdk/utils/utils.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-01-18 02:56:53.216345 dataverse-sdk-1.1.0/dataverse_sdk.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    13961 2024-01-18 02:56:53.000000 dataverse-sdk-1.1.0/dataverse_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2024-01-18 02:56:53.000000 dataverse-sdk-1.1.0/dataverse_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-01-18 02:56:53.000000 dataverse-sdk-1.1.0/dataverse_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       23 2024-01-18 02:56:53.000000 dataverse-sdk-1.1.0/dataverse_sdk.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2024-01-18 02:56:53.000000 dataverse-sdk-1.1.0/dataverse_sdk.egg-info/top_level.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-01-18 02:56:53.216772 dataverse-sdk-1.1.0/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      618 2024-01-18 02:49:01.000000 dataverse-sdk-1.1.0/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.135285 dataverse_sdk-1.2.1/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    14020 2024-05-21 02:04:17.135000 dataverse_sdk-1.2.1/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    13697 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/README.md
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.132289 dataverse_sdk-1.2.1/dataverse_sdk/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/__init__.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.133172 dataverse_sdk-1.2.1/dataverse_sdk/apis/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/apis/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    11172 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/dataverse_sdk/apis/backend.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    37533 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/dataverse_sdk/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1872 2024-01-18 02:49:01.000000 dataverse_sdk-1.2.1/dataverse_sdk/connections.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      740 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/dataverse_sdk/constants.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.133466 dataverse_sdk-1.2.1/dataverse_sdk/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      141 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/dataverse_sdk/exceptions/client.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.134145 dataverse_sdk-1.2.1/dataverse_sdk/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     3120 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/schemas/api.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    12556 2024-01-18 02:49:01.000000 dataverse_sdk-1.2.1/dataverse_sdk/schemas/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1216 2024-05-21 02:03:44.000000 dataverse_sdk-1.2.1/dataverse_sdk/schemas/common.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.134477 dataverse_sdk-1.2.1/dataverse_sdk/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      657 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/utils/utils.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.134775 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    14020 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       37 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-05-21 02:04:17.135329 dataverse_sdk-1.2.1/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      636 2024-05-21 02:03:44.000000 dataverse_sdk-1.2.1/setup.py
```

### Comparing `dataverse-sdk-1.1.0/PKG-INFO` & `dataverse_sdk-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 1.1.0
+Version: 1.2.1
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
 Requires-Dist: requests
+Requires-Dist: httpx>=0.23.0
 
 # Dataverse SDK For Python
 Dataverse is a MLOPs platform for assisting in data selection, data visualization and model training in computer vision.
 Use Dataverse-SDK for Python to help you to interact with the Dataverse platform by Python. Currently, the library supports:
   - Create Project with your input ontology and sensors
   - Get Project by project-id
   - Create Dataset from your AWS/Azure storage or local
@@ -37,15 +38,15 @@
 
 Interaction with the Dataverse site starts with an instance of the `DataverseClient` class. You need site url, an email-account and its password to instantiate the client object.
 
 ```Python
 from dataverse_sdk import *
 from dataverse_sdk.connections import get_connection
 client = DataverseClient(
-    host=DataverseHost.PRODUCTION, email="XXX", password="***", alias="default", force = False,
+    host=DataverseHost.PRODUCTION, email="XXX", password="***", alias="default", force = False, service_id="xxxx-xxxx-xx-xxx"
 )
 assert client is get_connection()
 
 # Should provide different alias if you are trying to connect to different workspaces
 client2 = DataverseClient(
     host=DataverseHost.PRODUCTION, email="account-2", password="***", alias="client2", force = False,
 )
@@ -373,8 +374,8 @@
 
 ## Contributing
 
 
 
 ## Links to language repos
 
-[Python Readme](https://github.com/linkernetworks/dataverse-sdk/tree/develop/python/README.md)
+[Python Readme](https://github.com/linkernetworks/dataverse-sdk/tree/master/python/README.md)
```

### Comparing `dataverse-sdk-1.1.0/README.md` & `dataverse_sdk-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 Interaction with the Dataverse site starts with an instance of the `DataverseClient` class. You need site url, an email-account and its password to instantiate the client object.
 
 ```Python
 from dataverse_sdk import *
 from dataverse_sdk.connections import get_connection
 client = DataverseClient(
-    host=DataverseHost.PRODUCTION, email="XXX", password="***", alias="default", force = False,
+    host=DataverseHost.PRODUCTION, email="XXX", password="***", alias="default", force = False, service_id="xxxx-xxxx-xx-xxx"
 )
 assert client is get_connection()
 
 # Should provide different alias if you are trying to connect to different workspaces
 client2 = DataverseClient(
     host=DataverseHost.PRODUCTION, email="account-2", password="***", alias="client2", force = False,
 )
@@ -361,8 +361,8 @@
 
 ## Contributing
 
 
 
 ## Links to language repos
 
-[Python Readme](https://github.com/linkernetworks/dataverse-sdk/tree/develop/python/README.md)
+[Python Readme](https://github.com/linkernetworks/dataverse-sdk/tree/master/python/README.md)
```

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk/__init__.py` & `dataverse_sdk-1.2.1/dataverse_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk/apis/backend.py` & `dataverse_sdk-1.2.1/dataverse_sdk/apis/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import Optional, Union
 from urllib.parse import urlencode
 
 import requests
 from requests import sessions
 from requests.adapters import HTTPAdapter, Retry
 
+from ..exceptions.client import BadRequest
+
 logger = logging.getLogger(__name__)
 
 
 class BackendAPI:
     adapter = HTTPAdapter(
         max_retries=Retry(
             total=10, backoff_factor=15, status_forcelist=[500, 502, 503, 504]
@@ -19,25 +21,26 @@
     )
 
     def __init__(
         self,
         host: str,
         email: str,
         password: str,
+        service_id: str,
     ):
         # TODO: Support api versioning
         self.host = host
-        self.headers = {"Content-Type": "application/json"}
+        self.headers = {
+            "Content-Type": "application/json",
+            "X-Request-Service-Id": service_id,
+        }
         self.access_token = None
         self.email = email
         self.password = password
-        self.login(
-            email=email,
-            password=password,
-        )
+        self.login(email=email, password=password)
 
     def send_request(
         self,
         url: str,
         method: str,
         attempts: int = 1,
         max_attempts: int = 5,
@@ -86,20 +89,22 @@
                 url=url,
                 method=method,
                 attempts=attempts + 1,
                 max_attempts=max_attempts,
                 **kwargs,
             )
 
+        if resp.status_code == 400:
+            raise BadRequest(resp.json())
+
         if not 200 <= resp.status_code <= 299:
             raise Exception(
                 f"[{parent_func}] request failed (kwargs: {kwargs})"
                 f", status code: {resp.status_code}, response detail: {resp.__dict__}"
             )
-
         return resp
 
     def login(self, email: str, password: str):
         if email is None:
             raise ValueError("Can't login with null email.")
         if password is None:
             raise ValueError("Can't login with null password.")
@@ -251,14 +256,15 @@
         render_pcd: bool = False,
         container_name: Optional[str] = None,
         sas_token: Optional[str] = None,
         description: Optional[str] = None,
         annotations: Optional[list[str]] = None,
         access_key_id: Optional[str] = None,
         secret_access_key: Optional[str] = None,
+        create_dataset_uuid: Optional[str] = None,
     ) -> dict:
         if auto_tagging is None:
             auto_tagging = []
         if annotations is None:
             annotations = []
         payload_data = {
             "name": name,
@@ -283,14 +289,17 @@
         if not (all(aws_access_key) or not any(aws_access_key)):
             raise ValueError("Need to assign both secret_access_key and access_key_id")
         if secret_access_key and access_key_id:
             payload_data.update(
                 {"secret_access_key": secret_access_key, "access_key_id": access_key_id}
             )
 
+        if create_dataset_uuid:
+            payload_data.update({"create_dataset_uuid": create_dataset_uuid})
+
         resp = self.send_request(
             url=f"{self.host}/api/datasets/",
             method="post",
             headers=self.headers,
             data=payload_data,
         )
         return resp.json()
@@ -300,42 +309,32 @@
             url=f"{self.host}/api/datasets/{dataset_id}/",
             method="get",
             headers=self.headers,
         )
 
         return resp.json()
 
-    def upload_files(
+    def generate_presigned_url(
         self,
-        dataset_id: int,
-        container_name: str,
-        is_finished: bool,
-        file_dict: dict[str, bytes],
+        file_paths: list,
+        create_dataset_uuid: Optional[str],
+        data_source: str,
     ):
-        file_dict["json"] = (
-            None,
-            json.dumps(
-                {
-                    "dataset_id": dataset_id,
-                    "container_name": container_name,
-                    "is_finished": is_finished,
-                }
-            ),
-            "application/json",
-        )
-
+        payload = {"filenames": file_paths, "data_source": data_source}
+        if create_dataset_uuid:
+            payload["create_dataset_uuid"] = create_dataset_uuid
         resp = self.send_request(
-            url=f"{self.host}/api/datasets/upload-files/",
+            url=f"{self.host}/api/datasets/upload-file-information/",
             method="post",
-            headers={"Authorization": self.headers["Authorization"]},
-            files=file_dict,
+            headers=self.headers,
+            data=payload,
         )
-        return resp
+        return resp.json()
 
     def update_dataset(self, dataset_id: int, **kwargs):
         resp = self.send_request(
             url=f"{self.host}/api/datasets/{dataset_id}/",
             method="patch",
             headers=self.headers,
             data=kwargs,
         )
-        return resp
+        return resp.json()
```

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk/client.py` & `dataverse_sdk-1.2.1/dataverse_sdk/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+import asyncio
 import logging
-from os.path import isfile
+from collections import deque
 from typing import Optional
 
+from httpx import AsyncClient, AsyncHTTPTransport, Response, Timeout
 from pydantic import ValidationError
 
 from .apis.backend import BackendAPI
-from .connections import add_connection, get_connection
+from .connections import (
+    add_connection,
+    get_connection,
+)
 from .constants import DataverseHost
-from .exceptions.client import ClientConnectionError
+from .exceptions.client import BadRequest, ClientConnectionError
 from .schemas.api import (
     AttributeAPISchema,
     DatasetAPISchema,
     OntologyAPISchema,
     ProjectAPISchema,
     ProjectTagAPISchema,
 )
@@ -45,14 +50,15 @@
 
 class DataverseClient:
     def __init__(
         self,
         host: DataverseHost,
         email: str,
         password: str,
+        service_id: str,
         alias: str = "default",
         force: bool = False,
     ) -> None:
         """
         Instantiate a Dataverse client.
 
         Parameters
@@ -64,31 +70,33 @@
         force: bool, whether replace the connection if alias exists, default is False
 
         Raises
         ------
         ValueError
         """
         if host not in DataverseHost:
-            raise ValueError("Invalid dataverse host, if the host is available?")
+            raise ValueError("Invalid dataverse host, is the host available?")
         self.host = host
         self._api_client = None
         self.alias = alias
-        self._init_api_client(email=email, password=password)
+        self._init_api_client(email=email, password=password, service_id=service_id)
         add_connection(alias=alias, conn=self, force=force)
 
     def _init_api_client(
         self,
         email: str,
         password: str,
+        service_id: str,
     ) -> None:
         try:
             self._api_client = BackendAPI(
                 host=self.host,
                 email=email,
                 password=password,
+                service_id=service_id,
             )
         except Exception as e:
             raise ClientConnectionError(f"Failed to initialize the api client: {e}")
 
     @staticmethod
     def _get_api_client(
         client: Optional["DataverseClient"] = None, client_alias: Optional[str] = None
@@ -825,32 +833,26 @@
         ------
         ValueError
         ValidationError
             raise exception if there is any error occurs when composing request body.
         ClientConnectionError
             raise exception if there is any error occurs when calling backend APIs.
         """
-        if data_source not in {DataSource.AWS, data_source.Azure}:
-            raise ValueError(
-                f"Data source ({data_source}) is not supported for SDK import"
-            )
-
         if annotations is None:
             annotations = []
         if auto_tagging is None:
             auto_tagging = []
 
         if type == DatasetType.ANNOTATED_DATA and len(annotations) == 0:
             raise ValueError(
                 "Annotated data should provide at least one annotation folder name (groundtruth or model_name)"
             )
         api, client_alias = DataverseClient._get_api_client(
             client=client, client_alias=client_alias
         )
-
         sensor_ids = [sensor.id for sensor in sensors]
         project_id = project.id
         try:
             raw_dataset_data: dict = DatasetAPISchema(
                 name=name,
                 project_id=project_id,
                 sensor_ids=sensor_ids,
@@ -872,79 +874,182 @@
                 **kwargs,
             ).dict(exclude_none=True)
         except ValidationError as e:
             raise ValidationError(
                 f"Something wrong when composing the final dataset data: {e}"
             )
 
-        try:
-            dataset_data = api.create_dataset(**raw_dataset_data)
-        except Exception as e:
-            raise ClientConnectionError(f"Failed to create the dataset: {e}")
-
+        if data_source == DataSource.SDK:
+            create_dataset_uuid = DataverseClient.upload_files_from_local(
+                api, raw_dataset_data
+            )
+            raw_dataset_data["create_dataset_uuid"] = create_dataset_uuid
+        dataset_data = api.create_dataset(**raw_dataset_data)
         dataset_data.update(
             {
                 "project": project,
                 "sensors": sensors,
                 "sequential": sequential,
                 "generate_metadata": generate_metadata,
                 "auto_tagging": auto_tagging,
                 "annotations": annotations,
             }
         )
+        return Dataset(**dataset_data, client_alias=client_alias)
 
-        if data_source in {DataSource.Azure, DataSource.AWS}:
-            return Dataset(**dataset_data, client_alias=client_alias)
+    @staticmethod
+    def upload_files_from_local(api: BackendAPI, raw_dataset_data: dict) -> dict:
+        loop = asyncio.get_event_loop()
+        data_folder = raw_dataset_data["data_folder"]
+        # TODO: support more format
+        # Current only support scanning data_folder
+        # meaning , support Visionai format
+        # raw_dataset_data.get("annotation_folder"),
+        # raw_dataset_data.get("calibration_folder"),
+        # raw_dataset_data.get("lidar_folder"),
+        file_paths = DataverseClient._find_all_paths(data_folder)
+        upload_task_queue, create_dataset_uuid, failed_urls = loop.run_until_complete(
+            DataverseClient.run_generate_presigned_urls(
+                file_paths=file_paths, api=api, data_folder=data_folder
+            )
+        )
+        if failed_urls:
+            raise ClientConnectionError(f"unable to generate urls for: {failed_urls}")
 
-        # TODO open for the sdk-local uploading
-        # start uploading from local
-        folder_paths: list[Optional[str]] = [
-            raw_dataset_data.get("data_folder"),
-            raw_dataset_data.get("annotation_folder"),
-            raw_dataset_data.get("calibration_folder"),
-            raw_dataset_data.get("lidar_folder"),
-        ]
-        annotation_file = raw_dataset_data.get("annotation_file")
+        if not create_dataset_uuid:
+            raise ClientConnectionError(
+                "something went wrong, missing create dataset uuid"
+            )
+
+        failed_urls = loop.run_until_complete(
+            DataverseClient.run_upload_tasks(upload_task_queue)
+        )
+        if failed_urls:
+            raise ClientConnectionError(f"failed to upload urls: {failed_urls}")
+        return create_dataset_uuid
+
+    @staticmethod
+    async def run_generate_presigned_urls(
+        file_paths: list, api: BackendAPI, data_folder: str
+    ) -> tuple[deque, str, list[str]]:
+        max_retry_count, batch_size = 3, 50
+
+        failed_urls = []
+        upload_task_queue = deque()
+
+        # TODO: convert the following code to async tasks loop
+        generate_url_queue = deque()
+        for i in range(0, len(file_paths), batch_size):
+            generate_url_queue.append((file_paths[i : i + batch_size], 0))
+
+        create_dataset_uuid: str = None
+        while len(generate_url_queue) != 0:
+            batched_file_paths, retry_count = generate_url_queue.popleft()
+            if retry_count >= max_retry_count:
+                failed_urls.extend(batched_file_paths)
+
+            # NOTE: This is extremely slow to do it over here
+            # this replaces the full file path to relative file path
+            # i.e <long data folder path>/data/image.jpg -> /data/image.jpg
+            filtered_paths = [
+                path.replace(data_folder, "") for path in batched_file_paths
+            ]
+            try:
+                resp = api.generate_presigned_url(
+                    file_paths=filtered_paths,
+                    create_dataset_uuid=create_dataset_uuid,
+                    data_source=DataSource.SDK,
+                )
+                url_infos: list[dict] = resp["url_info"]
+                create_dataset_uuid = resp["dataset_info"]["create_dataset_uuid"]
 
+                upload_task_queue.append((batched_file_paths, url_infos))
+
+            except KeyError:
+                logging.exception("Is api schema changed?")
+                raise
+            except BadRequest as e:
+                logging.exception(e)
+                raise
+            except Exception:
+                generate_url_queue.append((batched_file_paths, retry_count + 1))
+        return upload_task_queue, create_dataset_uuid, failed_urls
+
+    @staticmethod
+    async def run_upload_tasks(upload_task_queue: deque) -> list[str]:
+        tasks = []
+        client = AsyncThirdPartyAPI()
+        for batched_file_paths, upload_file_infos in upload_task_queue:
+
+            async def f(
+                paths: list[str],
+                upload_infos: list[dict],
+                async_client: AsyncThirdPartyAPI,
+            ) -> list[str]:
+                failed_urls = []
+                for path, info in zip(paths, upload_infos):
+                    try:
+                        with open(path, "rb") as file:
+                            await async_client.upload_file(
+                                method=info["method"],
+                                target_url=info["url"],
+                                file=file.read(),
+                                content_type=info["content_type"],
+                            )
+                    except Exception as e:
+                        logging.exception(e)
+                        failed_urls.append(path)
+
+                return failed_urls
+
+            tasks.append(
+                f(
+                    paths=batched_file_paths,
+                    upload_infos=upload_file_infos,
+                    async_client=client,
+                )
+            )
+
+        failed_urls = []
+        for results in await asyncio.gather(*tasks):
+            failed_urls.extend(results)
+        return failed_urls
+
+    @staticmethod
+    def _find_all_paths(*paths) -> list[str]:
         all_filepaths: list[str] = []
-        for path in folder_paths:
-            if path is not None:
-                all_filepaths.extend(get_filepaths(path))
-
-        if annotation_file is not None:
-            if not isfile(annotation_file):
-                raise ValueError("annotation_file expects a file destination")
-
-            all_filepaths.append(annotation_file)
-
-        # TODO: find a better way to get client_container_name
-        # instead of request backend again (generated while create dataset)
-        container_name: dict = api.get_dataset(dataset_data["id"])[
-            "client_container_name"
-        ]
+        for path in paths:
+            all_filepaths.extend(get_filepaths(path))
+        return all_filepaths
+
+
+class AsyncThirdPartyAPI:
+    transport = AsyncHTTPTransport(
+        retries=5,
+    )
 
+    def __init__(self):
+        self.client = AsyncClient(transport=self.transport, timeout=Timeout(5))
+
+    async def async_send_request(self, url: str, method: str, **kwargs) -> Response:
         try:
-            batch_size = 5
-            for i in range(0, len(all_filepaths), batch_size):
-                file_dict: dict[str, bytes] = {
-                    fpath: open(fpath, "rb").read()
-                    for fpath in all_filepaths[i : i + batch_size]
-                }
+            resp: Response = await self.client.request(method=method, url=url, **kwargs)
 
-                api.upload_files(
-                    dataset_id=dataset_data["id"],
-                    container_name=container_name,
-                    file_dict=file_dict,
-                    is_finished=False,
-                )
+        except Exception:
+            logging.exception("async send request error")
 
-            # request finished status to backend
-            api.upload_files(
-                dataset_id=dataset_data["id"],
-                container_name=container_name,
-                is_finished=True,
-                file_dict=dict(),
+        if not 200 <= resp.status_code <= 299:
+            raise Exception(
+                f"status code: {resp.status_code}, response detail: {resp.content}"
             )
-        except Exception as e:
-            raise ClientConnectionError(f"failed to upload files: {e}")
 
-        return Dataset(**dataset_data, client_alias=client_alias)
+        return resp
+
+    async def upload_file(
+        self, method: str, target_url: str, file: bytes, content_type: str
+    ):
+        await self.async_send_request(
+            method=method,
+            url=target_url,
+            content=file,
+            headers={"Content-Type": content_type},
+        )
```

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk/connections.py` & `dataverse_sdk-1.2.1/dataverse_sdk/connections.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk/constants.py` & `dataverse_sdk-1.2.1/dataverse_sdk/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 class BaseEnumMeta(EnumMeta):
     _value_set: Optional[set[Any]] = None
 
     def __contains__(cls, item):
         if cls._value_set is None:
             cls._value_set: set[Any] = {v.value for v in cls.__members__.values()}
-
         return item in cls._value_set
 
 
 class DataverseHost(str, Enum, metaclass=BaseEnumMeta):
-    DEV = "https://dev.dataverse-dev.linkervision.ai"
-    DEV2 = "https://dev2.dataverse-dev.linkervision.ai"
-    DEV3 = "https://dev3.dataverse-dev.linkervision.ai"
-    STAGING = "https://staging.dataverse-dev.linkervision.ai"
-    DEMO = "https://demo.dataverse-dev.linkervision.ai"
+    DEV = "https://dev.dataverse.linkervision.ai"
+    DEV2 = "https://dev2.dataverse.linkervision.ai"
+    DEV3 = "https://dev3.dataverse.linkervision.ai"
+    STAGING = "https://staging.dataverse.linkervision.ai"
+    DEMO = "https://demo.dataverse.linkervision.ai"
     PRODUCTION = "https://dataverse.linkervision.ai"
     LOCAL = "http://localhost:8000"
```

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk/schemas/api.py` & `dataverse_sdk-1.2.1/dataverse_sdk/schemas/api.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk/schemas/client.py` & `dataverse_sdk-1.2.1/dataverse_sdk/schemas/client.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk/schemas/common.py` & `dataverse_sdk-1.2.1/dataverse_sdk/schemas/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     NUMBER = "number"
     TEXT = "text"
 
 
 class OntologyImageType(str, Enum, metaclass=BaseEnumMeta):
     _2D_BOUNDING_BOX = "2d_bounding_box"
     SEMANTIC_SEGMENTATION = "semantic_segmentation"
+    INSTANCE_SEGMENTATION = "instance_segmentation"
     CLASSIFICATION = "classification"
     POINT = "point"
     POLYGON = "polygon"
     POLYLINE = "polyline"
 
 
 class OntologyPcdType(str, Enum, metaclass=BaseEnumMeta):
@@ -47,8 +48,7 @@
     READY = "ready"
 
 
 class DataSource(str, Enum, metaclass=BaseEnumMeta):
     Azure = "azure"
     AWS = "aws"
     SDK = "sdk"
-    LOCAL = "local"
```

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk/utils/utils.py` & `dataverse_sdk-1.2.1/dataverse_sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk.egg-info/PKG-INFO` & `dataverse_sdk-1.2.1/dataverse_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 1.1.0
+Version: 1.2.1
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
 Requires-Dist: requests
+Requires-Dist: httpx>=0.23.0
 
 # Dataverse SDK For Python
 Dataverse is a MLOPs platform for assisting in data selection, data visualization and model training in computer vision.
 Use Dataverse-SDK for Python to help you to interact with the Dataverse platform by Python. Currently, the library supports:
   - Create Project with your input ontology and sensors
   - Get Project by project-id
   - Create Dataset from your AWS/Azure storage or local
@@ -37,15 +38,15 @@
 
 Interaction with the Dataverse site starts with an instance of the `DataverseClient` class. You need site url, an email-account and its password to instantiate the client object.
 
 ```Python
 from dataverse_sdk import *
 from dataverse_sdk.connections import get_connection
 client = DataverseClient(
-    host=DataverseHost.PRODUCTION, email="XXX", password="***", alias="default", force = False,
+    host=DataverseHost.PRODUCTION, email="XXX", password="***", alias="default", force = False, service_id="xxxx-xxxx-xx-xxx"
 )
 assert client is get_connection()
 
 # Should provide different alias if you are trying to connect to different workspaces
 client2 = DataverseClient(
     host=DataverseHost.PRODUCTION, email="account-2", password="***", alias="client2", force = False,
 )
@@ -373,8 +374,8 @@
 
 ## Contributing
 
 
 
 ## Links to language repos
 
-[Python Readme](https://github.com/linkernetworks/dataverse-sdk/tree/develop/python/README.md)
+[Python Readme](https://github.com/linkernetworks/dataverse-sdk/tree/master/python/README.md)
```

### Comparing `dataverse-sdk-1.1.0/dataverse_sdk.egg-info/SOURCES.txt` & `dataverse_sdk-1.2.1/dataverse_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-1.1.0/setup.py` & `dataverse_sdk-1.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "dataverse-sdk"
-PACKAGE_VERSION = "1.1.0"
+PACKAGE_VERSION = "1.2.1"
 DESC = "Dataverse SDK For Python"
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
     packages=find_packages(),
-    python_requires=">=3.9, <4",
+    python_requires=">=3.10, <4",
     author=AUTHOR,
     url="",
     description=DESC,
-    install_requires=["pydantic==1.*", "requests"],
+    install_requires=["pydantic==1.*", "requests", "httpx>=0.23.0"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=["Programming Language :: Python :: 3"],
 )
```

