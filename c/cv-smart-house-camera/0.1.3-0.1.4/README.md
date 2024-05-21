# Comparing `tmp/cv_smart_house_camera-0.1.3.tar.gz` & `tmp/cv_smart_house_camera-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv_smart_house_camera-0.1.3.tar", max compression
+gzip compressed data, was "cv_smart_house_camera-0.1.4.tar", max compression
```

## Comparing `cv_smart_house_camera-0.1.3.tar` & `cv_smart_house_camera-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     4155 2024-05-20 17:14:19.319636 cv_smart_house_camera-0.1.3/cv_smart_house_camera/__init__.py
--rw-r--r--   0        0        0      733 2024-05-20 13:14:13.260707 cv_smart_house_camera-0.1.3/cv_smart_house_camera/cam_capture.py
--rw-r--r--   0        0        0       48 2024-05-20 12:13:33.324485 cv_smart_house_camera-0.1.3/cv_smart_house_camera/constants.py
--rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.3/cv_smart_house_camera/data/frames.py
--rw-r--r--   0        0        0     1099 2024-05-20 17:54:18.621626 cv_smart_house_camera-0.1.3/cv_smart_house_camera/generate_code.py
--rw-r--r--   0        0        0      292 2024-05-20 12:05:00.597313 cv_smart_house_camera-0.1.3/cv_smart_house_camera/helpers/poetry_install.py
--rw-r--r--   0        0        0      524 2024-05-20 17:54:18.626654 cv_smart_house_camera-0.1.3/cv_smart_house_camera/modules/modules_list.py
--rw-r--r--   0        0        0     1771 2024-05-20 17:54:20.117074 cv_smart_house_camera-0.1.3/cv_smart_house_camera/modules/modules_processing.py
--rw-r--r--   0        0        0     3501 2024-05-20 11:57:48.195278 cv_smart_house_camera-0.1.3/cv_smart_house_camera/proto_services/camera_service_pb2.py
--rw-r--r--   0        0        0     5512 2024-05-20 11:57:48.195278 cv_smart_house_camera-0.1.3/cv_smart_house_camera/proto_services/camera_service_twirp.py
--rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.3/cv_smart_house_camera/utils/get_local_ip.py
--rw-r--r--   0        0        0      515 2024-05-20 12:20:23.424894 cv_smart_house_camera-0.1.3/cv_smart_house_camera/utils/get_modules_from_toml.py
--rw-r--r--   0        0        0      683 2024-05-20 17:54:40.018869 cv_smart_house_camera-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.3/README.md
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4240 2024-05-21 18:52:38.431201 cv_smart_house_camera-0.1.4/cv_smart_house_camera/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-20 13:14:13.260707 cv_smart_house_camera-0.1.4/cv_smart_house_camera/cam_capture.py
+-rw-r--r--   0        0        0       48 2024-05-20 12:13:33.324485 cv_smart_house_camera-0.1.4/cv_smart_house_camera/constants.py
+-rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.4/cv_smart_house_camera/data/frames.py
+-rw-r--r--   0        0        0     1099 2024-05-20 17:59:27.440847 cv_smart_house_camera-0.1.4/cv_smart_house_camera/generate_code.py
+-rw-r--r--   0        0        0      292 2024-05-20 12:05:00.597313 cv_smart_house_camera-0.1.4/cv_smart_house_camera/helpers/poetry_install.py
+-rw-r--r--   0        0        0      183 2024-05-20 18:00:07.621973 cv_smart_house_camera-0.1.4/cv_smart_house_camera/modules/modules_list.py
+-rw-r--r--   0        0        0     1771 2024-05-20 17:54:20.117074 cv_smart_house_camera-0.1.4/cv_smart_house_camera/modules/modules_processing.py
+-rw-r--r--   0        0        0     3543 2024-05-21 18:56:28.902217 cv_smart_house_camera-0.1.4/cv_smart_house_camera/proto_services/camera_service_pb2.py
+-rw-r--r--   0        0        0     5512 2024-05-21 18:56:28.902217 cv_smart_house_camera-0.1.4/cv_smart_house_camera/proto_services/camera_service_twirp.py
+-rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.4/cv_smart_house_camera/utils/get_local_ip.py
+-rw-r--r--   0        0        0      515 2024-05-20 12:20:23.424894 cv_smart_house_camera-0.1.4/cv_smart_house_camera/utils/get_modules_from_toml.py
+-rw-r--r--   0        0        0      683 2024-05-21 19:03:30.879821 cv_smart_house_camera-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.4/README.md
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.4/PKG-INFO
```

### Comparing `cv_smart_house_camera-0.1.3/cv_smart_house_camera/__init__.py` & `cv_smart_house_camera-0.1.4/cv_smart_house_camera/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
         return Empty()
     
     def GetInstalledModules(self, ctx, request):
         formatted_modules = []
 
         for module in modules_list:
-            formatted_modules.append(camera_service.InstalledModule(name = module.get("name"), options = module.get("options")))
+            formatted_modules.append(camera_service.InstalledModule(name = module.get("name"), package_name = module.get("package_name"), options = module.get("options")))
 
         return camera_service.InstalledModules(modules=formatted_modules)
 
     def GetLastFrame(self, ctx, request):
         module_result = modules_result.get(request.module)
         if module_result is None or module_result.get("ok") == False:
             raise Exception(f"Module {request.module} failed processing")
@@ -99,14 +99,15 @@
     logging.basicConfig()
 
     # Install packages.
     poetry_install()
 
     # Add modules to the list
     for module in modules:
+        module.package_name = "internal"
         modules_list.append(module)
 
     app = TwirpASGIApp()
     services.append(CameraServiceServer(service=CameraService()))
 
     for service in services:
         app.add_service(service)
```

### Comparing `cv_smart_house_camera-0.1.3/cv_smart_house_camera/cam_capture.py` & `cv_smart_house_camera-0.1.4/cv_smart_house_camera/cam_capture.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.3/cv_smart_house_camera/generate_code.py` & `cv_smart_house_camera-0.1.4/cv_smart_house_camera/generate_code.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from cv_smart_house_camera.utils.get_modules_from_toml import get_modules_from_toml
 
 def generate_code():
     modules = get_modules_from_toml()
     import_code = []
     original_frame_processing = "def original_frame_processing(frame, frame_number):\n\treturn"
-    modules_list = ['{ "name": "Original Frame", "package_name": "original", "processing": original_frame_processing }']
+    modules_list = ['{ "name": "Original Frame", "package_name": "internal", "processing": original_frame_processing }']
 
 
 
     for package, version in modules:
         import_statement = f"import {package}"
         import_code.append(import_statement)
         module_item = f"""{{ "name": {package}.name, "package_name": "{package}", "processing": {package}.processing, "options": {package}.options }}"""
```

### Comparing `cv_smart_house_camera-0.1.3/cv_smart_house_camera/modules/modules_processing.py` & `cv_smart_house_camera-0.1.4/cv_smart_house_camera/modules/modules_processing.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.3/cv_smart_house_camera/proto_services/camera_service_pb2.py` & `cv_smart_house_camera-0.1.4/cv_smart_house_camera/proto_services/camera_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x63\x61mera_service.proto\x12\rcameraService\x1a\x1bgoogle/protobuf/empty.proto\")\n\x15IsCameraAliveResponse\x12\x10\n\x08is_alive\x18\x01 \x01(\x08\"C\n\x10InstalledModules\x12/\n\x07modules\x18\x01 \x03(\x0b\x32\x1e.cameraService.InstalledModule\"h\n\x0fInstalledModule\x12\x0c\n\x04name\x18\x01 \x01(\t\x12;\n\x07options\x18\x02 \x01(\x0b\x32%.cameraService.InstalledModuleOptionsH\x00\x88\x01\x01\x42\n\n\x08_options\"?\n\x15InstallModulesRequest\x12&\n\x07modules\x18\x01 \x03(\x0b\x32\x15.cameraService.Module\"*\n\x17UninstallModulesRequest\x12\x0f\n\x07modules\x18\x01 \x03(\t\"\'\n\x06Module\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"%\n\x13GetLastFrameRequest\x12\x0e\n\x06module\x18\x01 \x01(\t\"\x16\n\x05\x46rame\x12\r\n\x05\x66rame\x18\x01 \x01(\x0c\"h\n\x16InstalledModuleOptions\x12\x11\n\x04show\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x1d\n\x10processing_frame\x18\x02 \x01(\x05H\x01\x88\x01\x01\x42\x07\n\x05_showB\x13\n\x11_processing_frame2\x9c\x03\n\rCameraService\x12M\n\rIsCameraAlive\x12\x16.google.protobuf.Empty\x1a$.cameraService.IsCameraAliveResponse\x12N\n\x13GetInstalledModules\x12\x16.google.protobuf.Empty\x1a\x1f.cameraService.InstalledModules\x12N\n\x0eInstallModules\x12$.cameraService.InstallModulesRequest\x1a\x16.google.protobuf.Empty\x12R\n\x10UninstallModules\x12&.cameraService.UninstallModulesRequest\x1a\x16.google.protobuf.Empty\x12H\n\x0cGetLastFrame\x12\".cameraService.GetLastFrameRequest\x1a\x14.cameraService.Frameb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x63\x61mera_service.proto\x12\rcameraService\x1a\x1bgoogle/protobuf/empty.proto\")\n\x15IsCameraAliveResponse\x12\x10\n\x08is_alive\x18\x01 \x01(\x08\"C\n\x10InstalledModules\x12/\n\x07modules\x18\x01 \x03(\x0b\x32\x1e.cameraService.InstalledModule\"~\n\x0fInstalledModule\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0cpackage_name\x18\x02 \x01(\t\x12;\n\x07options\x18\x03 \x01(\x0b\x32%.cameraService.InstalledModuleOptionsH\x00\x88\x01\x01\x42\n\n\x08_options\"?\n\x15InstallModulesRequest\x12&\n\x07modules\x18\x01 \x03(\x0b\x32\x15.cameraService.Module\"*\n\x17UninstallModulesRequest\x12\x0f\n\x07modules\x18\x01 \x03(\t\"\'\n\x06Module\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"%\n\x13GetLastFrameRequest\x12\x0e\n\x06module\x18\x01 \x01(\t\"\x16\n\x05\x46rame\x12\r\n\x05\x66rame\x18\x01 \x01(\x0c\"h\n\x16InstalledModuleOptions\x12\x11\n\x04show\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x1d\n\x10processing_frame\x18\x02 \x01(\x05H\x01\x88\x01\x01\x42\x07\n\x05_showB\x13\n\x11_processing_frame2\x9c\x03\n\rCameraService\x12M\n\rIsCameraAlive\x12\x16.google.protobuf.Empty\x1a$.cameraService.IsCameraAliveResponse\x12N\n\x13GetInstalledModules\x12\x16.google.protobuf.Empty\x1a\x1f.cameraService.InstalledModules\x12N\n\x0eInstallModules\x12$.cameraService.InstallModulesRequest\x1a\x16.google.protobuf.Empty\x12R\n\x10UninstallModules\x12&.cameraService.UninstallModulesRequest\x1a\x16.google.protobuf.Empty\x12H\n\x0cGetLastFrame\x12\".cameraService.GetLastFrameRequest\x1a\x14.cameraService.Frameb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'camera_service_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   DESCRIPTOR._loaded_options = None
   _globals['_ISCAMERAALIVERESPONSE']._serialized_start=68
   _globals['_ISCAMERAALIVERESPONSE']._serialized_end=109
   _globals['_INSTALLEDMODULES']._serialized_start=111
   _globals['_INSTALLEDMODULES']._serialized_end=178
   _globals['_INSTALLEDMODULE']._serialized_start=180
-  _globals['_INSTALLEDMODULE']._serialized_end=284
-  _globals['_INSTALLMODULESREQUEST']._serialized_start=286
-  _globals['_INSTALLMODULESREQUEST']._serialized_end=349
-  _globals['_UNINSTALLMODULESREQUEST']._serialized_start=351
-  _globals['_UNINSTALLMODULESREQUEST']._serialized_end=393
-  _globals['_MODULE']._serialized_start=395
-  _globals['_MODULE']._serialized_end=434
-  _globals['_GETLASTFRAMEREQUEST']._serialized_start=436
-  _globals['_GETLASTFRAMEREQUEST']._serialized_end=473
-  _globals['_FRAME']._serialized_start=475
-  _globals['_FRAME']._serialized_end=497
-  _globals['_INSTALLEDMODULEOPTIONS']._serialized_start=499
-  _globals['_INSTALLEDMODULEOPTIONS']._serialized_end=603
-  _globals['_CAMERASERVICE']._serialized_start=606
-  _globals['_CAMERASERVICE']._serialized_end=1018
+  _globals['_INSTALLEDMODULE']._serialized_end=306
+  _globals['_INSTALLMODULESREQUEST']._serialized_start=308
+  _globals['_INSTALLMODULESREQUEST']._serialized_end=371
+  _globals['_UNINSTALLMODULESREQUEST']._serialized_start=373
+  _globals['_UNINSTALLMODULESREQUEST']._serialized_end=415
+  _globals['_MODULE']._serialized_start=417
+  _globals['_MODULE']._serialized_end=456
+  _globals['_GETLASTFRAMEREQUEST']._serialized_start=458
+  _globals['_GETLASTFRAMEREQUEST']._serialized_end=495
+  _globals['_FRAME']._serialized_start=497
+  _globals['_FRAME']._serialized_end=519
+  _globals['_INSTALLEDMODULEOPTIONS']._serialized_start=521
+  _globals['_INSTALLEDMODULEOPTIONS']._serialized_end=625
+  _globals['_CAMERASERVICE']._serialized_start=628
+  _globals['_CAMERASERVICE']._serialized_end=1040
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cv_smart_house_camera-0.1.3/cv_smart_house_camera/proto_services/camera_service_twirp.py` & `cv_smart_house_camera-0.1.4/cv_smart_house_camera/proto_services/camera_service_twirp.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.3/cv_smart_house_camera/utils/get_modules_from_toml.py` & `cv_smart_house_camera-0.1.4/cv_smart_house_camera/utils/get_modules_from_toml.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.3/pyproject.toml` & `cv_smart_house_camera-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cv-smart-house-camera"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = [ "Your Name <you@example.com>",]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 flask = "^3.0.3"
```

### Comparing `cv_smart_house_camera-0.1.3/PKG-INFO` & `cv_smart_house_camera-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv-smart-house-camera
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
```

