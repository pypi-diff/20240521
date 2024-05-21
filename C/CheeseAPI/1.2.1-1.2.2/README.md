# Comparing `tmp/cheeseapi-1.2.1.tar.gz` & `tmp/cheeseapi-1.2.2.tar.gz`

## Comparing `cheeseapi-1.2.1.tar` & `cheeseapi-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/app.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/cors.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/exception.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/file.py
--rw-r--r--   0        0        0    32431 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/request.py
--rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/response.py
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/route.py
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/schedule.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/server.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/signal.py
--rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/text.py
--rw-r--r--   0        0        0    12949 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/validator.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/LICENSE
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/file.py
+-rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/response.py
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/text.py
+-rw-r--r--   0        0        0    12949 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/validator.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/PKG-INFO
```

### Comparing `cheeseapi-1.2.1/CheeseAPI/app.py` & `cheeseapi-1.2.2/CheeseAPI/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import multiprocessing, os
+import multiprocessing, os, setproctitle, sys
 from typing import Dict, Any, List
 
 from CheeseAPI.text import Text
 from CheeseAPI.server import Server
 from CheeseAPI.workspace import Workspace
 from CheeseAPI.handle import Handle
 from CheeseAPI.signal import _Signal
@@ -272,8 +272,11 @@
 
         app.run()
         ```
         '''
 
         return self._preferred_localModules
 
+if ' '.join(sys.argv) in setproctitle.getproctitle():
+    setproctitle.setproctitle('CheeseAPI')
+
 app: App = App()
```

### Comparing `cheeseapi-1.2.1/CheeseAPI/cors.py` & `cheeseapi-1.2.2/CheeseAPI/cors.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/exception.py` & `cheeseapi-1.2.2/CheeseAPI/exception.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/file.py` & `cheeseapi-1.2.2/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/handle.py` & `cheeseapi-1.2.2/CheeseAPI/handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import time, os, inspect, socket, multiprocessing, signal, http, ipaddress, datetime
+import time, os, inspect, socket, multiprocessing, signal, http, ipaddress, datetime, traceback
 from typing import TYPE_CHECKING, Dict, Tuple, List
 
 import asyncio, uvloop, setproctitle, websockets
 from CheeseLog import logger
 
 from CheeseAPI.response import BaseResponse, FileResponse, Response
 from CheeseAPI.exception import Route_404_Exception, Route_405_Exception
@@ -105,76 +105,86 @@
 
                 self.loadLocalModule(foldernames[i])
 
             for text in self._app._text.loadedLocalModules():
                 logger.loaded(text[0], text[1], refreshed = True)
 
     def server_start(self):
-        self._app._handle.server_beforeStarting()
-        if self._app.signal.server_beforeStarting.receivers:
-            self._app.signal.server_beforeStarting.send()
-
         try:
-            ipaddress.IPv4Address(self._app.server.host)
-            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        except ipaddress.AddressValueError:
-            sock = socket.socket(socket.AF_INET6, socket.SOCK_STREAM)
-        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        sock.bind((self._app.server.host, self._app.server.port))
-        sock.listen(self._app.server.backlog)
-        sock.set_inheritable(True)
-
-        processes: List[multiprocessing.Process] = []
-        multiprocessing.allow_connection_pickling()
-        for i in range(self._app.server.workers - 1):
-            process = multiprocessing.Process(target = self.worker_start, args = (sock,), name = self._app._text.workerProcess_title)
-            process.start()
-            processes.append(process)
-
-        self.worker_start(sock, True)
-
-        for process in processes:
-            process.terminate()
-            process.join()
-
-        for text in self._app._text.server_stopping():
-            logger.ending(text[0], text[1])
-
-        self.server_afterStopping()
-        if self._app.signal.server_afterStopping.receivers:
-            self._app.signal.server_afterStopping.send()
-
-        logger.destroy()
+            self._app._handle.server_beforeStarting()
+            if self._app.signal.server_beforeStarting.receivers:
+                self._app.signal.server_beforeStarting.send()
 
-        os.killpg(os.getpid(), signal.SIGKILL)
+            try:
+                ipaddress.IPv4Address(self._app.server.host)
+                sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            except ipaddress.AddressValueError:
+                sock = socket.socket(socket.AF_INET6, socket.SOCK_STREAM)
+            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            sock.bind((self._app.server.host, self._app.server.port))
+            sock.listen(self._app.server.backlog)
+            sock.set_inheritable(True)
+
+            processes: List[multiprocessing.Process] = []
+            multiprocessing.allow_connection_pickling()
+            for i in range(self._app.server.workers - 1):
+                process = multiprocessing.Process(target = self.worker_start, args = (sock,), name = self._app._text.workerProcess_title)
+                process.start()
+                processes.append(process)
+
+            self.worker_start(sock, True)
+
+            for process in processes:
+                process.terminate()
+                process.join()
+
+            for text in self._app._text.server_stopping():
+                logger.ending(text[0], text[1])
+
+            self.server_afterStopping()
+            if self._app.signal.server_afterStopping.receivers:
+                self._app.signal.server_afterStopping.send()
+        except KeyboardInterrupt:
+            ...
+        except:
+            logger.error(f'''
+{logger.encode(traceback.format_exc()[:-1])}''')
+        finally:
+            logger.destroy()
+            os.killpg(os.getpid(), signal.SIGKILL)
 
     def worker_beforeStarting(self):
         for text in self._app._text.worker_starting():
             logger.debug(text[0], text[1])
 
     def worker_start(self, sock, master: bool = False):
-        if not master:
-            setproctitle.setproctitle(self._app._text.workerProcess_title)
-
-        self.worker_beforeStarting()
-        if self._app.signal.worker_beforeStarting.receivers:
-            self._app.signal.worker_beforeStarting.send()
-
-        asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-        asyncio.run(self.worker_run(sock, master))
-
-        with self._app._managers_['lock']:
-            self._app._managers_['server.workers'].value -= 1
-
-            for text in self._app._text.worker_stopping():
-                logger.debug(text[0], text[1])
+        try:
+            if not master:
+                setproctitle.setproctitle(self._app._text.workerProcess_title)
 
-            self.worker_afterStopping()
-            if self._app.signal.worker_afterStopping.receivers:
-                self._app.signal.worker_afterStopping.send()
+            self.worker_beforeStarting()
+            if self._app.signal.worker_beforeStarting.receivers:
+                self._app.signal.worker_beforeStarting.send()
+
+            asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+            asyncio.run(self.worker_run(sock, master))
+
+            with self._app._managers_['lock']:
+                self._app._managers_['server.workers'].value -= 1
+
+                for text in self._app._text.worker_stopping():
+                    logger.debug(text[0], text[1])
+
+                self.worker_afterStopping()
+                if self._app.signal.worker_afterStopping.receivers:
+                    self._app.signal.worker_afterStopping.send()
+        except:
+            logger.error(f'''The process {os.getpid()} stopped
+{logger.encode(traceback.format_exc()[:-1])}''', f'''The process <blue>{os.getpid()}</blue> stopped
+{logger.encode(traceback.format_exc()[:-1])}''')
 
     async def worker_run(self, sock, master: bool):
         from CheeseAPI.app import app
         from CheeseAPI.protocol import HttpProtocol
 
         app._g = self._app.g
         app._managers = self._app.managers
@@ -340,32 +350,32 @@
                 await self._app.signal.http_custom.async_send(**{
                     'request': protocol.request,
                     'response': protocol.response,
                     **protocol.kwargs
                 })
 
             await self.http_response(protocol)
-        except BaseException as e:
+        except Exception as e:
             try:
                 await self.http_500(protocol, e)
                 if self._app.signal.http_500.receivers:
                     await self._app.signal.http_500.async_send(**{
                         'request': protocol.request,
                         'response': protocol.response,
                         'e': e,
                         **protocol.kwargs
                     })
                 await self.http_response(protocol)
-            except BaseException as e:
+            except Exception as e:
                 await self.http_500(protocol, e, True)
                 await self.http_response(protocol, True)
 
     async def http_static(self, protocol: 'HttpProtocol'):
         if self._app.server.static and self._app.workspace.static and protocol.request.path.startswith(self._app.server.static) and protocol.request.method == http.HTTPMethod.GET:
-            for key in [ '', '.html', '/index.html' ]:
+            for key in [ '', '.html', 'index.html', '/index.html' ]:
                 try:
                     protocol.response = FileResponse(os.path.join(self._app.workspace.static, protocol.request.path[1:] + key))
 
                     await self.http_afterRequest(protocol)
                     if self._app.signal.http_afterRequest.receivers:
                         await self._app.signal.http_afterRequest.async_send(**{
                             'request': protocol.request,
```

### Comparing `cheeseapi-1.2.1/CheeseAPI/protocol.py` & `cheeseapi-1.2.2/CheeseAPI/protocol.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/request.py` & `cheeseapi-1.2.2/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/response.py` & `cheeseapi-1.2.2/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/route.py` & `cheeseapi-1.2.2/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/schedule.py` & `cheeseapi-1.2.2/CheeseAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/server.py` & `cheeseapi-1.2.2/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/signal.py` & `cheeseapi-1.2.2/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/text.py` & `cheeseapi-1.2.2/CheeseAPI/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,17 @@
 
 class Text:
     def __init__(self, app: 'App'):
         self._app: 'App' = app
         self.progressBar: ProgressBar = ProgressBar()
 
         self.response_server: str = 'CheeseAPI'
-        self._process_title: str = 'CheeseAPI'
-        self.workerProcess_title: str = 'CheeseAPI:Process'
+        self.workerProcess_title: str = f'{setproctitle.getproctitle()}:Process'
         self.logger: str = '%Y_%m_%d.log'
 
-        setproctitle.setproctitle(self._process_title)
-
     def server_information(self) -> List[Tuple[str, str]]:
         return [
             (f'The master process {os.getpid()} started', f'The master process <blue>{os.getpid()}</blue> started'),
             (f'''Workspace Information:
 Base: {self._app.workspace.base}''' + (f'''
 Static: {self._app.workspace.static}''' if self._app.workspace.static and self._app.server.static else '') + (f'''
 Log: {self._app.workspace.log}''' if self._app.workspace.log and self._app.workspace.logger else '') + (f'''
@@ -163,17 +160,7 @@
         return f'The {scope}.{key} cannot be less than {min}'
 
     def validator_maxMessage(self, scope: str, key: str, max: object) -> str:
         return f'The {scope}.{key} cannot be larger than {max}'
 
     def validator_enumMessage(self, scope: str, key: str, enum: List[Any]) -> str:
         return f'The {scope}.{key} cannot be a value other than {enum}'
-
-    @property
-    def process_title(self) -> str:
-        return self._process_title
-
-    @process_title.setter
-    def process_title(self, value: str):
-        self._process_title = value
-
-        setproctitle.setproctitle(self._process_title)
```

### Comparing `cheeseapi-1.2.1/CheeseAPI/validator.py` & `cheeseapi-1.2.2/CheeseAPI/validator.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/websocket.py` & `cheeseapi-1.2.2/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/CheeseAPI/workspace.py` & `cheeseapi-1.2.2/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/LICENSE` & `cheeseapi-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/README.md` & `cheeseapi-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.1/pyproject.toml` & `cheeseapi-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.2.1"
+version = "1.2.2"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-1.2.1/PKG-INFO` & `cheeseapi-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.2.1
+Version: 1.2.2
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: cheeselog==1.0.*
 Requires-Dist: cheesesignal==1.1.*
```

