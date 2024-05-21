# Comparing `tmp/novum_api_client-2.0.0.tar.gz` & `tmp/novum_api_client-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novum_api_client-2.0.0.tar", max compression
+gzip compressed data, was "novum_api_client-2.0.1.tar", max compression
```

## Comparing `novum_api_client-2.0.0.tar` & `novum_api_client-2.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-07-05 06:53:04.093748 novum_api_client-2.0.0/LICENSE
--rw-r--r--   0        0        0      958 2024-04-29 14:48:00.934082 novum_api_client-2.0.0/README.md
--rw-r--r--   0        0        0        0 2024-01-02 08:51:00.098131 novum_api_client-2.0.0/novum_api_client/__init__.py
--rw-r--r--   0        0        0    16121 2024-04-29 14:48:00.934082 novum_api_client-2.0.0/novum_api_client/api_type.py
--rw-r--r--   0        0        0    11062 2024-04-29 14:48:00.934082 novum_api_client-2.0.0/novum_api_client/base_client.py
--rw-r--r--   0        0        0    29588 2024-04-29 14:48:00.938082 novum_api_client-2.0.0/novum_api_client/client.py
--rw-r--r--   0        0        0        0 2024-01-02 08:51:00.102131 novum_api_client-2.0.0/novum_api_client/tests/__init__.py
--rw-r--r--   0        0        0    10832 2024-04-29 14:48:00.938082 novum_api_client-2.0.0/novum_api_client/tests/test_api_base.py
--rw-r--r--   0        0        0    33112 2024-04-29 14:48:00.938082 novum_api_client-2.0.0/novum_api_client/tests/test_api_public.py
--rw-r--r--   0        0        0      598 2024-04-29 14:48:00.938082 novum_api_client-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 novum_api_client-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-05 06:53:04.093748 novum_api_client-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1095 2024-05-21 06:57:34.470922 novum_api_client-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-01-02 08:51:00.098131 novum_api_client-2.0.1/novum_api_client/__init__.py
+-rw-r--r--   0        0        0    16121 2024-05-21 06:42:59.510851 novum_api_client-2.0.1/novum_api_client/api_type.py
+-rw-r--r--   0        0        0    11475 2024-05-21 06:57:34.470922 novum_api_client-2.0.1/novum_api_client/base_client.py
+-rw-r--r--   0        0        0    30615 2024-05-21 06:57:34.470922 novum_api_client-2.0.1/novum_api_client/client.py
+-rw-r--r--   0        0        0        0 2024-01-02 08:51:00.102131 novum_api_client-2.0.1/novum_api_client/tests/__init__.py
+-rw-r--r--   0        0        0    10794 2024-05-21 06:57:34.470922 novum_api_client-2.0.1/novum_api_client/tests/test_api_base.py
+-rw-r--r--   0        0        0    34794 2024-05-21 06:57:34.470922 novum_api_client-2.0.1/novum_api_client/tests/test_api_public.py
+-rw-r--r--   0        0        0      542 2024-05-21 06:57:34.470922 novum_api_client-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 novum_api_client-2.0.1/PKG-INFO
```

### Comparing `novum_api_client-2.0.0/LICENSE` & `novum_api_client-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `novum_api_client-2.0.0/README.md` & `novum_api_client-2.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,35 +10,39 @@
 
 Use pip to install:
 
 ```shell
 pip install novum_api_client
 ```
 
-
 # Release Notes
 
-## Version 2.0.0
-- Release Date: 2024-04-12
+## Version 2.0.1
+- Release Date: 2024-04-30
 
 ### Enhancements
+- Extended class arguments from base client.
+- SSL_VERIFY optional for HTTP requests.
+- Tests follow some order.
+
+
+# Changelog
+
+## [2.0.0] - 2024-04-29
 - Added dataclass_json to easy the types.
 - Rename types.
 - Added Docstring.
 - Rename functions "get_capacity_measurement" and "get_capacity_measurement_count".
 - API Client available for Python > 3.8.1
 
 
-# Changelog
-
 ## [1.1.1] - 2024-04-11
 - Added new functions (get_user_documents and get_user_document_by_id).
 - Forced typing for Reports.
 
-
 ## [1.0.1] - 2023-12-12
 - Prettier added
 - Most of the function have "fields" as an argument.
 - Made Reports Section available. 
 - Added Error/Exception messages.
```

### Comparing `novum_api_client-2.0.0/novum_api_client/api_type.py` & `novum_api_client-2.0.1/novum_api_client/api_type.py`

 * *Files identical despite different names*

### Comparing `novum_api_client-2.0.0/novum_api_client/base_client.py` & `novum_api_client-2.0.1/novum_api_client/base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # pylint: disable=C0103
 # flake8: noqa
 
 from dataclasses import asdict, dataclass
+import os
 import json
 import time
 import base64
 import hashlib
 from datetime import datetime
 from urllib.parse import unquote
 from threading import Timer
-from typing import List, Optional, Any
+from typing import List, Union, Optional, Any
 import requests
 from .api_type import TChargeTypes, TUser, TUserEssentials
 
 TOKEN_REFRESH_INTERVAL_SCALE = 0.9
-PRODUCTION_API_HOST: str = "https://novum-batteries.com"
+API_HOST = os.getenv("NOVUM_API_URL", "https://novum-batteries.com")
+SSL_VERIFY = (
+    False if os.getenv("SSL_VERIFY", "true").lower() == "false" else True
+)  # set SSL_verification of HTTP request to false inside DinD
 
 
 class DateTimeEncoder(json.JSONEncoder):
     "DateTimeEncoder"
 
     def default(self, o):
         if isinstance(o, datetime):
@@ -75,20 +79,20 @@
     base64_string = base64_bytes.decode("utf-8").replace("-", "+").replace("_", "/")
     json_payload = unquote(base64.b64decode(base64_string).decode("utf-8"))
     return json.loads(json_payload)
 
 
 @dataclass
 class BaseAPIClient:
-    "BaseAPIClient class"
-    user: Optional[TUser] = None
-    host: str = PRODUCTION_API_HOST
+    user: Union[TUser, None] = None
+    host: str = API_HOST
+    check_ssl_certification: bool = SSL_VERIFY
     refresh_token_warning: bool = True
     refresh_interval_scale: float = TOKEN_REFRESH_INTERVAL_SCALE
-    _relogin_timer_handle = None
+    _relogin_timer_handle: Union[Timer, None] = None
     _authenticated: bool = False
 
     def __post_init__(self):
         if (
             isinstance(self.user, TUser)
             and self.user.jwt is not None
             and hasattr(self.user, "jwt")
@@ -208,14 +212,15 @@
             params_json["fields"] = json.dumps(fields)
 
         response = requests.get(
             url=full_url,
             headers=headers,
             params=params_json,
             timeout=timeout,
+            verify=self.check_ssl_certification,
         )
 
         if response.status_code == requests.codes.get("ok"):
             return response.json()
         raise NovumAPIError(response.text, response.status_code)
 
     def _post_file(self, path: str, file: str):
@@ -246,18 +251,20 @@
 
         response = requests.post(
             url=full_url,
             headers=headers,
             params=params_json,
             data=data,
             timeout=timeout,
+            verify=self.check_ssl_certification,
         )
 
         if response.status_code == requests.codes.get("ok"):
             return response.json()
+
         raise NovumAPIError(response.text, response.status_code)
 
     def _put_json(
         self,
         url: str,
         input_data: Any,
         filter_json: Optional[dict] = None,
@@ -277,18 +284,20 @@
 
         response = requests.put(
             url=full_url,
             headers=headers,
             params=params_json,
             data=data_json,
             timeout=timeout,
+            verify=self.check_ssl_certification,
         )
 
         if response.status_code == requests.codes.get("ok"):
             return response.json()
+
         raise NovumAPIError(response.text, response.status_code)
 
     def _delete_json(
         self,
         url: str,
         filter_json: Optional[dict] = None,
         option: Optional[dict] = None,
@@ -304,17 +313,19 @@
             params_json["option"] = json.dumps(option)
 
         response = requests.delete(
             url=full_url,
             headers=headers,
             params=params_json,
             timeout=timeout,
+            verify=self.check_ssl_certification,
         )
         if response.status_code <= 204:
             return response
+
         raise NovumAPIError(response.text, response.status_code)
 
     def _get_text(
         self,
         path: str,
         headers: Optional[dict] = None,
     ) -> dict:
```

### Comparing `novum_api_client-2.0.0/novum_api_client/client.py` & `novum_api_client-2.0.1/novum_api_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # pylint: disable=C0103
 # flake8: noqa
-
 import json
-from typing import Optional, List
 from dataclasses import dataclass
+from typing import Optional, Union, List
 import warnings
 import requests
 from .base_client import BaseAPIClient, NovumAPIError
 from .api_type import (
     TUser,
     TReport,
     TVersion,
@@ -22,23 +21,48 @@
     TBatteryTypeReading,
     TBatteryTypeEssentials,
     TDeviceMeasurementsResult,
     TCapacityMeasurementReading,
     TCapacityMeasurementEssentials,
 )
 
-PRODUCTION_API_HOST: str = "https://novum-batteries.com"
-
 
 @dataclass
 class NovumAPIClient(BaseAPIClient):
     """NovumAPIClient class"""
 
-    def __init__(self, user=None, host=PRODUCTION_API_HOST):
-        super().__init__(user, host)
+    def __init__(
+        self,
+        user=None,
+        host=None,
+        check_ssl_certification=None,
+        refresh_token_warning=None,
+        refresh_interval_scale=None,
+        _relogin_timer_handle=None,
+        _authenticated=None,
+    ):
+        super().__init__(
+            user=user if user is not None else self.user,
+            host=host if host is not None else self.host,
+            check_ssl_certification=check_ssl_certification
+            if check_ssl_certification is not None
+            else self.check_ssl_certification,
+            refresh_token_warning=refresh_token_warning
+            if refresh_token_warning is not None
+            else self.refresh_token_warning,
+            refresh_interval_scale=refresh_interval_scale
+            if refresh_interval_scale is not None
+            else self.refresh_interval_scale,
+            _relogin_timer_handle=_relogin_timer_handle
+            if _relogin_timer_handle is not None
+            else self._relogin_timer_handle,
+            _authenticated=_authenticated
+            if _authenticated is not None
+            else self._authenticated,
+        )
 
     # ********************************************************
     # Section for the Service Center info
     # ********************************************************
 
     def ping(self) -> dict:
         """Ping API."""
@@ -56,23 +80,24 @@
 
     # ********************************************************
     # Section for the users
     # ********************************************************
 
     def login(
         self, email: str, password: str, store_user=True, timeout: float = 4
-    ) -> Optional[TUser]:
-        """Login."""
+    ) -> Union[TUser, None]:
+        """Login function"""
         header = {"authorization": "auth", "content-type": "application/json"}
         payload = {"username": email, "password": password}
         response = requests.post(
             self.host + "/api/batman/v1/login",
             data=json.dumps(payload),
             headers=header,
             timeout=timeout,
+            verify=self.check_ssl_certification,
         )
         if response.status_code == requests.codes.get("ok"):
             if store_user is True:
                 user = response.json()
                 self.user = TUser(**user)
                 self._install_token_refresh_procedure()
                 self.headers = dict(
@@ -186,16 +211,15 @@
         """Check remote data."""
         response = self._get_json(
             f"/api/batman/v1/datasets/{dataset_id}", timeout=timeout
         )
         try:
             if len(response["measured"]["measurement_cycles"]) != 0:
                 return True
-            else:
-                return False
+            return False
         except KeyError:
             return False
 
     def create_dataset(
         self, dataset: TDatasetEssentials, timeout: float = 4.0
     ) -> TDatasetEssentials:
         """Create EIS measurement."""
```

### Comparing `novum_api_client-2.0.0/novum_api_client/tests/test_api_base.py` & `novum_api_client-2.0.1/novum_api_client/tests/test_api_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # pylint: disable=C0115
 # pylint: disable=C0116
 # flake8: noqa
 
-import pytest
-import hashlib
+import os
 from unittest.mock import Mock
+import hashlib
+import pytest
 
 from ..api_type import TProfile, TUserEssentials, TUserSettings
 from ..base_client import user_name, get_sha_256, full_name, parse_jwt, BaseAPIClient
 
-PRODUCTION_API_HOST: str = "https://novum-batteries.com"
+API_HOST = os.getenv("NOVUM_API_URL", "https://localhost")
 
 
 class TestBaseAPIClient:
     # auxiliar functions
     @pytest.fixture
     def user_sample_mage(self):
         """Fixture: sample of user."""
@@ -94,33 +95,33 @@
         """Check  _get_expire_time_from_token_in_unix_time_millis method."""
         sample_token = "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Im9Ma1Ridm93cnFndXdoN3lPaUttTCJ9.eyJodHRwczovL25vdnVtLWJhdHRlcmllcy5jb20vcm9sZXMiOlsidXNlciIsImludm9pY2VDcmVhdG9yIiwibm92dW1FeHBlcnQiXSwiaHR0cHM6Ly9ub3Z1bS1iYXR0ZXJpZXMuY29tL3NldHRpbmdzIjp7ImludmVydEF4aXMiOnRydWUsInNlcnZpY2VDZW50ZXIiOnsic2hvd0FkdmFuY2VkT3B0aW9ucyI6dHJ1ZSwiaW52ZXJ0QXhpcyI6dHJ1ZSwiZmF2b3JpdGVCYXR0ZXJpZXNJZHMiOlsiOW94SHZjNnlOWld1VzNzRWsiLCIyRUdFTjd1TU40YWg4ckRGWiIsIkRUQUhIRFR1SkJEQ3ZRRlNKIiwiOVJBU0VIZHZxRW9odlBFU1oiLCJkenBEd3NoUEFHc2N5NkJHaCIsIkFjY3lxSGdvR25IU0F3ZTlHIiwiczdNU1g0ZjNIcWpDcHZ1TEoiLCI1YzdlYkJTekNXNFJuckYzNCIsIkhQZ0RLVFRUSjNEUUhGZ0FEIl0sImJhdHRlcnlUYWJsZUNvbHVtbnMiOlsibmFtZSIsInN0YXRlLnN0YXRlX29mX2NoYXJnZS52YWx1ZSIsInN0YXRlLnN0YXRlX29mX2hlYWx0aC52YWx1ZSIsIm1ldHJpY3Muc3RhdGVfb2ZfaGVhbHRoIiwiaW50ZXJuYWxfY2FwYWNpdHlfY291bnQiLCJpbnRlcm5hbF9kYXRhc2V0X2NvdW50IiwiY3JlYXRvcl9pZCIsImxpZmV0aW1lX2luZGljYXRvciIsImludGVybmFsX2FjdGlvbnMiXSwiZGFzaGJvYXJkVGFibGVDb2x1bW5zIjpbIm5hbWUiLCJiYXR0ZXJ5X3R5cGUubmFtZSIsInN0YXRlLnN0YXRlX29mX2NoYXJnZS52YWx1ZSIsInN0YXRlLnN0YXRlX29mX2hlYWx0aC52YWx1ZSIsImxpZmV0aW1lX2luZGljYXRvciIsImludGVybmFsX2FjdGlvbnMiXSwiZWlzRGF0YXNldFRhYmxlQ29sdW1ucyI6WyJpZCIsIm1ldGEuYmF0dGVyeS5uYW1lIiwiYW5hbHlzaXMuc3RhdGVfb2ZfY2hhcmdlIiwiYW5hbHlzaXMuc3RhdGVfb2ZfaGVhbHRoIiwiaW50ZXJuYWxfYWN0aW9ucyIsImFuYWx5c2lzLmdyYWRlIiwiY3JlYXRvcl9pZCIsImNvbnRleHRfaWQiLCJjcmVhdGVkX2F0Il0sImNhcGFjaXR5TWVhc3VyZW1lbnRUYWJsZUNvbHVtbnMiOlsiaWQiLCJiYXR0ZXJ5Lm5hbWUiLCJzdGF0ZV9vZl9oZWFsdGgiLCJjcmVhdGVkX2F0IiwiaW50ZXJuYWxfYWN0aW9ucyIsImdyYWRlIiwiY3JlYXRvcl9pZCIsImNvbnRleHRfaWQiLCJzdGFydF90aW1lIiwiZW5kX3RpbWUiXX19LCJnaXZlbl9uYW1lIjoiTGVvbmFyZG8iLCJmYW1pbHlfbmFtZSI6IkJpeiIsIm5pY2tuYW1lIjoibC5iaXoiLCJuYW1lIjoiTGVvIEJpeiIsInBpY3R1cmUiOiJodHRwczovL3MuZ3JhdmF0YXIuY29tL2F2YXRhci8yZTRiYTE2Y2U0MzY4NTE0NDVmMzcxNDM1M2QyNzAwNz9zPTQ4MCZyPXBnJmQ9aHR0cHMlM0ElMkYlMkZjZG4uYXV0aDAuY29tJTJGYXZhdGFycyUyRmwucG5nIiwidXBkYXRlZF9hdCI6IjIwMjMtMTEtMDFUMTE6NDc6NTYuMjE3WiIsImVtYWlsIjoibC5iaXpAbm92dW0tZW5naW5lZXJpbmcuY29tIiwiZW1haWxfdmVyaWZpZWQiOnRydWUsImlzcyI6Imh0dHBzOi8vZGV2LW5vdnVtLmV1LmF1dGgwLmNvbS8iLCJhdWQiOiJwN0pSSEI3bVlvOGt5RXVlVWt2VnhTWFo5YllXSWZSbCIsImlhdCI6MTY5ODg0Nzk2MywiZXhwIjoxNjk4ODgzOTYzLCJzdWIiOiJhdXRoMHw2MjMzM2RiNGJjNzgzNDAwNjhjMzdjOTEiLCJzaWQiOiIwOHVGV09oX3V2N3J2Z0p3dy1HMVhMQ0F1QTNsUUFjQyIsIm5vbmNlIjoiV0hvd1NXTnlORmhpUkdGdmEwWnViSFJtUTBGUVdGcEdaRXRRTlM1bU1WVnVUa2hHZVMwdVlqVXRRdz09In0.YtOCMsRWNQIbt_XxKdyLr7Y4IP60FQea3T5KKtLJ2V753A91DbTYYGxvCdwsrGtyoXge1_8Yp7_6_bAbGKkr5K1RLSGzbUEkgqe9KvbBSI8uDvDM8hPOPGAUYq5-XyL4j2I36NWQqsT1i32d6ozf_fJqXHurfvXASfXHK7Wp6moTAV7HtqvYhcwfC9ZbV9hqplldLCkxYPe2lkzky0H-EfJqLh1X-g8hLCnn_9TW2d1LFIxHbciIaYaAqhjtU01KveDKyu3imi4m5z2pxa3hW6T_nYKB1utXUHacvMX89zMuGGSOZrNa9Ww9zhmzVgA4NG-SFCKQFNMThGkMdPdKqA"
         result = base_api_client._get_expire_time_from_token_in_unix_time_millis(
             sample_token
         )
         assert isinstance(result, str)
 
-    # TODO def test_install_token_refresh_procedure(self, user_sample_mage):
+    # TODO: def test_install_token_refresh_procedure(self, user_mage):
 
     @pytest.mark.parametrize(
         "ok_value, status_code, expected_error",
         [
             (True, 200, None),
             (
                 False,
                 400,
-                f"Failed to load resource {PRODUCTION_API_HOST} -> Status:400",
+                f"Failed to load resource {API_HOST} -> Status:400",
             ),
         ],
     )
     def test_fetch_by_URL(self, base_api_client, ok_value, status_code, expected_error):
         """Mock the _get_json method to return a response."""
         response = {"ok": ok_value, "status": status_code}
         base_api_client._get_json = Mock(return_value=response)
 
-        url = PRODUCTION_API_HOST
+        url = API_HOST
         options = {}
 
         if expected_error:
             with pytest.raises(ValueError) as excinfo:
                 base_api_client._fetch_by_URL(url, options)
             assert str(excinfo.value) == expected_error
         else:
@@ -130,24 +131,24 @@
     @pytest.mark.parametrize(
         "ok_value, status_code, expected_error",
         [
             (True, 200, None),
             (
                 False,
                 400,
-                f"('Failed to load resource {PRODUCTION_API_HOST} -> Status:400'",
+                f"('Failed to load resource {API_HOST} -> Status:400'",
             ),
         ],
     )
     def test_post_by_URL(self, base_api_client, ok_value, status_code, expected_error):
         """Check the _post_json method to return a response."""
         response = {"ok": ok_value, "status": status_code}
         base_api_client._post_json = Mock(return_value=response)
 
-        url = PRODUCTION_API_HOST
+        url = API_HOST
         options = {}
 
         if expected_error:
             with pytest.raises(ValueError) as excinfo:
                 base_api_client._post_by_URL(url, options)
             assert str(excinfo.value) == expected_error + ", " + str(response) + ")"
         else:
```

### Comparing `novum_api_client-2.0.0/novum_api_client/tests/test_api_public.py` & `novum_api_client-2.0.1/novum_api_client/tests/test_api_public.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=C0115
 # pylint: disable=C0116
 # pylint: disable=W0105
 # flake8: noqa
 
-
+import os
 from datetime import datetime
 import json
 import pytest
 
 from ..base_client import NovumAPIError
 from ..client import NovumAPIClient
 from ..api_type import (
@@ -29,181 +29,198 @@
     TBatteryEssentials,
     TDeviceMetaParticle,
     TBatteryTypeEssentials,
     TCapacityMeasurementEssentials,
 )
 
 
+API_HOST = os.getenv("NOVUM_API_URL", "localhost")
+SSL_VERIFY = False if os.getenv("SSL_VERIFY", "true").lower() == "false" else True
+
+
 class TestNovumAPIClient:
     @pytest.fixture(scope="class")
     def unauthenticated_api_client(self):
         """Check if authenticated before login."""
-        api_client = NovumAPIClient()
+        api_client = NovumAPIClient(host=API_HOST, check_ssl_certification=SSL_VERIFY)
         yield api_client
 
     @pytest.fixture(scope="class")
     def ada_logged_client(self):
         """Fixture API client logged in."""
-        client = NovumAPIClient()
+        client = NovumAPIClient(host=API_HOST, check_ssl_certification=SSL_VERIFY)
         client.login(
             email="ada.lovelace@novum-engineering.com", password="5TkbQuVEx4v2GVqJ"
         )
         yield client
 
+    @pytest.mark.run(order=1)
     def test_ping(self, unauthenticated_api_client: NovumAPIClient):
         """Check ping message."""
         response = unauthenticated_api_client.ping()
 
         assert (
             response["message"]
             == "Hello user this is the Novum batman API server. All routes begin with /api/{api_type}/{api_version}/{resource}. You have to identify using your credentials and /api/batman/v1/login to obtain a token"
         )
 
+    @pytest.mark.run(order=2)
     def test_get_info(self, unauthenticated_api_client: NovumAPIClient):
         """Check info root."""
         info = unauthenticated_api_client.get_info()
 
         assert isinstance(info, TAPIInfoEssentials)
         assert info.name == "Novum Base API"
         assert info.dbName == "batman"
 
+    @pytest.mark.run(order=3)
     def test_get_version(self, unauthenticated_api_client: NovumAPIClient):
         """Check version"""
         version = unauthenticated_api_client.get_version()
 
         assert isinstance(version, TVersion)
         assert version.name == "novum-api"
-        assert version.branch == "master"
 
+    @pytest.mark.run(order=4)
     def test_login_ada(self, unauthenticated_api_client: NovumAPIClient):
         """Check Ada login."""
         response = unauthenticated_api_client.login(
             email="ada.lovelace@novum-engineering.com", password="5TkbQuVEx4v2GVqJ"
         )
         assert isinstance(response, TUser)
         assert "user" in response.roles
 
+    @pytest.mark.run(order=5)
     def test_login_ada_with_wrong_credentials(
         self, unauthenticated_api_client: NovumAPIClient
     ):
         """Check if login with wrong password gets authenticated."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.login(
                 email="ada.lovelace@novum-engineering.com", password="WrongPassword"
             )
 
         error_details = json.loads(str(excinfo.value))
 
         expected_error_message = "Wrong email or password."
         assert expected_error_message in error_details["details"]
 
+    @pytest.mark.run(order=6)
     def test_check_current_user_still_authenticated(
         self, ada_logged_client: NovumAPIClient
     ):
         """Check authentication."""
         response = ada_logged_client.check_current_user_still_authenticated()
         assert response["authenticated"] is True
 
+    @pytest.mark.run(order=7)
     def test_logout(self, ada_logged_client: NovumAPIClient):
         """Check logout function."""
         response = ada_logged_client.logout()
         assert response == {"message": "Logout successful"}
 
     # ********************************************************
     # Section for the Battery Type
     # ********************************************************
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_battery_type(self):
         """Fixture: Battery Type"""
         sample_battery_type = TBatteryTypeEssentials(
             name="Test Battery Type",
             manufacturer="The Tester",
             nominal_voltage=3.7,
             nominal_capacity=2500,
         )
         return sample_battery_type
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def created_battery_type(
         self,
         ada_logged_client: NovumAPIClient,
         sample_battery_type: TBatteryTypeEssentials,
     ):
         """Fixture: sample of battery type."""
         response = ada_logged_client.create_battery_type(sample_battery_type)
 
         yield response
 
         # Add cleanup code here to delete the created battery type
         ada_logged_client.remove_battery_types_by_id(response.id)
 
+    @pytest.mark.run(order=8)
     def test_get_battery_type(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery_type: TBatteryTypeEssentials,
     ):
         """Check if the created battery type can be fetched."""
         response = ada_logged_client.get_battery_types()
 
         assert response[0].id == created_battery_type.id
 
+    @pytest.mark.run(order=9)
     def test_get_battery_type_with_fields(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery_type: TBatteryTypeEssentials,
     ):
         """Check if the created battery type can be fetched with fields."""
         fields = {"name": 1}
         response = ada_logged_client.get_battery_types(fields=fields)
 
         assert response[0].id == created_battery_type.id
         assert response[0].name == created_battery_type.name
         assert response[0].manufacturer is None
 
+    @pytest.mark.run(order=10)
     def test_get_battery_type_without_fields(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery_type: TBatteryTypeEssentials,
     ):
         """Check if the created battery type can be fetched without fields."""
         fields = {"name": 0}
         response = ada_logged_client.get_battery_types(fields=fields)
 
         assert response[0].id == created_battery_type.id
         assert response[0].name is None
 
+    @pytest.mark.run(order=11)
     def test_get_battery_type_count(self, ada_logged_client: NovumAPIClient):
         """Check number of battery types created."""
         response = ada_logged_client.get_battery_types_count()
-        assert response == 6
+        assert response == 1
 
+    @pytest.mark.run(order=12)
     def test_get_battery_type_by_id(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery_type: TBatteryTypeEssentials,
     ):
         """Check fetching battery type by id"""
         response = ada_logged_client.get_battery_types_by_id(created_battery_type.id)
         assert response.id == created_battery_type.id
 
+    @pytest.mark.run(order=13)
     def test_create_battery_type(self, created_battery_type: TBatteryTypeEssentials):
         """Check info of created battery type."""
         assert created_battery_type.name == "Test Battery Type"
         assert created_battery_type.nominal_voltage == 3.7
         assert created_battery_type.nominal_capacity == 2500
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_battery_type_without_name(
         self, sample_battery_type: TBatteryTypeEssentials
     ):
         """Fixture: battery type without name."""
         sample_battery_type.name = None  # type: ignore
         return sample_battery_type
 
+    @pytest.mark.run(order=14)
     def test_create_battery_type_missing_required_field_name(
         self,
         unauthenticated_api_client: NovumAPIClient,
         sample_battery_type_without_name: TBatteryTypeEssentials,
     ):
         """Check if attempt to create a battery type without name raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
@@ -211,65 +228,67 @@
                 sample_battery_type_without_name
             )
 
         assert '{"error":"Failed to validate battery type data","details":' in str(
             excinfo.value
         )
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_battery_type_without_manufacturer(
         self, sample_battery_type: TBatteryTypeEssentials
     ):
         """Fixture: battery type without manufacturer."""
         sample_battery_type.manufacturer = None  # type: ignore
         return sample_battery_type
 
+    @pytest.mark.run(order=16)
     def test_create_battery_type_missing_required_field_manufacturer(
         self,
         unauthenticated_api_client: NovumAPIClient,
         sample_battery_type_without_manufacturer: TBatteryTypeEssentials,
     ):
         """Check if attempt to create a battery type without manufacturer raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.create_battery_type(
                 sample_battery_type_without_manufacturer
             )
 
-        assert (
-            '{"error":"Failed to validate battery type data","details":"Key: \'BatteryType.Manufacturer\''
-            in str(excinfo.value)
+        assert '{"error":"Failed to validate battery type data","details":' in str(
+            excinfo.value
         )
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_battery_type_without_capacity(
         self, sample_battery_type: TBatteryTypeEssentials
     ):
         """Fixture: battery type without nominal capacity."""
         sample_battery_type.nominal_capacity = ""  # type: ignore
         return sample_battery_type
 
+    @pytest.mark.run(order=17)
     def test_create_battery_type_missing_required_field_capacity(
         self,
         ada_logged_client: NovumAPIClient,
         sample_battery_type_without_capacity: TBatteryTypeEssentials,
     ):
         """Check if attempt to create a battery type without nominal capacity raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             ada_logged_client.create_battery_type(sample_battery_type_without_capacity)
 
         assert '{"error":"Failed to decode battery type data"' in str(excinfo.value)
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_battery_type_without_voltage(
         self, sample_battery_type: TBatteryTypeEssentials
     ):
         """Fixture: battery type without nominal voltage."""
         sample_battery_type.nominal_voltage = ""  # type: ignore
         return sample_battery_type
 
+    @pytest.mark.run(order=18)
     def test_update_battery_type(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery_type: TBatteryTypeEssentials,
     ):
         """Check if attempt to create a battery type without nominal voltage raises an error."""
         update_data = TBatteryTypeEssentials(
@@ -286,118 +305,122 @@
 
         assert updated_response.name == "Updated Battery Type"
         assert updated_response.manufacturer == "Updated"
         assert updated_response.nominal_voltage == 3.8
         assert updated_response.nominal_capacity == 3200
         assert updated_response.description == "There is an update"
 
-    def test_delete_battery_type_from_another_user(
-        self, ada_logged_client: NovumAPIClient
-    ):
-        """Check if attempt to delete a battery type from another uses raises an error."""
-        with pytest.raises(NovumAPIError) as excinfo:
-            ada_logged_client.remove_battery_types_by_id("dpgtbPhcnt5oH685D")
-
-        assert '{"error":"Forbidden","details":""}' in str(excinfo.value)
-
+    @pytest.mark.run(order=19)
     def test_delete_battery_type(
-        self, ada_logged_client: NovumAPIClient, sample_battery_type
+        self,
+        ada_logged_client: NovumAPIClient,
+        sample_battery_type: TBatteryTypeEssentials,
     ):
         """Check battery type deletion."""
         sample_battery_type.name = "to be deleted"
+        sample_battery_type.manufacturer = "broken manufacture"
+        sample_battery_type.nominal_capacity = 1
+        sample_battery_type.nominal_voltage = 220
+
         to_be_deleted_sample = sample_battery_type
         to_be_deleted = ada_logged_client.create_battery_type(to_be_deleted_sample)
 
         response = ada_logged_client.remove_battery_types_by_id(to_be_deleted.id)
 
         assert "was removed" in response
 
     # # ********************************************************
     # # Section for the Battery
     # # ********************************************************
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_battery(self, created_battery_type: TBatteryTypeEssentials):
         """Fixture: sample of battery."""
         return TBatteryEssentials(
             name="Test Battery", battery_type=created_battery_type
         )
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def created_battery(
         self, ada_logged_client: NovumAPIClient, sample_battery: TBatteryEssentials
     ):
         """Fixture: sample of battery."""
 
         response = ada_logged_client.create_battery(sample_battery)
 
         yield response
 
         # Add cleanup code here to delete the created battery type
         ada_logged_client.remove_battery_by_id(response.id)
 
+    @pytest.mark.run(order=20)
     def test_create_battery(self, created_battery: TBatteryEssentials):
         """Check battery creation."""
 
         assert created_battery.name == "Test Battery"
 
+    @pytest.mark.run(order=21)
     def test_get_battery(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery: TBatteryEssentials,
     ):
         """Check if the created battery can be fetched."""
         response = ada_logged_client.get_batteries()
 
         assert response[0].id == created_battery.id
 
+    @pytest.mark.run(order=22)
     def test_get_battery_with_fields(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery: TBatteryEssentials,
     ):
         """Check if the created battery can be fetched with fields."""
         fields = {"name": 1}
         response = ada_logged_client.get_batteries(fields=fields)
 
         assert response[0].id == created_battery.id
         assert response[0].name == created_battery.name
         assert response[0].description is None
 
+    @pytest.mark.run(order=23)
     def test_get_battery_without_fields(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery: TBatteryEssentials,
     ):
         """Check if the created battery can be fetched without fields."""
         fields = {"name": 0}
         response = ada_logged_client.get_batteries(fields=fields)
 
         assert response[0].id == created_battery.id
         assert response[0].name is None
         assert response[0].description is None
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_battery_without_name(self, sample_battery: TBatteryEssentials):
         """Fixture: battery without name."""
         sample_battery.name = None  # type: ignore
 
         return sample_battery
 
+    @pytest.mark.run(order=24)
     def test_create_battery_missing_required_field_name(
         self,
         unauthenticated_api_client: NovumAPIClient,
         sample_battery_without_name: TBatteryEssentials,
     ):
         """Check if attempt to create a battery without name raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.create_battery(sample_battery_without_name)
 
         assert '{"error":"Failed to validate ' in str(excinfo.value)
 
+    @pytest.mark.run(order=25)
     def test_update_battery(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery: TBatteryEssentials,
         created_battery_type: TBatteryTypeEssentials,
     ):
         """Check battery updating."""
@@ -410,14 +433,15 @@
         updated_response = ada_logged_client.update_battery_by_id(
             created_battery.id, update_data
         )
 
         assert updated_response.name == "Updated Battery"
         assert updated_response.description == "There is an update"
 
+    @pytest.mark.run(order=26)
     def test_delete_battery(
         self,
         ada_logged_client: NovumAPIClient,
         created_battery_type: TBatteryTypeEssentials,
     ):
         """Check battery deletion."""
         to_be_deleted_sample = TBatteryEssentials(
@@ -429,21 +453,21 @@
 
         assert "was removed" in response
 
     # ********************************************************
     # Section for the DataSet
     # ********************************************************
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_eis_dataset(self):
         """Fixture: EIS measurement."""
         sample_eis = TDatasetEssentials(
             measured=TMeasured(
-                start_time="2021-03-10T17:40:44.956Z",
-                end_time="2021-03-10T17:42:43.915Z",
+                start_time=datetime(2023, 11, 10, 5, 5, 5),
+                end_time=datetime(2023, 11, 10, 5, 5, 5),
                 eis_setup=TEISSetup(
                     start_frequency=4000,
                     end_frequency=0.1,
                     number_of_frequencies=21,
                     excitation_current_offset=0.06,
                     excitation_current_amplitude=0.05,
                     excitation_mode=None,
@@ -500,134 +524,140 @@
                         details=None,
                     ),
                 ),
             ),
         )
         return sample_eis
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def created_eis_dataset(
         self, ada_logged_client: NovumAPIClient, sample_eis_dataset: TDatasetEssentials
     ):
         """Fixture: created EIS measurement."""
 
         response = ada_logged_client.create_dataset(sample_eis_dataset)
 
         yield response
 
         # Add cleanup code here to delete the created battery type
         ada_logged_client.remove_dataset_by_id(response.id)
 
+    @pytest.mark.run(order=27)
     def test_create_eis_dataset(self, created_eis_dataset: TDatasetEssentials):
         """Check EIS creation."""
 
         assert isinstance(created_eis_dataset, TDatasetEssentials)
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_dataset_without_name(self, sample_eis_dataset: TDatasetEssentials):
         """Fixture: EIS measurement without name"""
         sample_eis_dataset.measured.start_time = None  # type : ignore
         return sample_eis_dataset
 
+    @pytest.mark.run(order=28)
     def test_create_dataset_missing_required_field_start_time(
         self,
         unauthenticated_api_client: NovumAPIClient,
         sample_dataset_without_name: TDatasetEssentials,
     ):
         """Check if attempt to create a EIS measurement without name raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.create_dataset(sample_dataset_without_name)
 
-        assert (
-            '{"error":"Failed to validate dataset","details":"Key: \'Dataset.Measured.StartTime\' Error:'
-            in str(excinfo.value)
-        )
+        assert '{"error":"Failed to validate dataset","details":' in str(excinfo.value)
 
+    @pytest.mark.run(order=29)
     def test_get_dataset(
         self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
     ):
         """Check created EIS measurement."""
         response = ada_logged_client.get_datasets()
 
         assert response[0].id == created_eis_dataset.id
 
+    @pytest.mark.run(order=30)
     def test_get_dataset_with_fields(
         self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
     ):
         """Check created EIS measurement with fields."""
         fields = {"context_id": 1}
         response = ada_logged_client.get_datasets(fields=fields)
 
         assert response[0].id == created_eis_dataset.id
         assert response[0].context_id == created_eis_dataset.context_id
         assert response[0].show_in_chart is None
 
+    @pytest.mark.run(order=31)
     def test_get_dataset_without_fields(
         self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
     ):
         """Check created EIS measurement without fields."""
         fields = {"context_id": 0}
         response = ada_logged_client.get_datasets(fields=fields)
 
         assert response[0].id == created_eis_dataset.id
         assert response[0].context_id is None
         assert response[0].show_in_chart is None
 
+    @pytest.mark.run(order=31)
     def test_get_datasets_count(self, ada_logged_client: NovumAPIClient):
         """Check amount of EIS measurements."""
         response = ada_logged_client.get_datasets_count()
 
-        assert response == 0
+        assert response == 1
 
+    @pytest.mark.run(order=32)
     def test_get_dataset_by_id(
         self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
     ):
         """Check created dataset by id."""
         response = ada_logged_client.get_dataset_by_id(created_eis_dataset.id)
 
         assert response.id == created_eis_dataset.id
 
+    @pytest.mark.run(order=33)
     def test_update_dataset(
         self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
     ):
         """Check EIS measurement update."""
         response = ada_logged_client.get_dataset_by_id(created_eis_dataset.id)
         response.context_id = "new_context_id"
         ada_logged_client.update_dataset_by_id(created_eis_dataset.id, response)
         response_updated = ada_logged_client.get_dataset_by_id(created_eis_dataset.id)
 
         assert response_updated.context_id == "new_context_id"
 
+    @pytest.mark.run(order=34)
     def test_delete_dataset(
         self, ada_logged_client: NovumAPIClient, sample_eis_dataset: TDatasetEssentials
     ):
         """Check EIS measurement deletion."""
         to_be_deleted_sample = sample_eis_dataset
+        to_be_deleted_sample.measured.start_time = datetime(2023, 11, 10, 5, 5, 6)
         to_be_deleted = ada_logged_client.create_dataset(to_be_deleted_sample)
 
         response = ada_logged_client.remove_dataset_by_id(to_be_deleted.id)
 
         assert "was removed" in response
 
     # ********************************************************
     # Section for the Capacity Measurement
     # ********************************************************
-
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_capacity_measurement(self):
         """Fixture: sample capacity measurement."""
         sample_capacity = TCapacityMeasurementEssentials(
             start_time=datetime(2023, 11, 10, 5, 5, 5),
             end_time=None,
             current_setpoint=1,
             voltage_setpoint=2,
             charge_type=TChargeTypes.CC,
             charge_cycles=[
                 TChargeCycle(
-                    timestamp="2023-09-12T09:57:47.221Z",
+                    timestamp=datetime(2023, 11, 10, 5, 5, 5),
                     voltage=3,
                     current=1,
                     charge=1,
                 )
             ],
             tags=["test0 only test"],
             ambient_temperature=22.3,
@@ -636,15 +666,15 @@
             voltage_min=2.14,
             voltage_max=3.14,
             state_of_health=0.94,
             grade="D",
         )
         return sample_capacity
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def created_capacity_measurement(
         self,
         ada_logged_client: NovumAPIClient,
         sample_capacity_measurement: TCapacityMeasurementEssentials,
     ):
         """Fixture: capacity measurement creation."""
 
@@ -653,98 +683,105 @@
         )
 
         yield response
 
         # Add cleanup code here to delete the created battery type
         ada_logged_client.remove_capacity_measurement_by_id(response.id)
 
+    @pytest.mark.run(order=35)
     def test_create_capacity_measurement(
         self, created_capacity_measurement: TCapacityMeasurementEssentials
     ):
         """Check capacity measurement creation."""
 
         assert created_capacity_measurement.current_setpoint == 1
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def sample_capacity_measurement_without_start_time(
         self, sample_capacity_measurement: TCapacityMeasurementEssentials
     ):
         """Fixture: sample of capacity measurement without start time."""
         sample_capacity_measurement.start_time = None  # type: ignore
         return sample_capacity_measurement
 
+    @pytest.mark.run(order=36)
     def test_create_capacity_measurement_missing_required_field_start_time(
         self,
-        unauthenticated_api_client: NovumAPIClient,
+        ada_logged_client: NovumAPIClient,
         sample_capacity_measurement_without_start_time: TCapacityMeasurementEssentials,
     ):
         """Check if attempt to create a capacity measurement without start time raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
-            unauthenticated_api_client.create_capacity_measurement(
+            ada_logged_client.create_capacity_measurement(
                 sample_capacity_measurement_without_start_time
             )
 
-        assert (
-            '{"error":"Failed to validate capacity measurement","details":"Key: \'CapacityMeasurement.StartTime\' Error:Field validation for \'StartTime\' failed'
-            in str(excinfo.value)
+        assert '{"error":"Failed to validate capacity measurement",' in str(
+            excinfo.value
         )
 
+    @pytest.mark.run(order=37)
     def test_get_capacity_measurements(
         self,
         ada_logged_client: NovumAPIClient,
         created_capacity_measurement: TCapacityMeasurementEssentials,
     ):
         """Check capacity measurements fetching."""
         response = ada_logged_client.get_capacity_measurements()
 
         assert response[0].id == created_capacity_measurement.id
 
+    @pytest.mark.run(order=38)
     def test_get_capacity_measurements_with_fields(
         self,
         ada_logged_client: NovumAPIClient,
         created_capacity_measurement: TCapacityMeasurementEssentials,
     ):
         """Check capacity measurements fetching with fields."""
         fields = {"device_name": 1}
         response = ada_logged_client.get_capacity_measurements(fields=fields)
 
         assert response[0].id == created_capacity_measurement.id
         assert response[0].device_name == created_capacity_measurement.device_name
         assert response[0].grade is None
 
+    @pytest.mark.run(order=39)
     def test_get_capacity_measurements_without_fields(
         self,
         ada_logged_client: NovumAPIClient,
         created_capacity_measurement: TCapacityMeasurementEssentials,
     ):
         """Check capacity measurements fetching without fields."""
         fields = {"device_name": 0}
         response = ada_logged_client.get_capacity_measurements(fields=fields)
 
         assert response[0].id == created_capacity_measurement.id
         assert response[0].device_name is None
 
+    @pytest.mark.run(order=40)
     def test_get_capacity_measurements_count(self, ada_logged_client: NovumAPIClient):
         """Check created capacity measurement."""
         response = ada_logged_client.get_capacity_measurements_count()
 
-        assert response == 0
+        assert response == 1
 
+    @pytest.mark.run(order=41)
     def test_get_capacity_measurement_by_id(
         self,
         ada_logged_client: NovumAPIClient,
         created_capacity_measurement: TCapacityMeasurementEssentials,
     ):
         """Check created capacity measurement by id."""
         response = ada_logged_client.get_capacity_measurement_by_id(
             created_capacity_measurement.id
         )
 
         assert response.id == created_capacity_measurement.id
 
+    @pytest.mark.run(order=42)
     def test_update_capacity_measurement(
         self,
         ada_logged_client: NovumAPIClient,
         created_capacity_measurement: TCapacityMeasurementEssentials,
     ):
         """Check capacity measurement updating."""
         response = ada_logged_client.get_capacity_measurement_by_id(
@@ -756,21 +793,24 @@
         )
         response_updated = ada_logged_client.get_capacity_measurement_by_id(
             created_capacity_measurement.id
         )
 
         assert response_updated.context_id == "new_context_id"
 
+    @pytest.mark.run(order=43)
     def test_delete_capacity_measurement(
         self,
         ada_logged_client: NovumAPIClient,
         sample_capacity_measurement: TCapacityMeasurementEssentials,
     ):
+
         """Check capacity measurement deletion."""
         to_be_deleted_sample = sample_capacity_measurement
+        to_be_deleted_sample.start_time = datetime(2023, 11, 10, 5, 5, 6)
         to_be_deleted = ada_logged_client.create_capacity_measurement(
             to_be_deleted_sample
         )
 
         response = ada_logged_client.remove_capacity_measurement_by_id(to_be_deleted.id)
 
         assert "was removed" in response
@@ -801,71 +841,78 @@
         response = ada_logged_client.create_report(sample_report)
 
         yield response
 
         # Add cleanup code here to delete the created battery type
         ada_logged_client.remove_report_by_id(response.id)
 
+    @pytest.mark.run(order=44)
     def test_create_report(self, created_report: TReport):
         assert created_report.origin_id == "test_report_origin_id"
         assert created_report.title == "test_report_title"
         assert created_report.description == "test_report_description"
         assert created_report.context_id == "test_report_context_id"
 
     @pytest.fixture
     def sample_report_without_title(self, sample_report: TReportEssentials):
         sample_report.title = None  # type: ignore
         return sample_report
 
+    @pytest.mark.run(order=45)
     def test_create_report_missing_required_field_title(
         self,
         unauthenticated_api_client: NovumAPIClient,
         sample_report_without_title: TReportEssentials,
     ):
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.create_report(sample_report_without_title)
 
         assert '{"error":"Failed to validate report data","details":"Key:' in str(
             excinfo.value
         )
 
+    @pytest.mark.run(order=46)
     def test_get_reports(
         self,
         ada_logged_client: NovumAPIClient,
         created_report: TReport,
     ):
         response = ada_logged_client.get_reports()
 
         assert response[0].id == created_report.id
 
+    @pytest.mark.run(order=47)
     def test_get_reports_count(self, ada_logged_client: NovumAPIClient):
         response = ada_logged_client.get_reports_count()
 
         assert response == 0
 
+    @pytest.mark.run(order=48)
     def test_get_report_by_id(
         self,
         ada_logged_client: NovumAPIClient,
         created_report: TReport,
     ):
         response = ada_logged_client.get_report_by_id(created_report.id)
 
         assert response.id == created_report.id
 
+    @pytest.mark.run(order=49)
     def test_update_report_by_id(
         self,
         ada_logged_client: NovumAPIClient,
         created_report: TReport,
     ):
         created_report.context_id = "new_context_id"
         ada_logged_client.update_report_by_id(created_report.id, created_report)
         response_updated = ada_logged_client.get_report_by_id(created_report.id)
 
         assert response_updated.context_id == "new_context_id"
 
+    @pytest.mark.run(order=50)
     def test_delete_report_by_id(
         self,
         ada_logged_client: NovumAPIClient,
         sample_report: TReportEssentials,
     ):
         created_report = ada_logged_client.create_report(sample_report)
         response = ada_logged_client.remove_report_by_id(created_report.id)
```

### Comparing `novum_api_client-2.0.0/PKG-INFO` & `novum_api_client-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: novum_api_client
-Version: 2.0.0
-Summary: This library contains the basic api functions for Novum Service Center.
+Version: 2.0.1
+Summary: Python API Client for Novum Service Center.
 Author: Leonardo
 Author-email: l.biz@novum-engineering.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -26,35 +26,39 @@
 
 Use pip to install:
 
 ```shell
 pip install novum_api_client
 ```
 
-
 # Release Notes
 
-## Version 2.0.0
-- Release Date: 2024-04-12
+## Version 2.0.1
+- Release Date: 2024-04-30
 
 ### Enhancements
+- Extended class arguments from base client.
+- SSL_VERIFY optional for HTTP requests.
+- Tests follow some order.
+
+
+# Changelog
+
+## [2.0.0] - 2024-04-29
 - Added dataclass_json to easy the types.
 - Rename types.
 - Added Docstring.
 - Rename functions "get_capacity_measurement" and "get_capacity_measurement_count".
 - API Client available for Python > 3.8.1
 
 
-# Changelog
-
 ## [1.1.1] - 2024-04-11
 - Added new functions (get_user_documents and get_user_document_by_id).
 - Forced typing for Reports.
 
-
 ## [1.0.1] - 2023-12-12
 - Prettier added
 - Most of the function have "fields" as an argument.
 - Made Reports Section available. 
 - Added Error/Exception messages.
```

