# Comparing `tmp/aiokcp-0.0.2.tar.gz` & `tmp/aiokcp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokcp-0.0.2.tar", last modified: Tue May 21 02:09:53 2024, max compression
+gzip compressed data, was "aiokcp-0.0.3.tar", last modified: Tue May 21 02:19:40 2024, max compression
```

## Comparing `aiokcp-0.0.2.tar` & `aiokcp-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 02:09:53.049266 aiokcp-0.0.2/
--rw-rw-rw-   0        0        0     1088 2024-05-20 09:29:30.000000 aiokcp-0.0.2/LICENSE
--rw-rw-rw-   0        0        0    12498 2024-05-21 02:09:53.044265 aiokcp-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    11758 2024-05-20 11:51:58.000000 aiokcp-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 02:09:52.983939 aiokcp-0.0.2/aiokcp/
--rw-rw-rw-   0        0        0      290 2024-05-13 01:37:48.000000 aiokcp-0.0.2/aiokcp/__init__.py
--rw-rw-rw-   0        0        0    15318 2024-05-20 09:25:00.000000 aiokcp-0.0.2/aiokcp/core.py
--rw-rw-rw-   0        0        0     1383 2024-05-20 06:43:34.000000 aiokcp-0.0.2/aiokcp/crypto.py
--rw-rw-rw-   0        0        0      308 2024-05-13 08:47:58.000000 aiokcp-0.0.2/aiokcp/exceptions.py
--rw-rw-rw-   0        0        0    33114 2024-05-13 08:39:55.000000 aiokcp-0.0.2/aiokcp/ikcp.c
--rw-rw-rw-   0        0        0    12436 2024-05-13 08:40:42.000000 aiokcp-0.0.2/aiokcp/ikcp.h
--rw-rw-rw-   0        0        0   744822 2024-05-20 15:40:22.000000 aiokcp-0.0.2/aiokcp/kcp.c
--rw-rw-rw-   0        0        0     1870 2024-05-20 07:35:38.000000 aiokcp-0.0.2/aiokcp/kcp.pyi
--rw-rw-rw-   0        0        0     1275 2024-05-14 03:27:01.000000 aiokcp-0.0.2/aiokcp/stream.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:09:53.029940 aiokcp-0.0.2/aiokcp/sync/
--rw-rw-rw-   0        0        0      286 2024-05-15 12:41:39.000000 aiokcp-0.0.2/aiokcp/sync/__init__.py
--rw-rw-rw-   0        0        0     3639 2024-05-20 07:36:56.000000 aiokcp-0.0.2/aiokcp/sync/server.py
--rw-rw-rw-   0        0        0    15643 2024-05-20 08:16:00.000000 aiokcp-0.0.2/aiokcp/sync/sock.py
--rw-rw-rw-   0        0        0      301 2024-05-14 02:30:51.000000 aiokcp-0.0.2/aiokcp/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:09:53.038273 aiokcp-0.0.2/aiokcp.egg-info/
--rw-rw-rw-   0        0        0    12498 2024-05-21 02:09:52.000000 aiokcp-0.0.2/aiokcp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2024-05-21 02:09:52.000000 aiokcp-0.0.2/aiokcp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 02:09:52.000000 aiokcp-0.0.2/aiokcp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-21 02:09:52.000000 aiokcp-0.0.2/aiokcp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 02:09:52.000000 aiokcp-0.0.2/aiokcp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2024-05-21 02:09:08.000000 aiokcp-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 02:09:53.049266 aiokcp-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-05-21 02:09:25.000000 aiokcp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:19:40.516199 aiokcp-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-20 09:29:30.000000 aiokcp-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    12498 2024-05-21 02:19:40.510198 aiokcp-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11758 2024-05-20 11:51:58.000000 aiokcp-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 02:19:40.449152 aiokcp-0.0.3/aiokcp/
+-rw-rw-rw-   0        0        0      290 2024-05-13 01:37:48.000000 aiokcp-0.0.3/aiokcp/__init__.py
+-rw-rw-rw-   0        0        0    15330 2024-05-21 02:17:57.000000 aiokcp-0.0.3/aiokcp/core.py
+-rw-rw-rw-   0        0        0     1397 2024-05-21 02:18:10.000000 aiokcp-0.0.3/aiokcp/crypto.py
+-rw-rw-rw-   0        0        0      308 2024-05-13 08:47:58.000000 aiokcp-0.0.3/aiokcp/exceptions.py
+-rw-rw-rw-   0        0        0    33114 2024-05-13 08:39:55.000000 aiokcp-0.0.3/aiokcp/ikcp.c
+-rw-rw-rw-   0        0        0    12436 2024-05-13 08:40:42.000000 aiokcp-0.0.3/aiokcp/ikcp.h
+-rw-rw-rw-   0        0        0   744822 2024-05-20 15:40:22.000000 aiokcp-0.0.3/aiokcp/kcp.c
+-rw-rw-rw-   0        0        0     1870 2024-05-20 07:35:38.000000 aiokcp-0.0.3/aiokcp/kcp.pyi
+-rw-rw-rw-   0        0        0     1275 2024-05-14 03:27:01.000000 aiokcp-0.0.3/aiokcp/stream.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:19:40.497201 aiokcp-0.0.3/aiokcp/sync/
+-rw-rw-rw-   0        0        0      286 2024-05-15 12:41:39.000000 aiokcp-0.0.3/aiokcp/sync/__init__.py
+-rw-rw-rw-   0        0        0     3639 2024-05-20 07:36:56.000000 aiokcp-0.0.3/aiokcp/sync/server.py
+-rw-rw-rw-   0        0        0    15660 2024-05-21 02:16:51.000000 aiokcp-0.0.3/aiokcp/sync/sock.py
+-rw-rw-rw-   0        0        0      301 2024-05-21 02:18:28.000000 aiokcp-0.0.3/aiokcp/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:19:40.505200 aiokcp-0.0.3/aiokcp.egg-info/
+-rw-rw-rw-   0        0        0    12498 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2024-05-21 02:19:15.000000 aiokcp-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 02:19:40.516199 aiokcp-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      637 2024-05-21 02:09:25.000000 aiokcp-0.0.3/setup.py
```

### Comparing `aiokcp-0.0.2/LICENSE` & `aiokcp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.2/PKG-INFO` & `aiokcp-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokcp
-Version: 0.0.2
+Version: 0.0.3
 Summary: KCP for asyncio and socketserver, based on kcp
 Author: ryanrain2016
 Author-email: ryanrain2016 <holidaylover2010@gmail.com>
 Project-URL: Homepage, https://github.com/ryanrain2016/aiokcp
 Project-URL: Issues, https://github.com/ryanrain2016/aiokcp/issues
 Keywords: asyncio,kcp,socket,aio,aiokcp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiokcp-0.0.2/README.md` & `aiokcp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.2/aiokcp/core.py` & `aiokcp-0.0.3/aiokcp/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import logging
 import time
 from dataclasses import dataclass
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 from .kcp import KCP
 from .utils import conv_bytes_to_id, random_id
 
 __all__ = ['create_connection', 'create_server', 'KCPStreamTransport', 'KCPServer']
 
 default_update_interval = 100  # ms
@@ -109,15 +109,15 @@
 
     def resume_reading(self) -> None:
         self._is_reading = True
         if self.protocol is not None:
             for data in self.kcp.get_all_received():
                 self.protocol.data_received(data)
 
-    def write(self, data: bytes | bytearray | memoryview) -> None:
+    def write(self, data: Union[bytes, bytearray, memoryview]) -> None:
         if not data or self.is_closing():
             return
         data = bytes(data)
         self.kcp.enqueue(data)
         self.kcp.update(int(time.perf_counter() * 1000))
         self.__update_activity()
```

### Comparing `aiokcp-0.0.2/aiokcp/crypto.py` & `aiokcp-0.0.3/aiokcp/crypto.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         key = PBKDF2HMAC(algorithm=hashes.SHA256(),
                                 length=32,
                                 salt=salt,
                                 iterations=100000).derive(key)
         return Fernet(base64.urlsafe_b64encode(key))
 
     class CryptoWrapper:
-        def __init__(self, key, salt):
+        def __init__(self, key: bytes, salt: bytes):
             self._crypto = _get_crypto(key, salt)
 
         def encrypt(self, data):
             data = self._crypto.encrypt(data)
             return base64.urlsafe_b64decode(data)
 
         def decrypt(self, data):
```

### Comparing `aiokcp-0.0.2/aiokcp/ikcp.c` & `aiokcp-0.0.3/aiokcp/ikcp.c`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.2/aiokcp/ikcp.h` & `aiokcp-0.0.3/aiokcp/ikcp.h`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.2/aiokcp/kcp.c` & `aiokcp-0.0.3/aiokcp/kcp.c`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.2/aiokcp/kcp.pyi` & `aiokcp-0.0.3/aiokcp/kcp.pyi`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.2/aiokcp/stream.py` & `aiokcp-0.0.3/aiokcp/stream.py`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.2/aiokcp/sync/server.py` & `aiokcp-0.0.3/aiokcp/sync/server.py`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.2/aiokcp/sync/sock.py` & `aiokcp-0.0.3/aiokcp/sync/sock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import enum
 import socket
 import threading
 import time
 from queue import PriorityQueue, Queue
-from typing import Optional
+from typing import Optional, Union
 
 from ..core import default_kcp_kwargs, default_timeout
 from ..kcp import KCP
 from ..utils import conv_bytes_to_id, random_id
 
 __all__ = ['KCPSocket', 'KCPSocketType']
 
@@ -317,21 +317,21 @@
                 view[:nbytes] = self._buffer[:nbytes]
                 if not (flags & socket.MSG_PEEK):
                     self._buffer = self._buffer[nbytes:]
                 return nbytes
             self._recv_condition.wait_for(lambda: self._buffer or self._is_closing, 10)
         return self.recv_into(buffer, nbytes, flags)
 
-    def sendall(self, data: bytes | bytearray | memoryview, flags=0):
+    def sendall(self, data: Union[bytes, bytearray, memoryview], flags=0):
         while data:
             sent = self.send(data, flags)
             data = data[sent:]
         return
 
-    def send(self, data: bytes | bytearray | memoryview, flags=0):
+    def send(self, data: Union[bytes, bytearray, memoryview], flags=0):
         if self._is_closing:
             return 0
         data = bytes(data)
         with self._kcp_lock:
             n = self.kcp.enqueue(data)
             self.kcp.update(int(time.perf_counter() * 1000))
             return n
```

### Comparing `aiokcp-0.0.2/aiokcp.egg-info/PKG-INFO` & `aiokcp-0.0.3/aiokcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokcp
-Version: 0.0.2
+Version: 0.0.3
 Summary: KCP for asyncio and socketserver, based on kcp
 Author: ryanrain2016
 Author-email: ryanrain2016 <holidaylover2010@gmail.com>
 Project-URL: Homepage, https://github.com/ryanrain2016/aiokcp
 Project-URL: Issues, https://github.com/ryanrain2016/aiokcp/issues
 Keywords: asyncio,kcp,socket,aio,aiokcp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiokcp-0.0.2/pyproject.toml` & `aiokcp-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiokcp"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="ryanrain2016", email="holidaylover2010@gmail.com" },
 ]
 description = "KCP for asyncio and socketserver, based on kcp"
 readme = "README.md"
 
 requires-python = ">=3.8"
```

### Comparing `aiokcp-0.0.2/setup.py` & `aiokcp-0.0.3/setup.py`

 * *Files identical despite different names*

