# Comparing `tmp/aiosalesforce-0.6.0.tar.gz` & `tmp/aiosalesforce-0.6.1.tar.gz`

## Comparing `aiosalesforce-0.6.0.tar` & `aiosalesforce-0.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/__init__.py
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/client.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/py.typed
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/sobject.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/utils.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/__init__.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/base.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/client_credentials_flow.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/jwt_bearer_flow.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/soap.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/__init__.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/_csv.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/client.py
--rw-r--r--   0        0        0    13848 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/ingest.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/__init__.py
--rw-r--r--   0        0        0    16130 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/batch.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/client.py
--rw-r--r--   0        0        0    18342 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/composite.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/exceptions.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/events/__init__.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/events/event_bus.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/events/events.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/retries/__init__.py
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/retries/policy.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/retries/rules.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/LICENSE
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/README.md
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/__init__.py
+-rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/client.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/py.typed
+-rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/sobject.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/utils.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/auth/__init__.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/auth/base.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/auth/client_credentials_flow.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/auth/jwt_bearer_flow.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/auth/soap.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/bulk/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/bulk/v2/__init__.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/bulk/v2/_csv.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/bulk/v2/client.py
+-rw-r--r--   0        0        0    13848 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/bulk/v2/ingest.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/composite/__init__.py
+-rw-r--r--   0        0        0    16274 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/composite/batch.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/composite/client.py
+-rw-r--r--   0        0        0    18486 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/composite/composite.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/composite/exceptions.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/events/__init__.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/events/event_bus.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/events/events.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/retries/__init__.py
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/retries/policy.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/src/aiosalesforce/retries/rules.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/README.md
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 aiosalesforce-0.6.1/PKG-INFO
```

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/__init__.py` & `aiosalesforce-0.6.1/src/aiosalesforce/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 __all__ = [
     "ClientCredentialsFlow",
     "JwtBearerFlow",
     "SoapLogin",
     "Salesforce",
     "BulkApiBatchConsumptionEvent",
```

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/client.py` & `aiosalesforce-0.6.1/src/aiosalesforce/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,14 +243,29 @@
 
         Use this client to perform CRUD operations on individual sObjects.
 
         """
         return SobjectClient(self)
 
     @cached_property
+    def composite(self) -> CompositeClient:
+        """
+        Salesforce REST API composite client.
+
+        Use this client to perform composite operations:
+        * Composite Batch
+        * Composite
+        * Composite Graph
+        * sObject Tree
+        * sObject Collections
+
+        """
+        return CompositeClient(self)
+
+    @cached_property
     def bulk_v1(self) -> NoReturn:
         """
         Salesforce Bulk API 1.0 client.
 
         Use this client to execute bulk ingest and query operations.
 
         """
@@ -261,21 +276,7 @@
         """
         Salesforce Bulk API 2.0 client.
 
         Use this client to execute bulk ingest and query operations.
 
         """
         return BulkClientV2(self)
-
-    @cached_property
-    def composite(self) -> CompositeClient:
-        """
-        Salesforce REST API composite client.
-
-        Use this client to perform composite operations:
-        * Composite Batch
-        * Composite
-        * Composite Graph
-        * sObject Tree
-
-        """
-        return CompositeClient(self)
```

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/exceptions.py` & `aiosalesforce-0.6.1/src/aiosalesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/sobject.py` & `aiosalesforce-0.6.1/src/aiosalesforce/sobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,25 +225,28 @@
         UpsertResponse
             Dataclass with 'id' and 'created' fields.
 
         """
         if validate:
             if isinstance(data, (str, bytes, bytearray)):
                 data = json_loads(data)
+            else:
+                # Copy payload to avoid mutating the original
+                data = json_loads(json_dumps(data))
             if not isinstance(data, dict):
                 raise TypeError(
                     f"data must be a dict, str, bytes, or bytearray, "
                     f"got {type(data).__name__}"
                 )
             try:
-                if data[external_id_field] != id_:
+                if str(data[external_id_field]) != str(id_):
                     raise ValueError(
                         f"External ID field '{external_id_field}' in data "
                         f"{data[external_id_field]} does not match "
-                        f"the provided external id {id_}"
+                        f"the provided external id '{id_}'"
                     )
                 data.pop(external_id_field)
             except KeyError:
                 pass
 
         response = await self.salesforce_client.request(
             "PATCH",
```

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/utils.py` & `aiosalesforce-0.6.1/src/aiosalesforce/utils.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/auth/base.py` & `aiosalesforce-0.6.1/src/aiosalesforce/auth/base.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/auth/client_credentials_flow.py` & `aiosalesforce-0.6.1/src/aiosalesforce/auth/client_credentials_flow.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/auth/jwt_bearer_flow.py` & `aiosalesforce-0.6.1/src/aiosalesforce/auth/jwt_bearer_flow.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/auth/soap.py` & `aiosalesforce-0.6.1/src/aiosalesforce/auth/soap.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/_csv.py` & `aiosalesforce-0.6.1/src/aiosalesforce/bulk/v2/_csv.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/client.py` & `aiosalesforce-0.6.1/src/aiosalesforce/bulk/v2/client.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/ingest.py` & `aiosalesforce-0.6.1/src/aiosalesforce/bulk/v2/ingest.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/composite/batch.py` & `aiosalesforce-0.6.1/src/aiosalesforce/composite/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,25 +372,28 @@
             Upsert subrequest.
             Exposes 'id' and 'created' properties.
 
         """
         if validate:
             if isinstance(data, (str, bytes, bytearray)):
                 data = json_loads(data)
+            else:
+                # Copy payload to avoid mutating the original
+                data = json_loads(json_dumps(data))
             if not isinstance(data, dict):
                 raise TypeError(
                     f"data must be a dict, str, bytes, or bytearray, "
                     f"got {type(data).__name__}"
                 )
             try:
-                if data[external_id_field] != id_:
+                if str(data[external_id_field]) != str(id_):
                     raise ValueError(
                         f"External ID field '{external_id_field}' in data "
                         f"{data[external_id_field]} does not match "
-                        f"the provided external id {id_}"
+                        f"the provided external id '{id_}'"
                     )
                 data.pop(external_id_field)
             except KeyError:
                 pass
 
         subrequest = SobjectUpsertSubrequest(
             "PATCH",
```

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/composite/client.py` & `aiosalesforce-0.6.1/src/aiosalesforce/composite/client.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/composite/composite.py` & `aiosalesforce-0.6.1/src/aiosalesforce/composite/composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,25 +433,28 @@
             Upsert subrequest.
             Exposes 'id' and 'created' properties.
 
         """
         if validate:
             if isinstance(data, (str, bytes, bytearray)):
                 data = json_loads(data)
+            else:
+                # Copy payload to avoid mutating the original
+                data = json_loads(json_dumps(data))
             if not isinstance(data, dict):
                 raise TypeError(
                     f"data must be a dict, str, bytes, or bytearray, "
                     f"got {type(data).__name__}"
                 )
             try:
-                if data[external_id_field] != id_:
+                if str(data[external_id_field]) != str(id_):
                     raise ValueError(
                         f"External ID field '{external_id_field}' in data "
                         f"{data[external_id_field]} does not match "
-                        f"the provided external id {id_}"
+                        f"the provided external id '{id_}'"
                     )
                 data.pop(external_id_field)
             except KeyError:
                 pass
 
         subrequest = SobjectUpsertSubrequest(
             self.composite_request.get_reference_id(f"{sobject}_upsert"),
```

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/events/event_bus.py` & `aiosalesforce-0.6.1/src/aiosalesforce/events/event_bus.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/events/events.py` & `aiosalesforce-0.6.1/src/aiosalesforce/events/events.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/retries/__init__.py` & `aiosalesforce-0.6.1/src/aiosalesforce/retries/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/retries/policy.py` & `aiosalesforce-0.6.1/src/aiosalesforce/retries/policy.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/src/aiosalesforce/retries/rules.py` & `aiosalesforce-0.6.1/src/aiosalesforce/retries/rules.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/LICENSE` & `aiosalesforce-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/pyproject.toml` & `aiosalesforce-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.6.0/PKG-INFO` & `aiosalesforce-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aiosalesforce
-Version: 0.6.0
+Version: 0.6.1
 Summary: Salesforce REST API client
 Project-URL: Homepage, https://github.com/georgebv/aiosalesforce
 Project-URL: Documentation, https://github.com/georgebv/aiosalesforce
 Project-URL: Repository, https://github.com/georgebv/aiosalesforce
 Author-email: Georgii Bocharov <bocharovgeorgii@gmail.com>
 License: Copyright 2024 Georgii Bocharov
         
@@ -73,14 +73,28 @@
   staying idiomatic to Python :snake:
 - **Salesforce first:** built with years of experience working with the Salesforce API
   it is configured to work out of the box and incorporates best practices and
   latest Salesforce API features :cloud:
 - **Track your API usage:** built-in support for tracking Salesforce API usage
   :chart_with_upwards_trend:
 
+Supported APIs:
+
+| API                 | Status | Description                              |
+| ------------------- | ------ | ---------------------------------------- |
+| SOQL Query          | ✅     | Execute SOQL queries                     |
+| sObject             | ✅     | CRUD operations on Salesforce objects    |
+| Composite Batch     | ✅     | Execute multiple independent subrequests |
+| Composite           | ✅     | Execute multiple dependent subrequests   |
+| Composite Graph     | 🕒     | Execute multiple composite graphs        |
+| sObject Tree        | 🕒     | Create one or more sObject trees         |
+| sObject Collections | 🕒     | Execute multiple sObject operations      |
+| Bulk API 1.0        | ❌     | Not planned (use Bulk API 2.0)           |
+| Bulk API 2.0        | ✅     | Bulk ingest and query operations         |
+
 ## Requirements
 
 `aiosalesforce` depends on:
 
 - Python 3.11+
 - [httpx](https://github.com/encode/httpx)
 - [orjson](https://github.com/ijl/orjson)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: aiosalesforce Version: 0.6.0 Summary: Salesforce
+Metadata-Version: 2.3 Name: aiosalesforce Version: 0.6.1 Summary: Salesforce
 REST API client Project-URL: Homepage, https://github.com/georgebv/
 aiosalesforce Project-URL: Documentation, https://github.com/georgebv/
 aiosalesforce Project-URL: Repository, https://github.com/georgebv/
 aiosalesforce Author-email: Georgii Bocharov
 gmail.com> License: Copyright 2024 Georgii Bocharov Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
@@ -36,29 +36,37 @@
 flexible and robust retrying configuration :gear: - **Fully typed:** every part
 of the library is fully typed and annotated :label: - **Intuitive:** API
 follows naming conventions of Salesforce's APIs while staying idiomatic to
 Python :snake: - **Salesforce first:** built with years of experience working
 with the Salesforce API it is configured to work out of the box and
 incorporates best practices and latest Salesforce API features :cloud: -
 **Track your API usage:** built-in support for tracking Salesforce API usage :
-chart_with_upwards_trend: ## Requirements `aiosalesforce` depends on: - Python
-3.11+ - [httpx](https://github.com/encode/httpx) - [orjson](https://github.com/
-ijl/orjson) Optional dependencies: - [PyJWT](https://github.com/jpadilla/pyjwt)
-- [cryptography](https://github.com/pyca/cryptography) ## Installation ```shell
-pip install aiosalesforce ``` To use the JWT Bearer Flow authentication install
-with the `jwt` extra: ```shell pip install aiosalesforce[jwt] ``` # Demo
-Example below shows how to: - Authenticate against Salesforce using the SOAP
-login method - Create a Salesforce client - Create a new Contact - Read a
-Contact by ID - Execute a SOQL query ```python import asyncio from
-aiosalesforce import Salesforce from aiosalesforce.auth import SoapLogin from
-httpx import AsyncClient # Reuse authentication session across multiple clients
-(refreshes automatically) auth = SoapLogin( username="your-username",
-password="your-password", security_token="your-security-token", ) async def
-main(): async with AsyncClient() as client: # Create a Salesforce client
-salesforce = Salesforce( client, base_url="https://your-
-instance.my.salesforce.com", auth=auth, ) # Create a new Contact contact_id =
-await salesforce.sobject.create( "Contact", { "FirstName": "John", "LastName":
-"Doe", "Email": "john.doe@example.com", }, ) print(f"Created Contact with ID:
-{contact_id}") # Read Contact by ID contact = await salesforce.sobject.get
-("Contact", contact_id) print(contact) # Execute a SOQL query async for record
-in salesforce.query("SELECT Id, Name FROM Contact"): print(record) if __name__
-== "__main__": asyncio.run(main()) ```
+chart_with_upwards_trend: Supported APIs: | API | Status | Description | | ----
+--------------- | ------ | ---------------------------------------- | | SOQL
+Query | â | Execute SOQL queries | | sObject | â | CRUD operations on
+Salesforce objects | | Composite Batch | â | Execute multiple independent
+subrequests | | Composite | â | Execute multiple dependent subrequests | |
+Composite Graph | ð | Execute multiple composite graphs | | sObject Tree |
+ð | Create one or more sObject trees | | sObject Collections | ð |
+Execute multiple sObject operations | | Bulk API 1.0 | â | Not planned (use
+Bulk API 2.0) | | Bulk API 2.0 | â | Bulk ingest and query operations | ##
+Requirements `aiosalesforce` depends on: - Python 3.11+ - [httpx](https://
+github.com/encode/httpx) - [orjson](https://github.com/ijl/orjson) Optional
+dependencies: - [PyJWT](https://github.com/jpadilla/pyjwt) - [cryptography]
+(https://github.com/pyca/cryptography) ## Installation ```shell pip install
+aiosalesforce ``` To use the JWT Bearer Flow authentication install with the
+`jwt` extra: ```shell pip install aiosalesforce[jwt] ``` # Demo Example below
+shows how to: - Authenticate against Salesforce using the SOAP login method -
+Create a Salesforce client - Create a new Contact - Read a Contact by ID -
+Execute a SOQL query ```python import asyncio from aiosalesforce import
+Salesforce from aiosalesforce.auth import SoapLogin from httpx import
+AsyncClient # Reuse authentication session across multiple clients (refreshes
+automatically) auth = SoapLogin( username="your-username", password="your-
+password", security_token="your-security-token", ) async def main(): async with
+AsyncClient() as client: # Create a Salesforce client salesforce = Salesforce
+( client, base_url="https://your-instance.my.salesforce.com", auth=auth, ) #
+Create a new Contact contact_id = await salesforce.sobject.create( "Contact",
+{ "FirstName": "John", "LastName": "Doe", "Email": "john.doe@example.com", }, )
+print(f"Created Contact with ID: {contact_id}") # Read Contact by ID contact =
+await salesforce.sobject.get("Contact", contact_id) print(contact) # Execute a
+SOQL query async for record in salesforce.query("SELECT Id, Name FROM
+Contact"): print(record) if __name__ == "__main__": asyncio.run(main()) ```
```

