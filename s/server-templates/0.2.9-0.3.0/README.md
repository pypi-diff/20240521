# Comparing `tmp/server_templates-0.2.9.tar.gz` & `tmp/server_templates-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server_templates-0.2.9.tar", last modified: Mon Apr 22 09:45:19 2024, max compression
+gzip compressed data, was "server_templates-0.3.0.tar", last modified: Tue May 21 10:26:30 2024, max compression
```

## Comparing `server_templates-0.2.9.tar` & `server_templates-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.193019 server_templates-0.2.9/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 server_templates-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     1970 2024-04-22 09:45:19.193019 server_templates-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2024-04-22 09:45:02.000000 server_templates-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.182577 server_templates-0.2.9/server_templates/
--rw-rw-rw-   0        0        0      196 2024-04-17 12:25:31.000000 server_templates-0.2.9/server_templates/__init__.py
--rw-rw-rw-   0        0        0     7623 2024-03-05 15:09:35.000000 server_templates-0.2.9/server_templates/client_requests.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.188565 server_templates-0.2.9/server_templates/server_aiohttp/
--rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.9/server_templates/server_aiohttp/__init__.py
--rw-rw-rw-   0        0        0    10652 2024-03-29 11:33:06.000000 server_templates-0.2.9/server_templates/server_aiohttp/main.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.190893 server_templates-0.2.9/server_templates/server_fastapi/
--rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.9/server_templates/server_fastapi/__init__.py
--rw-rw-rw-   0        0        0    21476 2024-04-22 09:44:37.000000 server_templates-0.2.9/server_templates/server_fastapi/main.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.191990 server_templates-0.2.9/server_templates.egg-info/
--rw-rw-rw-   0        0        0     1970 2024-04-22 09:45:19.000000 server_templates-0.2.9/server_templates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-04-22 09:45:19.000000 server_templates-0.2.9/server_templates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 09:45:19.000000 server_templates-0.2.9/server_templates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-22 09:45:19.000000 server_templates-0.2.9/server_templates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 09:45:19.194018 server_templates-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2092 2024-01-30 06:52:17.000000 server_templates-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:26:30.528895 server_templates-0.3.0/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 server_templates-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1970 2024-05-21 10:26:30.528895 server_templates-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2024-05-21 10:23:56.000000 server_templates-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 10:26:30.505021 server_templates-0.3.0/server_templates/
+-rw-rw-rw-   0        0        0      241 2024-04-24 11:47:38.000000 server_templates-0.3.0/server_templates/__init__.py
+-rw-rw-rw-   0        0        0     7120 2024-05-21 10:25:40.000000 server_templates-0.3.0/server_templates/client_requests.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:26:30.515615 server_templates-0.3.0/server_templates/server_aiohttp/
+-rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.3.0/server_templates/server_aiohttp/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-04-25 06:41:35.000000 server_templates-0.3.0/server_templates/server_aiohttp/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:26:30.523649 server_templates-0.3.0/server_templates/server_fastapi/
+-rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.3.0/server_templates/server_fastapi/__init__.py
+-rw-rw-rw-   0        0        0    23007 2024-05-14 12:59:21.000000 server_templates-0.3.0/server_templates/server_fastapi/main.py
+-rw-rw-rw-   0        0        0     1353 2024-05-14 13:08:49.000000 server_templates-0.3.0/server_templates/url.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:26:30.526895 server_templates-0.3.0/server_templates.egg-info/
+-rw-rw-rw-   0        0        0     1970 2024-05-21 10:26:30.000000 server_templates-0.3.0/server_templates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-05-21 10:26:30.000000 server_templates-0.3.0/server_templates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 10:26:30.000000 server_templates-0.3.0/server_templates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-21 10:26:30.000000 server_templates-0.3.0/server_templates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 10:26:30.531913 server_templates-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2092 2024-01-30 06:52:17.000000 server_templates-0.3.0/setup.py
```

### Comparing `server_templates-0.2.9/LICENSE` & `server_templates-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `server_templates-0.2.9/PKG-INFO` & `server_templates-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server_templates
-Version: 0.2.9
+Version: 0.3.0
 Summary: templates for servers
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/server_templates
 Keywords: api,api server,http server,aiohttp,FastApi
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# server_templates (v0.2.9)
+# server_templates (v0.3.0)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
```

### Comparing `server_templates-0.2.9/README.md` & `server_templates-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# server_templates (v0.2.9)
+# server_templates (v0.3.0)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
```

### Comparing `server_templates-0.2.9/server_templates/client_requests.py` & `server_templates-0.3.0/server_templates/client_requests.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,238 +2,220 @@
 from typing import *
 import requests
 from PyQt5.QtCore import QThread
 from collections import deque
 from enum import Enum, auto
 
 from object_info import ObjectInfo
+from logger_aux import Logger
+
+from server_templates.url import UrlCreator
 
 
 # =====================================================================================================================
 Type__Response = Union[None, requests.Response, requests.ConnectTimeout]
 Type__RequestBody = Union[str, dict]
 
 
 class ResponseMethod(Enum):
     POST = auto()
     GET = auto()
 
 
 # =====================================================================================================================
-class UrlCreator:
-    # SETTINGS -------------------------------------
-    PROTOCOL: Optional[str] = None
-    HOST: Optional[str] = None
-    PORT: Optional[int] = None
-    ROUTE: Optional[str] = None
-
-    def URL_create(
-            self,
-            protocol: Optional[str] = None,
-            host: Optional[str] = None,
-            port: Optional[int] = None,
-            route: Optional[str] = None,
-    ) -> str:
-        if protocol is None:
-            protocol = self.PROTOCOL or "http"
-        if host is None:
-            host = self.HOST or "localhost"
-        if port is None:
-            port = self.PORT or 80
-        if route is None:
-            route = self.ROUTE or ""
-
-        url = f"{protocol}://{host}:{port}/{route}"
-        return url
-
-
-class Client_RequestItem(UrlCreator, QThread):
+class Client_RequestItem(Logger, UrlCreator, QThread):
     """
     DONT USE IT AS ONE INSTANCE FOR SEVERAL REQUESTS!!!
     You need keep it only to manage results or sent in further time!
 
     So Only ONE REQUESTITEM FOR ONE Request!
 
     create object and wait result by wait() or connect slot finished
+
+    :param TIMEOUT_SEND: be careful! it is not so clear! timeout for connection is basically 3 sec!
+
     """
     # SETTINGS -------------------------------------
     START_ON_INIT: bool = None      # DONT DELETE!!! useful for delayed/pending requests
     TIMEOUT_SEND: float = 1
 
-    RETRY_LIMIT: int = 2
+    RETRY_LIMIT: int | None = 1
     RETRY_TIMEOUT: float = 0.5
+    retry_index: int = 0
 
     METHOD: ResponseMethod = ResponseMethod.POST
 
-    # AUX ------------------------------------------
-    BODY: Optional[Type__RequestBody] = None
-    # REQUEST: Optional[requests.Request] = None
-    RESPONSE: Optional[requests.Response] = None
-    EXCEPTION: Union[None, requests.ConnectTimeout, Exception] = None
-
-    attempt_all: int
-    attempt_circle: int
-    INDEX: int = 0
+    # INIT ------------------------------------------
+    BODY: Optional[Type__RequestBody]
+    # REQUEST: Optional[requests.Request]
+    RESPONSE: Optional[requests.Response]
+    EXX: Union[None, requests.ConnectTimeout, Exception]
     TIMESTAMP: float
 
+    # AUX ------------------------------------------
+    INDEX: int | None = None
+
     def __init__(
             self,
             body: Optional[Type__RequestBody] = None,
             method: Optional[ResponseMethod] = None,
 
             # url: Optional[str] = None,
             host: Optional[str] = None,
             port: Optional[int] = None,
             route: Optional[str] = None,
     ):
         super().__init__()
 
-        if body is not None:
-            self.BODY = body
+        # INITS ------------------------------------
         if method is not None:
             self.METHOD = method
 
+        self.BODY = body
+        self.RESPONSE = None
+        self.EXX = None
+        self.TIMESTAMP = 0
+
         # if url is None:
         #     url = self.HOST
         if host is not None:
             self.HOST = host
         if port is not None:
             self.PORT = port
         if route is not None:
             self.ROUTE = route
 
-        self.__class__.INDEX += 1
-        self.INDEX = int(self.__class__.INDEX)
-        self.attempt_all = 0
-        self.attempt_circle = 0
-        self.TIMESTAMP = time.time()
+        self.index__init()
 
+        # START ------------------------------------
         if self.START_ON_INIT:
             self.start()
 
+    def index__init(self) -> None:
+        if self.__class__.INDEX is None:
+            self.__class__.INDEX = 0
+        else:
+            self.__class__.INDEX += 1
+
+        self.INDEX = self.__class__.INDEX
+
     def check_success(self) -> bool:
         result = self.RESPONSE is not None and self.RESPONSE.ok
+        # self.LOGGER.debug(result)
         return result
 
     def __str__(self) -> str:
-        return f"[{self.INDEX=}/{self.attempt_all=}/{self.attempt_circle=}/{self.check_success()=}]{self.EXCEPTION=}/{self.RESPONSE=}"
+        return f"[{self.INDEX=}/len={self.__class__.INDEX}/{self.retry_index=}/{self.check_success()=}]{self.EXX=}/{self.RESPONSE=}"
 
     def __repr__(self) -> str:
         return str(self)
 
-    def run(self) -> None:
-        self.attempt_circle = 0
+    # ------------------------------------------------------------------------------------------------
+    def start(self, *args):
+        """
+        apply only one thread at once (from stack)!
+        """
+        if not self.isRunning():
+            self.LOGGER.debug("start")
 
-        url = self.URL_create()
+            super().start(*args)
 
-        while self.attempt_circle == 0 or self.attempt_circle < self.RETRY_LIMIT:
-            self.attempt_circle += 1
-            self.attempt_all += 1
-
-            self.RESPONSE = None
-            self.EXCEPTION = None
-
-            with requests.Session() as session:
-                try:
-                    if self.METHOD == ResponseMethod.POST:
-                        response = session.post(url=url, json=self.BODY or {}, timeout=self.TIMEOUT_SEND)
-                    elif self.METHOD == ResponseMethod.GET:
-                        response = session.get(url=url, timeout=self.TIMEOUT_SEND)
-                    self.RESPONSE = response
-                except Exception as exx:
-                    self.EXCEPTION = exx
+    def run(self) -> None:
+        self.LOGGER.debug("run")
+        while True:
+            self._send()
 
-            print(self)
+            # CHECK EXIT -------------------------------
             if self.check_success():
-                break
+                return
+
+            if self.RETRY_LIMIT and self.retry_index == self.RETRY_LIMIT - 1:
+                return
+            else:
+                time.sleep(self.RETRY_TIMEOUT)
+                self.retry_index += 1
 
-    # ---------------------------------------------------------------
-    # DONT USE anything LIKE THIS BELOW!!!
-    # def start(self, *args):
-    #     if not self.isRunning():
-    #         super().start(*args)
+    def _send(self) -> None:
+        self.TIMESTAMP = time.time()
+        self.RESPONSE = None
+        self.EXX = None
 
-    # def post(self, url=None, body=None):
-    #     self.start()
+        url = self.URL_create()
 
-    # def get(self, url=None):  #????
-    #     self.start()
+        with requests.Session() as session:
+            try:
+                if self.METHOD == ResponseMethod.POST:
+                    self.RESPONSE = session.post(url=url, json=self.BODY or {}, timeout=self.TIMEOUT_SEND)
+                elif self.METHOD == ResponseMethod.GET:
+                    self.RESPONSE = session.get(url=url, timeout=self.TIMEOUT_SEND)
+            except Exception as exx:
+                self.EXX = exx
 
+        self.LOGGER.debug(self)
 
-# =====================================================================================================================
-class Client_RequestsStack(QThread):
-    # TODO: save send data
 
+# =====================================================================================================================
+class Client_RequestsStack(Logger, QThread):
     # SETTINGS -------------------------------------
     REQUEST_CLS: Type[Client_RequestItem] = Client_RequestItem
 
     # AUX ------------------------------------------
     __stack: deque
-    request_last: Optional[Client_RequestItem] = None
 
-    def __init__(self, request_cls: Optional[Type[REQUEST_CLS]] = None):
+    def __init__(self):
         super().__init__()
-        if request_cls is not None:
-            self.REQUEST_CLS = request_cls
-
         self.__stack = deque()
 
     @property
     def stack(self) -> deque:
         return self.__stack
 
+    @property
+    def request_active(self) -> Optional[Client_RequestItem]:
+        if self.stack:
+            return self.stack[0]
+
     # ------------------------------------------------------------------------------------------------
     def start(self, *args):
         """
         apply only one thread at once (from stack)!
         """
         if not self.isRunning():
+            self.LOGGER.debug(f"start {self.request_active}")
             super().start(*args)
 
     # ------------------------------------------------------------------------------------------------
     def run(self):
-        stack_attempt = 0
-        while len(self.stack):
-            stack_attempt += 1
+        self.LOGGER.debug("[STACK]run")
 
-            # NEXT -----------------------------------------
-            # change last
-            if self.request_last is None or self.request_last.check_success():
-                stack_attempt = 0
-                self.request_last = self.stack[0]
-
-                if self.request_last.check_success():
-                    self.stack.popleft()
-                continue
-
-            # WORK -----------------------------------------
-            print()
-            print(f"{stack_attempt=}")
-            print(f"len={len(self.stack)}")
-            self.request_last.run()
+        # WORK -----------------------------------------
+        while len(self.stack):
+            self.LOGGER.debug(f"[STACK]run cycle with len={len(self.stack)}")
+            self.request_active.run()
 
-            if self.request_last.check_success():
+            if self.request_active.check_success():
                 self.stack.popleft()
-                continue
-
-            print(f"len={len(self.stack)}/{self.stack=}")
-            if stack_attempt == 2:
-                break
             else:
-                time.sleep(1)
+                break
 
-        if len(self.stack):
-            print(f"[WARN] stack is stopped by some errors")
+        # FINISH -----------------------------------------
+        if self.check_success():
+            self.LOGGER.info(f"[STACK] is empty")
         else:
-            print(f"[OK] stack is empty")
+            self.LOGGER.warn(f"[STACK] is stopped [at len={len(self.stack)}] by some errors [exx={self.request_active.EXX=}]")
 
-    def send(self, **kwargs) -> None:    # maybe rename to SEND???
+    def send(self, **kwargs) -> None:
         """
         work usually with POST
         """
-        # TODO: add locker???
         item = self.REQUEST_CLS(**kwargs)
         self.stack.append(item)
+        self.LOGGER.debug(f"[STACK].APPEND len={len(self.stack)}")
         self.start()
 
+    def check_success(self) -> bool:
+        result = self.request_active is None
+        self.LOGGER.debug(result)
+        return result
+
 
 # =====================================================================================================================
```

### Comparing `server_templates-0.2.9/server_templates/server_aiohttp/main.py` & `server_templates-0.3.0/server_templates/server_aiohttp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     # =================================================================================================================
     def run(self) -> None:
         """
         NOTE: this will block process!
         but if start() in thread - it would be OK!
 
-        EXCEPTION will not catch from start!!! but will CAUSE SYS_EXIT!!!
+        EXX will not catch from start!!! but will CAUSE SYS_EXIT!!!
         """
         try:
             web.run_app(app=self._app, port=self.PORT)
             # NOTE:
             # 1. dont use parameter host="localhost" - its incorrect! from other host you cant access by IP!!! - if not specified - OK!
 
             # this will not catch!!! cause of thread maybe!!!
```

### Comparing `server_templates-0.2.9/server_templates/server_fastapi/main.py` & `server_templates-0.3.0/server_templates/server_fastapi/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,81 @@
 from typing import *
 from enum import Enum
 from PyQt5.QtCore import QThread
+import time
 
 from object_info import ObjectInfo
+from server_templates.url import UrlCreator
 
 from fastapi import FastAPI, Path, Query, Body, Response
 from fastapi.responses import JSONResponse, RedirectResponse
 
 from pydantic import BaseModel
 import uvicorn
 
 from starlette import status
 from starlette.responses import Response
 
+from logger_aux import Logger
+
 
 # =====================================================================================================================
 class DataExample:
     int = 1
     float = 1.2
     str = "string"
     list = [1, "2"]
     dict = {1: "2", "22": 11}       # by FastAPI return={"1":"2","22":11}
 
 
 # =====================================================================================================================
+def _minimal():
+    import uvicorn
+    from fastapi import FastAPI, Response
+    from fastapi.responses import RedirectResponse
+
+    app = FastAPI()
+
+    @app.get("/")
+    async def redirect() -> Response:
+        return RedirectResponse(url="/docs")
+
+    @app.get("/{path}")
+    async def hello(path):
+        print(path)
+        return path
+
+    uvicorn.run(app, host="localhost", port=80)
+
+
+# =====================================================================================================================
 def create_app__FastApi(self: Any = None, data: Any = None) -> FastAPI:
+    class Item(BaseModel):
+        value: int
+
     # UNIVERSAL ======================================================
     if data is None:
         data = DataExample()
 
     app = FastAPI()
-    app.DATA = data
+    app.data = data
+    app.LOGGER = Logger("FastAPI").LOGGER
 
     # WORK -----------------------------------------------------------
     @app.get("/")
     async def redirect() -> Response:
         return RedirectResponse(url="/docs")
 
+    @app.post("/post/dict")
+    async def post(item: Item):
+        app.LOGGER.debug(item)
+        data.dict.update(item)
+        print(data.dict)
+        return item
+
     pass
     pass
     pass
     pass
     pass
     pass
 
@@ -501,37 +536,60 @@
     2=FROM PYTHON CODE
     https://stackoverflow.com/questions/62856818/how-can-i-run-the-fast-api-server-using-pycharm
     """
     pass
 
 
 # =====================================================================================================================
-class ServerFastApi_Thread(QThread):
+class ServerFastApi_Thread(Logger, QThread):
     """
     WORK IN both LINUX/Win!!!
     """
-    HOST: str = "0.0.0.0"
     PORT: int = 80
+    HOST: str = "0.0.0.0"
+    # HOST: str = "localhost"
+    """
+    HOST SETTINGS RULES
+    localhost - CANT ACCESS BY HOST_IP! only
+        http://localhost/ - OK!
+        http://127.0.0.1/ - OK!
+        http://192.168.75.140/ - FAIL!!!
+    
+    0.0.0.0 - ALL ARE OK!!!
+        http://localhost/ - OK!
+        http://127.0.0.1/ - OK!
+        http://192.168.75.140/ - OK!!!
+    """
 
     data: Any = None
     create_app: Callable[[Any], FastAPI] = create_app__FastApi
 
+    @property
+    def ROOT(self) -> str:
+        return UrlCreator().URL_create(host=self.HOST, port=self.PORT)
+
     def __init__(self, app: FastAPI = None, data: Any = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        if data is not None:
-            self.data = data
+        if data is None:
+            data = self.data
 
         if app is None:
-            app = self.create_app(data=self.data)
+            app = self.create_app(data=data)
         self.app = app
+        self.data = app.data
 
     def run(self):
+        self.LOGGER.debug("run")
         uvicorn.run(self.app, host=self.HOST, port=self.PORT)
 
+    def start(self, *args, **kwargs):
+        super().start()
+        time.sleep(1)
+
 
 def start_2__by_thread(app: FastAPI = None) -> Never:
     server = ServerFastApi_Thread(app)
     # server.run()
     server.start()
     server.wait()
```

### Comparing `server_templates-0.2.9/server_templates.egg-info/PKG-INFO` & `server_templates-0.3.0/server_templates.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server_templates
-Version: 0.2.9
+Version: 0.3.0
 Summary: templates for servers
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/server_templates
 Keywords: api,api server,http server,aiohttp,FastApi
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# server_templates (v0.2.9)
+# server_templates (v0.3.0)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
```

### Comparing `server_templates-0.2.9/setup.py` & `server_templates-0.3.0/setup.py`

 * *Files identical despite different names*

