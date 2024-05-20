# Comparing `tmp/heaven-0.3.4.tar.gz` & `tmp/heaven-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.3.4.tar", max compression
+gzip compressed data, was "heaven-0.3.5.tar", max compression
```

## Comparing `heaven-0.3.4.tar` & `heaven-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-09-07 11:01:19.761432 heaven-0.3.4/LICENSE
--rw-r--r--   0        0        0     1300 2023-09-07 11:01:19.761530 heaven-0.3.4/README.md
--rw-r--r--   0        0        0      216 2024-05-06 12:52:19.398896 heaven-0.3.4/heaven/__init__.py
--rw-r--r--   0        0        0      797 2024-05-06 12:52:03.442574 heaven-0.3.4/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-09-07 11:01:19.764194 heaven-0.3.4/heaven/context.py
--rw-r--r--   0        0        0      141 2023-09-07 11:01:19.764264 heaven-0.3.4/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-09-07 11:01:19.764353 heaven-0.3.4/heaven/form.py
--rw-r--r--   0        0        0     2946 2023-09-07 11:01:19.764429 heaven-0.3.4/heaven/mocks.py
--rw-r--r--   0        0        0     4487 2024-04-01 15:42:37.904117 heaven-0.3.4/heaven/request.py
--rw-r--r--   0        0        0     5384 2024-01-20 00:20:05.299419 heaven-0.3.4/heaven/response.py
--rw-r--r--   0        0        0    24785 2024-05-06 12:51:20.757757 heaven-0.3.4/heaven/router.py
--rw-r--r--   0        0        0        0 2023-09-07 11:01:19.764867 heaven-0.3.4/heaven/server.py
--rw-r--r--   0        0        0     1504 2023-09-07 20:48:02.654119 heaven-0.3.4/heaven/tutorials.py
--rw-r--r--   0        0        0     1180 2023-09-20 10:40:19.499167 heaven-0.3.4/heaven/utils.py
--rw-r--r--   0        0        0      526 2024-05-06 12:52:36.874215 heaven-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 heaven-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-09-07 11:01:19.761432 heaven-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1300 2023-09-07 11:01:19.761530 heaven-0.3.5/README.md
+-rw-r--r--   0        0        0      216 2024-05-20 22:36:38.009306 heaven-0.3.5/heaven/__init__.py
+-rw-r--r--   0        0        0      797 2024-05-06 12:52:03.442574 heaven-0.3.5/heaven/constants.py
+-rw-r--r--   0        0        0      723 2024-05-20 22:31:25.583130 heaven-0.3.5/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-09-07 11:01:19.764264 heaven-0.3.5/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-09-07 11:01:19.764353 heaven-0.3.5/heaven/form.py
+-rw-r--r--   0        0        0     2946 2023-09-07 11:01:19.764429 heaven-0.3.5/heaven/mocks.py
+-rw-r--r--   0        0        0     4487 2024-04-01 15:42:37.904117 heaven-0.3.5/heaven/request.py
+-rw-r--r--   0        0        0     5384 2024-01-20 00:20:05.299419 heaven-0.3.5/heaven/response.py
+-rw-r--r--   0        0        0    24862 2024-05-20 22:24:42.212561 heaven-0.3.5/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-09-07 11:01:19.764867 heaven-0.3.5/heaven/server.py
+-rw-r--r--   0        0        0     1504 2023-09-07 20:48:02.654119 heaven-0.3.5/heaven/tutorials.py
+-rw-r--r--   0        0        0     1180 2023-09-20 10:40:19.499167 heaven-0.3.5/heaven/utils.py
+-rw-r--r--   0        0        0      526 2024-05-20 22:56:12.231837 heaven-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 heaven-0.3.5/PKG-INFO
```

### Comparing `heaven-0.3.4/LICENSE` & `heaven-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.3.4/README.md` & `heaven-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `heaven-0.3.4/heaven/constants.py` & `heaven-0.3.5/heaven/constants.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.4/heaven/form.py` & `heaven-0.3.5/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.4/heaven/mocks.py` & `heaven-0.3.5/heaven/mocks.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.4/heaven/request.py` & `heaven-0.3.5/heaven/request.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.4/heaven/response.py` & `heaven-0.3.5/heaven/response.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.4/heaven/router.py` & `heaven-0.3.5/heaven/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     WILDCARD
 )
 
 from .errors import AbortException, SubdomainError, UrlDuplicateError, UrlError
 from .utils import preprocessor
 from .request import Request
 from .response import Response
-from .context import Context
+from .context import Context, Look
 
 
 methods = ['get', 'post', 'put', 'delete', 'connect', 'head', 'options', 'patch']
 
 
 Handler = Union[Callable[[Request, Response, Context], object], str]
 
@@ -357,14 +357,18 @@
         self.subdomains[DEFAULT] = Routes()
         self._buckets = {}
         self._configuration = _get_configuration(configurator)
         self._templater = None
         self._loader = None
         self.__daemons = []
 
+    @property
+    def _(self):
+        return Look(self._buckets)
+
     async def __call__(self, scope, receive, send):
         if scope['type'] == 'lifespan':
             while True:
                 message = await receive()
                 if message['type'] == 'lifespan.startup':
                     try: await self._register()
                     except: _notify()
```

### Comparing `heaven-0.3.4/heaven/tutorials.py` & `heaven-0.3.5/heaven/tutorials.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.4/heaven/utils.py` & `heaven-0.3.5/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.4/pyproject.toml` & `heaven-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heaven"
-version = "0.3.4"
+version = "0.3.5"
 description = "Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications."
 authors = ["Raymond Ortserga <ortserga@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `heaven-0.3.4/PKG-INFO` & `heaven-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.3.4
+Version: 0.3.5
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

