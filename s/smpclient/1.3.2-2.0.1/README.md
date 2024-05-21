# Comparing `tmp/smpclient-1.3.2.tar.gz` & `tmp/smpclient-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpclient-1.3.2.tar", max compression
+gzip compressed data, was "smpclient-2.0.1.tar", max compression
```

## Comparing `smpclient-1.3.2.tar` & `smpclient-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11421 2024-04-24 23:33:42.875688 smpclient-1.3.2/LICENSE
--rw-r--r--   0        0        0     2433 2024-04-24 23:33:42.875688 smpclient-1.3.2/README.md
--rw-r--r--   0        0        0     1081 2024-04-24 23:33:42.875688 smpclient-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     6022 2024-04-24 23:33:42.875688 smpclient-1.3.2/smpclient/__init__.py
--rw-r--r--   0        0        0      188 2024-04-24 23:33:42.875688 smpclient-1.3.2/smpclient/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/extensions/__init__.py
--rw-r--r--   0        0        0     2489 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/extensions/intercreate.py
--rw-r--r--   0        0        0     2750 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/generics.py
--rw-r--r--   0        0        0     8285 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/mcuboot.py
--rw-r--r--   0        0        0        0 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/py.typed
--rw-r--r--   0        0        0        0 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/__init__.py
--rw-r--r--   0        0        0      808 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/image_management.py
--rw-r--r--   0        0        0      599 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/os_management.py
--rw-r--r--   0        0        0      529 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/shell_management.py
--rw-r--r--   0        0        0        0 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/user/__init__.py
--rw-r--r--   0        0        0      457 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/user/intercreate.py
--rw-r--r--   0        0        0     1048 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/transport/__init__.py
--rw-r--r--   0        0        0     5537 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/transport/ble.py
--rw-r--r--   0        0        0     9514 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/transport/serial.py
--rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 smpclient-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11421 2024-05-21 00:24:58.233728 smpclient-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2501 2024-05-21 00:24:58.233728 smpclient-2.0.1/README.md
+-rw-r--r--   0        0        0     1822 2024-05-21 00:24:58.257728 smpclient-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7260 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/__init__.py
+-rw-r--r--   0        0        0      188 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/extensions/__init__.py
+-rw-r--r--   0        0        0     2473 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/extensions/intercreate.py
+-rw-r--r--   0        0        0     2836 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/generics.py
+-rw-r--r--   0        0        0     8321 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/mcuboot.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/py.typed
+-rw-r--r--   0        0        0        0 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/__init__.py
+-rw-r--r--   0        0        0      860 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/image_management.py
+-rw-r--r--   0        0        0     1444 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/os_management.py
+-rw-r--r--   0        0        0      494 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/shell_management.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/user/__init__.py
+-rw-r--r--   0        0        0      420 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/user/intercreate.py
+-rw-r--r--   0        0        0     2290 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/transport/__init__.py
+-rw-r--r--   0        0        0     6845 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/transport/ble.py
+-rw-r--r--   0        0        0     9663 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/transport/serial.py
+-rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 smpclient-2.0.1/PKG-INFO
```

### Comparing `smpclient-1.3.2/LICENSE` & `smpclient-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.2/README.md` & `smpclient-2.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,24 @@
    ```
    poetry add <my_new_dependency>
    ```
 6. add test or other development dependencies using [poetry groups](https://python-poetry.org/docs/managing-dependencies#dependency-groups):
    ```
    poetry add -G dev <my_dev_dependency>
    ```
+7. run tests for all supported python versions:
+   ```
+   tox
+   ```
 
 ## Development Environment Setup
 
 ### Install Dependencies
 
-- python >=3.10, <3.13
+- python >=3.8, <3.13
 - poetry: https://python-poetry.org/docs/#installation
 
 ### Create the venv
 
 ```
 poetry install
 ```
```

### Comparing `smpclient-1.3.2/pyproject.toml` & `smpclient-2.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -15,42 +15,82 @@
 [tool.poetry.scripts]
 mcuimg = "smpclient.mcuboot:mcuimg"
 
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.dependencies]
-python = ">=3.10, <3.13"
+python = ">=3.8.1, <3.13"
 pyserial = "^3.5"
-smp = "^0.3.4"
+smp = "^1.0.1"
 intelhex = "^2.3.0"
-bleak = "^0.21.1"
-
+bleak = "^0.22.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 black = "^23.11.0"
 flake8 = "^6.1.0"
 isort = "^5.12.0"
 mypy = "^1.7.0"
 mypy-extensions = "^1.0.0"
 pytest-asyncio = "^0.23.2"
 types-pyserial = "^3.5.0.11"
+tox = "^4.15.0"
 
 [tool.black]
 line-length = 100
-skip-string-normalization = 1
+skip-string-normalization = true
+extend-exclude = "dutfirmware|.venv|tests/fixtures|.tox"
 
 [tool.isort]
 profile = "black"
 line_length = 100
 multi_line_output = 3
+skip = [
+    ".venv",
+    "dutfirmware",
+    ".tox",
+]
 
 [tool.mypy]
 disallow_untyped_defs = true
-exclude = ['.venv']
+exclude = ['.venv', 'dutfirmware', '.tox']
 
 [tool.pytest.ini_options]
+norecursedirs = "dutfirmware/*"
 filterwarnings = [
     "ignore:The --rsyncdir:DeprecationWarning",
-]
+]
+
+[tool.tox]
+legacy_tox_ini = """
+    [tox]
+    min_version = 4.15
+    env_list =
+        py38
+        py39
+        py310
+        py311
+        py312
+
+    [testenv]
+    allowlist_externals =
+        poetry
+        black
+        isort
+        flake8
+        mypy
+        coverage
+    commands = 
+        poetry install
+        black --check .
+        isort --check-only .
+        flake8 .
+        mypy .
+        coverage erase
+        pytest --cov --maxfail=1
+"""
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `smpclient-1.3.2/smpclient/__init__.py` & `smpclient-2.0.1/smpclient/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """Simple Management Protocol (SMP) Client."""
 
+from __future__ import annotations
+
+import logging
 from hashlib import sha256
-from typing import AsyncIterator, Final, Tuple, cast
+from types import TracebackType
+from typing import AsyncIterator, Final, Tuple, Type, cast
 
 from pydantic import ValidationError
 from smp import header as smpheader
 from smp import message as smpmsg
 
 from smpclient.exceptions import SMPBadSequence, SMPUploadError
 from smpclient.generics import SMPRequest, TEr0, TEr1, TErr, TRep, error, flatten_error, success
 from smpclient.requests.image_management import ImageUploadWrite
+from smpclient.requests.os_management import MCUMgrParametersRead
 from smpclient.transport import SMPTransport
 
+logger = logging.getLogger(__name__)
+
 
 class SMPClient:
     def __init__(self, transport: SMPTransport, address: str):
         """Create a client to the SMP server `address`, using `transport`."""
         self._transport: Final = transport
         self._address: Final = address
 
     async def connect(self) -> None:
         """Connect to the SMP server."""
         await self._transport.connect(self._address)
+        await self._initialize()
 
     async def disconnect(self) -> None:
         """Disconnect from the SMP server."""
         await self._transport.disconnect()
 
     async def request(self, request: SMPRequest[TRep, TEr0, TEr1, TErr]) -> TRep | TErr:
         """Make an `SMPRequest` to the SMP server."""
@@ -34,72 +42,83 @@
 
         header = smpheader.Header.loads(frame[: smpheader.Header.SIZE])
 
         if header.sequence != request.header.sequence:  # type: ignore
             raise SMPBadSequence("Bad sequence")
 
         try:
-            return request.Response.loads(frame)  # type: ignore
+            return request._Response.loads(frame)  # type: ignore
         except ValidationError:
             return flatten_error(  # type: ignore
-                request.ErrorV0.loads(frame)
+                request._ErrorV0.loads(frame)
                 if header.version == smpheader.Version.V0
-                else request.ErrorV1.loads(frame)
+                else request._ErrorV1.loads(frame)
             )
 
     async def upload(
         self, image: bytes, slot: int = 0, upgrade: bool = False
     ) -> AsyncIterator[int]:
         """Iteratively upload an `image` to `slot`, yielding the offset."""
 
         if self._transport.max_unencoded_size < 23:
             raise Exception("Upload requires an MTU >=23.")
 
         response = await self.request(
             self._maximize_packet(
-                ImageUploadWrite(  # type: ignore
+                ImageUploadWrite(
                     off=0,
-                    data=b'',
+                    data=b"",
                     image=slot,
                     len=len(image),
                     sha=sha256(image).digest(),
                     upgrade=upgrade,
                 ),
                 image,
             )
         )
 
         if error(response):
             raise SMPUploadError(response)
         elif success(response):
+            if response.off is None:
+                raise SMPUploadError(f"No offset received: {response=}")
             yield response.off
         else:  # pragma: no cover
             raise Exception("Unreachable")
 
         # send chunks until the SMP server reports that the offset is at the end of the image
         while response.off != len(image):
             response = await self.request(
-                self._maximize_packet(ImageUploadWrite(off=response.off, data=b''), image)
+                self._maximize_packet(ImageUploadWrite(off=response.off, data=b""), image)
             )
             if error(response):
                 raise SMPUploadError(response)
             elif success(response):
+                if response.off is None:
+                    raise SMPUploadError(f"No offset received: {response=}")
                 yield response.off
             else:  # pragma: no cover
                 raise Exception("Unreachable")
 
     @property
     def address(self) -> str:
         return self._address
 
-    async def __aenter__(self) -> 'SMPClient':
+    async def __aenter__(self) -> "SMPClient":
         await self.connect()
         return self
 
-    async def __aexit__(self) -> None:
+    async def __aexit__(
+        self,
+        exc_type: Type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
+    ) -> None:
+        if exc_value is not None:
+            logger.error(f"Exception in SMPClient: {exc_type=}, {exc_value=}, {traceback=}")
         await self.disconnect()
 
     @staticmethod
     def _cbor_integer_size(integer: int) -> int:
         """CBOR integers are packed as small as possible."""
 
         # If the integer is less than 24, then the size is encoded in the same
@@ -153,7 +172,19 @@
             off=request.off,
             data=image[request.off : request.off + data_size],
             image=request.image,
             len=request.len,
             sha=request.sha,
             upgrade=request.upgrade,
         )
+
+    async def _initialize(self) -> None:
+        """Gather initialization information from the SMP server."""
+
+        mcumgr_parameters = await self.request(MCUMgrParametersRead())
+        if success(mcumgr_parameters):
+            logger.debug(f"MCUMgr parameters: {mcumgr_parameters}")
+            self._transport.initialize(mcumgr_parameters.buf_size)
+        elif error(mcumgr_parameters):
+            logger.error(f"MCUMgr parameters error: {mcumgr_parameters}")
+        else:
+            raise Exception("Unreachable")
```

### Comparing `smpclient-1.3.2/smpclient/extensions/intercreate.py` & `smpclient-2.0.1/smpclient/extensions/intercreate.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class ICUploadClient(SMPClient):
     """Support for Intercreate Group Upload."""
 
     async def ic_upload(self, data: bytes, image: int = 0) -> AsyncIterator[int]:
         """Iteratively upload `data` to the SMP server, yielding the offset."""
 
         response = await self.request(
-            ic.ImageUploadWrite(off=0, data=b'', image=image, len=len(data))  # type: ignore
+            ic.ImageUploadWrite(off=0, data=b'', image=image, len=len(data))
         )
 
         if error(response):
             raise SMPUploadError(response)
         elif success(response):
             yield response.off
         else:  # pragma: no cover
```

### Comparing `smpclient-1.3.2/smpclient/generics.py` & `smpclient-2.0.1/smpclient/generics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Some Generic helpers for the SMP module."""
 
+from __future__ import annotations
+
 from enum import IntEnum
-from typing import Protocol, Type, TypeGuard, TypeVar
+from typing import Protocol, Type, TypeVar, Union
 
 from smp import error as smperror
 from smp import header as smpheader
 from smp import message as smpmessage
+from typing_extensions import TypeGuard
 
 TErrEnum = TypeVar("TErrEnum", bound=IntEnum)
 TEr0 = TypeVar("TEr0", bound=smperror.ErrorV0)
 TEr1 = TypeVar("TEr1", bound=smperror.ErrorV1)
 TErr = TypeVar("TErr", bound='SMPError')
-TRep = TypeVar("TRep", bound=smpmessage.ReadResponse | smpmessage.WriteResponse)
+TRep = TypeVar("TRep", bound=Union[smpmessage.ReadResponse, smpmessage.WriteResponse])
 
 
 class SMPError(smperror.ErrorV0[TErrEnum]):
     """An abstraction on top of SMP that joins and flattens V0 and V1 `Error`s"""
 
     group: smpheader.GroupId | None = None
 
@@ -49,25 +52,25 @@
     Example:
     ```python
     class ImageManagementError(SMPError[smpimg.IMG_MGMT_ERR]):
         _GROUP_ID = smpheader.GroupId.IMAGE_MANAGEMENT
 
 
     class ImageStatesRead(smpimg.ImageStatesReadRequest):
-        Response = smpimg.ImageStatesReadResponse
-        ErrorV0 = smpimg.ImageManagementError1
-        ErrorV1 = smpimg.ImageManagementError2
-        Error = ImageManagementError
+        _Response = smpimg.ImageStatesReadResponse
+        _ErrorV0 = smpimg.ImageManagementError1
+        _ErrorV1 = smpimg.ImageManagementError2
+        _Error = ImageManagementError
     ```
     """
 
-    Response: Type[TRep]
-    ErrorV0: Type[TEr0]
-    ErrorV1: Type[TEr1]
-    Error: Type[TErr]
+    _Response: Type[TRep]
+    _ErrorV0: Type[TEr0]
+    _ErrorV1: Type[TEr1]
+    _Error: Type[TErr]
 
     @property
     def BYTES(self) -> bytes:  # pragma: no cover
         ...
 
 
 def error(response: TErr | TRep) -> TypeGuard[TErr]:
```

### Comparing `smpclient-1.3.2/smpclient/mcuboot.py` & `smpclient-2.0.1/smpclient/mcuboot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Tools for inspecting firmware images.
 
 Specification: https://docs.mcuboot.com/design.html
 """
 
+from __future__ import annotations
+
 import argparse
 import pathlib
 import struct
 from enum import IntEnum, IntFlag, unique
 from functools import cached_property
 from io import BufferedReader, BytesIO
 from typing import Dict, Final, List
```

### Comparing `smpclient-1.3.2/smpclient/requests/image_management.py` & `smpclient-2.0.1/smpclient/requests/image_management.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from typing import ClassVar
-
 from smp import header as smpheader
 from smp import image_management as smpimg
 
 from smpclient.generics import SMPError
 
 
 class ImageManagementError(SMPError[smpimg.IMG_MGMT_ERR]):
     _GROUP_ID = smpheader.GroupId.IMAGE_MANAGEMENT
 
 
 class _ImageGroupBase:
-    ErrorV0 = smpimg.ImageManagementErrorV0
-    ErrorV1 = smpimg.ImageManagementErrorV1
-    Error = ImageManagementError
+    _ErrorV0 = smpimg.ImageManagementErrorV0
+    _ErrorV1 = smpimg.ImageManagementErrorV1
+    _Error = ImageManagementError
 
 
 class ImageStatesRead(smpimg.ImageStatesReadRequest, _ImageGroupBase):
-    Response: ClassVar = smpimg.ImageStatesReadResponse
+    _Response = smpimg.ImageStatesReadResponse
 
 
 class ImageStatesWrite(smpimg.ImageStatesWriteRequest, _ImageGroupBase):
-    Response: ClassVar = smpimg.ImageStatesWriteResponse
+    _Response = smpimg.ImageStatesWriteResponse
 
 
 class ImageUploadWrite(smpimg.ImageUploadWriteRequest, _ImageGroupBase):
-    Response: ClassVar = smpimg.ImageUploadProgressWriteResponse
+    _Response = smpimg.ImageUploadProgressWriteResponse
+
+
+class ImageErase(smpimg.ImageEraseRequest, _ImageGroupBase):
+    _Response = smpimg.ImageEraseResponse
```

### Comparing `smpclient-1.3.2/smpclient/transport/ble.py` & `smpclient-2.0.1/smpclient/transport/ble.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """A Bluetooth Low Energy (BLE) SMPTransport."""
 
+from __future__ import annotations
+
 import asyncio
 import logging
+import platform
 import re
-from typing import Final
+from typing import Final, List
 from uuid import UUID
 
 from bleak import BleakClient, BleakGATTCharacteristic, BleakScanner
 from bleak.backends.device import BLEDevice
 from smp import header as smphdr
 
 from smpclient.exceptions import SMPClientException
+from smpclient.transport import SMPTransport
 
 SMP_SERVICE_UUID: Final = UUID("8D53DC1D-1DB7-4CD3-868B-8A527460AA84")
 SMP_CHARACTERISTIC_UUID: Final = UUID("DA2E7828-FBCE-4E01-AE9E-261174997C48")
 
-MAC_ADDRESS_PATTERN: Final = re.compile(r'([0-9A-F]{2}[:]){5}[0-9A-F]{2}$', flags=re.IGNORECASE)
+MAC_ADDRESS_PATTERN: Final = re.compile(r"([0-9A-F]{2}[:]){5}[0-9A-F]{2}$", flags=re.IGNORECASE)
 UUID_PATTERN: Final = re.compile(
-    r'^[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}\Z',
+    r"^[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}\Z",
     flags=re.IGNORECASE,
 )
 
 
 class SMPBLETransportException(SMPClientException):
     ...
 
@@ -33,23 +37,23 @@
 class SMPBLETransportNotSMPServer(SMPBLETransportException):
     ...
 
 
 logger = logging.getLogger(__name__)
 
 
-class SMPBLETransport:
+class SMPBLETransport(SMPTransport):
     def __init__(self) -> None:
         self._buffer = bytearray()
         self._notify_condition = asyncio.Condition()
         logger.debug(f"Initialized {self.__class__.__name__}")
 
     async def connect(self, address: str) -> None:
         logger.debug(f"Scanning for {address=}")
-        device = (
+        device: BLEDevice | None = (
             await BleakScanner.find_device_by_address(address)  # type: ignore # upstream fix
             if MAC_ADDRESS_PATTERN.match(address) or UUID_PATTERN.match(address)
             else await BleakScanner.find_device_by_name(address)  # type: ignore # upstream fix
         )
 
         if type(device) is BLEDevice:
             self._client = BleakClient(device, services=(str(SMP_SERVICE_UUID),))
@@ -60,29 +64,42 @@
         await self._client.connect()
         logger.debug(f"Connected to {device=}")
 
         smp_characteristic = self._client.services.get_characteristic(SMP_CHARACTERISTIC_UUID)
         if smp_characteristic is None:
             raise SMPBLETransportNotSMPServer("Missing the SMP characteristic UUID.")
         else:
+            logger.debug(f"Found SMP characteristic: {smp_characteristic=}")
+            logger.info(f"{smp_characteristic.max_write_without_response_size=}")
+            if (
+                platform.system() == "Windows"
+                and smp_characteristic.max_write_without_response_size == 20
+            ):
+                # https://github.com/hbldh/bleak/pull/1552#issuecomment-2105573291
+                logger.warning(
+                    "The SMP characteristic MTU is 20 bytes, possibly a Windows bug, checking again"
+                )
+                await asyncio.sleep(2)
+                smp_characteristic._max_write_without_response_size = (
+                    self._client._backend._session.max_pdu_size - 3  # type: ignore
+                )
+                logger.warning(f"{smp_characteristic.max_write_without_response_size=}")
+
             self._smp_characteristic = smp_characteristic
 
         logger.debug(f"Starting notify on {SMP_CHARACTERISTIC_UUID=}")
         await self._client.start_notify(SMP_CHARACTERISTIC_UUID, self._notify_callback)
         logger.debug(f"Started notify on {SMP_CHARACTERISTIC_UUID=}")
 
     async def disconnect(self) -> None:
         logger.debug(f"Disonnecting from {self._client.address}")
         await self._client.disconnect()
         logger.debug(f"Disconnected from {self._client.address}")
 
     async def send(self, data: bytes) -> None:
-        # TODO: Unclear whether Bleak + SMP spec support transport-level fragmentation.  We can
-        #       continue this manual fragmentation for now, but it is not ideal.
-
         logger.debug(f"Sending {len(data)} bytes, {self.mtu=}")
         for offset in range(0, len(data), self.mtu):
             await self._client.write_gatt_char(
                 self._smp_characteristic, data[offset : offset + self.mtu], response=False
             )
         logger.debug(f"Sent {len(data)} bytes")
 
@@ -128,10 +145,19 @@
         await self.send(data)
         return await self.receive()
 
     @property
     def mtu(self) -> int:
         return self._smp_characteristic.max_write_without_response_size
 
-    @property
-    def max_unencoded_size(self) -> int:
-        return self.mtu
+    @staticmethod
+    async def scan(timeout: int = 5) -> List[BLEDevice]:
+        """Scan for BLE devices."""
+        logger.debug(f"Scanning for BLE devices for {timeout} seconds")
+        devices: Final = await BleakScanner(service_uuids=[str(SMP_SERVICE_UUID)]).discover(
+            timeout=timeout, return_adv=True
+        )
+        smp_servers: Final = [
+            d for d, a in devices.values() if SMP_SERVICE_UUID in {UUID(u) for u in a.service_uuids}
+        ]
+        logger.debug(f"Found {len(smp_servers)} SMP devices: {smp_servers=}")
+        return smp_servers
```

### Comparing `smpclient-1.3.2/smpclient/transport/serial.py` & `smpclient-2.0.1/smpclient/transport/serial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """A serial SMPTransport."""
 
+from __future__ import annotations
+
 import asyncio
 import logging
 import math
 from enum import IntEnum, unique
 from functools import cached_property
 from typing import Final
 
 from serial import Serial
 from smp import packet as smppacket
+from typing_extensions import override
+
+from smpclient.transport import SMPTransport
 
 logger = logging.getLogger(__name__)
 
 
 def _base64_cost(size: int) -> int:
     """The worst case size required to encode `size` `bytes`."""
 
@@ -27,15 +32,15 @@
 
     if size < 4:
         return 0
 
     return math.floor(3 / 4 * size) - 2
 
 
-class SMPSerialTransport:
+class SMPSerialTransport(SMPTransport):
     _POLLING_INTERVAL_S = 0.005
 
     class _ReadBuffer:
         """The state of the read buffer."""
 
         @unique
         class State(IntEnum):
@@ -231,14 +236,15 @@
         return await self.receive()
 
     @property
     def mtu(self) -> int:
         return self._mtu
 
     @cached_property
+    @override
     def max_unencoded_size(self) -> int:
         """The serial transport encodes each packet instead of sending SMP messages as raw bytes.
 
         The worst case size of an encoded SMP packet is:
         ```
         base64_cost(
             len(smp_message) + len(frame_length) + len(frame_crc16)
```

### Comparing `smpclient-1.3.2/PKG-INFO` & `smpclient-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: smpclient
-Version: 1.3.2
+Version: 2.0.1
 Summary: Simple Management Protocol (SMP) Client for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
-Requires-Python: >=3.10,<3.13
+Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: bleak (>=0.21.1,<0.22.0)
+Requires-Dist: bleak (>=0.22.1,<0.23.0)
 Requires-Dist: intelhex (>=2.3.0,<3.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
-Requires-Dist: smp (>=0.3.4,<0.4.0)
+Requires-Dist: smp (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Simple Management Protocol (SMP) Client 
 
 `smpclient` implements the transport layer of the Simple Management Protocol.  This library can be
 used as a dependency in applications that use SMP over **serial (UART or USB)**, **Bluetooth (BLE)**,
 or **UDP** connections.  Some abstractions are provided for common routines like upgrading device
@@ -50,20 +51,24 @@
    ```
    poetry add <my_new_dependency>
    ```
 6. add test or other development dependencies using [poetry groups](https://python-poetry.org/docs/managing-dependencies#dependency-groups):
    ```
    poetry add -G dev <my_dev_dependency>
    ```
+7. run tests for all supported python versions:
+   ```
+   tox
+   ```
 
 ## Development Environment Setup
 
 ### Install Dependencies
 
-- python >=3.10, <3.13
+- python >=3.8, <3.13
 - poetry: https://python-poetry.org/docs/#installation
 
 ### Create the venv
 
 ```
 poetry install
 ```
```

