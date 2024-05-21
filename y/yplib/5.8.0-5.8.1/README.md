# Comparing `tmp/yplib-5.8.0.tar.gz` & `tmp/yplib-5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.8.0.tar", last modified: Thu May 16 07:21:45 2024, max compression
+gzip compressed data, was "yplib-5.8.1.tar", last modified: Tue May 21 08:18:07 2024, max compression
```

## Comparing `yplib-5.8.0.tar` & `yplib-5.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:21:45.068454 yplib-5.8.0/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.8.0/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-16 07:21:45.068454 yplib-5.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.8.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 07:21:45.068454 yplib-5.8.0/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-16 07:21:13.000000 yplib-5.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:21:45.068454 yplib-5.8.0/yplib/
--rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.8.0/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.8.0/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.8.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0    12851 2024-05-15 06:59:51.000000 yplib-5.8.0/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.8.0/yplib/file.py
--rw-rw-rw-   0        0        0     7361 2024-05-16 07:20:59.000000 yplib-5.8.0/yplib/http_util.py
--rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.8.0/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.8.0/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.8.0/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.8.0/yplib/markdown.py
--rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.8.0/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.8.0/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:21:45.068454 yplib-5.8.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-16 07:21:44.000000 yplib-5.8.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-16 07:21:44.000000 yplib-5.8.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:21:44.000000 yplib-5.8.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 07:21:44.000000 yplib-5.8.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 08:18:07.871639 yplib-5.8.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.8.1/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-21 08:18:07.871639 yplib-5.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.8.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 08:18:07.871639 yplib-5.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-21 08:17:47.000000 yplib-5.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:18:07.856614 yplib-5.8.1/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.8.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.8.1/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.8.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    12750 2024-05-21 08:16:54.000000 yplib-5.8.1/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.8.1/yplib/file.py
+-rw-rw-rw-   0        0        0     7361 2024-05-16 07:20:59.000000 yplib-5.8.1/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.8.1/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.8.1/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.8.1/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.8.1/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-21 08:16:59.000000 yplib-5.8.1/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.8.1/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:18:07.871639 yplib-5.8.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-21 08:18:07.000000 yplib-5.8.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-21 08:18:07.000000 yplib-5.8.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 08:18:07.000000 yplib-5.8.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 08:18:07.000000 yplib-5.8.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.8.0/LICENSE` & `yplib-5.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/setup.py` & `yplib-5.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.8.0",
+    version="5.8.1",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.8.0/yplib/__init__.py` & `yplib-5.8.1/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/yplib/chart.py` & `yplib-5.8.1/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/yplib/chart_html.py` & `yplib-5.8.1/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/yplib/db.py` & `yplib-5.8.1/yplib/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from yplib.index import *
 from yplib.http_util import *
 import pymysql
 import adbc_driver_manager
 import adbc_driver_flightsql.dbapi as flight_sql
 import warnings
 
-warnings.filterwarnings("ignore", message="Cannot disable autocommit", category=Warning)
+import threading
+
+# 创建一个线程本地存储对象
+thread_local = threading.local()
 
 
 # 有关数据库操作的类
 def get_connect(database=None, user=None, password=None, charset='utf8mb4', port=3306, host=None):
     return pymysql.connect(database=database, user=user, password=password, charset=charset, port=port, host=host)
 
 
@@ -57,46 +60,37 @@
 def get_doris_conn(db_config='doris'):
     config_db = get_config_data(db_config)
     my_uri = config_db['uri']
     my_db_kwargs = {
         adbc_driver_manager.DatabaseOptions.USERNAME.value: config_db['username'],
         adbc_driver_manager.DatabaseOptions.PASSWORD.value: config_db['password'],
     }
-    conn = flight_sql.connect(uri=my_uri, db_kwargs=my_db_kwargs)
+    conn = flight_sql.connect(uri=my_uri, db_kwargs=my_db_kwargs, autocommit=True)
     return conn
 
 
 # 执行 sql 语句, 并且提交, 默认值提交的了
 def exec_doris_sql(sql='', db_config='wh_doris', database='mx_risk'):
     exec_sql(sql, db_config=db_config, database=database)
     # conn = get_doris_conn(db_config)
     # cursor = conn.cursor()
     # cursor.execute(sql)
     # cursor.close()
     # conn.close()
 
 
-conn_doris = None
-
-
 def get_data_from_doris(sql='', db_config='doris'):
-    global conn_doris
-    # try:
-    if conn_doris is None:
-        conn_doris = get_doris_conn(db_config)
+    if not hasattr(thread_local, 'conn_doris'):
+        thread_local.conn_doris = get_doris_conn(db_config)
+    conn_doris = thread_local.conn_doris
     cursor = conn_doris.cursor()
     cursor.execute(sql)
     arrow_data = cursor.fetchallarrow()
     dataframe = arrow_data.to_pandas()
     json_data = dataframe.to_json(orient='records')
-    # finally:
-    #     if cursor is not None:
-    #         cursor.close()
-    #     if conn is not None:
-    #         conn.close()
     return json.loads(json_data)
 
 
 def get_data_line_one_from_doris(sql='', db_config='doris'):
     data_list = get_data_from_doris(sql, db_config=db_config)
     if len(data_list):
         return list(data_list[0].values())
```

### Comparing `yplib-5.8.0/yplib/file.py` & `yplib-5.8.1/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/yplib/http_util.py` & `yplib-5.8.1/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/yplib/index.py` & `yplib-5.8.1/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/yplib/mail.py` & `yplib-5.8.1/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/yplib/mail_html.py` & `yplib-5.8.1/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/yplib/markdown.py` & `yplib-5.8.1/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.0/yplib/multi_thread.py` & `yplib-5.8.1/yplib/multi_thread.py`

 * *Files identical despite different names*

