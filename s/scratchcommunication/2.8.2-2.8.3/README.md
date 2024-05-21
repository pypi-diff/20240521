# Comparing `tmp/scratchcommunication-2.8.2.tar.gz` & `tmp/scratchcommunication-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.8.2.tar", last modified: Tue May 21 08:39:52 2024, max compression
+gzip compressed data, was "scratchcommunication-2.8.3.tar", last modified: Tue May 21 09:26:25 2024, max compression
```

## Comparing `scratchcommunication-2.8.2.tar` & `scratchcommunication-2.8.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.230428 scratchcommunication-2.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18222 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 08:39:52.000000 scratchcommunication-2.8.2/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:39:52.230428 scratchcommunication-2.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:39:52.226428 scratchcommunication-2.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 08:39:45.000000 scratchcommunication-2.8.2/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:26:25.227041 scratchcommunication-2.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-21 09:26:25.227041 scratchcommunication-2.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:26:25.227041 scratchcommunication-2.8.3/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18222 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:26:25.227041 scratchcommunication-2.8.3/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:26:25.227041 scratchcommunication-2.8.3/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-21 09:26:25.000000 scratchcommunication-2.8.3/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 09:26:25.000000 scratchcommunication-2.8.3/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:26:25.000000 scratchcommunication-2.8.3/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 09:26:25.000000 scratchcommunication-2.8.3/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 09:26:25.000000 scratchcommunication-2.8.3/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:26:25.227041 scratchcommunication-2.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:26:25.227041 scratchcommunication-2.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 09:26:18.000000 scratchcommunication-2.8.3/tests/test1.py
```

### Comparing `scratchcommunication-2.8.2/LICENSE` & `scratchcommunication-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.2/PKG-INFO` & `scratchcommunication-2.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.8.2
+Version: 2.8.3
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.8.2/README.md` & `scratchcommunication-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.2/scratchcommunication/cloud.py` & `scratchcommunication-2.8.3/scratchcommunication/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.2/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.8.3/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.2/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.8.3/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.2/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.8.3/scratchcommunication/cloudrequests/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,34 +98,15 @@
                 
     
     def execute_request(self, name, *, args : Sequence[Any], kwargs : Mapping[str, Any], client : CloudSocketConnection) -> Union[str, float, int]:
         """
         Execute a request.
         """
         request_handling_function = self.requests[name]
-        return_converter = lambda x : x
-        if request_handling_function.auto_convert:
-            for idx, (arg, annotation) in enumerate(inspect.signature(request_handling_function).parameters.items()):
-                if not annotation.kind.value in [0, 1, 3]:
-                    continue
-                if inspect.Parameter.empty == annotation.annotation:
-                    continue
-                if not arg in kwargs:
-                    if not annotation.kind.value in [0, 1]:
-                        raise ValueError("Signature doesn't match")
-                    try:
-                        args[idx] = annotation.annotation(args[idx])
-                    except IndexError:
-                        pass
-                    continue
-                if not annotation.kind.value in [1, 3]:
-                    raise ValueError("Signature doesn't match")
-                kwargs[arg] = annotation.annotation(kwargs[arg])
-            if inspect.signature(request_handling_function).return_annotation != inspect.Signature.empty:
-                return_converter = inspect.signature(request_handling_function).return_annotation
+        args, kwargs, return_converter = type_casting(func=request_handling_function, signature=inspect.signature(request_handling_function), args=args, kwargs=kwargs)
         def respond():
             try:
                 response = str(return_converter(request_handling_function(*args, **kwargs)))
             except ErrorMessage as e:
                 response = " ".join(e.args)
             client.send(response)
         if request_handling_function.thread:
```

### Comparing `scratchcommunication-2.8.2/scratchcommunication/security.py` & `scratchcommunication-2.8.3/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.2/scratchcommunication/session.py` & `scratchcommunication-2.8.3/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.2/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.8.3/scratchcommunication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.8.2
+Version: 2.8.3
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.8.2/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.8.3/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.2/setup.py` & `scratchcommunication-2.8.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.8.2'
+VERSION = '2.8.3'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.8.2/tests/test1.py` & `scratchcommunication-2.8.3/tests/test1.py`

 * *Files identical despite different names*

