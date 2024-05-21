# Comparing `tmp/ariston-0.19.3.tar.gz` & `tmp/ariston-0.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ariston-0.19.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ariston-0.19.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ariston-0.19.3.tar` & `ariston-0.19.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2024-04-05 18:38:09.051755 ariston-0.19.3/LICENSE
--rw-r--r--   0        0        0     3539 2024-04-05 18:38:09.051755 ariston-0.19.3/README.md
--rw-r--r--   0        0        0     5962 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/__init__.py
--rw-r--r--   0        0        0    31109 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/ariston_api.py
--rw-r--r--   0        0        0    12128 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/base_device.py
--rw-r--r--   0        0        0    15230 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/bsb_device.py
--rw-r--r--   0        0        0    18190 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/const.py
--rw-r--r--   0        0        0     1927 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/device.py
--rw-r--r--   0        0        0     4024 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/evo_device.py
--rw-r--r--   0        0        0     1331 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/evo_lydos_device.py
--rw-r--r--   0        0        0     3923 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/evo_one_device.py
--rw-r--r--   0        0        0    38267 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/galevo_device.py
--rw-r--r--   0        0        0      830 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/lux2_device.py
--rw-r--r--   0        0        0     1515 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/lux_device.py
--rw-r--r--   0        0        0    11270 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/lydos_hybrid_device.py
--rw-r--r--   0        0        0    10247 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/nuos_split_device.py
--rw-r--r--   0        0        0     3545 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/velis_base_device.py
--rw-r--r--   0        0        0     4552 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/velis_device.py
--rw-r--r--   0        0        0      361 2024-04-05 18:38:09.051755 ariston-0.19.3/pyproject.toml
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 ariston-0.19.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-21 18:18:30.540487 ariston-0.19.4/LICENSE
+-rw-r--r--   0        0        0     3539 2024-05-21 18:18:30.540487 ariston-0.19.4/README.md
+-rw-r--r--   0        0        0     6044 2024-05-21 18:18:30.540487 ariston-0.19.4/ariston/__init__.py
+-rw-r--r--   0        0        0    31333 2024-05-21 18:18:30.540487 ariston-0.19.4/ariston/ariston_api.py
+-rw-r--r--   0        0        0    12128 2024-05-21 18:18:30.540487 ariston-0.19.4/ariston/base_device.py
+-rw-r--r--   0        0        0    15230 2024-05-21 18:18:30.540487 ariston-0.19.4/ariston/bsb_device.py
+-rw-r--r--   0        0        0    18190 2024-05-21 18:18:30.540487 ariston-0.19.4/ariston/const.py
+-rw-r--r--   0        0        0     1927 2024-05-21 18:18:30.540487 ariston-0.19.4/ariston/device.py
+-rw-r--r--   0        0        0     4024 2024-05-21 18:18:30.540487 ariston-0.19.4/ariston/evo_device.py
+-rw-r--r--   0        0        0     1331 2024-05-21 18:18:30.540487 ariston-0.19.4/ariston/evo_lydos_device.py
+-rw-r--r--   0        0        0     3923 2024-05-21 18:18:30.544487 ariston-0.19.4/ariston/evo_one_device.py
+-rw-r--r--   0        0        0    38267 2024-05-21 18:18:30.544487 ariston-0.19.4/ariston/galevo_device.py
+-rw-r--r--   0        0        0      830 2024-05-21 18:18:30.544487 ariston-0.19.4/ariston/lux2_device.py
+-rw-r--r--   0        0        0     1515 2024-05-21 18:18:30.544487 ariston-0.19.4/ariston/lux_device.py
+-rw-r--r--   0        0        0    11270 2024-05-21 18:18:30.544487 ariston-0.19.4/ariston/lydos_hybrid_device.py
+-rw-r--r--   0        0        0    10247 2024-05-21 18:18:30.544487 ariston-0.19.4/ariston/nuos_split_device.py
+-rw-r--r--   0        0        0     3545 2024-05-21 18:18:30.544487 ariston-0.19.4/ariston/velis_base_device.py
+-rw-r--r--   0        0        0     4552 2024-05-21 18:18:30.544487 ariston-0.19.4/ariston/velis_device.py
+-rw-r--r--   0        0        0      361 2024-05-21 18:18:30.544487 ariston-0.19.4/pyproject.toml
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 ariston-0.19.4/PKG-INFO
```

### Comparing `ariston-0.19.3/LICENSE` & `ariston-0.19.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/README.md` & `ariston-0.19.4/README.md`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/__init__.py` & `ariston-0.19.4/ariston/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,17 @@
         case SystemType.BSB.value:
             return AristonBsbDevice(api, device)
         case _:
             _LOGGER.exception("Unsupported system type %s", system_type)
             return None
 
 
-def _connect(username: str, password: str) -> AristonAPI:
+def _connect(username: str, password: str, api_url: str = ARISTON_API_URL) -> AristonAPI:
     """Connect to ariston api"""
-    api = AristonAPI(username, password)
+    api = AristonAPI(username, password, api_url)
     api.connect()
     return api
 
 
 def _discover(api: AristonAPI) -> list[dict[str, Any]]:
     """Retreive ariston devices from the cloud"""
     cloud_devices: list[dict[str, Any]] = []
@@ -145,17 +145,17 @@
 ) -> Optional[AristonBaseDevice]:
     """Get ariston device"""
     api = _connect(username, password)
     cloud_devices = _discover(api)
     return _get_device(cloud_devices, api, gateway, is_metric, language_tag)
 
 
-async def _async_connect(username: str, password: str) -> AristonAPI:
+async def _async_connect(username: str, password: str, api_url: str = ARISTON_API_URL) -> AristonAPI:
     """Async connect to ariston api"""
-    api = AristonAPI(username, password)
+    api = AristonAPI(username, password, api_url)
     if not await api.async_connect():
         raise ConnectionException
     return api
 
 
 async def _async_discover(api: AristonAPI) -> list[dict[str, Any]]:
     """Async retreive ariston devices from the cloud"""
```

### Comparing `ariston-0.19.3/ariston/ariston_api.py` & `ariston-0.19.4/ariston/ariston_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,16 @@
                     if not is_retry:
                         if self.connect():
                             return self.__request(method, path, params, body, True)
                         raise Exception("Login failed (password changed?)")
                     raise Exception("Invalid token")
                 case 404:
                     return None
+                case 429:
+                    raise RequestFailedError(response.status_code, response.text)
                 case _:
                     if not is_retry:
                         time.sleep(5)
                         return self.__request(method, path, params, body, True)
                     raise Exception(response.status_code)
 
         if len(response.content) > 0:
@@ -894,14 +896,16 @@
                                 return await self.__async_request(
                                     method, path, params, body, True
                                 )
                             raise Exception("Login failed (password changed?)")
                         raise Exception("Invalid token")
                     case 404:
                         return None
+                    case 429:
+                        raise RequestFailedError(response.status_code, response.text)
                     case _:
                         if not is_retry:
                             await asyncio.sleep(5)
                             return await self.__async_request(
                                 method, path, params, body, True
                             )
                         raise Exception(response.status)
```

### Comparing `ariston-0.19.3/ariston/base_device.py` & `ariston-0.19.4/ariston/base_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/bsb_device.py` & `ariston-0.19.4/ariston/bsb_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/const.py` & `ariston-0.19.4/ariston/const.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/device.py` & `ariston-0.19.4/ariston/device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/evo_device.py` & `ariston-0.19.4/ariston/evo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/evo_lydos_device.py` & `ariston-0.19.4/ariston/evo_lydos_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/evo_one_device.py` & `ariston-0.19.4/ariston/evo_one_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/galevo_device.py` & `ariston-0.19.4/ariston/galevo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/lux2_device.py` & `ariston-0.19.4/ariston/lux2_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/lux_device.py` & `ariston-0.19.4/ariston/lux_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/lydos_hybrid_device.py` & `ariston-0.19.4/ariston/lydos_hybrid_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/nuos_split_device.py` & `ariston-0.19.4/ariston/nuos_split_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/velis_base_device.py` & `ariston-0.19.4/ariston/velis_base_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/ariston/velis_device.py` & `ariston-0.19.4/ariston/velis_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.3/PKG-INFO` & `ariston-0.19.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariston
-Version: 0.19.3
+Version: 0.19.4
 Summary: Ariston module
 Author-email: Tamás Füstös <fustom@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: requests
```

