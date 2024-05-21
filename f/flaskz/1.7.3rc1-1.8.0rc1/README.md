# Comparing `tmp/flaskz-1.7.3rc1.tar.gz` & `tmp/flaskz-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.7.3rc1.tar", last modified: Tue Apr 16 02:00:09 2024, max compression
+gzip compressed data, was "flaskz-1.8.0rc1.tar", last modified: Tue May 21 03:02:48 2024, max compression
```

## Comparing `flaskz-1.7.3rc1.tar` & `flaskz-1.8.0rc1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.550594 flaskz-1.7.3rc1/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2023-12-29 07:22:00.000000 flaskz-1.7.3rc1/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     9710 2024-04-16 02:00:09.550215 flaskz-1.7.3rc1/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     9102 2024-04-15 11:36:23.000000 flaskz-1.7.3rc1/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.7.3rc1/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      778 2024-04-16 02:00:09.551653 flaskz-1.7.3rc1/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.506875 flaskz-1.7.3rc1/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.512737 flaskz-1.7.3rc1/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       25 2024-04-14 04:30:05.000000 flaskz-1.7.3rc1/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.516736 flaskz-1.7.3rc1/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.7.3rc1/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8563 2023-11-06 11:28:38.000000 flaskz-1.7.3rc1/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.520306 flaskz-1.7.3rc1/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.7.3rc1/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-12-11 08:39:54.000000 flaskz-1.7.3rc1/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)    22378 2024-04-15 12:15:00.000000 flaskz-1.7.3rc1/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.520831 flaskz-1.7.3rc1/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.7.3rc1/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.527060 flaskz-1.7.3rc1/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     6102 2024-02-02 04:22:48.000000 flaskz-1.7.3rc1/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    31531 2024-04-14 10:04:24.000000 flaskz-1.7.3rc1/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    11055 2024-01-22 02:47:13.000000 flaskz-1.7.3rc1/src/flaskz/models/_model.py
--rw-r--r--   0 taozh      (501) staff       (20)    20087 2024-04-07 02:45:01.000000 flaskz-1.7.3rc1/src/flaskz/models/_query_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    11212 2024-04-14 09:19:30.000000 flaskz-1.7.3rc1/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.7.3rc1/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.531391 flaskz-1.7.3rc1/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    21363 2024-01-01 06:50:15.000000 flaskz-1.7.3rc1/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.7.3rc1/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     4173 2023-12-30 16:50:29.000000 flaskz-1.7.3rc1/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.547250 flaskz-1.7.3rc1/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.7.3rc1/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2502 2023-12-30 16:37:35.000000 flaskz-1.7.3rc1/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2848 2023-12-30 16:37:56.000000 flaskz-1.7.3rc1/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7248 2024-04-14 10:55:34.000000 flaskz-1.7.3rc1/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    13669 2024-01-17 09:40:36.000000 flaskz-1.7.3rc1/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      860 2023-12-30 16:48:17.000000 flaskz-1.7.3rc1/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.7.3rc1/src/flaskz/utils/_magic.py
--rw-r--r--   0 taozh      (501) staff       (20)     1020 2023-12-30 16:50:25.000000 flaskz-1.7.3rc1/src/flaskz/utils/_private.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7933 2024-01-30 02:20:56.000000 flaskz-1.7.3rc1/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1201 2023-12-30 16:50:25.000000 flaskz-1.7.3rc1/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3045 2024-01-30 02:31:20.000000 flaskz-1.7.3rc1/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     4322 2023-12-30 13:56:42.000000 flaskz-1.7.3rc1/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.548505 flaskz-1.7.3rc1/src/flaskz.egg-info/
--rw-r--r--   0 taozh      (501) staff       (20)     9710 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      981 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       87 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.624008 flaskz-1.8.0rc1/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2023-12-29 07:22:00.000000 flaskz-1.8.0rc1/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)    10311 2024-05-21 03:02:48.623748 flaskz-1.8.0rc1/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     9710 2024-05-21 03:01:29.000000 flaskz-1.8.0rc1/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.8.0rc1/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      778 2024-05-21 03:02:48.624797 flaskz-1.8.0rc1/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.579816 flaskz-1.8.0rc1/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.586160 flaskz-1.8.0rc1/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       25 2024-05-21 03:01:38.000000 flaskz-1.8.0rc1/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.592264 flaskz-1.8.0rc1/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.8.0rc1/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8563 2023-11-06 11:28:38.000000 flaskz-1.8.0rc1/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.596192 flaskz-1.8.0rc1/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.8.0rc1/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-12-11 08:39:54.000000 flaskz-1.8.0rc1/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)    22535 2024-05-14 10:17:54.000000 flaskz-1.8.0rc1/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.598135 flaskz-1.8.0rc1/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.8.0rc1/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.605485 flaskz-1.8.0rc1/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6102 2024-02-02 04:22:48.000000 flaskz-1.8.0rc1/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    31603 2024-05-13 10:53:54.000000 flaskz-1.8.0rc1/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    11055 2024-01-22 02:47:13.000000 flaskz-1.8.0rc1/src/flaskz/models/_model.py
+-rw-r--r--   0 taozh      (501) staff       (20)    20087 2024-04-07 02:45:01.000000 flaskz-1.8.0rc1/src/flaskz/models/_query_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    13701 2024-05-15 09:49:31.000000 flaskz-1.8.0rc1/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.8.0rc1/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.609709 flaskz-1.8.0rc1/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    29975 2024-05-07 04:04:59.000000 flaskz-1.8.0rc1/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.8.0rc1/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     4173 2023-12-30 16:50:29.000000 flaskz-1.8.0rc1/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.621692 flaskz-1.8.0rc1/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.8.0rc1/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2502 2023-12-30 16:37:35.000000 flaskz-1.8.0rc1/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2848 2023-12-30 16:37:56.000000 flaskz-1.8.0rc1/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7248 2024-04-14 10:55:34.000000 flaskz-1.8.0rc1/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    13669 2024-01-17 09:40:36.000000 flaskz-1.8.0rc1/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      860 2023-12-30 16:48:17.000000 flaskz-1.8.0rc1/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.8.0rc1/src/flaskz/utils/_magic.py
+-rw-r--r--   0 taozh      (501) staff       (20)     1020 2023-12-30 16:50:25.000000 flaskz-1.8.0rc1/src/flaskz/utils/_private.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     9439 2024-05-14 07:19:13.000000 flaskz-1.8.0rc1/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1201 2023-12-30 16:50:25.000000 flaskz-1.8.0rc1/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3045 2024-01-30 02:31:20.000000 flaskz-1.8.0rc1/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     4322 2023-12-30 13:56:42.000000 flaskz-1.8.0rc1/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-05-21 03:02:48.622648 flaskz-1.8.0rc1/src/flaskz.egg-info/
+-rw-r--r--   0 taozh      (501) staff       (20)    10311 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      981 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       87 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2024-05-21 03:02:48.000000 flaskz-1.8.0rc1/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.7.3rc1/LICENSE` & `flaskz-1.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/PKG-INFO` & `flaskz-1.8.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.7.3rc1
+Version: 1.8.0rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,34 +17,41 @@
 Requires-Dist: requests>=2
 Provides-Extra: ext
 Requires-Dist: pycryptodome>=3.15.0; extra == "ext"
 Requires-Dist: paramiko>=3.0.0; extra == "ext"
 
 ## 关于
 
-*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
+*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展工具集, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
 
 ## 使用
 
 1. [☞数据库初始化&常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_model_init.html)
 2. [☞数据模型扩展类](http://zhangyiheng.com/blog/articles/py_flaskz_model_mixin.html)
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.7.3rc1** `2024/04/16`
+- **1.8.0rc1** `2024/05/21`
+    - [A] 扩展`flaskz.rest`路由生成模块
+        - 添加`register_model_bulk_route`函数, 用于生成指定数据模型的批量增删改路由
+        - 添加`register_model_bulk_add_route`函数, 用于生成指定数据模型的批量添加路由
+        - 添加`register_model_bulk_delete_route`函数, 用于生成指定数据模型的批量删除路由
+        - 添加`register_model_bulk_update_route`函数, 用于生成指定数据模型的批量更新路由
+    - [A] 添加`flaskz.utils.request`函数以替代`flaskz.utils.api_request`函数
+
+- **1.7.3** `2024/05/01`
     - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
     - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
-    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认启用)
+    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认复用)
     - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
     - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
-
 - **1.7.2** `2024/02/01`
     - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
     - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
 - **1.7.1** `2024/01/05`
     - [F] 修复SQLAlchemy<2.0.0版本时, `flaskz.models._util.py`中`BinaryExpression`类的导入问题
 - **1.7.0** `2024/01/01`
     - [C] `SQLAlchemy`依赖的版本从`>=1.3.13(EOL)`升级到`>=1.4.0(Maintenance)`
```

### Comparing `flaskz-1.7.3rc1/README.md` & `flaskz-1.8.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 ## 关于
 
-*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
+*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展工具集, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
 
 ## 使用
 
 1. [☞数据库初始化&常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_model_init.html)
 2. [☞数据模型扩展类](http://zhangyiheng.com/blog/articles/py_flaskz_model_mixin.html)
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.7.3rc1** `2024/04/16`
+- **1.8.0rc1** `2024/05/21`
+    - [A] 扩展`flaskz.rest`路由生成模块
+        - 添加`register_model_bulk_route`函数, 用于生成指定数据模型的批量增删改路由
+        - 添加`register_model_bulk_add_route`函数, 用于生成指定数据模型的批量添加路由
+        - 添加`register_model_bulk_delete_route`函数, 用于生成指定数据模型的批量删除路由
+        - 添加`register_model_bulk_update_route`函数, 用于生成指定数据模型的批量更新路由
+    - [A] 添加`flaskz.utils.request`函数以替代`flaskz.utils.api_request`函数
+
+- **1.7.3** `2024/05/01`
     - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
     - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
-    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认启用)
+    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认复用)
     - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
     - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
-
 - **1.7.2** `2024/02/01`
     - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
     - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
 - **1.7.1** `2024/01/05`
     - [F] 修复SQLAlchemy<2.0.0版本时, `flaskz.models._util.py`中`BinaryExpression`类的导入问题
 - **1.7.0** `2024/01/01`
     - [C] `SQLAlchemy`依赖的版本从`>=1.3.13(EOL)`升级到`>=1.4.0(Maintenance)`
```

### Comparing `flaskz-1.7.3rc1/setup.cfg` & `flaskz-1.8.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.7.3rc1
+version = 1.8.0rc1
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls =
```

### Comparing `flaskz-1.7.3rc1/src/flaskz/auth/_jws.py` & `flaskz-1.8.0rc1/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/ext/cypher.py` & `flaskz-1.8.0rc1/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/ext/ssh.py` & `flaskz-1.8.0rc1/src/flaskz/ext/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,20 +167,20 @@
         else:
             self._timeout = 10
 
         if hostname is None and 'host' in kwargs:
             hostname = kwargs.pop('host', None)
 
         self._pre_commands = None  # @2024-04-14 add
+        self._pre_commands_run = False
         pre_commands = kwargs.pop('pre_commands', None)
         if type(pre_commands) is str:
             pre_commands = [pre_commands]
         if type(pre_commands) is list and len(pre_commands) > 0:
             self._pre_commands = pre_commands
-            self._pre_commands_run = False
 
         # self.transport = paramiko.Transport((hostname, port))
         self.transport = paramiko.Transport(_create_socket(hostname=hostname, port=port, timeout=self._timeout))
         _connect_kwargs = kwargs.pop('connect_kwargs', None) or {}  # kwargs for Transport.connect()
         self.transport.connect(username=username, password=password, **_connect_kwargs)
         if self.transport.is_authenticated() is not True:  # @2023-12-28 add(Oops, unhandled type 3 ('unimplemented'))
             raise AuthenticationException('Authentication failed.')
@@ -226,18 +226,19 @@
          :param recv: wait for the result or not.
          :param clean: clean output info or not, default True(clean)
          :param prompt: the prompt of the command line
 
          :return: the output of the command
         """
 
-        if self._pre_commands and self._pre_commands_run is False:
-            # self._run_command('', False)
-            for pre_command in self._pre_commands:
-                self._run_command(pre_command, False)
+        if self._pre_commands_run is False and self._pre_commands:
+            self._run_command('', False)
+            pre_command_len = len(self._pre_commands)
+            for index, pre_command in enumerate(self._pre_commands):
+                self._run_command(pre_command, index == pre_command_len - 1)
             self._pre_commands_run = True
 
         if prompt is None:  # prompt is False for config
             prompt = self.get_prompt()  # 1.get prompt 2.remove welcome
 
         command, recv, clean = _get_command_arg(command, recv, clean)
         output = self._run_command(command, recv, prompt)
@@ -446,15 +447,15 @@
                 continue
             else:
                 recv_start = None
                 if count == 0:  # Solve the problem of incomplete data
                     time.sleep(recv_start_delay)
             count += 1
             data = self.channel.recv(recv_max_bytes)
-            info = data.decode()
+            info = data.decode('utf-8', 'backslashreplace')  # @2024-04-18 data.decode() --> current
             res = info.replace(' \r', '')
             res_list.append(res)
             if len(info) < recv_max_bytes:  # read speed > write speed
                 if (prompt is not None and info.endswith(prompt)) or info.endswith(self.recv_endswith):
                     time.sleep(0.02)  # Make sure recv is finished, info.endswith(self.recv_endswith) Not 100% sure
                     if not self.channel.recv_ready():
                         break
```

### Comparing `flaskz-1.7.3rc1/src/flaskz/log/__init__.py` & `flaskz-1.8.0rc1/src/flaskz/log/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/models/__init__.py` & `flaskz-1.8.0rc1/src/flaskz/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/models/_base.py` & `flaskz-1.8.0rc1/src/flaskz/models/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,15 +536,14 @@
 
         :return: the deleted count
         """
         with db_session() as session:
             return session.query(cls).delete()
 
     # -------------------------------------------query-------------------------------------------
-
     @classmethod
     def query(cls):
         """
         Return a 'Query' object corresponding to this class.
 
         Example:
             query = TemplateModel.query()
@@ -607,14 +606,16 @@
 
         Example:
             ins = User.query_by_pk(1)
 
         :param pk_value:
         :return:
         """
+        if pk_value is None:  # @2024-05-14 add
+            return None
         with db_session(do_commit=False) as session:
             # instance = session.query(cls).get(pk_value)
             instance = _session_get(session, cls, pk_value)
         return instance
 
     @classmethod
     def query_by(cls, by_dict, return_first=False):
```

### Comparing `flaskz-1.7.3rc1/src/flaskz/models/_model.py` & `flaskz-1.8.0rc1/src/flaskz/models/_model.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/models/_query_util.py` & `flaskz-1.8.0rc1/src/flaskz/models/_query_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/models/_util.py` & `flaskz-1.8.0rc1/src/flaskz/models/_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from flask import g
 from sqlalchemy import text, or_, and_, inspect
 from sqlalchemy.sql.elements import BinaryExpression  # @2024-01-04 update, BinaryExpression not in sqlalchemy.__init__.py when sqlalchemy<2.0.0
 
 from . import DBSession
 from ._base import BaseModelMixin
-from ..utils import get_g_cache, set_g_cache, remove_g_cache
+from ..utils import get_g_cache, set_g_cache, remove_g_cache, get_dict_mapping, get_ins_mapping
 
 __all__ = ['create_instance', 'create_relationships',
-           'query_all_models', 'query_multiple_model',
+           'query_all_models', 'query_multiple_model', 'query_from_g_cache',
            'append_debug_queries', 'get_debug_queries', 'append_query_filter',
            'get_db_session', 'db_session', 'close_db_session',
            'model_to_dict', 'refresh_instance',
            'is_model_mixin_instance']
 
 
 def create_instance(model_cls, data, create_relationship=True):
@@ -105,14 +105,65 @@
     :param cls_list:
     :return:If failed, returns the failed tuple, otherwise, returns the the data list.
     """
 
     return query_all_models(*cls_list)
 
 
+def query_from_g_cache(model_class, by_value, attr=None, to_dict=True, mapping_key=None, cache_key=None):
+    """
+    Query data from g(flask), if data not exist, query first and cache.
+
+    .. versionadded:: 1.8.0
+
+    Example:
+        query_from_g_cache(User, 1)  # return 'dict' of User properties with id=1
+        query_from_g_cache(User, 1, 'username')  # return 'username' property of User with id=1
+        query_from_g_cache(User, 'admin', mapping_key='username')  # use 'username' as key of the cached dict
+        query_from_g_cache(User, 1, to_dict=False)  # id=1(ins) # cache 'instance'
+        query_from_g_cache(User, False)  # return 'all' users
+
+    :param model_class: the model class to query and cache, ex)User
+    :param by_value: the value to query, if False return all items ex) 1/'admin'
+    :param attr: the attribute of the data to return, ex)'username'/'email'
+    :param to_dict: cache data as dict or not, ex) True/False
+    :param mapping_key: the key used to create data mapping, if None, use the primary filed of the model_class, ex)'username'
+    :param cache_key: the key used to cache data, if None use 'flaskz_' + class_name + '_model_cached_items'
+    :return:
+    """
+    if by_value is None:
+        return None
+    class_name = model_class.get_class_name()
+    if cache_key is None:
+        cache_key = 'flaskz_' + class_name + '_model_cached_items'
+    mapping = get_g_cache(cache_key)
+
+    if mapping is None:
+        if mapping_key is None:  # if key is None, use primary_field of the model_class
+            mapping_key = model_class.get_primary_field()
+        success, data = model_class.query_all()
+        if success:
+            if to_dict is True or type(to_dict) is dict:
+                _to_dict_option = to_dict if type(to_dict) is dict else None
+                mapping = get_dict_mapping(model_to_dict(data, _to_dict_option), mapping_key)
+            else:
+                mapping = get_ins_mapping(data, mapping_key)
+            set_g_cache(cache_key, mapping)
+    if mapping:
+        if by_value is False:  # if pk_value is False, return all items
+            return list(mapping.values())
+        item = mapping.get(by_value)
+        if item and attr is not None:
+            if to_dict is True:
+                return item.get(attr)
+            else:
+                return getattr(item, attr, None)
+        return item
+
+
 def append_debug_queries(query):
     if _has_flask_g_context():  # @2022-07-26 add,
         debug_queries = getattr(g, 'z_debug_queries', None)
         if debug_queries is None:
             g.z_debug_queries = debug_queries = []
         debug_queries.append(query)
```

### Comparing `flaskz-1.7.3rc1/src/flaskz/res_status_codes.py` & `flaskz-1.8.0rc1/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/rest/__init__.py` & `flaskz-1.8.0rc1/src/flaskz/rest/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -112,14 +112,47 @@
         register_model_upsert_route(app, model, rule, module, to_json_option=to_json_option, strict_slash=strict_slash)
     if 'query' in types:
         register_model_query_route(app, model, rule, module, to_json_option=to_json_option, strict_slash=strict_slash)
     if 'pss' in types:
         register_model_query_pss_route(app, model, rule, module, to_json_option=to_json_option, strict_slash=strict_slash, get_pss_config=get_pss_config)
     if multi_models and ('multi' in types or 'multiple' in types):
         register_models_query_route(app, multi_models, rule, module)
+    if 'bulk_add' in types:
+        register_model_bulk_add_route(app, model, rule, module, strict_slash=strict_slash)
+    if 'bulk_delete' in types:
+        register_model_bulk_delete_route(app, model, rule, module, strict_slash=strict_slash)
+    if 'bulk_update' in types:
+        register_model_bulk_update_route(app, model, rule, module, strict_slash=strict_slash)
+    return app
+
+
+def register_model_bulk_route(app, model, rule, module=None, types=None, strict_slash=True):
+    """
+    Register url rules for bulk operations of the specified model class to the application/blueprint.
+
+    .. versionadded:: 1.8 @2024-05-03
+
+    Example:
+        register_model_bulk_route(api_bp, User, 'users', 'users')
+
+    :param app: Flask application / Blueprint instance
+    :param model: The DB model class, ex)User
+    :param rule: The URL rule string, ex)/users
+    :param module: The module name for permission check, ex)users
+    :param types: The types of the route, default is ['bulk_add', 'bulk_delete', 'bulk_update']
+    :param strict_slash: If not false, the rule url will end with slash
+    :return:
+    """
+    types = get_list(types, ['bulk_add', 'bulk_delete', 'bulk_update'])
+    if 'bulk_add' in types:
+        register_model_bulk_add_route(app, model, rule, module, strict_slash=strict_slash)
+    if 'bulk_delete' in types:
+        register_model_bulk_delete_route(app, model, rule, module, strict_slash=strict_slash)
+    if 'bulk_update' in types:
+        register_model_bulk_update_route(app, model, rule, module, strict_slash=strict_slash)
     return app
 
 
 def register_model_add_route(app, model, rule, module=None, action='add', methods=None, to_json_option=None, strict_slash=True, endpoint=None):
     """
     Register a add type URL rule for the specified model class to the application/blueprint.
 
@@ -134,19 +167,19 @@
     :param methods: The methods of the route, default is ['POST']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
     :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['POST']
-    rule, did_rule = _get_route_rule(rule, strict_slash)
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash)
 
-    @app.route(rule, methods=methods, endpoint=endpoint)
+    @app.route(base_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
-    @gen_route_method('add', rule)
+    @gen_route_method('add', base_rule)
     def add():
         request_json = request.json
         req_log_data = json.dumps(request_json)
 
         success, data = model.add(request_json)
         res_data = model_to_dict(data, to_json_option)
 
@@ -176,19 +209,19 @@
     :param methods: The methods of the route, default is ['DELETE']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
     :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['DELETE']
-    rule, did_rule = _get_route_rule(rule, strict_slash)
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash, did_suffix='<did>')
 
     @app.route(did_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
-    @gen_route_method('delete', rule)
+    @gen_route_method('delete', base_rule)
     def delete(did):
         success, data = model.delete(did)
         res_data = model_to_dict(data, to_json_option)
 
         res_log_data = get_log_data(res_data)
         log_operation(module, 'delete', success, did, res_log_data)
         flaskz_logger.info(get_rest_log_msg('Delete {} data'.format(model.get_class_name()), did, success, res_log_data))
@@ -212,20 +245,20 @@
     :param methods: The methods of the route, default is ['PATCH']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
     :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['PATCH']
-    rule, did_rule = _get_route_rule(rule, strict_slash)
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash, did_suffix='<did>')
 
-    @app.route(rule, methods=methods, endpoint=endpoint)
+    @app.route(base_rule, methods=methods, endpoint=endpoint)
     @app.route(did_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
-    @gen_route_method('update', rule)
+    @gen_route_method('update', base_rule)
     def update(did=None):
         request_json = request.json
         if did is not None:
             request_json[model.get_primary_field()] = did  # use pk in url
         req_log_data = json.dumps(request_json)
 
         success, data = model.update(request_json)
@@ -254,19 +287,19 @@
     :param methods: The methods of the route, default is ['PATCH']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
     :param rule_suffix: The upsert suffix, default is 'upsert'
     :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     """
     methods = methods or ['POST']
-    rule, upsert_rule = _get_route_rule(rule, strict_slash, rule_suffix)
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash, rule_suffix=rule_suffix)
 
-    @app.route(upsert_rule, methods=methods, endpoint=endpoint)
+    @app.route(suffix_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
-    @gen_route_method('upsert', rule)
+    @gen_route_method('upsert', base_rule)
     def upsert():
         request_json = request.json
         req_log_data = json.dumps(request_json)
 
         if request_json.get(model.get_primary_field()):
             upsert_action = "update"
             success, data = model.update(request_json)
@@ -297,20 +330,20 @@
     :param methods: The methods of the route, default is ['GET']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
     :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['GET']
-    rule, did_rule = _get_route_rule(rule, strict_slash)
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash, did_suffix='<did>')
 
-    @app.route(rule, methods=methods, endpoint=endpoint)
+    @app.route(base_rule, methods=methods, endpoint=endpoint)
     @app.route(did_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
-    @gen_route_method('query', rule)
+    @gen_route_method('query', base_rule)
     def query(did=None):
         if did is None:
             success, data = model.query_all()
         else:
             try:
                 data = model.query_by_pk(did)
                 if data:
@@ -348,19 +381,19 @@
     :param strict_slash: If not false, the rule url will end with slash
     :param rule_suffix: The pss suffix, default is 'query_pss'
     :param get_pss_config: Callback function used to generate pss config.
     :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['GET', 'POST']
-    rule, pss_rule = _get_route_rule(rule, strict_slash, rule_suffix)
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash, rule_suffix=rule_suffix)
 
-    @app.route(pss_rule, methods=methods, endpoint=endpoint)
+    @app.route(suffix_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
-    @gen_route_method('query_pss', rule)
+    @gen_route_method('query_pss', base_rule)
     def query_pss():
         request_json = get_request_json({})  # @2023-06-15, request.json --> get_request_json({})
         req_log_data = json.dumps(request_json)
 
         if callable(get_pss_config):  # @2023-10-13 add
             request_json = get_pss_config(request_json)  # @2023-10-23 fix, get_pss_config-->request_json
 
@@ -400,19 +433,19 @@
     :param strict_slash: If not false, the rule url will end with slash
     :param rule_suffix: The pss suffix, default is 'multi'
     :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
 
     :return:
     """
     methods = methods or ['GET']
-    rule, multi_rule = _get_route_rule(rule, strict_slash, rule_suffix)
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash, rule_suffix=rule_suffix)
 
-    @app.route(multi_rule, methods=methods, endpoint=endpoint)
+    @app.route(suffix_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
-    @gen_route_method('query_multi', rule)
+    @gen_route_method('query_multi', base_rule)
     def query_multi():
         model_cls_list = []
         multi_list = []
         for key in models:
             item = models[key]
             item_option = {}
             m_cls = None
@@ -439,25 +472,166 @@
             for index, item in enumerate(multi_list):
                 res_data[item.get('field')] = model_to_dict(result[index], item.get('option'))
 
         flaskz_logger.debug(get_rest_log_msg('Query multi {} data'.format(model_cls_list), None, success, res_data))
         return create_response(success, res_data)
 
 
-def _get_route_rule(rule, strict_slash=True, suffix='<did>'):
+def register_model_bulk_add_route(app, model, rule, module=None, action='add', methods=None, strict_slash=True, rule_suffix='bulk', endpoint=None):
+    """
+    Register bulk add type URL rule for the specified model class to the application/blueprint.
+
+    .. versionadded:: 1.8 @2024-05-03
+
+    Examples:
+        register_model_bulk_add_route(api_blueprint, User, 'users', 'users')
+
+    :param app: Flask application / Blueprints instance
+    :param model: The DB model class, ex)User
+    :param rule: The URL rule string, ex)/users
+    :param module: The module name for permission check, ex)users
+    :param action: The action of the module for permission check, ex)add
+    :param methods: The methods of the route, default is ['POST']
+    :param strict_slash: If not false, the rule url will end with slash
+    :param rule_suffix: The upsert suffix, default is 'bulk-add'
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
+    :return:
+    """
+    methods = methods or ['POST']
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash, rule_suffix=rule_suffix)
+
+    @app.route(suffix_rule, methods=methods, endpoint=endpoint)
+    @rest_permission_required(module, action)
+    @gen_route_method('bulk_add', base_rule)
+    def bulk_add():
+        request_json = request.json
+        req_log_data = json.dumps(request_json)
+        try:
+            model.bulk_add(request_json)
+            success, res_data = True, request_json
+        except Exception as e:
+            flaskz_logger.exception(e)
+            success, res_data = False, res_status_codes.db_add_err
+
+        res_log_data = get_log_data(res_data)
+        log_operation(module, 'add', success, req_log_data, res_log_data)
+        flaskz_logger.info(get_rest_log_msg('Bulk add {} data'.format(model.get_class_name()), req_log_data, success, res_log_data))
+
+        return create_response(success, res_data)
+
+
+def register_model_bulk_delete_route(app, model, rule, module=None, action='delete', methods=None, strict_slash=True, rule_suffix='bulk', endpoint=None):
+    """
+    Register bulk delete type URL rule for the specified model class to the application/blueprint.
+
+    .. versionadded:: 1.8 @2024-05-03
+
+    Examples:
+        register_model_bulk_delete_route(api_blueprint, User, 'users', 'users')
+
+    :param app: Flask application / Blueprints instance
+    :param model: The DB model class, ex)User
+    :param rule: The URL rule string, ex)/users
+    :param module: The module name for permission check, ex)users
+    :param action: The action of the module for permission check, ex)delete
+    :param methods: The methods of the route, default is ['DELETE']
+    :param strict_slash: If not false, the rule url will end with slash
+    :param rule_suffix: The upsert suffix, default is 'bulk-delete'
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
+    :return:
+    """
+    methods = methods or ['DELETE']
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash, did_suffix='<ids>', rule_suffix=rule_suffix)
+
+    @app.route(suffix_rule, methods=methods, endpoint=endpoint)
+    @app.route(did_rule, methods=methods, endpoint=endpoint)
+    @rest_permission_required(module, action)
+    @gen_route_method('bulk_delete', base_rule)
+    def bulk_delete(ids=None):
+        req_log_data = ids
+        if ids is None:
+            request_json = request.json
+            req_log_data = json.dumps(request_json)
+            ids = request_json
+            if type(request_json) is dict:
+                ids = request_json.get('ids') or request_json.get('id', [])
+        else:
+            ids = ids.split(',')
+        try:
+            success, res_data = True, model.bulk_delete(ids)
+        except Exception as e:
+            flaskz_logger.exception(e)
+            success, res_data = False, res_status_codes.db_delete_err
+
+        res_log_data = get_log_data(res_data)
+        log_operation(module, 'delete', success, req_log_data, res_log_data)
+        flaskz_logger.info(get_rest_log_msg('Bulk delete {} data'.format(model.get_class_name()), req_log_data, success, res_log_data))
+
+        return create_response(success, res_data)
+
+
+def register_model_bulk_update_route(app, model, rule, module=None, action='update', methods=None, strict_slash=True, rule_suffix='bulk', endpoint=None):
+    """
+    Register bulk update type URL rule for the specified model class to the application/blueprint.
+
+    .. versionadded:: 1.8 @2024-05-03
+
+    Examples:
+        register_model_bulk_update_route(api_blueprint, User, 'users', 'users')
+
+    :param app: Flask application / Blueprints instance
+    :param model: The DB model class, ex)User
+    :param rule: The URL rule string, ex)/users
+    :param module: The module name for permission check, ex)users
+    :param action: The action of the module for permission check, ex)update
+    :param methods: The methods of the route, default is ['PATCH']
+    :param strict_slash: If not false, the rule url will end with slash
+    :param rule_suffix: The upsert suffix, default is 'bulk-update'
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
+    :return:
+    """
+    methods = methods or ['PATCH']
+    base_rule, did_rule, suffix_rule = _gen_route_rule(rule, strict_slash=strict_slash, rule_suffix=rule_suffix)
+
+    @app.route(suffix_rule, methods=methods, endpoint=endpoint)
+    @rest_permission_required(module, action)
+    @gen_route_method('bulk_update', base_rule)
+    def bulk_update():
+        request_json = request.json
+        req_log_data = json.dumps(request_json)
+        try:
+            model.bulk_update(request_json)
+            success, res_data = True, request_json
+        except Exception as e:
+            flaskz_logger.exception(e)
+            success, res_data = False, res_status_codes.db_update_err
+
+        res_log_data = get_log_data(res_data)
+        log_operation(module, 'update', success, req_log_data, res_log_data)
+        flaskz_logger.info(get_rest_log_msg('Bulk update {} data'.format(model.get_class_name()), req_log_data, success, res_log_data))
+
+        return create_response(success, res_data)
+
+
+def _gen_route_rule(rule, *, strict_slash=True, did_suffix=None, rule_suffix=None):
     if not rule.startswith('/'):
         rule = '/' + rule
+    base_rule = rule
+    suffix_rule = rule
+    did_rule = None
 
-    if not rule.endswith('/'):
-        suffix_rule = rule + '/' + suffix
-    else:
-        suffix_rule = rule + suffix
+    if rule_suffix is not None:
+        suffix_rule = rule = rule.rstrip('/') + '/' + rule_suffix
+
+    if did_suffix is not None:
+        did_rule = rule.rstrip('/') + '/' + did_suffix
 
     if strict_slash is not False:
-        if not rule.endswith('/'):
-            rule = rule + '/'
-        suffix_rule += '/'
-    return rule, suffix_rule
+        base_rule = base_rule.rstrip('/') + '/'
+        suffix_rule = suffix_rule.rstrip('/') + '/'
+        did_rule = did_rule.rstrip('/') + '/' if did_rule else None
+
+    return base_rule, did_rule, suffix_rule
 
 
 from ._mgmt import *
 from ._util import *
```

### Comparing `flaskz-1.7.3rc1/src/flaskz/rest/_mgmt.py` & `flaskz-1.8.0rc1/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/rest/_util.py` & `flaskz-1.8.0rc1/src/flaskz/rest/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_app.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_app.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_cache.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_cls.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_cls.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_common.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_common.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_func.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_magic.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_private.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_private.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_request_api.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_request_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import inspect
 import textwrap
 from urllib import parse as urllib_parse
 
-from flask import request
+from flask import request as flask_request
 from requests import Session, sessions
 from requests.adapters import HTTPAdapter
 
 from ._common import is_dict
 from .. import res_status_codes
 from ..log import flaskz_logger
 
-__all__ = ['api_request', 'forward_request', 'append_url_search_params']
+__all__ = ['request', 'api_request', 'forward_request', 'append_url_search_params']
 
 _session_request_kwargs = None
 
 
 def api_request(url, method="GET", url_params=None, base_url="", raw_response=False, **kwargs):
     """
     Request an api.
@@ -48,15 +48,58 @@
     :param method:
     :param url_params:
     :param raw_response:
     :param base_url:
     :param kwargs:
     :return:
     """
+    # warnings.warn('flaskz.utils.api_request() has been replaced by flaskz.utils.request()', category=DeprecationWarning)
 
+    success, result = request(url, method=method, url_params=url_params, base_url=base_url, raw_response=raw_response, **kwargs)
+    if success:
+        return result
+    return res_status_codes.api_request_err, result
+
+
+def request(url, method="GET", url_params=None, base_url="", raw_response=False, **kwargs):
+    """
+    Request an api.
+
+   .. versionadded:: 1.8.0 - add to replace api_request @2024-05-02
+
+    Example
+        # post request
+        request('req_url', 'POST', json=payload)
+        request({'url': 'req_url', 'method': 'POST'}, json=payload)
+
+        # get request
+        request('req_url', headers={'Authorization': 'eyJhbGciOiJIUzUxMiIs......'})
+
+        # base url
+        request('req_url', base_url='base_url') # url --> 'base_url/req_url'
+
+        # url_variables
+        request('req_url/{id}/', url_variables={'id': 1}) # url --> 'req_url/1/'
+
+        # url_search_params
+        request('req_url', url_search_params={'id': 1}) # url --> 'req_url?id=1'
+
+        # http_kwargs
+        request('req_url', http_kwargs={ # --> HTTPAdapter parameters
+            'pool_connections': 10, 'pool_maxsize': 100, 'max_retries': 10
+        })
+
+    :param url:
+    :param method:
+    :param url_params:
+    :param raw_response:
+    :param base_url:
+    :param kwargs:
+    :return:
+    """
     _method = method
     if is_dict(url):
         _url = url.get('url')
         if 'method' in url:
             _method = url.get("method")
     else:
         _url = url
@@ -93,21 +136,21 @@
             'status_code': status_code,
             # 'result': slice_str(result, 60, 10, '\n......\n'),
             'result': textwrap.shorten(result, 1000)  # @2022-05-26:将日志输出由slice_str改为了shorten
         }))
         if kwargs.get('close') is not False:  # @2024-01-09 add
             res.close()
         if raw_response is True:
-            return res
-        return result
+            return True, res
+        return True, result
     except Exception as e:
         result = str(e)
         flaskz_logger.exception('Api request failed:\n' + result)
 
-    return res_status_codes.api_request_err, result
+    return False, result
 
 
 def forward_request(url, payload=None, raw_response=False, error_code=500, **kwargs):
     """
     Forward the request to other service.
 
     Example:
@@ -126,33 +169,31 @@
     :param url: The forward url
     :return:
     """
     req_kwargs = {'url': url}
     _payload = payload or ['method', 'data', 'json', 'headers', 'cookies']
     for item in _payload:
         if item == 'json':  # @2022-05-06: fix request.json -->BadRequest('Content-Type was not 'application/json')
-            req_kwargs[item] = request.get_json(force=True, silent=True)
+            req_kwargs[item] = flask_request.get_json(force=True, silent=True)
         else:
-            req_kwargs[item] = getattr(request, item, None)
-    req_kwargs['params'] = request.args  # @2022-06-25 add query string
+            req_kwargs[item] = getattr(flask_request, item, None)
+    req_kwargs['params'] = flask_request.args  # @2022-06-25 add query string
     req_kwargs.update(kwargs)  # kwargs high priority
 
     url_params = req_kwargs.get('url_params')
     if url_params is None:  # if url_params is none, append request.view_args
-        req_kwargs['url_params'] = request.view_args or {}
+        req_kwargs['url_params'] = flask_request.view_args or {}
 
     req_kwargs['raw_response'] = True
 
-    res = api_request(**req_kwargs)
+    success, res = request(**req_kwargs)
+    if success is False:
+        return res, error_code
     if raw_response is True:
         return res
-
-    if type(res) is tuple:
-        return res[1], error_code
-
     return res.text, res.status_code, res.headers.items()
 
 
 def append_url_search_params(url, params):  # @2022-05-09: add
     """
     Appends specified key/value pair as search parameter.
     Only append the key if its value is None.
```

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_request_args.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_request_args.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_response.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_response.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz/utils/_timer.py` & `flaskz-1.8.0rc1/src/flaskz/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3rc1/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.8.0rc1/src/flaskz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.7.3rc1
+Version: 1.8.0rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,34 +17,41 @@
 Requires-Dist: requests>=2
 Provides-Extra: ext
 Requires-Dist: pycryptodome>=3.15.0; extra == "ext"
 Requires-Dist: paramiko>=3.0.0; extra == "ext"
 
 ## 关于
 
-*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
+*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展工具集, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
 
 ## 使用
 
 1. [☞数据库初始化&常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_model_init.html)
 2. [☞数据模型扩展类](http://zhangyiheng.com/blog/articles/py_flaskz_model_mixin.html)
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.7.3rc1** `2024/04/16`
+- **1.8.0rc1** `2024/05/21`
+    - [A] 扩展`flaskz.rest`路由生成模块
+        - 添加`register_model_bulk_route`函数, 用于生成指定数据模型的批量增删改路由
+        - 添加`register_model_bulk_add_route`函数, 用于生成指定数据模型的批量添加路由
+        - 添加`register_model_bulk_delete_route`函数, 用于生成指定数据模型的批量删除路由
+        - 添加`register_model_bulk_update_route`函数, 用于生成指定数据模型的批量更新路由
+    - [A] 添加`flaskz.utils.request`函数以替代`flaskz.utils.api_request`函数
+
+- **1.7.3** `2024/05/01`
     - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
     - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
-    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认启用)
+    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认复用)
     - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
     - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
-
 - **1.7.2** `2024/02/01`
     - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
     - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
 - **1.7.1** `2024/01/05`
     - [F] 修复SQLAlchemy<2.0.0版本时, `flaskz.models._util.py`中`BinaryExpression`类的导入问题
 - **1.7.0** `2024/01/01`
     - [C] `SQLAlchemy`依赖的版本从`>=1.3.13(EOL)`升级到`>=1.4.0(Maintenance)`
```

### Comparing `flaskz-1.7.3rc1/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.8.0rc1/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

