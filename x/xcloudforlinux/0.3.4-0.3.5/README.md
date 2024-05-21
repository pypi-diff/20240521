# Comparing `tmp/xcloudforlinux-0.3.4.tar.gz` & `tmp/xcloudforlinux-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcloudforlinux-0.3.4.tar", last modified: Tue May 21 06:59:02 2024, max compression
+gzip compressed data, was "xcloudforlinux-0.3.5.tar", last modified: Tue May 21 07:34:36 2024, max compression
```

## Comparing `xcloudforlinux-0.3.4.tar` & `xcloudforlinux-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 06:59:02.894528 xcloudforlinux-0.3.4/
--rw-rw-rw-   0        0        0       38 2024-05-14 15:45:57.000000 xcloudforlinux-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2909 2024-05-21 06:59:02.892515 xcloudforlinux-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     2574 2024-05-06 06:00:51.000000 xcloudforlinux-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 06:59:02.894528 xcloudforlinux-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-05-21 06:58:45.000000 xcloudforlinux-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:59:02.791412 xcloudforlinux-0.3.4/xcloudforlinux/
--rw-rw-rw-   0        0        0      168 2024-05-21 03:19:43.000000 xcloudforlinux-0.3.4/xcloudforlinux/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:59:02.884291 xcloudforlinux-0.3.4/xcloudforlinux/resources/
--rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/XCloudJDBC-2.10.6.7.jar
--rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
--rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/libthrift-0.9.2.jar
--rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/log4j-1.2.17.jar
--rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/lz4-1.3.0.jar
--rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-api-1.7.5.jar
--rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-log4j12-1.7.5.jar
--rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-simple-1.7.5.jar
--rw-rw-rw-   0        0        0     8057 2024-05-21 06:58:06.000000 xcloudforlinux-0.3.4/xcloudforlinux/xcloudforlinux.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:59:02.821052 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/
--rw-rw-rw-   0        0        0     2909 2024-05-21 06:59:01.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      662 2024-05-21 06:59:02.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 06:59:01.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-21 06:59:01.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-21 06:59:01.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 07:34:36.500703 xcloudforlinux-0.3.5/
+-rw-rw-rw-   0        0        0       38 2024-05-14 15:45:57.000000 xcloudforlinux-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2909 2024-05-21 07:34:36.498703 xcloudforlinux-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2574 2024-05-06 06:00:51.000000 xcloudforlinux-0.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 07:34:36.500703 xcloudforlinux-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-05-21 07:26:30.000000 xcloudforlinux-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:34:36.432109 xcloudforlinux-0.3.5/xcloudforlinux/
+-rw-rw-rw-   0        0        0      168 2024-05-21 03:19:43.000000 xcloudforlinux-0.3.5/xcloudforlinux/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:34:36.495701 xcloudforlinux-0.3.5/xcloudforlinux/resources/
+-rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloudforlinux-0.3.5/xcloudforlinux/resources/XCloudJDBC-2.10.6.7.jar
+-rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloudforlinux-0.3.5/xcloudforlinux/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
+-rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.5/xcloudforlinux/resources/libthrift-0.9.2.jar
+-rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.5/xcloudforlinux/resources/log4j-1.2.17.jar
+-rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.5/xcloudforlinux/resources/lz4-1.3.0.jar
+-rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloudforlinux-0.3.5/xcloudforlinux/resources/slf4j-api-1.7.5.jar
+-rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloudforlinux-0.3.5/xcloudforlinux/resources/slf4j-log4j12-1.7.5.jar
+-rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloudforlinux-0.3.5/xcloudforlinux/resources/slf4j-simple-1.7.5.jar
+-rw-rw-rw-   0        0        0     8052 2024-05-21 07:25:56.000000 xcloudforlinux-0.3.5/xcloudforlinux/xcloudforlinux.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:34:36.455532 xcloudforlinux-0.3.5/xcloudforlinux.egg-info/
+-rw-rw-rw-   0        0        0     2909 2024-05-21 07:34:35.000000 xcloudforlinux-0.3.5/xcloudforlinux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2024-05-21 07:34:36.000000 xcloudforlinux-0.3.5/xcloudforlinux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 07:34:35.000000 xcloudforlinux-0.3.5/xcloudforlinux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 07:34:35.000000 xcloudforlinux-0.3.5/xcloudforlinux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-21 07:34:35.000000 xcloudforlinux-0.3.5/xcloudforlinux.egg-info/top_level.txt
```

### Comparing `xcloudforlinux-0.3.4/PKG-INFO` & `xcloudforlinux-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcloudforlinux
-Version: 0.3.4
+Version: 0.3.5
 Summary: 这是一个国信行云数据库并发查询python程序,主要应用于自动通报
 Home-page: https://github.com/bailulue
 Author: bailu
 Author-email: yabailu@chinatelecom.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xcloudforlinux-0.3.4/README.md` & `xcloudforlinux-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.4/setup.py` & `xcloudforlinux-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xcloudforlinux',
-    version='0.3.4',
+    version='0.3.5',
     packages=find_packages(),
     package_data={
         'xcloudforlinux': ['resources/*.jar'],
     },
     include_package_data=True,
     install_requires=[
         'JPype1==1.5.0'
```

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux/resources/XCloudJDBC-2.10.6.7.jar` & `xcloudforlinux-0.3.5/xcloudforlinux/resources/XCloudJDBC-2.10.6.7.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar` & `xcloudforlinux-0.3.5/xcloudforlinux/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux/resources/libthrift-0.9.2.jar` & `xcloudforlinux-0.3.5/xcloudforlinux/resources/libthrift-0.9.2.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux/resources/log4j-1.2.17.jar` & `xcloudforlinux-0.3.5/xcloudforlinux/resources/log4j-1.2.17.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux/resources/lz4-1.3.0.jar` & `xcloudforlinux-0.3.5/xcloudforlinux/resources/lz4-1.3.0.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-api-1.7.5.jar` & `xcloudforlinux-0.3.5/xcloudforlinux/resources/slf4j-api-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-log4j12-1.7.5.jar` & `xcloudforlinux-0.3.5/xcloudforlinux/resources/slf4j-log4j12-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-simple-1.7.5.jar` & `xcloudforlinux-0.3.5/xcloudforlinux/resources/slf4j-simple-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux/xcloudforlinux.py` & `xcloudforlinux-0.3.5/xcloudforlinux/xcloudforlinux.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,24 +113,22 @@
 
 class ClientManager:
     def __init__(self, client_configs, max_cursors=10):
         self.start_jvm()
         self.client_configs = client_configs
         self.max_cursors = max_cursors
         self.process_pool = ThreadPoolExecutor(max_workers=len(client_configs))
-
     def __enter__(self):
         return self
-
     def start_jvm(self):
-        if not jpype.startJVM():
+        if not jpype.isJVMStarted():
             start_jvm()
     def __exit__(self, exc_type, exc_val, exc_tb):
         if jpype.isJVMStarted():
-            jpype.shutdownJVM()
+            shutdown_jvm()
     def execute_queries(self, queries, if_header_included = False):
         # 确定根据查询数量动态调整启动的客户端数量
         num_queries = len(queries)
         if num_queries < self.max_cursors:
             num_clients = 1
         else:
             num_clients = min(len(self.client_configs), self.max_cursors)
```

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux.egg-info/PKG-INFO` & `xcloudforlinux-0.3.5/xcloudforlinux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcloudforlinux
-Version: 0.3.4
+Version: 0.3.5
 Summary: 这是一个国信行云数据库并发查询python程序,主要应用于自动通报
 Home-page: https://github.com/bailulue
 Author: bailu
 Author-email: yabailu@chinatelecom.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xcloudforlinux-0.3.4/xcloudforlinux.egg-info/SOURCES.txt` & `xcloudforlinux-0.3.5/xcloudforlinux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

