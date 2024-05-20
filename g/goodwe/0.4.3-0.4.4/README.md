# Comparing `tmp/goodwe-0.4.3.tar.gz` & `tmp/goodwe-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodwe-0.4.3.tar", last modified: Sun May 19 18:21:52 2024, max compression
+gzip compressed data, was "goodwe-0.4.4.tar", last modified: Mon May 20 21:59:00 2024, max compression
```

## Comparing `goodwe-0.4.3.tar` & `goodwe-0.4.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:21:52.662389 goodwe-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-19 18:21:40.000000 goodwe-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-19 18:21:52.662389 goodwe-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-19 18:21:40.000000 goodwe-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 18:21:48.000000 goodwe-0.4.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:21:52.658389 goodwe-0.4.3/goodwe/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    43890 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/et.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/inverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    28306 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    37679 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:21:52.662389 goodwe-0.4.3/goodwe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-19 18:21:52.000000 goodwe-0.4.3/goodwe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 18:21:52.000000 goodwe-0.4.3/goodwe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:21:52.000000 goodwe-0.4.3/goodwe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 18:21:52.000000 goodwe-0.4.3/goodwe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-19 18:21:40.000000 goodwe-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-19 18:21:52.662389 goodwe-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:21:52.662389 goodwe-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    29883 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    73945 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_et.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:59:00.463199 goodwe-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 21:58:53.000000 goodwe-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-20 21:59:00.463199 goodwe-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-20 21:58:53.000000 goodwe-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 21:58:57.000000 goodwe-0.4.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:59:00.463199 goodwe-0.4.4/goodwe/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43890 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28563 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37679 2024-05-20 21:58:53.000000 goodwe-0.4.4/goodwe/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:59:00.463199 goodwe-0.4.4/goodwe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-20 21:59:00.000000 goodwe-0.4.4/goodwe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-20 21:59:00.000000 goodwe-0.4.4/goodwe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:59:00.000000 goodwe-0.4.4/goodwe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 21:59:00.000000 goodwe-0.4.4/goodwe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 21:58:53.000000 goodwe-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-20 21:59:00.463199 goodwe-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:59:00.463199 goodwe-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-05-20 21:58:53.000000 goodwe-0.4.4/tests/test_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29883 2024-05-20 21:58:53.000000 goodwe-0.4.4/tests/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73945 2024-05-20 21:58:53.000000 goodwe-0.4.4/tests/test_et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-20 21:58:53.000000 goodwe-0.4.4/tests/test_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-20 21:58:53.000000 goodwe-0.4.4/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-05-20 21:58:53.000000 goodwe-0.4.4/tests/test_sensor.py
```

### Comparing `goodwe-0.4.3/LICENSE` & `goodwe-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/PKG-INFO` & `goodwe-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.4.3
+Version: 0.4.4
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.4.3/README.md` & `goodwe-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe/__init__.py` & `goodwe-0.4.4/goodwe/__init__.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe/const.py` & `goodwe-0.4.4/goodwe/const.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe/dt.py` & `goodwe-0.4.4/goodwe/dt.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe/es.py` & `goodwe-0.4.4/goodwe/es.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe/et.py` & `goodwe-0.4.4/goodwe/et.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe/exceptions.py` & `goodwe-0.4.4/goodwe/exceptions.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe/inverter.py` & `goodwe-0.4.4/goodwe/inverter.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe/modbus.py` & `goodwe-0.4.4/goodwe/modbus.py`

 * *Files 5% similar despite different names*

```diff
@@ -217,30 +217,31 @@
     data[6] is source address
     data[7] is command return type
     data[8] is response payload length (for read commands)
     """
     if len(data) <= 8:
         logger.debug("Response is too short.")
         return False
-    expected_length = int.from_bytes(data[4:6], byteorder='big', signed=False) + 6
-    # The weird expected_length != 12 is work around Goodwe bug answering wrong (hardcoded 6) length.
-    if len(data) < expected_length and expected_length != 12:
-        raise PartialResponseException(len(data), expected_length)
+
+    # The Modbus/TCP message length check is completely ignore due to Goodwe bugs
+    # expected_length = int.from_bytes(data[4:6], byteorder='big', signed=False) + 6
+    # if len(data) < expected_length:
+    #    raise PartialResponseException(len(data), expected_length)
 
     if data[7] == MODBUS_READ_CMD:
         expected_length = data[8] + 9
         if len(data) < expected_length:
             raise PartialResponseException(len(data), expected_length)
         if data[8] != value * 2:
             logger.debug("Response has unexpected length: %d, expected %d.", data[8], value * 2)
             return False
     elif data[7] in (MODBUS_WRITE_CMD, MODBUS_WRITE_MULTI_CMD):
         if len(data) < 12:
-            logger.debug("Response has unexpected length: %d, expected %d.", len(data), 14)
-            raise PartialResponseException(len(data), expected_length)
+            logger.debug("Response has unexpected length: %d, expected %d.", len(data), 12)
+            return False
         response_offset = int.from_bytes(data[8:10], byteorder='big', signed=False)
         if response_offset != offset:
             logger.debug("Response has wrong offset: %X, expected %X.", response_offset, offset)
             return False
         response_value = int.from_bytes(data[10:12], byteorder='big', signed=True)
         if response_value != value:
             logger.debug("Response has wrong value: %X, expected %X.", response_value, value)
```

### Comparing `goodwe-0.4.3/goodwe/model.py` & `goodwe-0.4.4/goodwe/model.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe/protocol.py` & `goodwe-0.4.4/goodwe/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         self.timeout: int = timeout
         self.retries: int = retries
         self.keep_alive: bool = True
         self.protocol: asyncio.Protocol | None = None
         self.response_future: Future | None = None
         self.command: ProtocolCommand | None = None
         self._partial_data: bytes | None = None
+        self._partial_missing: int = 0
 
     def _ensure_lock(self) -> asyncio.Lock:
         """Validate (or create) asyncio Lock.
 
            The asyncio.Lock must always be created from within's asyncio loop,
            so it cannot be eagerly created in constructor.
            Additionally, since asyncio.run() creates and closes its own loop,
@@ -121,31 +122,29 @@
 
     def datagram_received(self, data: bytes, addr: Tuple[str, int]) -> None:
         """On datagram received"""
         if self._timer:
             self._timer.cancel()
             self._timer = None
         try:
-            if self._partial_data:
-                logger.debug("Received another response fragment: %s.", data.hex())
+            if self._partial_data and self._partial_missing == len(data):
+                logger.debug("Composed fragmented response: %s + %s", self._partial_data.hex(), data.hex())
                 data = self._partial_data + data
-            if self.command.validator(data):
-                if self._partial_data:
-                    logger.debug("Composed fragmented response: %s", data.hex())
-                else:
-                    logger.debug("Received: %s", data.hex())
                 self._partial_data = None
+                self._partial_missing = 0
+            if self.command.validator(data):
+                logger.debug("Received: %s", data.hex())
                 self.response_future.set_result(data)
             else:
                 logger.debug("Received invalid response: %s", data.hex())
                 asyncio.get_running_loop().call_soon(self._retry_mechanism)
-        except PartialResponseException:
-            logger.debug("Received response fragment: %s", data.hex())
+        except PartialResponseException as ex:
+            logger.debug("Received response fragment (%d of %d): %s", ex.length, ex.expected, data.hex())
             self._partial_data = data
-            return
+            self._partial_missing = ex.expected - ex.length
         except asyncio.InvalidStateError:
             logger.debug("Response already handled: %s", data.hex())
         except RequestRejectedException as ex:
             logger.debug("Received exception response: %s", data.hex())
             self.response_future.set_exception(ex)
             self._close_transport()
 
@@ -165,14 +164,16 @@
             await response_future
             return response_future
 
     def _send_request(self, command: ProtocolCommand, response_future: Future) -> None:
         """Send message via transport"""
         self.command = command
         self.response_future = response_future
+        self._partial_data = None
+        self._partial_missing = 0
         payload = command.request_bytes()
         if self._retry > 0:
             logger.debug("Sending: %s - retry #%s/%s", self.command, self._retry, self.retries)
         else:
             logger.debug("Sending: %s", self.command)
         self._transport.sendto(payload)
         self._timer = asyncio.get_running_loop().call_later(self.timeout, self._retry_mechanism)
@@ -262,33 +263,31 @@
         self._close_transport()
 
     def data_received(self, data: bytes) -> None:
         """On data received"""
         if self._timer:
             self._timer.cancel()
         try:
-            if self._partial_data:
-                logger.debug("Received another response fragment: %s.", data.hex())
+            if self._partial_data and self._partial_missing == len(data):
+                logger.debug("Composed fragmented response: %s + %s", self._partial_data.hex(), data.hex())
                 data = self._partial_data + data
+                self._partial_data = None
+                self._partial_missing = 0
             if self.command.validator(data):
-                if self._partial_data:
-                    logger.debug("Composed fragmented response: %s", data.hex())
-                else:
-                    logger.debug("Received: %s", data.hex())
+                logger.debug("Received: %s", data.hex())
                 self._retry = 0
-                self._partial_data = None
                 self.response_future.set_result(data)
             else:
                 logger.debug("Received invalid response: %s", data.hex())
                 self.response_future.set_exception(RequestRejectedException())
                 self._close_transport()
-        except PartialResponseException:
-            logger.debug("Received response fragment: %s", data.hex())
+        except PartialResponseException as ex:
+            logger.debug("Received response fragment (%d of %d): %s", ex.length, ex.expected, data.hex())
             self._partial_data = data
-            return
+            self._partial_missing = ex.expected - ex.length
         except asyncio.InvalidStateError:
             logger.debug("Response already handled: %s", data.hex())
         except RequestRejectedException as ex:
             logger.debug("Received exception response: %s", data.hex())
             self.response_future.set_exception(ex)
             # self._close_transport()
 
@@ -331,14 +330,16 @@
             if self._lock and self._lock.locked():
                 self._lock.release()
 
     def _send_request(self, command: ProtocolCommand, response_future: Future) -> None:
         """Send message via transport"""
         self.command = command
         self.response_future = response_future
+        self._partial_data = None
+        self._partial_missing = 0
         payload = command.request_bytes()
         if self._retry > 0:
             logger.debug("Sending: %s - retry #%s/%s", self.command, self._retry, self.retries)
         else:
             logger.debug("Sending: %s", self.command)
         self._transport.write(payload)
         self._timer = asyncio.get_running_loop().call_later(self.timeout, self._timeout_mechanism)
```

### Comparing `goodwe-0.4.3/goodwe/sensor.py` & `goodwe-0.4.4/goodwe/sensor.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/goodwe.egg-info/PKG-INFO` & `goodwe-0.4.4/goodwe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.4.3
+Version: 0.4.4
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.4.3/setup.cfg` & `goodwe-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/tests/test_dt.py` & `goodwe-0.4.4/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/tests/test_es.py` & `goodwe-0.4.4/tests/test_es.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/tests/test_et.py` & `goodwe-0.4.4/tests/test_et.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/tests/test_modbus.py` & `goodwe-0.4.4/tests/test_modbus.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/tests/test_protocol.py` & `goodwe-0.4.4/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.3/tests/test_sensor.py` & `goodwe-0.4.4/tests/test_sensor.py`

 * *Files identical despite different names*

