# Comparing `tmp/co6co-0.0.4.tar.gz` & `tmp/co6co-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "co6co-0.0.4.tar", last modified: Sat May 11 06:44:42 2024, max compression
+gzip compressed data, was "co6co-0.0.5.tar", last modified: Tue May 21 06:54:37 2024, max compression
```

## Comparing `co6co-0.0.4.tar` & `co6co-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.211477 co6co-0.0.4/
--rw-rw-rw-   0        0        0       13 2023-08-16 08:48:34.000000 co6co-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      433 2024-05-11 06:44:42.210478 co6co-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-08-18 01:57:56.000000 co6co-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.175032 co6co-0.0.4/co6co/
--rw-rw-rw-   0        0        0     1070 2024-05-11 06:44:40.000000 co6co-0.0.4/co6co/__init__.py
--rw-rw-rw-   0        0        0      281 2024-01-05 09:13:48.000000 co6co-0.0.4/co6co/demo.test.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.192696 co6co-0.0.4/co6co/enums/
--rw-rw-rw-   0        0        0     2253 2024-04-10 08:24:13.000000 co6co-0.0.4/co6co/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.194693 co6co-0.0.4/co6co/task/
--rw-rw-rw-   0        0        0        0 2024-01-19 08:21:45.000000 co6co-0.0.4/co6co/task/__init__.py
--rw-rw-rw-   0        0        0     2219 2024-03-14 02:19:00.000000 co6co-0.0.4/co6co/task/thread.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.204550 co6co-0.0.4/co6co/utils/
--rw-rw-rw-   0        0        0     2674 2024-03-29 09:20:58.000000 co6co-0.0.4/co6co/utils/File.py
--rw-rw-rw-   0        0        0      920 2024-03-18 01:38:20.000000 co6co-0.0.4/co6co/utils/__init__.py
--rw-rw-rw-   0        0        0     6035 2023-12-18 01:29:31.000000 co6co-0.0.4/co6co/utils/hash.py
--rw-rw-rw-   0        0        0     2400 2023-09-14 01:40:45.000000 co6co-0.0.4/co6co/utils/http.py
--rw-rw-rw-   0        0        0      512 2023-12-18 01:29:31.000000 co6co-0.0.4/co6co/utils/json_util.py
--rw-rw-rw-   0        0        0     3478 2024-04-29 08:11:33.000000 co6co-0.0.4/co6co/utils/log.py
--rw-rw-rw-   0        0        0     1393 2024-05-07 09:41:22.000000 co6co-0.0.4/co6co/utils/tool_util.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.189349 co6co-0.0.4/co6co.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-11 06:44:42.000000 co6co-0.0.4/co6co.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2024-05-11 06:44:42.000000 co6co-0.0.4/co6co.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 06:44:42.000000 co6co-0.0.4/co6co.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-11 06:44:42.000000 co6co-0.0.4/co6co.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-08-16 08:23:34.000000 co6co-0.0.4/co6co.egg-info/zip-safe
--rw-rw-rw-   0        0        0       30 2023-08-17 03:39:37.000000 co6co-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0      684 2024-04-22 05:42:25.000000 co6co-0.0.4/service.encode.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 06:44:42.211477 co6co-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1116 2024-02-27 01:32:43.000000 co6co-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.209479 co6co-0.0.4/tests/
--rw-rw-rw-   0        0        0      356 2024-02-27 01:32:43.000000 co6co-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0      255 2024-02-27 01:32:43.000000 co6co-0.0.4/tests/unittest.md
--rw-rw-rw-   0        0        0     1934 2024-02-27 01:32:43.000000 co6co-0.0.4/tests/v_utils_test.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:54:37.094602 co6co-0.0.5/
+-rw-rw-rw-   0        0        0       13 2023-08-16 08:48:34.000000 co6co-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      433 2024-05-21 06:54:37.093621 co6co-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-08-18 01:57:56.000000 co6co-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 06:54:37.062631 co6co-0.0.5/co6co/
+-rw-rw-rw-   0        0        0     1070 2024-05-21 06:54:19.000000 co6co-0.0.5/co6co/__init__.py
+-rw-rw-rw-   0        0        0      281 2024-01-05 09:13:48.000000 co6co-0.0.5/co6co/demo.test.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:54:37.081606 co6co-0.0.5/co6co/enums/
+-rw-rw-rw-   0        0        0     2253 2024-04-10 08:24:13.000000 co6co-0.0.5/co6co/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:54:37.082606 co6co-0.0.5/co6co/task/
+-rw-rw-rw-   0        0        0        0 2024-01-19 08:21:45.000000 co6co-0.0.5/co6co/task/__init__.py
+-rw-rw-rw-   0        0        0     2219 2024-03-14 02:19:00.000000 co6co-0.0.5/co6co/task/thread.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:54:37.089613 co6co-0.0.5/co6co/utils/
+-rw-rw-rw-   0        0        0     2674 2024-03-29 09:20:58.000000 co6co-0.0.5/co6co/utils/File.py
+-rw-rw-rw-   0        0        0     1088 2024-05-21 06:30:28.000000 co6co-0.0.5/co6co/utils/__init__.py
+-rw-rw-rw-   0        0        0     6035 2023-12-18 01:29:31.000000 co6co-0.0.5/co6co/utils/hash.py
+-rw-rw-rw-   0        0        0     2400 2023-09-14 01:40:45.000000 co6co-0.0.5/co6co/utils/http.py
+-rw-rw-rw-   0        0        0      512 2023-12-18 01:29:31.000000 co6co-0.0.5/co6co/utils/json_util.py
+-rw-rw-rw-   0        0        0     3478 2024-04-29 08:11:33.000000 co6co-0.0.5/co6co/utils/log.py
+-rw-rw-rw-   0        0        0     1393 2024-05-07 09:41:22.000000 co6co-0.0.5/co6co/utils/tool_util.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:54:37.080607 co6co-0.0.5/co6co.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-21 06:54:36.000000 co6co-0.0.5/co6co.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2024-05-21 06:54:36.000000 co6co-0.0.5/co6co.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:54:36.000000 co6co-0.0.5/co6co.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 06:54:36.000000 co6co-0.0.5/co6co.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-16 08:23:34.000000 co6co-0.0.5/co6co.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       30 2023-08-17 03:39:37.000000 co6co-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0      684 2024-04-22 05:42:25.000000 co6co-0.0.5/service.encode.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:54:37.094602 co6co-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1116 2024-02-27 01:32:43.000000 co6co-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:54:37.092603 co6co-0.0.5/tests/
+-rw-rw-rw-   0        0        0      356 2024-02-27 01:32:43.000000 co6co-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      255 2024-02-27 01:32:43.000000 co6co-0.0.5/tests/unittest.md
+-rw-rw-rw-   0        0        0     1934 2024-02-27 01:32:43.000000 co6co-0.0.5/tests/v_utils_test.py
```

### Comparing `co6co-0.0.4/co6co/__init__.py` & `co6co-0.0.5/co6co/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     return None
 
 
 __all__ = ['utils']  # 针对模块公开接口的一种约定，以提供了”白名单“的形式暴露接口。
 # 如果定义了__all__，
 # 使用from xxx import *导入该文件时，只会导入 __all__ 列出的成员，可以其他成员都被排除在外。
 
-__version_info = (0, 0, 4)
+__version_info = (0, 0, 5)
 __version__ = ".".join([str(x) for x in __version_info])
```

### Comparing `co6co-0.0.4/co6co/enums/__init__.py` & `co6co-0.0.5/co6co/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/co6co/task/thread.py` & `co6co-0.0.5/co6co/task/thread.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/co6co/utils/File.py` & `co6co-0.0.5/co6co/utils/File.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/co6co/utils/__init__.py` & `co6co-0.0.5/co6co/utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #-*- coding:utf-8 -*-
 import re,random,string,time,datetime
 from types import FunctionType
-
+import inspect
 def isBase64(content:str)->bool:
     _reg="^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{4}|[A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)$"
     group=re.match(_reg,content)
     if group !=None:return True
     return False
 
 def getRandomStr(length:int,scope:str=string.ascii_letters+string.digits)->str:
@@ -22,10 +22,16 @@
     return f"{time.strftime(format)}"
 
 def isCallable(func):
     return isinstance(func,FunctionType)
     return callable(func) # 返回true 也不一定能调用成功/返回失败一定调用失败
     return type(func) is FunctionType 
     return hasattr (func,"__call__")
+ 
+def is_async(func):
+    """
+    方法是否是异步的
+    """
+    return inspect.iscoroutinefunction(func) or inspect.isasyncgenfunction(func)
```

### Comparing `co6co-0.0.4/co6co/utils/hash.py` & `co6co-0.0.5/co6co/utils/hash.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/co6co/utils/http.py` & `co6co-0.0.5/co6co/utils/http.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/co6co/utils/json_util.py` & `co6co-0.0.5/co6co/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/co6co/utils/log.py` & `co6co-0.0.5/co6co/utils/log.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/co6co/utils/tool_util.py` & `co6co-0.0.5/co6co/utils/tool_util.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/co6co.egg-info/SOURCES.txt` & `co6co-0.0.5/co6co.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/service.encode.txt` & `co6co-0.0.5/service.encode.txt`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/setup.py` & `co6co-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.4/tests/v_utils_test.py` & `co6co-0.0.5/tests/v_utils_test.py`

 * *Files identical despite different names*

