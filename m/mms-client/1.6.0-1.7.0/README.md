# Comparing `tmp/mms_client-1.6.0.tar.gz` & `tmp/mms_client-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_client-1.6.0.tar", max compression
+gzip compressed data, was "mms_client-1.7.0.tar", max compression
```

## Comparing `mms_client-1.6.0.tar` & `mms_client-1.7.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1211 2024-05-08 04:45:03.930758 mms_client-1.6.0/LICENSE
--rw-r--r--   0        0        0    14741 2024-05-08 04:45:03.930758 mms_client-1.6.0/README.md
--rw-r--r--   0        0        0     2913 2024-05-08 04:45:03.930758 mms_client-1.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 04:45:03.930758 mms_client-1.6.0/src/mms_client/__init__.py
--rw-r--r--   0        0        0      676 2024-05-08 04:45:03.930758 mms_client-1.6.0/src/mms_client/client.py
--rw-r--r--   0        0        0        0 2024-05-08 04:45:03.930758 mms_client-1.6.0/src/mms_client/py.typed
--rw-r--r--   0        0        0    10702 2024-05-08 04:45:03.930758 mms_client-1.6.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
--rw-r--r--   0        0        0     9894 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
--rw-r--r--   0        0        0   109679 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/mi-market.xsd
--rw-r--r--   0        0        0    76166 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
--rw-r--r--   0        0        0    13276 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/mi-report.xsd
--rw-r--r--   0        0        0    69149 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/mpr.xsd
--rw-r--r--   0        0        0    31524 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/omi.xsd
--rw-r--r--   0        0        0        0 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/security/__init__.py
--rw-r--r--   0        0        0     1489 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/security/certs.py
--rw-r--r--   0        0        0     2149 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/security/crypto.py
--rw-r--r--   0        0        0        0 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/__init__.py
--rw-r--r--   0        0        0    26309 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/base.py
--rw-r--r--   0        0        0     9031 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/market.py
--rw-r--r--   0        0        0      626 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/omi.py
--rw-r--r--   0        0        0     3815 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/registration.py
--rw-r--r--   0        0        0      642 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/report.py
--rw-r--r--   0        0        0        0 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/__init__.py
--rw-r--r--   0        0        0    14139 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/award.py
--rw-r--r--   0        0        0     9710 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/base.py
--rw-r--r--   0        0        0     1629 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/enums.py
--rw-r--r--   0        0        0    14785 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/fields.py
--rw-r--r--   0        0        0     2706 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/market.py
--rw-r--r--   0        0        0     6791 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/offer.py
--rw-r--r--   0        0        0     1381 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/registration.py
--rw-r--r--   0        0        0     2667 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/reserve.py
--rw-r--r--   0        0        0    65974 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/resource.py
--rw-r--r--   0        0        0     4399 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/transport.py
--rw-r--r--   0        0        0        0 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/__init__.py
--rw-r--r--   0        0        0     2057 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/auditing.py
--rw-r--r--   0        0        0     3005 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/errors.py
--rw-r--r--   0        0        0    29638 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/serialization.py
--rw-r--r--   0        0        0    10156 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/web.py
--rw-r--r--   0        0        0    16025 1970-01-01 00:00:00.000000 mms_client-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-21 04:45:07.168733 mms_client-1.7.0/LICENSE
+-rw-r--r--   0        0        0    15116 2024-05-21 04:45:07.168733 mms_client-1.7.0/README.md
+-rw-r--r--   0        0        0     2939 2024-05-21 04:45:07.168733 mms_client-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-21 04:45:07.168733 mms_client-1.7.0/src/mms_client/__init__.py
+-rw-r--r--   0        0        0      676 2024-05-21 04:45:07.168733 mms_client-1.7.0/src/mms_client/client.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:45:07.168733 mms_client-1.7.0/src/mms_client/py.typed
+-rw-r--r--   0        0        0    10702 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
+-rw-r--r--   0        0        0     9894 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
+-rw-r--r--   0        0        0   109679 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/schemas/xsd/mi-market.xsd
+-rw-r--r--   0        0        0    76166 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
+-rw-r--r--   0        0        0    13276 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/schemas/xsd/mi-report.xsd
+-rw-r--r--   0        0        0    69149 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/schemas/xsd/mpr.xsd
+-rw-r--r--   0        0        0    31524 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/schemas/xsd/omi.xsd
+-rw-r--r--   0        0        0        0 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/security/__init__.py
+-rw-r--r--   0        0        0     3018 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/security/certs.py
+-rw-r--r--   0        0        0     2345 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/security/crypto.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/services/__init__.py
+-rw-r--r--   0        0        0    27914 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/services/base.py
+-rw-r--r--   0        0        0     9153 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/services/market.py
+-rw-r--r--   0        0        0      626 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/services/omi.py
+-rw-r--r--   0        0        0     3815 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/services/registration.py
+-rw-r--r--   0        0        0      642 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/services/report.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/__init__.py
+-rw-r--r--   0        0        0    14139 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/award.py
+-rw-r--r--   0        0        0     9530 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/base.py
+-rw-r--r--   0        0        0     1629 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/enums.py
+-rw-r--r--   0        0        0    14785 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/fields.py
+-rw-r--r--   0        0        0     2706 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/market.py
+-rw-r--r--   0        0        0     6791 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/offer.py
+-rw-r--r--   0        0        0     1381 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/registration.py
+-rw-r--r--   0        0        0     2667 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/reserve.py
+-rw-r--r--   0        0        0    65974 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/resource.py
+-rw-r--r--   0        0        0     4395 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/types/transport.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/utils/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/utils/auditing.py
+-rw-r--r--   0        0        0     3005 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/utils/errors.py
+-rw-r--r--   0        0        0     8871 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/utils/multipart_transport.py
+-rw-r--r--   0        0        0    30293 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/utils/serialization.py
+-rw-r--r--   0        0        0    10816 2024-05-21 04:45:07.172733 mms_client-1.7.0/src/mms_client/utils/web.py
+-rw-r--r--   0        0        0    16447 1970-01-01 00:00:00.000000 mms_client-1.7.0/PKG-INFO
```

### Comparing `mms_client-1.6.0/LICENSE` & `mms_client-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/README.md` & `mms_client-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 The underlying API sends and receives XML documents. Each of these request or responses, which we will hereafter refer to as *outer* requests and responses, contains metadata about the request/response as well as three fields which are extremely important to successful communication with the API:
 - Attachments data, included as a list of elements with the binary data in a base-64 encoded format
 - Payload data, encoded in a base-64 encoded format
 - Payload signature, which is the SHA256 hash of the payload XML data, then signed with an RSA key, in a base-64 encoded format
 
 After the data has been converted and added to the outer request object, it is sent to the appropriate server endpoint via a Zeep client. The client certificate is also injected into the request using a PCKS12 adaptor.
 
+## Domain
+The domain to use when signing the content ID to MTOM attachments is specified when creating the client. This is not verified by the server, but it is used to generate the content ID for the MTOM attachments. As such, it is important to ensure that the domain is correct.
+
 # Serialization
 This library relies on Pydantic 2 and the pydantic-xml library for serialization/deserialization. As such, any type in this library can be converted to not only XML, but to JSON as well. This is extremely useful if you're trying to build a pass-through API service or something similar.
 
 ## Client Types
 Clients cannot call any and all endpoints in this API, willy-nilly. Some endpoints are restricted to particular clients. At the moment, there are three clients: Balance Service Providers (BSPs), Market Operators (MOs), and Transmission Service Operators (TSOs). Most likely you're operating as a BSP or MO, in which case you'll have access to most or all endpoints. However, it makes little sense for a TSO to be able to submit bids on their own power, so they are restricted to a read-only role in most cases.
 
 Note that MOs and BSPs access the MMS service using the same endpoints, but have distinct permissions. As such, both client types are supported explicitly here.
@@ -106,15 +109,15 @@
 from mms_client.types.offer import Direction, OfferData, OfferStack
 from mms_client.utils.web import ClientType
 
 # Create a certificate
 cert = Certificate("/path/to/my/cert.p12", "fake_passphrase")
 
 # Create a new MMS client
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert)
+client = MmsClient(domain="mydomain.com", participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert)
 
 # Create our request offer
 request_offer = OfferData(
     stack=[
         OfferStack(
             number=1,
             unit_price=100,
@@ -140,22 +143,22 @@
 
 There's a lot of code here but it's not terribly difficult to understand. All this does is pull in the authentication data, create the client, create the payload, submit it to the server and retrieve the response.
 
 ## Connecting to a Test Server
 If you want to test your MMS connection, you can try using the test server:
 
 ```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, test=True)
+client = MmsClient(domain="mydomain.com", participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, test=True)
 ```
 
 ## Connecting as a Market Admin
 If you're connecting as a market operator (MO), you can connect in admin mode:
 
 ```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
+client = MmsClient(domain="mydomain.com", participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
 ```
 
 ## Auditing XML Requests & Responses
 A common requirement for this sort of library is recording or saving the raw XML requests and responses for audit/logging purposes. This library supports this workflow through the `mms_client.utils.auditing.AuditPlugin` object. This object intercepts the XML request at the Zeep client level right before it is sent to the MMS and, similarly, intercepts the XML response immediately after it is received from the MMS. Before passing these objects on, without modifying them, it records the XML data as a byte string and passes it to two methods: `audit_request` and `audit_response`. These can be overridden by any object that inherits from this class, allowing the user to direct this data to whatever store they prefer to use for auditing or logging.
 
 ```python
 class TestAuditPlugin(AuditPlugin):
@@ -166,15 +169,15 @@
 
     def audit_request(self, mms_request: bytes) -> None:
         self.request = mms_request
 
     def audit_response(self, mms_response: bytes) -> None:
         self.response = mms_response
 
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, plugins=[TestAuditPlugin()])
+client = MmsClient(domain="mydomain.com", participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, plugins=[TestAuditPlugin()])
 ```
 
 This same input allows for the user to create their own plugins and add them to the Zeep client, allowing for a certain amount of extensibility.
 
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
 - MarketQuery_ReserveRequirementQuery
```

### Comparing `mms_client-1.6.0/pyproject.toml` & `mms_client-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms_client"
-version = "v1.6.0"
+version = "v1.7.0"
 description = "API client for accessing the MMS"
 authors = ["Ryan Wood <ryan.wood@electroroute.co.jp>"]
 readme = "README.md"
 packages = [{ include = "mms_client", from = "src" }]
 homepage = "https://github.com/ElectroRoute-Japan/mms-client"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -28,14 +28,15 @@
 pydantic = "^2.6.3"
 pendulum = "^3.0.0"
 xmlschema = "^3.0.2"
 cryptography = "^42.0.5"
 pydantic-xml = "^2.9.0"
 lxml = "^5.1.0"
 backoff = "^2.2.1"
+pycryptodomex = "^3.20.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 isort = "^5.13.2"
 mypy = "^1.8.0"
 pylint = "^3.1.0"
 xenon = "^0.9.1"
```

### Comparing `mms_client-1.6.0/src/mms_client/client.py` & `mms_client-1.7.0/src/mms_client/client.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl` & `mms_client-1.7.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl` & `mms_client-1.7.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/schemas/xsd/mi-market.xsd` & `mms_client-1.7.0/src/mms_client/schemas/xsd/mi-market.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd` & `mms_client-1.7.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/schemas/xsd/mi-report.xsd` & `mms_client-1.7.0/src/mms_client/schemas/xsd/mi-report.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/schemas/xsd/mpr.xsd` & `mms_client-1.7.0/src/mms_client/schemas/xsd/mpr.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/schemas/xsd/omi.xsd` & `mms_client-1.7.0/src/mms_client/schemas/xsd/omi.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/services/base.py` & `mms_client-1.7.0/src/mms_client/services/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Contains the client layer for communicating with the MMS server."""
 
+from base64 import b64decode
 from dataclasses import dataclass
 from logging import getLogger
 from typing import Dict
 from typing import Generic
 from typing import List
 from typing import Optional
 from typing import Protocol
@@ -244,35 +245,38 @@
     """Base end-client for the MMS server.
 
     This class is used to communicate with the MMS server.
     """
 
     def __init__(
         self,
+        domain: str,
         participant: str,
         user: str,
         client_type: ClientType,
         cert: Certificate,
         plugins: Optional[List[Plugin]] = None,
         is_admin: bool = False,
         test: bool = False,
     ):
         """Create a new MMS client with the given participant, user, client type, and authentication.
 
         Arguments:
+        domain (str):               The domain to use when signing the content ID to MTOM attachments.
         participant (str):          The MMS code of the business entity to which the requesting user belongs.
         user (str):                 The user name of the person making the request.
         client_type (ClientType):   The type of client to use for making requests to the MMS server.
         cert (Certificate):         The certificate to use for signing requests.
         plugins (List[Plugin]):     A list of plugins to add to the Zeep client. This can be useful for auditing or
                                     other purposes.
         is_admin (bool):            Whether the user is an admin (i.e. is a market operator).
         test (bool):                Whether to use the test server.
         """
         # First, save the base field associated with the client
+        self._domain = domain
         self._participant = participant
         self._user = user
         self._client_type = client_type
         self._is_admin = is_admin
         self._test = test
 
         # Next, save the security-related fields associated with the client
@@ -325,26 +329,31 @@
         Arguments:
         envelope (Envelope):            The payload envelope to submit to the MMS server.
         payload (Payload):              The data to submit to the MMS server.
         config (EndpointConfiguration): The configuration for the endpoint.
 
         Returns:    The response from the MMS server.
         """
+        # Create a new ZWrapper for the given service
+        wrapper = self._get_wrapper(config.service)
+
         # First, create the MMS request from the payload and data.
         logger.debug(
             f"{config.name}: Starting request. Envelope: {type(envelope).__name__}, Data: {type(payload).__name__}",
         )
-        request = self._to_mms_request(config.request_type, config.service.serializer.serialize(envelope, payload))
+        request = self._to_mms_request(
+            wrapper, config.request_type, config.service.serializer.serialize(envelope, payload)
+        )
 
         # Next, submit the request to the MMS server and get and verify the response.
-        resp = self._get_wrapper(config.service).submit(request)
+        resp = wrapper.submit(request)
         self._verify_mms_response(resp, config)
 
         # Now, extract the attachments from the response
-        attachments = {a.name: a.data for a in resp.attachments}
+        attachments = {a.name: b64decode(a.data) for a in resp.attachments}
 
         # Finally, deserialize and verify the response
         envelope_type = config.response_envelope_type or type(envelope)
         data_type = config.response_data_type or type(payload)
         data: Response[E, P] = config.service.serializer.deserialize(resp.payload, envelope_type, data_type)
         self._verify_response(data, config)
 
@@ -365,36 +374,39 @@
         Arguments:
         envelope (Envelope):            The payload envelope to submit to the MMS server.
         payload (Payload):              The data to submit to the MMS server.
         config (EndpointConfiguration): The configuration for the endpoint.
 
         Returns:    The multi-response from the MMS server.
         """
+        # Create a new ZWrapper for the given service
+        wrapper = self._get_wrapper(config.service)
+
         # First, create the MMS request from the payload and data.
         is_list = isinstance(payload, list)
         data_type = type(payload[0]) if is_list else type(payload)  # type: ignore[index]
         logger.debug(
             (
                 f"{config.name}: Starting multi-request. Envelope: {type(envelope).__name__}, "
                 f"Data: {data_type.__name__}"
             ),
         )
         serialized = (
             config.service.serializer.serialize_multi(envelope, payload, data_type)  # type: ignore[arg-type]
             if is_list
             else config.service.serializer.serialize(envelope, payload)  # type: ignore[type-var]
         )
-        request = self._to_mms_request(config.request_type, serialized)
+        request = self._to_mms_request(wrapper, config.request_type, serialized)
 
         # Next, submit the request to the MMS server and get and verify the response.
-        resp = self._get_wrapper(config.service).submit(request)
+        resp = wrapper.submit(request)
         self._verify_mms_response(resp, config)
 
         # Now, extract the attachments from the response
-        attachments = {a.name: a.data for a in resp.attachments}
+        attachments = {a.name: b64decode(a.data) for a in resp.attachments}
 
         # Finally, deserialize and verify the response
         envelope_type = config.response_envelope_type or type(envelope)
         data_type = config.response_data_type or data_type
         data: MultiResponse[E, P] = config.service.serializer.deserialize_multi(
             resp.payload,
             envelope_type,
@@ -406,54 +418,79 @@
         logger.debug(
             f"{config.name}: Returning multi-response. Envelope: {envelope_type.__name__}, Data: {data_type.__name__}",
         )
         return data, attachments
 
     def _to_mms_request(
         self,
+        client: ZWrapper,
         req_type: RequestType,
         data: bytes,
         return_req: bool = False,
         attachments: Optional[Dict[str, bytes]] = None,
     ) -> MmsRequest:
         """Convert the given data to an MMS request.
 
         Arguments:
+        client (ZWrapper):              The Zeep client to use for submitting the request.
         req_type (RequestType):         The type of request to submit to the MMS server.
         data (bytes):                   The data to submit to the MMS server.
         return_req (bool):              Whether to return the request data in the response. This is False by default.
         attachments (Dict[str, bytes]): The attachments to send with the request.
 
         Arguments:    The MMS request to submit to the MMS server.
         """
-        # Convert the attachments to the correct the MMS format
+        # First, convert the attachments to the correct the MMS format
         attachment_data = (
-            [
-                Attachment(signature=self._signer.sign(data), name=name, binaryData=data)
-                for name, data in attachments.items()
-            ]
-            if attachments
-            else []
+            [self._to_mms_attachment(client, name, data) for name, data in attachments.items()] if attachments else []
         )
 
+        # Next, convert the payload to a base-64 string
+        tag, signature = self._register_and_sign(client, "payload", data)
+
         # Embed the data and the attachments in the MMS request and return it
         logger.debug(
             f"Creating MMS request of type {req_type.name} to send {len(data)} bytes of data and "
             f"{len(attachment_data)} attachments."
         )
         return MmsRequest(
             requestType=req_type,
             adminRole=self._is_admin,
             requestDataType=RequestDataType.XML,
             sendRequestDataOnSuccess=return_req,
-            requestSignature=self._signer.sign(data),
-            requestData=data,
+            requestSignature=signature,
+            requestData=tag,
             attachmentData=attachment_data,
         )
 
+    def _to_mms_attachment(self, client: ZWrapper, name: str, data: bytes) -> Attachment:  # pragma: no cover
+        """Convert the given data to an MMS attachment.
+
+        Arguments:
+        client (ZWrapper):  The Zeep client to use for submitting the request.
+        name (str):         The name of the attachment.
+        data (bytes):       The data to be attached.
+
+        Returns:    The MMS attachment.
+        """
+        # Convert the data to a base-64 string
+        tag, signature = self._register_and_sign(client, name, data)
+
+        # Create the MMS attachment and return it
+        return Attachment(signature=signature, name=name, binaryData=tag)
+
+    def _register_and_sign(self, client: ZWrapper, name: str, data: bytes) -> Tuple[str, str]:
+        tag = client.register_attachment(name, data)
+
+        # Next, sign the data
+        signature = self._signer.sign(data)
+
+        # Finally, convert the encoded data to a string and return it and the signature
+        return tag, signature.decode("UTF-8")
+
     def _verify_mms_response(self, resp: MmsResponse, config: EndpointConfiguration) -> None:
         """Verify that the given MMS response is valid.
 
         Arguments:
         resp (MmsResponse):     The MMS response to verify.
 
         Raises:
@@ -593,14 +630,15 @@
 
         Arguments:
         service (ServiceConfiguration):  The service for which to get the wrapper.
         """
         if service.interface not in self._wrappers:
             logger.debug(f"Creating wrapper for {service.interface.name} interface.")
             self._wrappers[service.interface] = ZWrapper(
+                self._domain,
                 self._client_type,
                 service.interface,
                 self._cert.to_adapter(),
                 self._plugins,
                 True,
                 self._test,
             )
```

### Comparing `mms_client-1.6.0/src/mms_client/services/market.py` & `mms_client-1.7.0/src/mms_client/services/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,33 +40,34 @@
         "MarketQuery_ReserveRequirementQuery",
         config,
         RequestType.INFO,
         resp_envelope_type=MarketSubmit,
         resp_data_type=ReserveRequirement,
     )
     def query_reserve_requirements(
-        self: ClientProto, request: ReserveRequirementQuery, date: Optional[Date] = None
+        self: ClientProto, request: ReserveRequirementQuery, days: int, date: Optional[Date] = None
     ) -> List[ReserveRequirement]:
         """Query the MMS server for reserve requirements.
 
         This endpoint is accessible to all client types.
 
         Arguments:
         request (ReserveRequirementQuery):  The query to submit to the MMS server.
         date (Date):                        The date of the transaction in the format "YYYY-MM-DD". This value defaults
                                             to the current date.
+        days (int):                         The number of days ahead for which the data is being queried.
 
         Returns:    A list of reserve requirements that match the query.
         """
         # NOTE: The return type does not match the method definition but the decorator will return the correct type
         return MarketQuery(  # type: ignore[return-value]
             date=date or Date.today(),
             participant=self.participant,
             user=self.user,
-            days=1,
+            days=days,
         )
 
     @mms_endpoint("MarketSubmit_OfferData", config, RequestType.INFO, [ClientType.BSP])
     def put_offer(
         self: ClientProto, request: OfferData, market_type: MarketType, days: int, date: Optional[Date] = None
     ) -> OfferData:
         """Submit an offer to the MMS server.
@@ -163,15 +164,15 @@
             date=date or Date.today(),
             participant=self.participant,
             user=self.user,
             market_type=market_type,
             days=days,
         )
 
-    @mms_endpoint("MarketQuery_AwardResultsQuery", config, RequestType.INFO, resp_data_type=AwardResponse)
+    @mms_endpoint("MarketQuery_AwardResultsQuery", config, RequestType.MARKET, resp_data_type=AwardResponse)
     def query_awards(self: ClientProto, request: AwardQuery, days: int, date: Optional[Date] = None) -> AwardResponse:
         """Query the MMS server for award results.
 
         This endpoint is accessible to all client types.
 
         If no values are specified for Area, Associated Area, Power Generation Unit Code, or GC Registration Flag,
         the results for all areas will be retrieved. If one or more of these criteria are specified, the results will
```

### Comparing `mms_client-1.6.0/src/mms_client/services/omi.py` & `mms_client-1.7.0/src/mms_client/services/omi.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/services/registration.py` & `mms_client-1.7.0/src/mms_client/services/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/services/report.py` & `mms_client-1.7.0/src/mms_client/services/report.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/types/award.py` & `mms_client-1.7.0/src/mms_client/types/award.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/types/base.py` & `mms_client-1.7.0/src/mms_client/types/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,20 +111,17 @@
 
     MARKET = "mi-market.xsd"
     REPORT = "mi-report.xsd"
     REGISTRATION = "mpr.xsd"
     OMI = "omi.xsd"
 
 
-class PayloadBase(BaseXmlModel, nsmap={"xsi": "http://www.w3.org/2001/XMLSchema-instance"}):
+class PayloadBase(BaseXmlModel):
     """Represents the base fields for an MMS request payload."""
 
-    # The XML schema to use for validation
-    location: SchemaType = attr(name="noNamespaceSchemaLocation", ns="xsi")
-
 
 class BaseResponse(BaseXmlModel, Generic[E], tag="BaseResponse"):
     """Contains the base data extracted from the MMS response in a format we can use."""
 
     # The processing statistics returned with the payload. This will not be present in requests, and will be populated
     # in responses.
     statistics: ProcessingStatistics = element(tag="ProcessingStatistics")
```

### Comparing `mms_client-1.6.0/src/mms_client/types/enums.py` & `mms_client-1.7.0/src/mms_client/types/enums.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/types/fields.py` & `mms_client-1.7.0/src/mms_client/types/fields.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/types/market.py` & `mms_client-1.7.0/src/mms_client/types/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/types/offer.py` & `mms_client-1.7.0/src/mms_client/types/offer.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/types/registration.py` & `mms_client-1.7.0/src/mms_client/types/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/types/reserve.py` & `mms_client-1.7.0/src/mms_client/types/reserve.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/types/resource.py` & `mms_client-1.7.0/src/mms_client/types/resource.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/types/transport.py` & `mms_client-1.7.0/src/mms_client/types/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     # The signature used to encrypt the attachment
     signature: str = Field(alias="signature")
 
     # The name of the attachment file
     name: str = Field(alias="name")
 
     # The attachment file data
-    data: bytes = Field(alias="binaryData")
+    data: str = Field(alias="binaryData")
 
 
 class MmsRequest(BaseModel):
     """Base class for all MMS requests."""
 
     # The API subsystem to which the request is sent.
     subsystem: RequestType = Field(alias="requestType")
@@ -79,15 +79,15 @@
     # Wether the response data should be compressed (for future use only)
     response_compressed: bool = Field(default=False, alias="sendResponseDataCompressed")
 
     # The signature used to encrypt the request payload
     signature: str = Field(alias="requestSignature")
 
     # The base-64 encoded payload of the request
-    payload: bytes = Field(alias="requestData")
+    payload: str = Field(alias="requestData")
 
     # Any attached files to be sent with the request. Only 20 of these are allowed for OMI requests. For MI requests,
     # the limit is 40.
     attachments: List[Attachment] = Field(default=[], alias="attachmentData")
 
     def to_arguments(self) -> dict:
         """Convert the request to a dictionary of arguments for use in the MMS client."""
```

### Comparing `mms_client-1.6.0/src/mms_client/utils/auditing.py` & `mms_client-1.7.0/src/mms_client/utils/auditing.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/utils/errors.py` & `mms_client-1.7.0/src/mms_client/utils/errors.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.6.0/src/mms_client/utils/serialization.py` & `mms_client-1.7.0/src/mms_client/utils/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         # Next, inject the payload and data into the payload class
         # NOTE: this returns a type that inherits from PayloadBase and the arguments provided to the initializer
         # here are correct, but mypy thinks they are incorrect because it doesn't understand the the inherited type
         payload = payload_cls(request_envelope, request_data, self._xsd.value)  # type: ignore[call-arg, misc]
 
         # Finally, convert the payload to XML and return it
         # NOTE: we provided the encoding here so this will return bytes, not a string
-        return payload.to_xml(skip_empty=True, encoding="utf-8", xml_declaration=True)  # type: ignore[return-value]
+        return self._to_canoncialized_xml(payload)
 
     def serialize_multi(self, request_envelope: E, request_data: List[P], request_type: Type[P]) -> bytes:
         """Serialize the envelope and data to a byte string for sending to the MMS server.
 
         Arguments:
         request_envelope (Envelope):    The envelope to be serialized.
         request_data (List[Payload]):    The data to be serialized.
@@ -100,15 +100,15 @@
         # Next, inject the payload and data into the payload class
         # NOTE: this returns a type that inherits from PayloadBase and the arguments provided to the initializer
         # here are correct, but mypy thinks they are incorrect because it doesn't understand the the inherited type
         payload = payload_cls(request_envelope, request_data, self._xsd.value)  # type: ignore[call-arg, misc]
 
         # Finally, convert the payload to XML and return it
         # NOTE: we provided the encoding here so this will return bytes, not a string
-        return payload.to_xml(skip_empty=True, encoding="utf-8", xml_declaration=True)  # type: ignore[return-value]
+        return self._to_canoncialized_xml(payload)
 
     def deserialize(self, data: bytes, envelope_type: Type[E], data_type: Type[P]) -> Response[E, P]:
         """Deserialize the data to a response object.
 
         Arguments:
         data (bytes):                   The raw data to be deserialized.
         envelope_type (Type[Envelope]): The type of envelope to be constructed.
@@ -128,14 +128,38 @@
         data_type (Type[Payload]):      The type of data to be constructed.
 
         Returns:    A multi-response object containing the envelope and data extracted from the raw data.
         """
         tree = self._from_xml(data)
         return self._from_tree_multi(tree, envelope_type, data_type)
 
+    def _to_canoncialized_xml(self, payload: PayloadBase) -> bytes:
+        """Convert the payload to a canonicalized XML string.
+
+        Arguments:
+        payload (PayloadBase): The payload to be converted.
+
+        Returns:    The canonicalized XML string.
+        """
+        # First, convert the payload to a raw XML string
+        raw: bytes = payload.to_xml(
+            skip_empty=True,
+            encoding="utf-8",
+            xml_declaration=False,
+        )  # type: ignore[assignment]
+
+        # Next, parse it back into an XML tree
+        unparsed = parse(BytesIO(raw))
+
+        # Finally, convert the XML tree to a canonicalized XML string and return it
+        buffer = BytesIO()
+        unparsed.write_c14n(buffer)
+        buffer.seek(0)
+        return buffer.read()
+
     def _from_tree(self, raw: Element, envelope_type: Type[E], data_type: Type[P]) -> Response[E, P]:
         """Convert the raw data to a response object.
 
         Arguments:
         raw (Element):                  The raw data to be converted.
         envelope_type (Type[Envelope]): The type of envelope to be constructed.
         data_type (Type[Payload]):      The type of data to be constructed.
```

### Comparing `mms_client-1.6.0/src/mms_client/utils/web.py` & `mms_client-1.7.0/src/mms_client/utils/web.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 from backoff import expo
 from backoff import on_exception
 from requests import Session
 from requests_pkcs12 import Pkcs12Adapter
 from zeep import Client
 from zeep import Plugin
-from zeep import Transport
 from zeep.cache import SqliteCache
 from zeep.exceptions import TransportError
 from zeep.xsd.valueobjects import CompoundValue
 
 from mms_client.types.transport import MmsRequest
 from mms_client.types.transport import MmsResponse
+from mms_client.utils.multipart_transport import MultipartTransport
 
 # Set the default logger for the MMS client
 logger = getLogger(__name__)
 
 
 class ClientType(StrEnum):
     """Identifies the type of client to use.
@@ -130,24 +130,26 @@
     Note that this is the lowest layer of the client, and is only responsible for handing off the final request to the
     Zeep client. This class is meant to be used by the higher-level client classes that take in the actual request and
     return the actual response.
     """
 
     def __init__(
         self,
+        domain: str,
         client: ClientType,
         interface: Interface,
         adapter: Pkcs12Adapter,
         plugins: Optional[List[Plugin]] = None,
         cache: bool = True,
         test: bool = False,
     ):
         """Create a new Zeep wrapper object for a specific MMS service endpoint.
 
         Arguments:
+        domain (str):               The domain to use when signing the content ID to MTOM attachments.
         client (ClientType):        The type of client to use. This can be either "bsp" (Balancing Service Provider) or
                                     "tso" (Transmission System Operator). This will determine which service endpoint to
                                     use.
         interface (Interface):      The type of interface to use. This can be either "omi" (Other Market Initiator) or
                                     "mi" (Market Initiator). This will determine which service endpoint to use as well
                                     as the service and port to use.
         adapter (Pkcs12Adapter):    The PKCS12 adapter containing the certificate and private key to use for
@@ -187,21 +189,33 @@
         sess = Session()
         sess.mount(self._endpoint.selected, adapter)
         if not test:
             sess.mount(self._endpoint.backup, adapter)
 
         # Finally, we create the Zeep client with the given WSDL file location, session, and cache settings and then,
         # from that client, we create the SOAP service with the given service binding and selected endpoint.
+        self._transport = MultipartTransport(domain, cache=SqliteCache() if cache else None, session=sess)
         self._client = Client(
             wsdl=str(location.resolve()),
-            transport=Transport(cache=SqliteCache() if cache else None, session=sess),
+            transport=self._transport,
             plugins=plugins,
         )
         self._create_service()
 
+    def register_attachment(self, name: str, attachment: bytes) -> str:
+        """Register a multipart attachment.
+
+        Arguments:
+        name (str):         The name of the attachment.
+        attachment (bytes): The data to be attached.
+
+        Returns:    The content ID of the attachment, which should be used in place of the attachment data.
+        """
+        return self._transport.register_attachment(name, attachment)
+
     @on_exception(expo, TransportError, max_tries=3, giveup=fatal_code, logger=logger)  # type: ignore[arg-type]
     def submit(self, req: MmsRequest) -> MmsResponse:
         """Submit the given request to the MMS server and return the response.
 
         Arguments:
         req (MmsRequest):   The MMS request to submit.
```

### Comparing `mms_client-1.6.0/PKG-INFO` & `mms_client-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-client
-Version: 1.6.0
+Version: 1.7.0
 Summary: API client for accessing the MMS
 Home-page: https://github.com/ElectroRoute-Japan/mms-client
 Author: Ryan Wood
 Author-email: ryan.wood@electroroute.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic :: 2
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: lxml (>=5.1.0,<6.0.0)
 Requires-Dist: pendulum (>=3.0.0,<4.0.0)
+Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pydantic-xml (>=2.9.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-pkcs12 (>=1.24,<2.0)
 Requires-Dist: xmlschema (>=3.0.2,<4.0.0)
 Requires-Dist: zeep (>=4.2.1,<5.0.0)
 Description-Content-Type: text/markdown
@@ -39,14 +40,17 @@
 The underlying API sends and receives XML documents. Each of these request or responses, which we will hereafter refer to as *outer* requests and responses, contains metadata about the request/response as well as three fields which are extremely important to successful communication with the API:
 - Attachments data, included as a list of elements with the binary data in a base-64 encoded format
 - Payload data, encoded in a base-64 encoded format
 - Payload signature, which is the SHA256 hash of the payload XML data, then signed with an RSA key, in a base-64 encoded format
 
 After the data has been converted and added to the outer request object, it is sent to the appropriate server endpoint via a Zeep client. The client certificate is also injected into the request using a PCKS12 adaptor.
 
+## Domain
+The domain to use when signing the content ID to MTOM attachments is specified when creating the client. This is not verified by the server, but it is used to generate the content ID for the MTOM attachments. As such, it is important to ensure that the domain is correct.
+
 # Serialization
 This library relies on Pydantic 2 and the pydantic-xml library for serialization/deserialization. As such, any type in this library can be converted to not only XML, but to JSON as well. This is extremely useful if you're trying to build a pass-through API service or something similar.
 
 ## Client Types
 Clients cannot call any and all endpoints in this API, willy-nilly. Some endpoints are restricted to particular clients. At the moment, there are three clients: Balance Service Providers (BSPs), Market Operators (MOs), and Transmission Service Operators (TSOs). Most likely you're operating as a BSP or MO, in which case you'll have access to most or all endpoints. However, it makes little sense for a TSO to be able to submit bids on their own power, so they are restricted to a read-only role in most cases.
 
 Note that MOs and BSPs access the MMS service using the same endpoints, but have distinct permissions. As such, both client types are supported explicitly here.
@@ -138,15 +142,15 @@
 from mms_client.types.offer import Direction, OfferData, OfferStack
 from mms_client.utils.web import ClientType
 
 # Create a certificate
 cert = Certificate("/path/to/my/cert.p12", "fake_passphrase")
 
 # Create a new MMS client
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert)
+client = MmsClient(domain="mydomain.com", participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert)
 
 # Create our request offer
 request_offer = OfferData(
     stack=[
         OfferStack(
             number=1,
             unit_price=100,
@@ -172,22 +176,22 @@
 
 There's a lot of code here but it's not terribly difficult to understand. All this does is pull in the authentication data, create the client, create the payload, submit it to the server and retrieve the response.
 
 ## Connecting to a Test Server
 If you want to test your MMS connection, you can try using the test server:
 
 ```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, test=True)
+client = MmsClient(domain="mydomain.com", participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, test=True)
 ```
 
 ## Connecting as a Market Admin
 If you're connecting as a market operator (MO), you can connect in admin mode:
 
 ```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
+client = MmsClient(domain="mydomain.com", participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
 ```
 
 ## Auditing XML Requests & Responses
 A common requirement for this sort of library is recording or saving the raw XML requests and responses for audit/logging purposes. This library supports this workflow through the `mms_client.utils.auditing.AuditPlugin` object. This object intercepts the XML request at the Zeep client level right before it is sent to the MMS and, similarly, intercepts the XML response immediately after it is received from the MMS. Before passing these objects on, without modifying them, it records the XML data as a byte string and passes it to two methods: `audit_request` and `audit_response`. These can be overridden by any object that inherits from this class, allowing the user to direct this data to whatever store they prefer to use for auditing or logging.
 
 ```python
 class TestAuditPlugin(AuditPlugin):
@@ -198,15 +202,15 @@
 
     def audit_request(self, mms_request: bytes) -> None:
         self.request = mms_request
 
     def audit_response(self, mms_response: bytes) -> None:
         self.response = mms_response
 
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, plugins=[TestAuditPlugin()])
+client = MmsClient(domain="mydomain.com", participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, plugins=[TestAuditPlugin()])
 ```
 
 This same input allows for the user to create their own plugins and add them to the Zeep client, allowing for a certain amount of extensibility.
 
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
 - MarketQuery_ReserveRequirementQuery
```

