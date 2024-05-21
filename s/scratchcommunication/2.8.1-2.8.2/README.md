# Comparing `tmp/scratchcommunication-2.8.1.tar.gz` & `tmp/scratchcommunication-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.8.1.tar", last modified: Mon May 20 17:28:09 2024, max compression
+gzip compressed data, was "scratchcommunication-2.8.2.tar", last modified: Tue May 21 08:39:52 2024, max compression
```

## Comparing `scratchcommunication-2.8.1.tar` & `scratchcommunication-2.8.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.123522 scratchcommunication-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-20 17:28:09.123522 scratchcommunication-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.119522 scratchcommunication-2.8.1/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18222 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.119522 scratchcommunication-2.8.1/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.123522 scratchcommunication-2.8.1/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:28:09.123522 scratchcommunication-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.119522 scratchcommunication-2.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.230428 scratchcommunication-2.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18222 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:39:52.230428 scratchcommunication-2.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/tests/test1.py
```

### Comparing `scratchcommunication-2.8.1/LICENSE` & `scratchcommunication-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.1/PKG-INFO` & `scratchcommunication-2.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.8.1
+Version: 2.8.2
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.8.1/README.md` & `scratchcommunication-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.1/scratchcommunication/cloud.py` & `scratchcommunication-2.8.2/scratchcommunication/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.1/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.8.2/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.1/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.8.2/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.1/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.8.2/scratchcommunication/cloudrequests/requests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Submodule for handling incoming requests.
 """
 import re, warnings, ast, inspect, traceback, time
-from typing import Union, Mapping, Sequence, Any
+from inspect import Parameter
+from copy import deepcopy
+from typing import Union, Mapping, Sequence, Any, Callable
 from types import FunctionType
 from func_timeout import StoppableThread
 from scratchcommunication.cloud_socket import CloudSocketConnection, CloudSocket
 from .basetypes import BaseRequestHandler, StopRequestHandler, NotUsingAThread
 
 class RequestHandler(BaseRequestHandler):
     """
@@ -136,15 +138,77 @@
         """
         Stop the request handler.
         """
         if self.uses_thread:
             raise NotUsingAThread("Can't stop a request handler that is not using a thread.")
         self.thread.stop(StopRequestHandler)
         self.cloud_socket.stop()
-                    
+                   
+                   
+KW = Parameter.KEYWORD_ONLY
+KWPS = Parameter.POSITIONAL_OR_KEYWORD
+PS = Parameter.POSITIONAL_ONLY
+MKW = Parameter.VAR_KEYWORD
+MPS = Parameter.VAR_POSITIONAL
+DO_NOTHING = lambda x: x
+
+def type_cast(func):
+    def wrapper(*args, **kwargs):
+        args, kwargs, return_ann = type_casting(func=func, signature=inspect.signature(func), args=args, kwargs=kwargs)
+        return return_ann(func(*args, **kwargs))
+    wrapper.__name__ = func.__name__
+    return wrapper
+
+def type_casting(*, func : FunctionType, signature : inspect.Signature, args : tuple, kwargs : dict) -> tuple[tuple, dict, Callable]:
+    args = list(deepcopy(args))
+    kwargs = dict(deepcopy(kwargs))
+    for idx, ((kw, param), arg) in enumerate(zip(signature.parameters.items(), args)):
+        if param.kind in (PS, KWPS):
+            if kw in kwargs:
+                raise TypeError(f"{func.__name__}() got multiple values for argument '{kw}'")
+            try:
+                args[idx] = (param.annotation if not param.annotation in (Any, signature.empty) else DO_NOTHING)(arg)
+            except TypeError:
+                pass
+        if param.kind == MPS:
+            items_converter = (param.annotation if not param.annotation in (Any, signature.empty) else DO_NOTHING)
+            item_converter = (items_converter.__args__[0] if hasattr(items_converter, "__args__") else DO_NOTHING) or DO_NOTHING
+            try:
+                args[idx:] = [item_converter(arg) for arg in items_converter(args[idx:])]
+            except TypeError:
+                pass
+            
+    last_idx = None
+    for idx, (kw, arg) in enumerate(kwargs.items()):
+        try:
+            param = signature.parameters[kw]
+            assert param.kind != MKW
+        except (KeyError, AssertionError):
+            last_idx = idx
+            break
+        if param.kind in (KW, KWPS):
+            try:
+                kwargs[kw] = (param.annotation if not param.annotation in (Any, signature.empty) else DO_NOTHING)(arg)
+            except TypeError:
+                pass
+            
+    if last_idx is not None:
+        for param in signature.parameters.values():
+            if param.kind == MKW:
+                items_converter = (param.annotation if not param.annotation in (Any, signature.empty) else DO_NOTHING)
+                item_converters = (items_converter.__args__[:2] if hasattr(items_converter, "__args__") else (DO_NOTHING, DO_NOTHING)) or (DO_NOTHING, DO_NOTHING)
+                try:
+                    kwargs.update({item_converters[0](k): item_converters[1](v) for k, v in dict(items_converter({i: j for i, j in list(kwargs.items())[last_idx:]})).items()})
+                except TypeError:
+                    pass
+        
+    return_callable = DO_NOTHING
+    if signature.return_annotation != inspect.Signature.empty and signature.return_annotation != Any:
+        return_callable = signature.return_annotation
+    return args, kwargs, return_callable
 
 def parse_python_request(msg : str, name : str):
     """
     Parse a request in the format of a python function call.
     """
     parsed = ast.parse(msg).body[0].value
     assert parsed.func.id == name
```

### Comparing `scratchcommunication-2.8.1/scratchcommunication/security.py` & `scratchcommunication-2.8.2/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.1/scratchcommunication/session.py` & `scratchcommunication-2.8.2/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.1/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.8.2/scratchcommunication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.8.1
+Version: 2.8.2
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.8.1/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.8.2/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.1/setup.py` & `scratchcommunication-2.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.8.1'
+VERSION = '2.8.2'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.8.1/tests/test1.py` & `scratchcommunication-2.8.2/tests/test1.py`

 * *Files identical despite different names*

