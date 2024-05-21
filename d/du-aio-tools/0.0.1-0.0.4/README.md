# Comparing `tmp/du_aio_tools-0.0.1.tar.gz` & `tmp/du_aio_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "du_aio_tools-0.0.1.tar", last modified: Mon Feb 26 07:52:46 2024, max compression
+gzip compressed data, was "du_aio_tools-0.0.4.tar", last modified: Tue May 21 06:38:02 2024, max compression
```

## Comparing `du_aio_tools-0.0.1.tar` & `du_aio_tools-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 07:52:46.161004 du_aio_tools-0.0.1/
--rw-rw-rw-   0        0        0      346 2024-02-26 07:52:46.159503 du_aio_tools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       91 2024-02-26 07:44:02.000000 du_aio_tools-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-26 07:52:46.143503 du_aio_tools-0.0.1/du_aio_tools/
--rw-rw-rw-   0        0        0        0 2022-12-16 08:31:49.000000 du_aio_tools-0.0.1/du_aio_tools/__init__.py
--rw-rw-rw-   0        0        0     2748 2024-02-26 07:42:04.000000 du_aio_tools-0.0.1/du_aio_tools/base_conn.py
--rw-rw-rw-   0        0        0     8621 2024-02-26 07:10:17.000000 du_aio_tools-0.0.1/du_aio_tools/base_spider.py
--rw-rw-rw-   0        0        0      201 2024-02-26 07:42:04.000000 du_aio_tools-0.0.1/du_aio_tools/exceptions.py
--rw-rw-rw-   0        0        0     2235 2024-02-19 09:14:48.000000 du_aio_tools-0.0.1/du_aio_tools/rsa.py
--rw-rw-rw-   0        0        0      528 2024-02-26 07:30:47.000000 du_aio_tools-0.0.1/du_aio_tools/schemas.py
--rw-rw-rw-   0        0        0      948 2024-02-26 07:28:57.000000 du_aio_tools-0.0.1/du_aio_tools/time.py
-drwxrwxrwx   0        0        0        0 2024-02-26 07:52:46.151504 du_aio_tools-0.0.1/du_aio_tools.egg-info/
--rw-rw-rw-   0        0        0      346 2024-02-26 07:52:45.000000 du_aio_tools-0.0.1/du_aio_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-02-26 07:52:46.000000 du_aio_tools-0.0.1/du_aio_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 07:52:45.000000 du_aio_tools-0.0.1/du_aio_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-02-26 07:52:45.000000 du_aio_tools-0.0.1/du_aio_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-02-26 07:52:45.000000 du_aio_tools-0.0.1/du_aio_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 07:52:46.161004 du_aio_tools-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1684 2024-02-26 07:52:32.000000 du_aio_tools-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-26 07:52:46.158004 du_aio_tools-0.0.1/tests/
--rw-rw-rw-   0        0        0      114 2024-02-18 02:18:14.000000 du_aio_tools-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2108 2024-02-26 07:08:32.000000 du_aio_tools-0.0.1/tests/conn.py
--rw-rw-rw-   0        0        0      937 2024-02-20 00:57:30.000000 du_aio_tools-0.0.1/tests/t1.py
--rw-rw-rw-   0        0        0      543 2024-02-26 07:13:24.000000 du_aio_tools-0.0.1/tests/t_html.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:38:02.994034 du_aio_tools-0.0.4/
+-rw-rw-rw-   0        0        0      515 2024-05-21 06:38:02.993537 du_aio_tools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2024-03-06 06:35:10.000000 du_aio_tools-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 06:38:02.982610 du_aio_tools-0.0.4/du_aio_tools/
+-rw-rw-rw-   0        0        0      856 2024-03-07 07:26:59.000000 du_aio_tools-0.0.4/du_aio_tools/Iterator_xml.py
+-rw-rw-rw-   0        0        0        0 2022-12-16 08:31:49.000000 du_aio_tools-0.0.4/du_aio_tools/__init__.py
+-rw-rw-rw-   0        0        0     2789 2024-05-21 06:37:14.000000 du_aio_tools-0.0.4/du_aio_tools/base_conn.py
+-rw-rw-rw-   0        0        0     8691 2024-05-21 06:37:14.000000 du_aio_tools-0.0.4/du_aio_tools/base_spider.py
+-rw-rw-rw-   0        0        0      201 2024-02-26 07:42:04.000000 du_aio_tools-0.0.4/du_aio_tools/exceptions.py
+-rw-rw-rw-   0        0        0     2235 2024-02-19 09:14:48.000000 du_aio_tools-0.0.4/du_aio_tools/rsa.py
+-rw-rw-rw-   0        0        0      528 2024-02-26 07:30:47.000000 du_aio_tools-0.0.4/du_aio_tools/schemas.py
+-rw-rw-rw-   0        0        0     1501 2024-03-06 04:13:04.000000 du_aio_tools-0.0.4/du_aio_tools/time.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:38:02.988570 du_aio_tools-0.0.4/du_aio_tools.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-21 06:38:02.000000 du_aio_tools-0.0.4/du_aio_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:38:02.994531 du_aio_tools-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2024-05-21 06:34:41.000000 du_aio_tools-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:38:02.992544 du_aio_tools-0.0.4/tests/
+-rw-rw-rw-   0        0        0      114 2024-02-18 02:18:14.000000 du_aio_tools-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2108 2024-02-26 07:08:32.000000 du_aio_tools-0.0.4/tests/conn.py
+-rw-rw-rw-   0        0        0      937 2024-02-20 00:57:30.000000 du_aio_tools-0.0.4/tests/t1.py
+-rw-rw-rw-   0        0        0      543 2024-02-26 07:13:24.000000 du_aio_tools-0.0.4/tests/t_html.py
```

### Comparing `du_aio_tools-0.0.1/du_aio_tools/base_conn.py` & `du_aio_tools-0.0.4/du_aio_tools/base_conn.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # @author: Dyz
 # @file: base_conn.py
 # @software: PyCharm
 import functools
 import warnings
 from typing import Optional
 
+from tortoise.models import ModelMeta
 from tortoise import BaseDBAsyncClient, Model, fields, Tortoise
 
 
 async def init_db(tortoise_orm, create: bool = False):
     """
     >>> {
         "connections": {
@@ -65,14 +66,15 @@
 
         return wrap
 
     return _load_db
 
 
 class MyModel(Model):
+
     @classmethod
     async def truncate_model(cls, using_db: Optional[BaseDBAsyncClient] = None):
         """截断表"""
         db = using_db or cls._choose_db(True)
         data = await cls.all().limit(1)
         if data:
             return await db.execute_query('TRUNCATE TABLE {}'.format(cls._meta.db_table))
```

### Comparing `du_aio_tools-0.0.1/du_aio_tools/base_spider.py` & `du_aio_tools-0.0.4/du_aio_tools/base_spider.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from pathlib import Path
 
 import httpx
 from requests import Session
 from fake_useragent import UserAgent
 from tenacity import retry, stop_after_attempt, wait_fixed
 
-from du_tools.exceptions import HTTPError
+from du_aio_tools.exceptions import HTTPError
+from du_aio_tools.time import timer
 
-logger = logging.getLogger("dutools.BaseSpider")
+logger = logging.getLogger("du_aio_tools.BaseSpider")
 
 MAX_RETRY = 3  # 最大重试次数
 WAIT_FIXED = 3  # 重试间隔 3s
 TIMEOUT = 10  # 重试间隔 10s
 
 
 class BaseDataSpider:
@@ -108,14 +109,15 @@
         result = []
         for _ in range(len(arr) - 1):
             s_pos, e_pos = arr[_], arr[_ + 1] - 1
             result.append([s_pos, e_pos])
         result[-1][-1] = file_size - 1
         return result
 
+    @timer
     def download(self, url, file: Path, method='get', **kwargs):
         """requests 数据流 方式下载文件"""
         if not file.exists():
             file.touch()  # 创建文件
 
         if method.lower() == 'get':  # 1M
             res = self.get(url, **kwargs, stream=True)
@@ -168,14 +170,15 @@
             res = await self.aio_get(url, headers=headers, **kwargs)
         else:
             res = await self.aio_post(url, headers=headers, **kwargs)
         with open(file, "rb+") as f:
             f.seek(s_pos)
             f.write(res.content)
 
+    @timer
     async def aio_download(self, url, file: Path, method='get', **kwargs):
         """httpx 异步分片式 下载文件"""
         if not file.exists():
             file.touch()  # 创建文件
 
         res = httpx.head(url, **kwargs)
         filesize = int(res.headers['Content-Length'])
```

### Comparing `du_aio_tools-0.0.1/du_aio_tools/rsa.py` & `du_aio_tools-0.0.4/du_aio_tools/rsa.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.1/du_aio_tools/schemas.py` & `du_aio_tools-0.0.4/du_aio_tools/schemas.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.1/du_aio_tools/time.py` & `du_aio_tools-0.0.4/du_aio_tools/time.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 # -*- coding: utf-8 -*-
 # @time: 2022/4/21 16:50
 # @author: Dyz
 # @file: time.py
 # @software: PyCharm
 import asyncio
 from functools import wraps
+from pathlib import Path
 from time import gmtime, strftime, time
 
 
+def get_args_file(*args, **kwargs):
+    """从传入参数中找寻file相关的参数"""
+    for file in args:
+        if isinstance(file, Path):
+            return file
+    for key, val in kwargs.items():
+        if isinstance(val, Path):
+            return val
+
+
+def _timer(func, start_time, *args, **kwargs):
+    """计时与打印"""
+    time_ = strftime("%H:%M:%S", gmtime(time() - start_time))
+    if 'download' in str(func.__name__):
+        file = get_args_file(*args, **kwargs)
+        print(f'{file or str(func.__name__)} 耗时: {time_}')
+    else:
+        print(f'{func.__name__} 耗时: {time_}')
+
+
 def timer(func):
     """ 计算时间装饰器 """
     if asyncio.iscoroutinefunction(func):
+        # 用于装饰异步函数
         @wraps(func)
         async def aio_wrapper(*args, **kwargs):
             start_time = time()
             res = await func(*args, **kwargs)
-            time_ = strftime("%H:%M:%S", gmtime(time() - start_time))
-            print(f'{func.__name__} 耗时: {time_}')
+            _timer(func, start_time, *args, **kwargs)
             return res
 
         return aio_wrapper
 
     else:
         @wraps(func)
         def wrapper(*args, **kwargs):
             start_time = time()
             res = func(*args, **kwargs)
-            time_ = strftime("%H:%M:%S", gmtime(time() - start_time))
-            print(f'{func.__name__} 耗时: {time_}')
+            _timer(func, start_time, *args, **kwargs)
             return res
 
         return wrapper
```

### Comparing `du_aio_tools-0.0.1/setup.py` & `du_aio_tools-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 # @Software: PyCharm
 
 import os
 from setuptools import find_packages, setup
 
 # 提供一些有用的信息
 NAME = 'du_aio_tools'  # Python 包的名称，即在 pip install 时后面跟的包名
-VERSION = '0.0.1'  # 包的版本，每次上传到 PyPI 都需要改变这个版本号，否则只会往存储空间增加新内容，无法达到预期
+VERSION = '0.0.4'  # 包的版本，每次上传到 PyPI 都需要改变这个版本号，否则只会往存储空间增加新内容，无法达到预期
 DESCRIPTION = "async tools"  # 关于该包的剪短描述
 if os.path.exists('README.md'):  # 如果需要，可以加入一段较长的描述，比如读取 README.md，该段长描述会直接显示在 PyPI 的页面上
     with open('README.md', encoding='utf-8') as f:
         LONG_DESCRIPTION = f.read()
 else:
     LONG_DESCRIPTION = DESCRIPTION
 AUTHOR = 'DYZ'  # 留下大名
 AUTHOR_EMAIL = 'duyuchau@gmail.com'  # 留下邮箱
 LICENSE = 'MIT'  # 定义合适自己的许可证，实在不知道，那就 MIT 吧
 PLATFORMS = [  # 支持的平台，如果所有平台都支持，可以填 all
     'all',
 ]
 
 REQUIRES = [
-    'pydantic==1.10.2',
-    'pycryptodome==3.16.0',
-    'httpx==0.23.1',
-    'requests==2.31.0',
-    'fake_useragent==1.1.3'
+    'pydantic~=1.10.2',
+    # 'pydantic~=2.7.0',
+    'pycryptodome',
+    'httpx',
+    'requests',
+    'fake_useragent',
+    'tenacity',
 ]
 
 # 需要的信息就在 setup() 中加上，不需要的可以不加
 setup(
     name=NAME,
     version=VERSION,
     description=(
```

### Comparing `du_aio_tools-0.0.1/tests/conn.py` & `du_aio_tools-0.0.4/tests/conn.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.1/tests/t1.py` & `du_aio_tools-0.0.4/tests/t1.py`

 * *Files identical despite different names*

### Comparing `du_aio_tools-0.0.1/tests/t_html.py` & `du_aio_tools-0.0.4/tests/t_html.py`

 * *Files identical despite different names*

