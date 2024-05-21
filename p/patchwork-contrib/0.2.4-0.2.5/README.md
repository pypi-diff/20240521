# Comparing `tmp/patchwork-contrib-0.2.4.tar.gz` & `tmp/patchwork-contrib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/patchwork-contrib-0.2.4.tar", last modified: Mon Jan 15 20:52:43 2024, max compression
+gzip compressed data, was "dist/patchwork-contrib-0.2.5.tar", last modified: Tue May 21 16:18:06 2024, max compression
```

## Comparing `patchwork-contrib-0.2.4.tar` & `patchwork-contrib-0.2.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1177 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork/contrib/common/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7646 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/common/connector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/
--rw-rw-rw-   0 root         (0) root         (0)      240 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/tokens/
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/tokens/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4073 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/tokens/jwt.py
--rw-rw-rw-   0 root         (0) root         (0)     3225 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/tokens/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     1009 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/patchwork/contrib/fastapi/tokens/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork_contrib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1177 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork_contrib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork_contrib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork_contrib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork_contrib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      105 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork_contrib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/patchwork_contrib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1707 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 20:52:43.000000 patchwork-contrib-0.2.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3203 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/tests/test_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     1866 2024-01-15 20:52:32.000000 patchwork-contrib-0.2.4/tests/test_fastapi_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork/contrib/common/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10125 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/common/connector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5442 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/tokens/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/tokens/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4073 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/tokens/jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3225 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/tokens/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/patchwork/contrib/fastapi/tokens/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork_contrib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork_contrib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork_contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork_contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork_contrib.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork_contrib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/patchwork_contrib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:18:06.000000 patchwork-contrib-0.2.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4610 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/tests/test_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2024-05-21 16:17:53.000000 patchwork-contrib-0.2.5/tests/test_fastapi_jwt.py
```

### Comparing `patchwork-contrib-0.2.4/LICENSE` & `patchwork-contrib-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork-contrib-0.2.4/PKG-INFO` & `patchwork-contrib-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-contrib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Patchwork Contrib
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-contrib-0.2.4/README.md` & `patchwork-contrib-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `patchwork-contrib-0.2.4/patchwork/contrib/common/connector.py` & `patchwork-contrib-0.2.5/patchwork/contrib/common/connector.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,23 +42,65 @@
 
 
 class ConnectorNotFound(ConnectorResponseError):
     def __init__(self):
         super().__init__(code=404)
 
 
+class ConnectorPreconditionFailed(ConnectorResponseError):
+    def __init__(self, version: int = None, supported: int = None):
+        self.version = version
+        self.version_compatible = supported
+        super().__init__(code=412)
+
+
 class ConnectorTooManyAttempts(ConnectorResponseError):
     def __init__(self, retry_after: int):
         self.retry_after = retry_after
         super().__init__(code=429)
 
 
 T = TypeVar('T')
 
 
+def int_or_none(value: Union[str, int, None]) -> Union[int, None]:
+    if value is None:
+        return None
+    elif isinstance(value, int):
+        return value
+    else:
+        try:
+            return int(value)
+        except ValueError:
+            return None
+
+
+def match_version(requested_version: str, current_version: int, min_supported: int) -> Union[int, bool, None]:
+
+    if requested_version[0] == '>':
+        greater_than = int_or_none(requested_version[1:])
+        if not greater_than or current_version <= greater_than:
+            return False
+        return current_version
+
+    elif requested_version[0] == '<':
+        lower_than = int_or_none(requested_version[1:])
+        if not lower_than or min_supported >= lower_than:
+            return False
+        return max(lower_than - 1, current_version)
+
+    elif requested_version[0] == '=':
+        version = int_or_none(requested_version[1:])
+        if not version or not (min_supported <= version <= current_version):
+            return False
+        else:
+            return max(version, current_version)
+
+    return None
+
 class PrometheusMixin:
 
     settings: Any
     connector_version: str
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -72,26 +114,23 @@
             "timeout": self.settings.timeout
         })
 
     async def send(
             self,
             method: Literal['get', 'head', 'post', 'put', 'patch', 'delete'],
             url: str = '/',
-            *,
-            payload: BaseModel = None,
-            response_model: Type[T] = Any,
-            **options,
+            **kwargs
     ) -> Union[T, None]:
         with request_time.labels(
             method=method,
             url=url,
             user_agent=self.settings.user_agent,
             version=self.connector_version
         ).time():
-            return await super().send(method, url, payload=payload, response_model=response_model, **options)
+            return await super().send(method, url, **kwargs)
 
 
 class HTTPConnector(Component):
 
     class Config(Component.Config):
         timeout: int = 60
         max_conn_limit: int = 100
@@ -133,17 +172,28 @@
             self,
             method: Literal['get', 'head', 'post', 'put', 'patch', 'delete'],
             url: str = '/',
             *,
             payload: BaseModel = None,
             response_model: Type[T] = Any,
             data=None,
+            api_version: str=None,
             **options,
     ) -> Union[T, None]:
 
+        options.setdefault('headers', {})
+        if api_version is not None:
+            # validate API version request
+            if __debug__:
+                # check version format only in debug to catch programmer mistakes
+                if api_version[0] not in {'<', '>', '='} or int_or_none(api_version[1:]) is None:
+                    raise ValueError(f'invalid API version requested: {api_version}')
+
+            options['headers']['X-API-Version'] = api_version
+
         if data is None:
             if payload is not None:
                 # use pydantic JSON encoder instead of aiohttp, as pydantic one supports all types
                 # supported by pydantic
                 data = payload.model_dump_json().encode('utf-8')
 
         if method == 'get':
@@ -163,14 +213,24 @@
         elif method == 'delete':
             assert data is None, \
                 "payload is forbidden on DELETE method"
             response = await self.session.delete(url, **options)
         else:
             raise NotImplementedError('not supported HTTP method')
 
+        if api_version and response.ok:
+            resp_version = int_or_none(response.headers.get('X-API-Version'))
+
+            if not resp_version or not match_version(api_version, resp_version, resp_version):
+                # API version requested but no version returned or unsupported version returned
+                raise ConnectorPreconditionFailed(
+                    version=resp_version,
+                    supported=int_or_none(response.headers.get('X-API-Version-Compatible'))
+                )
+
         try:
             return await self._handle_response(response, response_model)
         except ConnectorResponseError:
             # response errors just re-raise
             if not response.closed:
                 response.close()
             raise
@@ -217,13 +277,18 @@
             if response_model is not Any and response_model is not None:
                 raise ValueError('response data expected, but 204 No Content response received')
             return None
         elif response.status == 403:
             raise ConnectorForbidden()
         elif response.status == 404:
             raise ConnectorNotFound()
+        elif response.status == 412:
+            raise ConnectorPreconditionFailed(
+                version=int_or_none(response.headers.get('X-API-Version')),
+                supported=int_or_none(response.headers.get('X-API-Version-Compatible'))
+            )
         elif response.status == 422:
             raise ConnectorBadData(await response.json())
         elif response.status == 429:
             raise ConnectorTooManyAttempts(int(response.headers.get('Retry-After', '0')))
         else:
             raise ConnectorResponseError(code=response.status)
```

### Comparing `patchwork-contrib-0.2.4/patchwork/contrib/fastapi/settings.py` & `patchwork-contrib-0.2.5/patchwork/contrib/fastapi/settings.py`

 * *Files identical despite different names*

### Comparing `patchwork-contrib-0.2.4/patchwork/contrib/fastapi/tokens/jwt.py` & `patchwork-contrib-0.2.5/patchwork/contrib/fastapi/tokens/jwt.py`

 * *Files identical despite different names*

### Comparing `patchwork-contrib-0.2.4/patchwork/contrib/fastapi/tokens/middleware.py` & `patchwork-contrib-0.2.5/patchwork/contrib/fastapi/tokens/middleware.py`

 * *Files identical despite different names*

### Comparing `patchwork-contrib-0.2.4/patchwork/contrib/fastapi/tokens/utils.py` & `patchwork-contrib-0.2.5/patchwork/contrib/fastapi/tokens/utils.py`

 * *Files identical despite different names*

### Comparing `patchwork-contrib-0.2.4/patchwork_contrib.egg-info/PKG-INFO` & `patchwork-contrib-0.2.5/patchwork_contrib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-contrib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Patchwork Contrib
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-contrib-0.2.4/patchwork_contrib.egg-info/SOURCES.txt` & `patchwork-contrib-0.2.5/patchwork_contrib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patchwork-contrib-0.2.4/setup.py` & `patchwork-contrib-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `patchwork-contrib-0.2.4/tests/test_connector.py` & `patchwork-contrib-0.2.5/tests/test_connector.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from aiohttp import web, StreamReader
 from pydantic import BaseModel
 
 import pytest
 
 from patchwork.contrib.common import HTTPConnector
-from patchwork.contrib.common.connector import ConnectorError
+from patchwork.contrib.common.connector import ConnectorError, ConnectorPreconditionFailed
 
 
 class TestModel(BaseModel):
     pass
 
 
 @pytest.mark.asyncio
@@ -99,8 +99,35 @@
     connector = HTTPConnector(endpoint_url=str(data_endpoint.make_url('/')))
 
     async with connector:
         response = await connector.send('get', '/', response_model=AsyncIterable)
         assert isinstance(response, StreamReader)
         await asyncio.sleep(0.1)
         async for chunk, _ in response.iter_chunks():
-            assert chunk == b'content'
+            assert chunk == b'content'
+
+
+@pytest.mark.asyncio
+async def test_api_version_exact(aiohttp_raw_server):
+    async def handler(request):
+        return web.json_response({}, headers={'X-API-Version': '2'})
+
+    data_endpoint = await aiohttp_raw_server(handler)
+    await data_endpoint.start_server()
+
+    connector = HTTPConnector(endpoint_url=str(data_endpoint.make_url('/')))
+    async with connector:
+        assert await connector.send('get', '/', response_model=TestModel, api_version='=2'), "exact version"
+        assert await connector.send('get', '/', response_model=TestModel, api_version='>1'), "greater than version"
+        assert await connector.send('get', '/', response_model=TestModel, api_version='<3'), "lower than version"
+
+        with pytest.raises(ConnectorPreconditionFailed):    # exact not match
+            await connector.send('get', '/', response_model=TestModel, api_version='=1')
+
+        with pytest.raises(ConnectorPreconditionFailed):    # greater not match
+            await connector.send('get', '/', response_model=TestModel, api_version='>2')
+
+        with pytest.raises(ConnectorPreconditionFailed):    # lower not match
+            await connector.send('get', '/', response_model=TestModel, api_version='<2')
+
+        with pytest.raises(ValueError): #   invalid version
+            assert await connector.send('get', '/', response_model=TestModel, api_version='1')
```

### Comparing `patchwork-contrib-0.2.4/tests/test_fastapi_jwt.py` & `patchwork-contrib-0.2.5/tests/test_fastapi_jwt.py`

 * *Files identical despite different names*

