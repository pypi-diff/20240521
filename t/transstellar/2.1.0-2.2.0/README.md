# Comparing `tmp/transstellar-2.1.0.tar.gz` & `tmp/transstellar-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transstellar-2.1.0.tar", max compression
+gzip compressed data, was "transstellar-2.2.0.tar", max compression
```

## Comparing `transstellar-2.1.0.tar` & `transstellar-2.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      371 2024-05-15 08:33:45.971919 transstellar-2.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/__init__.py
--rw-r--r--   0        0        0      276 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/api_client/__init__.py
--rw-r--r--   0        0        0      420 2024-03-25 08:02:28.069753 transstellar-2.1.0/src/transstellar/api_client/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4429 2024-03-25 08:02:28.073753 transstellar-2.1.0/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc
--rw-r--r--   0        0        0     3065 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/api_client/api_client.py
--rw-r--r--   0        0        0      189 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/api_client/errors/__init__.py
--rw-r--r--   0        0        0      352 2024-03-25 08:02:28.073753 transstellar-2.1.0/src/transstellar/api_client/errors/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      383 2024-03-07 09:16:29.850062 transstellar-2.1.0/src/transstellar/api_client/errors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.1.0/src/transstellar/api_client/errors/__pycache__/client_error.cpython-312.pyc
--rw-r--r--   0        0        0      355 2024-03-07 09:16:29.850062 transstellar-2.1.0/src/transstellar/api_client/errors/__pycache__/client_error.cpython-38.pyc
--rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.1.0/src/transstellar/api_client/errors/__pycache__/server_error.cpython-312.pyc
--rw-r--r--   0        0        0      355 2024-03-07 09:16:29.854062 transstellar-2.1.0/src/transstellar/api_client/errors/__pycache__/server_error.cpython-38.pyc
--rw-r--r--   0        0        0      412 2024-03-25 08:02:28.073753 transstellar-2.1.0/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-312.pyc
--rw-r--r--   0        0        0      367 2024-03-07 09:16:29.854062 transstellar-2.1.0/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-38.pyc
--rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/api_client/errors/client_error.py
--rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/api_client/errors/server_error.py
--rw-r--r--   0        0        0      102 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/api_client/errors/unauthorized_error.py
--rw-r--r--   0        0        0      831 2024-05-06 07:57:56.408911 transstellar-2.1.0/src/transstellar/framework/__init__.py
--rw-r--r--   0        0        0      925 2024-05-14 08:42:29.711243 transstellar-2.1.0/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5740 2024-05-15 08:25:58.694609 transstellar-2.1.0/src/transstellar/framework/__pycache__/application.cpython-312.pyc
--rw-r--r--   0        0        0      832 2024-05-06 07:03:19.734569 transstellar-2.1.0/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc
--rw-r--r--   0        0        0      856 2024-03-20 08:12:14.536313 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0        0        0      595 2024-03-25 08:02:27.945759 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc
--rw-r--r--   0        0        0      595 2024-05-03 10:38:32.725071 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     1553 2024-05-15 07:21:51.348116 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc
--rw-r--r--   0        0        0     1012 2024-03-20 09:47:02.256105 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0        0        0     1012 2024-03-25 08:02:27.945759 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1012 2024-05-03 10:38:32.725071 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     3237 2024-03-21 03:52:22.082583 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0        0        0     3237 2024-04-30 08:38:09.180119 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     3237 2024-05-03 10:38:32.737071 transstellar-2.1.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     1210 2024-03-25 08:02:27.957759 transstellar-2.1.0/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc
--rw-r--r--   0        0        0    11790 2024-05-15 08:25:58.758608 transstellar-2.1.0/src/transstellar/framework/__pycache__/element.cpython-312.pyc
--rw-r--r--   0        0        0      212 2024-03-25 08:02:28.005756 transstellar-2.1.0/src/transstellar/framework/__pycache__/handle_error.cpython-312.pyc
--rw-r--r--   0        0        0     1882 2024-03-25 08:02:28.005756 transstellar-2.1.0/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc
--rw-r--r--   0        0        0      646 2024-03-25 08:02:27.941759 transstellar-2.1.0/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc
--rw-r--r--   0        0        0     2428 2024-03-25 08:02:27.945759 transstellar-2.1.0/src/transstellar/framework/__pycache__/logger.cpython-312.pyc
--rw-r--r--   0        0        0     1010 2024-03-25 08:02:28.005756 transstellar-2.1.0/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc
--rw-r--r--   0        0        0      892 2024-03-25 08:02:27.941759 transstellar-2.1.0/src/transstellar/framework/__pycache__/module.cpython-312.pyc
--rw-r--r--   0        0        0     1232 2024-05-14 08:42:29.807242 transstellar-2.1.0/src/transstellar/framework/__pycache__/router.cpython-312.pyc
--rw-r--r--   0        0        0     2463 2024-03-25 08:02:27.949759 transstellar-2.1.0/src/transstellar/framework/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0        0        0     3177 2024-05-15 08:25:49.498670 transstellar-2.1.0/src/transstellar/framework/application.py
--rw-r--r--   0        0        0      273 2024-05-06 06:58:08.437282 transstellar-2.1.0/src/transstellar/framework/application_bootstrapper.py
--rw-r--r--   0        0        0      104 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/framework/base_api_test.py
--rw-r--r--   0        0        0      545 2024-05-15 07:02:34.774249 transstellar-2.1.0/src/transstellar/framework/base_page.py
--rw-r--r--   0        0        0      305 2024-03-25 07:22:27.425371 transstellar-2.1.0/src/transstellar/framework/base_test.py
--rw-r--r--   0        0        0     1426 2024-04-30 08:37:17.948017 transstellar-2.1.0/src/transstellar/framework/base_ui_test.py
--rw-r--r--   0        0        0      410 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/framework/config_service.py
--rw-r--r--   0        0        0     7426 2024-05-15 08:25:33.518778 transstellar-2.1.0/src/transstellar/framework/element.py
--rw-r--r--   0        0        0       77 2024-03-25 07:22:27.421371 transstellar-2.1.0/src/transstellar/framework/handle_error.py
--rw-r--r--   0        0        0     1194 2024-03-25 07:22:27.421371 transstellar-2.1.0/src/transstellar/framework/handle_ui_error.py
--rw-r--r--   0        0        0      151 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/framework/loggable.py
--rw-r--r--   0        0        0     1087 2024-03-25 07:22:27.437371 transstellar-2.1.0/src/transstellar/framework/logger.py
--rw-r--r--   0        0        0      348 2024-03-25 07:21:52.372907 transstellar-2.1.0/src/transstellar/framework/main_config.py
--rw-r--r--   0        0        0      288 2024-03-25 07:22:27.429371 transstellar-2.1.0/src/transstellar/framework/module.py
--rw-r--r--   0        0        0      520 2024-05-06 07:57:56.408911 transstellar-2.1.0/src/transstellar/framework/router.py
--rw-r--r--   0        0        0     1351 2024-03-25 07:22:27.437371 transstellar-2.1.0/src/transstellar/framework/utils.py
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 transstellar-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      371 2024-05-21 08:08:12.521601 transstellar-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/__init__.py
+-rw-r--r--   0        0        0      276 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/api_client/__init__.py
+-rw-r--r--   0        0        0      420 2024-03-25 08:02:28.069753 transstellar-2.2.0/src/transstellar/api_client/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4429 2024-03-25 08:02:28.073753 transstellar-2.2.0/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc
+-rw-r--r--   0        0        0     3065 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/api_client/api_client.py
+-rw-r--r--   0        0        0      189 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/api_client/errors/__init__.py
+-rw-r--r--   0        0        0      352 2024-03-25 08:02:28.073753 transstellar-2.2.0/src/transstellar/api_client/errors/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      383 2024-03-07 09:16:29.850062 transstellar-2.2.0/src/transstellar/api_client/errors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.2.0/src/transstellar/api_client/errors/__pycache__/client_error.cpython-312.pyc
+-rw-r--r--   0        0        0      355 2024-03-07 09:16:29.850062 transstellar-2.2.0/src/transstellar/api_client/errors/__pycache__/client_error.cpython-38.pyc
+-rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.2.0/src/transstellar/api_client/errors/__pycache__/server_error.cpython-312.pyc
+-rw-r--r--   0        0        0      355 2024-03-07 09:16:29.854062 transstellar-2.2.0/src/transstellar/api_client/errors/__pycache__/server_error.cpython-38.pyc
+-rw-r--r--   0        0        0      412 2024-03-25 08:02:28.073753 transstellar-2.2.0/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-312.pyc
+-rw-r--r--   0        0        0      367 2024-03-07 09:16:29.854062 transstellar-2.2.0/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-38.pyc
+-rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/api_client/errors/client_error.py
+-rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/api_client/errors/server_error.py
+-rw-r--r--   0        0        0      102 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/api_client/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      831 2024-05-06 07:57:56.408911 transstellar-2.2.0/src/transstellar/framework/__init__.py
+-rw-r--r--   0        0        0      925 2024-05-14 08:42:29.711243 transstellar-2.2.0/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5930 2024-05-21 08:06:59.700363 transstellar-2.2.0/src/transstellar/framework/__pycache__/application.cpython-312.pyc
+-rw-r--r--   0        0        0      832 2024-05-06 07:03:19.734569 transstellar-2.2.0/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc
+-rw-r--r--   0        0        0      856 2024-03-20 08:12:14.536313 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0      595 2024-03-25 08:02:27.945759 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0      595 2024-05-03 10:38:32.725071 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1553 2024-05-15 07:21:51.348116 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc
+-rw-r--r--   0        0        0     1012 2024-03-20 09:47:02.256105 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     1012 2024-03-25 08:02:27.945759 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1012 2024-05-03 10:38:32.725071 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     3237 2024-03-21 03:52:22.082583 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     3237 2024-04-30 08:38:09.180119 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     3237 2024-05-03 10:38:32.737071 transstellar-2.2.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1210 2024-03-25 08:02:27.957759 transstellar-2.2.0/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc
+-rw-r--r--   0        0        0    11790 2024-05-15 08:25:58.758608 transstellar-2.2.0/src/transstellar/framework/__pycache__/element.cpython-312.pyc
+-rw-r--r--   0        0        0      212 2024-03-25 08:02:28.005756 transstellar-2.2.0/src/transstellar/framework/__pycache__/handle_error.cpython-312.pyc
+-rw-r--r--   0        0        0     1882 2024-03-25 08:02:28.005756 transstellar-2.2.0/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc
+-rw-r--r--   0        0        0      646 2024-03-25 08:02:27.941759 transstellar-2.2.0/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc
+-rw-r--r--   0        0        0     2428 2024-03-25 08:02:27.945759 transstellar-2.2.0/src/transstellar/framework/__pycache__/logger.cpython-312.pyc
+-rw-r--r--   0        0        0     1010 2024-03-25 08:02:28.005756 transstellar-2.2.0/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc
+-rw-r--r--   0        0        0      892 2024-03-25 08:02:27.941759 transstellar-2.2.0/src/transstellar/framework/__pycache__/module.cpython-312.pyc
+-rw-r--r--   0        0        0     1232 2024-05-14 08:42:29.807242 transstellar-2.2.0/src/transstellar/framework/__pycache__/router.cpython-312.pyc
+-rw-r--r--   0        0        0     2463 2024-03-25 08:02:27.949759 transstellar-2.2.0/src/transstellar/framework/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0        0        0     3303 2024-05-21 08:06:22.379762 transstellar-2.2.0/src/transstellar/framework/application.py
+-rw-r--r--   0        0        0      273 2024-05-06 06:58:08.437282 transstellar-2.2.0/src/transstellar/framework/application_bootstrapper.py
+-rw-r--r--   0        0        0      104 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/framework/base_api_test.py
+-rw-r--r--   0        0        0      545 2024-05-15 07:02:34.774249 transstellar-2.2.0/src/transstellar/framework/base_page.py
+-rw-r--r--   0        0        0      305 2024-03-25 07:22:27.425371 transstellar-2.2.0/src/transstellar/framework/base_test.py
+-rw-r--r--   0        0        0     1426 2024-04-30 08:37:17.948017 transstellar-2.2.0/src/transstellar/framework/base_ui_test.py
+-rw-r--r--   0        0        0      410 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/framework/config_service.py
+-rw-r--r--   0        0        0     7426 2024-05-15 08:25:33.518778 transstellar-2.2.0/src/transstellar/framework/element.py
+-rw-r--r--   0        0        0       77 2024-03-25 07:22:27.421371 transstellar-2.2.0/src/transstellar/framework/handle_error.py
+-rw-r--r--   0        0        0     1194 2024-03-25 07:22:27.421371 transstellar-2.2.0/src/transstellar/framework/handle_ui_error.py
+-rw-r--r--   0        0        0      151 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/framework/loggable.py
+-rw-r--r--   0        0        0     1087 2024-03-25 07:22:27.437371 transstellar-2.2.0/src/transstellar/framework/logger.py
+-rw-r--r--   0        0        0      348 2024-03-25 07:21:52.372907 transstellar-2.2.0/src/transstellar/framework/main_config.py
+-rw-r--r--   0        0        0      288 2024-03-25 07:22:27.429371 transstellar-2.2.0/src/transstellar/framework/module.py
+-rw-r--r--   0        0        0      520 2024-05-06 07:57:56.408911 transstellar-2.2.0/src/transstellar/framework/router.py
+-rw-r--r--   0        0        0     1351 2024-03-25 07:22:27.437371 transstellar-2.2.0/src/transstellar/framework/utils.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 transstellar-2.2.0/PKG-INFO
```

### Comparing `transstellar-2.1.0/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/api_client/api_client.py` & `transstellar-2.2.0/src/transstellar/api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__init__.py` & `transstellar-2.2.0/src/transstellar/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/application.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/application.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Wed May 15 08:25:49 2024 UTC, .py size: 3177 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 8d71 4466 690c 0000  .........qDfi...
+00000000: cb0d 0d0a 0000 0000 fe55 4c66 e70c 0000  .........ULf....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 8000 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6402  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6400 6403 6c04 6d05  l.m.Z...d.d.l.m.
 00000050: 5a05 0100 6400 6404 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
 00000060: 6400 6405 6c08 6d09 5a09 6d0a 5a0a 0100  d.d.l.m.Z.m.Z...
 00000070: 6400 6406 6c0b 6d0c 5a0c 0100 6407 6408  d.d.l.m.Z...d.d.
@@ -261,99 +261,111 @@
 00001040: d117 31d0 3243 d317 44d8 1b27 a809 a07b  ..1.2C..D..'...{
 00001050: b024 d019 37d8 161a 976c 916c d716 29d1  .$..7....l.l..).
 00001060: 1629 d716 30d1 1630 d031 41d3 1642 f607  .)..0..0.1A..B..
 00001070: 040d 0ef0 0900 0c21 f702 010d 15f0 0001  .......!........
 00001080: 0d15 fa73 0b00 0000 b401 4222 03c2 2205  ...s......B"..".
 00001090: 422b 07da 0672 6574 7572 6e63 0100 0000  B+...returnc....
 000010a0: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-000010b0: f366 0100 0097 0074 0100 0000 0000 0000  .f.....t........
+000010b0: f3c6 0100 0097 0074 0100 0000 0000 0000  .......t........
 000010c0: 006a 0200 0000 0000 0000 0000 0000 0000  .j..............
 000010d0: 0000 0000 0064 01ab 0100 0000 0000 0001  .....d..........
 000010e0: 0074 0400 0000 0000 0000 006a 0600 0000  .t.........j....
 000010f0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
 00001100: 0900 0000 0000 0000 0000 0000 0000 0000  ................
 00001110: 0000 0064 0264 03ab 0200 0000 0000 007d  ...d.d.........}
 00001120: 017c 006a 0a00 0000 0000 0000 0000 0000  .|.j............
 00001130: 0000 0000 0000 006a 0900 0000 0000 0000  .......j........
 00001140: 0000 0000 0000 0000 0000 0064 0464 05ab  ...........d.d..
-00001150: 0200 0000 0000 007d 0274 0d00 0000 0000  .......}.t......
-00001160: 0000 00ab 0000 0000 0000 007d 037c 036a  ...........}.|.j
-00001170: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-00001180: 0000 0064 06ab 0100 0000 0000 0001 007c  ...d...........|
-00001190: 036a 0f00 0000 0000 0000 0000 0000 0000  .j..............
-000011a0: 0000 0000 0064 07ab 0100 0000 0000 0001  .....d..........
-000011b0: 0074 1100 0000 0000 0000 007c 017c 03ac  .t.........|.|..
-000011c0: 08ab 0200 0000 0000 007d 047c 046a 1300  .........}.|.j..
-000011d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011e0: 007c 02ab 0100 0000 0000 0001 0074 0100  .|...........t..
-000011f0: 0000 0000 0000 006a 0200 0000 0000 0000  .......j........
-00001200: 0000 0000 0000 0000 0000 0064 09ab 0100  ...........d....
-00001210: 0000 0000 0001 007c 0453 0029 0a4e 7a13  .......|.S.).Nz.
-00001220: 496e 6974 6961 6c69 7a69 6e67 2064 7269  Initializing dri
-00001230: 7665 72da 1553 454c 454e 4955 4d5f 434d  ver..SELENIUM_CM
-00001240: 445f 4558 4543 5554 4f52 7a1b 6874 7470  D_EXECUTORz.http
-00001250: 3a2f 2f73 656c 656e 6975 6d3a 3434 3434  ://selenium:4444
-00001260: 2f77 642f 6875 62da 1469 6d70 6c69 6369  /wd/hub..implici
-00001270: 746c 795f 7761 6974 5f74 696d 65e9 0a00  tly_wait_time...
-00001280: 0000 7a0c 2d2d 6e6f 2d73 616e 6462 6f78  ..z.--no-sandbox
-00001290: 7a17 2d2d 6469 7361 626c 652d 6465 762d  z.--disable-dev-
-000012a0: 7368 6d2d 7573 6167 6529 02da 1063 6f6d  shm-usage)...com
-000012b0: 6d61 6e64 5f65 7865 6375 746f 7272 1200  mand_executorr..
-000012c0: 0000 7a12 4472 6976 6572 2069 6e69 7469  ..z.Driver initi
-000012d0: 616c 697a 6564 290a 7218 0000 0072 1900  alized).r....r..
-000012e0: 0000 7245 0000 0072 4600 0000 721a 0000  ..rE...rF...r...
-000012f0: 0072 1200 0000 7206 0000 00da 0c61 6464  .r....r......add
-00001300: 5f61 7267 756d 656e 7472 0700 0000 da0f  _argumentr......
-00001310: 696d 706c 6963 6974 6c79 5f77 6169 7429  implicitly_wait)
-00001320: 0572 1e00 0000 da15 7365 6c65 6e69 756d  .r......selenium
-00001330: 5f63 6d64 5f65 7865 6375 746f 7272 4f00  _cmd_executorrO.
-00001340: 0000 7212 0000 0072 1100 0000 7305 0000  ..r....r....s...
-00001350: 0020 2020 2020 721f 0000 0072 2300 0000  .     r....r#...
-00001360: 7a1b 4170 706c 6963 6174 696f 6e2e 5f5f  z.Application.__
-00001370: 696e 6974 5f64 7269 7665 725f 5f67 0000  init_driver__g..
-00001380: 0073 9400 0000 8000 dc08 0f8f 0c89 0cd0  .s..............
-00001390: 152a d408 2bdc 2022 a70a a10a a70e a10e  .*..+. "........
-000013a0: d80c 23d0 2542 f303 0221 0ad0 081d f006  ..#.%B...!......
-000013b0: 0020 249f 7c99 7cd7 1f2f d11f 2fd0 3046  . $.|.|../../.0F
-000013c0: c802 d31f 4bd0 081c dc12 1f93 2f88 07d8  ....K......./...
-000013d0: 080f d708 1cd1 081c 985e d408 2cd8 080f  .........^..,...
-000013e0: d708 1cd1 081c d01d 36d4 0837 dc11 17d0  ........6..7....
-000013f0: 293e c807 d411 5088 06d8 080e d708 1ed1  )>....P.........
-00001400: 081e d01f 33d4 0834 dc08 0f8f 0c89 0cd0  ....3..4........
-00001410: 1529 d408 2ae0 0f15 880d 7221 0000 004e  .)..*.....r!...N
-00001420: 2919 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00001430: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00001440: 6e61 6d65 5f5f 7204 0000 00da 0f5f 5f61  name__r......__a
-00001450: 6e6e 6f74 6174 696f 6e73 5f5f da03 7374  nnotations__..st
-00001460: 7272 0500 0000 7208 0000 00da 0361 6e79  rr....r......any
-00001470: 7213 0000 00da 0462 6f6f 6c72 1400 0000  r......boolr....
-00001480: da04 6469 6374 7220 0000 0072 2500 0000  ..dictr ...r%...
-00001490: 7228 0000 0072 1a00 0000 7203 0000 0072  r(...r....r....r
-000014a0: 0a00 0000 7230 0000 0072 1d00 0000 7236  ....r0...r....r6
-000014b0: 0000 0072 3900 0000 721c 0000 0072 2300  ...r9...r....r#.
-000014c0: 0000 a900 7221 0000 0072 1f00 0000 720d  ....r!...r....r.
-000014d0: 0000 0072 0d00 0000 0e00 0000 7393 0000  ...r........s...
-000014e0: 0085 00d8 0f17 d304 17d8 1114 d304 14d8  ................
-000014f0: 0d1b d304 1bd8 0c15 d304 15d8 0d10 834c  ...............L
-00001500: d818 1d80 4b90 14d3 041d d813 1880 4688  ....K.........F.
-00001510: 44d3 0418 f004 1205 2598 74f3 0012 0525  D.......%.t....%
-00001520: f228 0805 1cf2 1401 0520 f006 0105 2790  .(....... ....'.
-00001530: 73f3 0001 0527 f006 0205 39a8 44b0 16a9  s....'....9.D...
-00001540: 4cf3 0002 0539 f008 0105 2ca0 64f3 0001  L....9....,.d...
-00001550: 052c f006 0805 1498 13f3 0008 0514 f214  .,..............
-00001560: 0d05 2bf2 1e0a 050e f018 0d05 16a0 19f4  ..+.............
-00001570: 000d 0516 7221 0000 0072 0d00 0000 2912  ....r!...r....).
-00001580: 7218 0000 0072 4500 0000 da06 7479 7069  r....rE.....typi
-00001590: 6e67 7203 0000 00da 0869 6e6a 6563 746f  ngr......injecto
-000015a0: 7272 0400 0000 da06 7079 7465 7374 7205  rr......pytestr.
-000015b0: 0000 00da 1273 656c 656e 6975 6d2e 7765  .....selenium.we
-000015c0: 6264 7269 7665 7272 0600 0000 7207 0000  bdriverr....r...
-000015d0: 00da 2373 656c 656e 6975 6d2e 7765 6264  ..#selenium.webd
-000015e0: 7269 7665 722e 7265 6d6f 7465 2e77 6562  river.remote.web
-000015f0: 6472 6976 6572 7208 0000 0072 2f00 0000  driverr....r/...
-00001600: 720a 0000 0072 1b00 0000 720b 0000 0072  r....r....r....r
-00001610: 0d00 0000 725d 0000 0072 2100 0000 721f  ....r]...r!...r.
-00001620: 0000 00fa 083c 6d6f 6475 6c65 3e72 6300  .....<module>rc.
-00001630: 0000 0100 0000 732c 0000 00f0 0301 0101  ......s,........
-00001640: db00 0edb 0009 dd00 17e5 001d dd00 21df  ..............!.
-00001650: 0034 dd00 39e5 001a dd00 1af7 0666 0101  .4..9........f..
-00001660: 16f2 0066 0101 1672 2100 0000            ...f...r!...
+00001150: 0200 0000 0000 007d 027c 006a 0a00 0000  .......}.|.j....
+00001160: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00001170: 0900 0000 0000 0000 0000 0000 0000 0000  ................
+00001180: 0000 0064 0664 07ab 0200 0000 0000 007d  ...d.d.........}
+00001190: 0374 0d00 0000 0000 0000 00ab 0000 0000  .t..............
+000011a0: 0000 007d 047c 046a 0f00 0000 0000 0000  ...}.|.j........
+000011b0: 0000 0000 0000 0000 0000 0064 08ab 0100  ...........d....
+000011c0: 0000 0000 0001 007c 046a 0f00 0000 0000  .......|.j......
+000011d0: 0000 0000 0000 0000 0000 0000 0064 09ab  .............d..
+000011e0: 0100 0000 0000 0001 007c 046a 0f00 0000  .........|.j....
+000011f0: 0000 0000 0000 0000 0000 0000 0000 0064  ...............d
+00001200: 0a7c 039b 009d 02ab 0100 0000 0000 0001  .|..............
+00001210: 0074 1100 0000 0000 0000 007c 017c 04ac  .t.........|.|..
+00001220: 0bab 0200 0000 0000 007d 057c 056a 1300  .........}.|.j..
+00001230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001240: 007c 02ab 0100 0000 0000 0001 0074 0100  .|...........t..
+00001250: 0000 0000 0000 006a 0200 0000 0000 0000  .......j........
+00001260: 0000 0000 0000 0000 0000 0064 0cab 0100  ...........d....
+00001270: 0000 0000 0001 007c 0553 0029 0d4e 7a13  .......|.S.).Nz.
+00001280: 496e 6974 6961 6c69 7a69 6e67 2064 7269  Initializing dri
+00001290: 7665 72da 1553 454c 454e 4955 4d5f 434d  ver..SELENIUM_CM
+000012a0: 445f 4558 4543 5554 4f52 7a1b 6874 7470  D_EXECUTORz.http
+000012b0: 3a2f 2f73 656c 656e 6975 6d3a 3434 3434  ://selenium:4444
+000012c0: 2f77 642f 6875 62da 1469 6d70 6c69 6369  /wd/hub..implici
+000012d0: 746c 795f 7761 6974 5f74 696d 65e9 0a00  tly_wait_time...
+000012e0: 0000 da08 7469 6d65 7a6f 6e65 7a13 416d  ....timezonez.Am
+000012f0: 6572 6963 612f 4c6f 735f 416e 6765 6c65  erica/Los_Angele
+00001300: 737a 0c2d 2d6e 6f2d 7361 6e64 626f 787a  sz.--no-sandboxz
+00001310: 172d 2d64 6973 6162 6c65 2d64 6576 2d73  .--disable-dev-s
+00001320: 686d 2d75 7361 6765 7a0b 2d2d 7469 6d65  hm-usagez.--time
+00001330: 7a6f 6e65 3d29 02da 1063 6f6d 6d61 6e64  zone=)...command
+00001340: 5f65 7865 6375 746f 7272 1200 0000 7a12  _executorr....z.
+00001350: 4472 6976 6572 2069 6e69 7469 616c 697a  Driver initializ
+00001360: 6564 290a 7218 0000 0072 1900 0000 7245  ed).r....r....rE
+00001370: 0000 0072 4600 0000 721a 0000 0072 1200  ...rF...r....r..
+00001380: 0000 7206 0000 00da 0c61 6464 5f61 7267  ..r......add_arg
+00001390: 756d 656e 7472 0700 0000 da0f 696d 706c  umentr......impl
+000013a0: 6963 6974 6c79 5f77 6169 7429 0672 1e00  icitly_wait).r..
+000013b0: 0000 da15 7365 6c65 6e69 756d 5f63 6d64  ....selenium_cmd
+000013c0: 5f65 7865 6375 746f 7272 4f00 0000 7251  _executorrO...rQ
+000013d0: 0000 0072 1200 0000 7211 0000 0073 0600  ...r....r....s..
+000013e0: 0000 2020 2020 2020 721f 0000 0072 2300  ..      r....r#.
+000013f0: 0000 7a1b 4170 706c 6963 6174 696f 6e2e  ..z.Application.
+00001400: 5f5f 696e 6974 5f64 7269 7665 725f 5f67  __init_driver__g
+00001410: 0000 0073 c000 0000 8000 dc08 0f8f 0c89  ...s............
+00001420: 0cd0 152a d408 2bdc 2022 a70a a10a a70e  ...*..+. "......
+00001430: a10e d80c 23d0 2542 f303 0221 0ad0 081d  ....#.%B...!....
+00001440: f006 0020 249f 7c99 7cd7 1f2f d11f 2fd0  ... $.|.|../../.
+00001450: 3046 c802 d31f 4bd0 081c d813 1797 3c91  0F....K.......<.
+00001460: 3cd7 1323 d113 23a0 4ad0 3045 d313 4688  <..#..#.J.0E..F.
+00001470: 08dc 121f 932f 8807 d808 0fd7 081c d108  ...../..........
+00001480: 1c98 5ed4 082c d808 0fd7 081c d108 1cd0  ..^..,..........
+00001490: 1d36 d408 37d8 080f d708 1cd1 081c 987b  .6..7..........{
+000014a0: a838 a82a d01d 35d4 0836 dc11 17d0 293e  .8.*..5..6....)>
+000014b0: c807 d411 5088 06d8 080e d708 1ed1 081e  ....P...........
+000014c0: d01f 33d4 0834 dc08 0f8f 0c89 0cd0 1529  ..3..4.........)
+000014d0: d408 2ae0 0f15 880d 7221 0000 004e 2919  ..*.....r!...N).
+000014e0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000014f0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00001500: 6d65 5f5f 7204 0000 00da 0f5f 5f61 6e6e  me__r......__ann
+00001510: 6f74 6174 696f 6e73 5f5f da03 7374 7272  otations__..strr
+00001520: 0500 0000 7208 0000 00da 0361 6e79 7213  ....r......anyr.
+00001530: 0000 00da 0462 6f6f 6c72 1400 0000 da04  .....boolr......
+00001540: 6469 6374 7220 0000 0072 2500 0000 7228  dictr ...r%...r(
+00001550: 0000 0072 1a00 0000 7203 0000 0072 0a00  ...r....r....r..
+00001560: 0000 7230 0000 0072 1d00 0000 7236 0000  ..r0...r....r6..
+00001570: 0072 3900 0000 721c 0000 0072 2300 0000  .r9...r....r#...
+00001580: a900 7221 0000 0072 1f00 0000 720d 0000  ..r!...r....r...
+00001590: 0072 0d00 0000 0e00 0000 7393 0000 0085  .r........s.....
+000015a0: 00d8 0f17 d304 17d8 1114 d304 14d8 0d1b  ................
+000015b0: d304 1bd8 0c15 d304 15d8 0d10 834c d818  .............L..
+000015c0: 1d80 4b90 14d3 041d d813 1880 4688 44d3  ..K.........F.D.
+000015d0: 0418 f004 1205 2598 74f3 0012 0525 f228  ......%.t....%.(
+000015e0: 0805 1cf2 1401 0520 f006 0105 2790 73f3  ....... ....'.s.
+000015f0: 0001 0527 f006 0205 39a8 44b0 16a9 4cf3  ...'....9.D...L.
+00001600: 0002 0539 f008 0105 2ca0 64f3 0001 052c  ...9....,.d....,
+00001610: f006 0805 1498 13f3 0008 0514 f214 0d05  ................
+00001620: 2bf2 1e0a 050e f018 0f05 16a0 19f4 000f  +...............
+00001630: 0516 7221 0000 0072 0d00 0000 2912 7218  ..r!...r....).r.
+00001640: 0000 0072 4500 0000 da06 7479 7069 6e67  ...rE.....typing
+00001650: 7203 0000 00da 0869 6e6a 6563 746f 7272  r......injectorr
+00001660: 0400 0000 da06 7079 7465 7374 7205 0000  ......pytestr...
+00001670: 00da 1273 656c 656e 6975 6d2e 7765 6264  ...selenium.webd
+00001680: 7269 7665 7272 0600 0000 7207 0000 00da  riverr....r.....
+00001690: 2373 656c 656e 6975 6d2e 7765 6264 7269  #selenium.webdri
+000016a0: 7665 722e 7265 6d6f 7465 2e77 6562 6472  ver.remote.webdr
+000016b0: 6976 6572 7208 0000 0072 2f00 0000 720a  iverr....r/...r.
+000016c0: 0000 0072 1b00 0000 720b 0000 0072 0d00  ...r....r....r..
+000016d0: 0000 725e 0000 0072 2100 0000 721f 0000  ..r^...r!...r...
+000016e0: 00fa 083c 6d6f 6475 6c65 3e72 6400 0000  ...<module>rd...
+000016f0: 0100 0000 732c 0000 00f0 0301 0101 db00  ....s,..........
+00001700: 0edb 0009 dd00 17e5 001d dd00 21df 0034  ............!..4
+00001710: dd00 39e5 001a dd00 1af7 0668 0101 16f2  ..9........h....
+00001720: 0068 0101 1672 2100 0000                 .h...r!...
```

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/element.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/element.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/logger.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/logger.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/module.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/module.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/router.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/router.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/__pycache__/utils.cpython-312.pyc` & `transstellar-2.2.0/src/transstellar/framework/__pycache__/utils.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/application.py` & `transstellar-2.2.0/src/transstellar/framework/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,17 @@
 
     def __init_driver__(self) -> WebDriver:
         logging.info("Initializing driver")
         selenium_cmd_executor = os.environ.get(
             "SELENIUM_CMD_EXECUTOR", "http://selenium:4444/wd/hub"
         )
         implicitly_wait_time = self.options.get("implicitly_wait_time", 10)
+        timezone = self.options.get("timezone", "America/Los_Angeles")
         options = ChromeOptions()
         options.add_argument("--no-sandbox")
         options.add_argument("--disable-dev-shm-usage")
+        options.add_argument(f"--timezone={timezone}")
         driver = Remote(command_executor=selenium_cmd_executor, options=options)
         driver.implicitly_wait(implicitly_wait_time)
         logging.info("Driver initialized")
 
         return driver
```

### Comparing `transstellar-2.1.0/src/transstellar/framework/base_page.py` & `transstellar-2.2.0/src/transstellar/framework/base_page.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/base_ui_test.py` & `transstellar-2.2.0/src/transstellar/framework/base_ui_test.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/element.py` & `transstellar-2.2.0/src/transstellar/framework/element.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/handle_ui_error.py` & `transstellar-2.2.0/src/transstellar/framework/handle_ui_error.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/logger.py` & `transstellar-2.2.0/src/transstellar/framework/logger.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/router.py` & `transstellar-2.2.0/src/transstellar/framework/router.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/src/transstellar/framework/utils.py` & `transstellar-2.2.0/src/transstellar/framework/utils.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.1.0/PKG-INFO` & `transstellar-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transstellar
-Version: 2.1.0
+Version: 2.2.0
 Summary: A pytest framework
 Author: Onramplab Dev
 Author-email: dev@onramplab.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: injector (>=0.21.0,<0.22.0)
```

