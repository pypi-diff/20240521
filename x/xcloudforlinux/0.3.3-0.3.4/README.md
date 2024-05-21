# Comparing `tmp/xcloudforlinux-0.3.3.tar.gz` & `tmp/xcloudforlinux-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcloudforlinux-0.3.3.tar", last modified: Tue May 21 06:34:36 2024, max compression
+gzip compressed data, was "xcloudforlinux-0.3.4.tar", last modified: Tue May 21 06:59:02 2024, max compression
```

## Comparing `xcloudforlinux-0.3.3.tar` & `xcloudforlinux-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 06:34:36.290294 xcloudforlinux-0.3.3/
--rw-rw-rw-   0        0        0       38 2024-05-14 15:45:57.000000 xcloudforlinux-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2909 2024-05-21 06:34:36.288285 xcloudforlinux-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2574 2024-05-06 06:00:51.000000 xcloudforlinux-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 06:34:36.290294 xcloudforlinux-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-05-21 06:33:50.000000 xcloudforlinux-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:34:36.222610 xcloudforlinux-0.3.3/xcloudforlinux/
--rw-rw-rw-   0        0        0      168 2024-05-21 03:19:43.000000 xcloudforlinux-0.3.3/xcloudforlinux/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:34:36.283618 xcloudforlinux-0.3.3/xcloudforlinux/resources/
--rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloudforlinux-0.3.3/xcloudforlinux/resources/XCloudJDBC-2.10.6.7.jar
--rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloudforlinux-0.3.3/xcloudforlinux/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
--rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.3/xcloudforlinux/resources/libthrift-0.9.2.jar
--rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.3/xcloudforlinux/resources/log4j-1.2.17.jar
--rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.3/xcloudforlinux/resources/lz4-1.3.0.jar
--rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloudforlinux-0.3.3/xcloudforlinux/resources/slf4j-api-1.7.5.jar
--rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloudforlinux-0.3.3/xcloudforlinux/resources/slf4j-log4j12-1.7.5.jar
--rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloudforlinux-0.3.3/xcloudforlinux/resources/slf4j-simple-1.7.5.jar
--rw-rw-rw-   0        0        0     8057 2024-05-21 06:33:37.000000 xcloudforlinux-0.3.3/xcloudforlinux/xcloudforlinux.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:34:36.244615 xcloudforlinux-0.3.3/xcloudforlinux.egg-info/
--rw-rw-rw-   0        0        0     2909 2024-05-21 06:34:35.000000 xcloudforlinux-0.3.3/xcloudforlinux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      662 2024-05-21 06:34:36.000000 xcloudforlinux-0.3.3/xcloudforlinux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 06:34:35.000000 xcloudforlinux-0.3.3/xcloudforlinux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-21 06:34:35.000000 xcloudforlinux-0.3.3/xcloudforlinux.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-21 06:34:35.000000 xcloudforlinux-0.3.3/xcloudforlinux.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 06:59:02.894528 xcloudforlinux-0.3.4/
+-rw-rw-rw-   0        0        0       38 2024-05-14 15:45:57.000000 xcloudforlinux-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2909 2024-05-21 06:59:02.892515 xcloudforlinux-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2574 2024-05-06 06:00:51.000000 xcloudforlinux-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:59:02.894528 xcloudforlinux-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-05-21 06:58:45.000000 xcloudforlinux-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:59:02.791412 xcloudforlinux-0.3.4/xcloudforlinux/
+-rw-rw-rw-   0        0        0      168 2024-05-21 03:19:43.000000 xcloudforlinux-0.3.4/xcloudforlinux/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:59:02.884291 xcloudforlinux-0.3.4/xcloudforlinux/resources/
+-rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/XCloudJDBC-2.10.6.7.jar
+-rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
+-rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/libthrift-0.9.2.jar
+-rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/log4j-1.2.17.jar
+-rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/lz4-1.3.0.jar
+-rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-api-1.7.5.jar
+-rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-log4j12-1.7.5.jar
+-rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-simple-1.7.5.jar
+-rw-rw-rw-   0        0        0     8057 2024-05-21 06:58:06.000000 xcloudforlinux-0.3.4/xcloudforlinux/xcloudforlinux.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:59:02.821052 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/
+-rw-rw-rw-   0        0        0     2909 2024-05-21 06:59:01.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2024-05-21 06:59:02.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:59:01.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 06:59:01.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-21 06:59:01.000000 xcloudforlinux-0.3.4/xcloudforlinux.egg-info/top_level.txt
```

### Comparing `xcloudforlinux-0.3.3/PKG-INFO` & `xcloudforlinux-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcloudforlinux
-Version: 0.3.3
+Version: 0.3.4
 Summary: 这是一个国信行云数据库并发查询python程序,主要应用于自动通报
 Home-page: https://github.com/bailulue
 Author: bailu
 Author-email: yabailu@chinatelecom.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xcloudforlinux-0.3.3/README.md` & `xcloudforlinux-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.3/setup.py` & `xcloudforlinux-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xcloudforlinux',
-    version='0.3.3',
+    version='0.3.4',
     packages=find_packages(),
     package_data={
         'xcloudforlinux': ['resources/*.jar'],
     },
     include_package_data=True,
     install_requires=[
         'JPype1==1.5.0'
```

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux/resources/XCloudJDBC-2.10.6.7.jar` & `xcloudforlinux-0.3.4/xcloudforlinux/resources/XCloudJDBC-2.10.6.7.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar` & `xcloudforlinux-0.3.4/xcloudforlinux/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux/resources/libthrift-0.9.2.jar` & `xcloudforlinux-0.3.4/xcloudforlinux/resources/libthrift-0.9.2.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux/resources/log4j-1.2.17.jar` & `xcloudforlinux-0.3.4/xcloudforlinux/resources/log4j-1.2.17.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux/resources/lz4-1.3.0.jar` & `xcloudforlinux-0.3.4/xcloudforlinux/resources/lz4-1.3.0.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux/resources/slf4j-api-1.7.5.jar` & `xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-api-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux/resources/slf4j-log4j12-1.7.5.jar` & `xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-log4j12-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux/resources/slf4j-simple-1.7.5.jar` & `xcloudforlinux-0.3.4/xcloudforlinux/resources/slf4j-simple-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux/xcloudforlinux.py` & `xcloudforlinux-0.3.4/xcloudforlinux/xcloudforlinux.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -109,18 +109,18 @@
 def run_query_in_process(ip, username, password, queries,max_cursors = 10,if_header_included = False):
     print('ClientManagement运行查询')
     with DatabaseClient(ip, username, password, max_cursors,if_header_included) as client:
         return client.execute_queries(queries)  # 修改为接收一个查询列表
 
 class ClientManager:
     def __init__(self, client_configs, max_cursors=10):
+        self.start_jvm()
         self.client_configs = client_configs
         self.max_cursors = max_cursors
         self.process_pool = ThreadPoolExecutor(max_workers=len(client_configs))
-        self.start_jvm()
 
     def __enter__(self):
         return self
 
     def start_jvm(self):
         if not jpype.startJVM():
             start_jvm()
```

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux.egg-info/PKG-INFO` & `xcloudforlinux-0.3.4/xcloudforlinux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcloudforlinux
-Version: 0.3.3
+Version: 0.3.4
 Summary: 这是一个国信行云数据库并发查询python程序,主要应用于自动通报
 Home-page: https://github.com/bailulue
 Author: bailu
 Author-email: yabailu@chinatelecom.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xcloudforlinux-0.3.3/xcloudforlinux.egg-info/SOURCES.txt` & `xcloudforlinux-0.3.4/xcloudforlinux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

