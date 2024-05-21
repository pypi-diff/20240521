# Comparing `tmp/openobd_protocol-0.12.0.tar.gz` & `tmp/openobd_protocol-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd_protocol-0.12.0.tar", last modified: Thu May 16 13:41:33 2024, max compression
+gzip compressed data, was "openobd_protocol-0.13.0.tar", last modified: Tue May 21 09:52:46 2024, max compression
```

## Comparing `openobd_protocol-0.12.0.tar` & `openobd_protocol-0.13.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:41:33.743915 openobd_protocol-0.12.0/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-16 13:41:33.743915 openobd_protocol-0.12.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 13:41:33.743915 openobd_protocol-0.12.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:41:33.717915 openobd_protocol-0.12.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:41:33.723915 openobd_protocol-0.12.0/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1359 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:41:33.737915 openobd_protocol-0.12.0/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     1978 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      462 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2565 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2349 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      405 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8395 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:41:33.740915 openobd_protocol-0.12.0/src/openobd_protocol/SessionController/
--rw-r--r--   0 root         (0) root         (0)     2496 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/SessionController/SessionServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    11126 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2499 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/SessionController/Session_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2446 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/SessionController/Session_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1712 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:41:33.742915 openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     1748 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2973 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-16 13:41:28.000000 openobd_protocol-0.12.0/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:41:33.742915 openobd_protocol-0.12.0/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-16 13:41:33.000000 openobd_protocol-0.12.0/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1610 2024-05-16 13:41:33.000000 openobd_protocol-0.12.0/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 13:41:33.000000 openobd_protocol-0.12.0/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-05-16 13:41:33.000000 openobd_protocol-0.12.0/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-16 13:41:33.000000 openobd_protocol-0.12.0/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.928763 openobd_protocol-0.13.0/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-21 09:52:46.928763 openobd_protocol-0.13.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 09:52:46.928763 openobd_protocol-0.13.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.913763 openobd_protocol-0.13.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.919763 openobd_protocol-0.13.0/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.922763 openobd_protocol-0.13.0/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      462 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8395 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.924763 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     2861 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    15019 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/Session_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/Session_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.927763 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.927763 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd_protocol-0.12.0/LICENSE` & `openobd_protocol-0.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/PKG-INFO` & `openobd_protocol-0.13.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.12.0
+Version: 0.13.0
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.12.0/pyproject.toml` & `openobd_protocol-0.13.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/Authentication_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/Authentication_pb2.pyi` & `openobd_protocol-0.13.0/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/BasicResponse_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/BasicResponse_pb2.pyi` & `openobd_protocol-0.13.0/src/openobd_protocol/BasicResponse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd_protocol-0.13.0/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd_protocol-0.13.0/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/SessionController/SessionServices_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 from openobd_protocol.SessionController import Session_pb2 as openobd__protocol_dot_SessionController_dot_Session__pb2
 from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\x1a\x30openobd_protocol/SessionController/Session.proto\x1a$openobd_protocol/BasicResponse.proto2\xd3\x05\n\x0fSessionServices\x12\x91\x01\n\x0fgetSessionToken\x12=.com.jifeline.OpenOBD.Protocol.SessionController.Authenticate\x1a=.com.jifeline.OpenOBD.Protocol.SessionController.SessionToken\"\x00\x12\x8e\x01\n\rcreateSession\x12=.com.jifeline.OpenOBD.Protocol.SessionController.StartSession\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x88\x01\n\ngetSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x8b\x01\n\rdeleteSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x81\x01\n\x0egetSessionList\x12+.com.jifeline.OpenOBD.Protocol.EmptyRequest\x1a@.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfoList\"\x00\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\x1a\x30openobd_protocol/SessionController/Session.proto\x1a$openobd_protocol/BasicResponse.proto2\x8c\x08\n\x0fSessionServices\x12\x91\x01\n\x0fgetSessionToken\x12=.com.jifeline.OpenOBD.Protocol.SessionController.Authenticate\x1a=.com.jifeline.OpenOBD.Protocol.SessionController.SessionToken\"\x00\x12\x99\x01\n\x18startSessionOnConnection\x12=.com.jifeline.OpenOBD.Protocol.SessionController.ConnectionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x91\x01\n\x14startSessionOnTicket\x12\x39.com.jifeline.OpenOBD.Protocol.SessionController.TicketId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x97\x01\n\x17startSessionOnConnector\x12<.com.jifeline.OpenOBD.Protocol.SessionController.ConnectorId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x88\x01\n\ngetSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x8b\x01\n\rdeleteSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x81\x01\n\x0egetSessionList\x12+.com.jifeline.OpenOBD.Protocol.EmptyRequest\x1a@.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfoList\"\x00\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.SessionServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
   _globals['_SESSIONSERVICES']._serialized_start=229
-  _globals['_SESSIONSERVICES']._serialized_end=952
+  _globals['_SESSIONSERVICES']._serialized_end=1265
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py` & `openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,17 +26,27 @@
             channel: A grpc.Channel.
         """
         self.getSessionToken = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSessionToken',
                 request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.Authenticate.SerializeToString,
                 response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionToken.FromString,
                 )
-        self.createSession = channel.unary_unary(
-                '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/createSession',
-                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.StartSession.SerializeToString,
+        self.startSessionOnConnection = channel.unary_unary(
+                '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/startSessionOnConnection',
+                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.ConnectionId.SerializeToString,
+                response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
+                )
+        self.startSessionOnTicket = channel.unary_unary(
+                '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/startSessionOnTicket',
+                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.TicketId.SerializeToString,
+                response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
+                )
+        self.startSessionOnConnector = channel.unary_unary(
+                '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/startSessionOnConnector',
+                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.ConnectorId.SerializeToString,
                 response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
                 )
         self.getSession = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSession',
                 request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.SerializeToString,
                 response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
                 )
@@ -67,15 +77,27 @@
 
     def getSessionToken(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def createSession(self, request, context):
+    def startSessionOnConnection(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def startSessionOnTicket(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def startSessionOnConnector(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def getSession(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -99,17 +121,27 @@
 def add_SessionServicesServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'getSessionToken': grpc.unary_unary_rpc_method_handler(
                     servicer.getSessionToken,
                     request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.Authenticate.FromString,
                     response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionToken.SerializeToString,
             ),
-            'createSession': grpc.unary_unary_rpc_method_handler(
-                    servicer.createSession,
-                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.StartSession.FromString,
+            'startSessionOnConnection': grpc.unary_unary_rpc_method_handler(
+                    servicer.startSessionOnConnection,
+                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.ConnectionId.FromString,
+                    response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.SerializeToString,
+            ),
+            'startSessionOnTicket': grpc.unary_unary_rpc_method_handler(
+                    servicer.startSessionOnTicket,
+                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.TicketId.FromString,
+                    response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.SerializeToString,
+            ),
+            'startSessionOnConnector': grpc.unary_unary_rpc_method_handler(
+                    servicer.startSessionOnConnector,
+                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.ConnectorId.FromString,
                     response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.SerializeToString,
             ),
             'getSession': grpc.unary_unary_rpc_method_handler(
                     servicer.getSession,
                     request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.FromString,
                     response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.SerializeToString,
             ),
@@ -157,26 +189,60 @@
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSessionToken',
             openobd__protocol_dot_SessionController_dot_Session__pb2.Authenticate.SerializeToString,
             openobd__protocol_dot_SessionController_dot_Session__pb2.SessionToken.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def createSession(request,
+    def startSessionOnConnection(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/startSessionOnConnection',
+            openobd__protocol_dot_SessionController_dot_Session__pb2.ConnectionId.SerializeToString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def startSessionOnTicket(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/startSessionOnTicket',
+            openobd__protocol_dot_SessionController_dot_Session__pb2.TicketId.SerializeToString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def startSessionOnConnector(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/createSession',
-            openobd__protocol_dot_SessionController_dot_Session__pb2.StartSession.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/startSessionOnConnector',
+            openobd__protocol_dot_SessionController_dot_Session__pb2.ConnectorId.SerializeToString,
             openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def getSession(request,
             target,
```

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/SessionController/Session_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/SessionController/Session_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,28 +11,32 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0openobd_protocol/SessionController/Session.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\"\'\n\x0cStartSession\x12\x17\n\x0f\x63onnection_uuid\x18\x01 \x01(\t\"r\n\x0bSessionInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\t\x12\x15\n\rgrpc_endpoint\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\t\"]\n\x0c\x41uthenticate\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x15\n\rclient_secret\x18\x02 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x03 \x01(\t\x12\x12\n\ncluster_id\x18\x04 \x01(\t\"\x1d\n\x0cSessionToken\x12\r\n\x05token\x18\x01 \x01(\t\"a\n\x0fSessionInfoList\x12N\n\x08sessions\x18\x01 \x03(\x0b\x32<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x17\n\tSessionId\x12\n\n\x02id\x18\x01 \x01(\tB\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0openobd_protocol/SessionController/Session.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\"\x16\n\x08TicketId\x12\n\n\x02id\x18\x01 \x01(\t\"\x1a\n\x0c\x43onnectionId\x12\n\n\x02id\x18\x01 \x01(\t\"\x19\n\x0b\x43onnectorId\x12\n\n\x02id\x18\x01 \x01(\t\"r\n\x0bSessionInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\t\x12\x15\n\rgrpc_endpoint\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\t\"]\n\x0c\x41uthenticate\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x15\n\rclient_secret\x18\x02 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x03 \x01(\t\x12\x12\n\ncluster_id\x18\x04 \x01(\t\"\x1d\n\x0cSessionToken\x12\r\n\x05token\x18\x01 \x01(\t\"a\n\x0fSessionInfoList\x12N\n\x08sessions\x18\x01 \x03(\x0b\x32<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x17\n\tSessionId\x12\n\n\x02id\x18\x01 \x01(\tB\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.Session_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_STARTSESSION']._serialized_start=132
-  _globals['_STARTSESSION']._serialized_end=171
-  _globals['_SESSIONINFO']._serialized_start=173
-  _globals['_SESSIONINFO']._serialized_end=287
-  _globals['_AUTHENTICATE']._serialized_start=289
-  _globals['_AUTHENTICATE']._serialized_end=382
-  _globals['_SESSIONTOKEN']._serialized_start=384
-  _globals['_SESSIONTOKEN']._serialized_end=413
-  _globals['_SESSIONINFOLIST']._serialized_start=415
-  _globals['_SESSIONINFOLIST']._serialized_end=512
-  _globals['_SESSIONID']._serialized_start=514
-  _globals['_SESSIONID']._serialized_end=537
+  _globals['_TICKETID']._serialized_start=132
+  _globals['_TICKETID']._serialized_end=154
+  _globals['_CONNECTIONID']._serialized_start=156
+  _globals['_CONNECTIONID']._serialized_end=182
+  _globals['_CONNECTORID']._serialized_start=184
+  _globals['_CONNECTORID']._serialized_end=209
+  _globals['_SESSIONINFO']._serialized_start=211
+  _globals['_SESSIONINFO']._serialized_end=325
+  _globals['_AUTHENTICATE']._serialized_start=327
+  _globals['_AUTHENTICATE']._serialized_end=420
+  _globals['_SESSIONTOKEN']._serialized_start=422
+  _globals['_SESSIONTOKEN']._serialized_end=451
+  _globals['_SESSIONINFOLIST']._serialized_start=453
+  _globals['_SESSIONINFOLIST']._serialized_end=550
+  _globals['_SESSIONID']._serialized_start=552
+  _globals['_SESSIONID']._serialized_end=575
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/SessionController/Session_pb2.pyi` & `openobd_protocol-0.13.0/src/openobd_protocol/SessionController/Session_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,31 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class StartSession(_message.Message):
-    __slots__ = ("connection_uuid",)
-    CONNECTION_UUID_FIELD_NUMBER: _ClassVar[int]
-    connection_uuid: str
-    def __init__(self, connection_uuid: _Optional[str] = ...) -> None: ...
+class TicketId(_message.Message):
+    __slots__ = ("id",)
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    def __init__(self, id: _Optional[str] = ...) -> None: ...
+
+class ConnectionId(_message.Message):
+    __slots__ = ("id",)
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    def __init__(self, id: _Optional[str] = ...) -> None: ...
+
+class ConnectorId(_message.Message):
+    __slots__ = ("id",)
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    def __init__(self, id: _Optional[str] = ...) -> None: ...
 
 class SessionInfo(_message.Message):
     __slots__ = ("id", "status", "created_at", "grpc_endpoint", "authentication_token")
     ID_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     GRPC_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/Status_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/Status_pb2.pyi` & `openobd_protocol-0.13.0/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol.egg-info/PKG-INFO` & `openobd_protocol-0.13.0/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.12.0
+Version: 0.13.0
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.12.0/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd_protocol-0.13.0/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

