# Comparing `tmp/lbz-0.6.5.tar.gz` & `tmp/lbz-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbz-0.6.5.tar", last modified: Wed Jan 31 14:11:10 2024, max compression
+gzip compressed data, was "lbz-0.6.6.tar", last modified: Tue May 21 07:19:17 2024, max compression
```

## Comparing `lbz-0.6.5.tar` & `lbz-0.6.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:10.989672 lbz-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-31 14:11:02.000000 lbz-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-01-31 14:11:10.989672 lbz-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-01-31 14:11:02.000000 lbz-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:10.985672 lbz-0.6.5/lbz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:10.985672 lbz-0.6.5/lbz/authz/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/authz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/authz/authorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/authz/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/authz/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/aws_boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/aws_ssm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:10.985672 lbz-0.6.5/lbz/dev/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/dev/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/dev/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:10.989672 lbz-0.6.5/lbz/events/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/events/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/events/broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/events/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/events/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/jwt_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:10.989672 lbz-0.6.5/lbz/lambdas/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/lambdas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/lambdas/broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/lambdas/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/lambdas/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/lambdas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/lambdas/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:10.989672 lbz-0.6.5/lbz/rest/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/rest/api_gateway_event.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/rest/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-01-31 14:11:02.000000 lbz-0.6.5/lbz/type_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:11:10.985672 lbz-0.6.5/lbz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-01-31 14:11:10.000000 lbz-0.6.5/lbz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-31 14:11:10.000000 lbz-0.6.5/lbz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 14:11:10.000000 lbz-0.6.5/lbz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-31 14:11:10.000000 lbz-0.6.5/lbz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-31 14:11:10.000000 lbz-0.6.5/lbz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-01-31 14:11:10.989672 lbz-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-01-31 14:11:02.000000 lbz-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:17.712111 lbz-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 07:19:10.000000 lbz-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-21 07:19:17.712111 lbz-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-21 07:19:10.000000 lbz-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:17.708111 lbz-0.6.6/lbz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:17.712111 lbz-0.6.6/lbz/authz/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/authz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/authz/authorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/authz/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/authz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/aws_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/aws_ssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:17.712111 lbz-0.6.6/lbz/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/dev/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/dev/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:17.712111 lbz-0.6.6/lbz/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/events/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/events/broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/events/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/jwt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:17.712111 lbz-0.6.6/lbz/lambdas/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/lambdas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/lambdas/broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/lambdas/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/lambdas/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/lambdas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/lambdas/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:17.712111 lbz-0.6.6/lbz/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/rest/api_gateway_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/rest/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-21 07:19:10.000000 lbz-0.6.6/lbz/type_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:19:17.708111 lbz-0.6.6/lbz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-21 07:19:17.000000 lbz-0.6.6/lbz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-21 07:19:17.000000 lbz-0.6.6/lbz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:19:17.000000 lbz-0.6.6/lbz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 07:19:17.000000 lbz-0.6.6/lbz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 07:19:17.000000 lbz-0.6.6/lbz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-21 07:19:17.712111 lbz-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 07:19:10.000000 lbz-0.6.6/setup.py
```

### Comparing `lbz-0.6.5/LICENSE` & `lbz-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/PKG-INFO` & `lbz-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbz
-Version: 0.6.5
+Version: 0.6.6
 Summary: AWS Lambda REST ToolBox
 Home-page: https://github.com/pdyba/lambdalizator
 Author: Piotr Dyba
 Author-email: piotr.dyba@localbini.com
 License: LICENSE
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lbz-0.6.5/README.md` & `lbz-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/_cfg.py` & `lbz-0.6.6/lbz/_cfg.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/authentication.py` & `lbz-0.6.6/lbz/authentication.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/authz/authorizer.py` & `lbz-0.6.6/lbz/authz/authorizer.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/authz/decorators.py` & `lbz-0.6.6/lbz/authz/decorators.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/authz/utils.py` & `lbz-0.6.6/lbz/authz/utils.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/aws_boto3.py` & `lbz-0.6.6/lbz/aws_boto3.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/collector.py` & `lbz-0.6.6/lbz/collector.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/configuration.py` & `lbz-0.6.6/lbz/configuration.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/dev/server.py` & `lbz-0.6.6/lbz/dev/server.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/dev/test.py` & `lbz-0.6.6/lbz/dev/test.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/events/api.py` & `lbz-0.6.6/lbz/events/api.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/events/broker.py` & `lbz-0.6.6/lbz/events/broker.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/events/enums.py` & `lbz-0.6.6/lbz/events/enums.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/events/event.py` & `lbz-0.6.6/lbz/events/event.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/exceptions.py` & `lbz-0.6.6/lbz/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 class LambdaFWException(Exception):
     """Standardised for AWS Lambda exception class."""
 
     message = HTTPStatus.INTERNAL_SERVER_ERROR.description
     status_code = HTTPStatus.INTERNAL_SERVER_ERROR.value
     error_code: str | None = None
 
-    def __init__(self, message: str = "", error_code: str | None = None) -> None:
+    def __init__(
+        self, message: str = "", error_code: str | None = None, extra: dict | None = None
+    ) -> None:
         super().__init__(message)
-        if message:
-            self.message = message
-        if error_code:
-            self.error_code = error_code
+
+        self.message = message or self.message
+        self.error_code = error_code or self.error_code
+        self.extra = extra or {}
 
     def __str__(self) -> str:
         if self.error_code is not None:
             return f"[{self.status_code}] {self.error_code} - {self.message}"
         return f"[{self.status_code}] {self.message}"
```

### Comparing `lbz-0.6.5/lbz/handlers.py` & `lbz-0.6.6/lbz/handlers.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/jwt_utils.py` & `lbz-0.6.6/lbz/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/lambdas/broker.py` & `lbz-0.6.6/lbz/lambdas/broker.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/lambdas/client.py` & `lbz-0.6.6/lbz/lambdas/client.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/lambdas/enums.py` & `lbz-0.6.6/lbz/lambdas/enums.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/lambdas/response.py` & `lbz-0.6.6/lbz/lambdas/response.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/misc.py` & `lbz-0.6.6/lbz/misc.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/request.py` & `lbz-0.6.6/lbz/request.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/resource.py` & `lbz-0.6.6/lbz/resource.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/response.py` & `lbz-0.6.6/lbz/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import json
+from copy import deepcopy
 
 from lbz.exceptions import LambdaFWException
 from lbz.misc import deprecated
 from lbz.rest import ContentType
 
 
 class Response:
@@ -30,15 +31,15 @@
 
     def __repr__(self) -> str:
         return f"<Response(status_code={self.status_code})>"
 
     @classmethod
     def from_exception(cls, error: LambdaFWException, request_id: str) -> Response:
         """Creates a proper standardised Response for Errors."""
-        resp_data = {"message": error.message, "request_id": request_id}
+        resp_data = {**deepcopy(error.extra), "message": error.message, "request_id": request_id}
         if error.error_code:
             resp_data["error_code"] = error.error_code
 
         return cls(resp_data, status_code=error.status_code)
 
     @property
     def is_json(self) -> bool:
```

### Comparing `lbz-0.6.5/lbz/rest/api_gateway_event.py` & `lbz-0.6.6/lbz/rest/api_gateway_event.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/router.py` & `lbz-0.6.6/lbz/router.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz/type_defs.py` & `lbz-0.6.6/lbz/type_defs.py`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/lbz.egg-info/PKG-INFO` & `lbz-0.6.6/lbz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbz
-Version: 0.6.5
+Version: 0.6.6
 Summary: AWS Lambda REST ToolBox
 Home-page: https://github.com/pdyba/lambdalizator
 Author: Piotr Dyba
 Author-email: piotr.dyba@localbini.com
 License: LICENSE
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lbz-0.6.5/lbz.egg-info/SOURCES.txt` & `lbz-0.6.6/lbz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/setup.cfg` & `lbz-0.6.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `lbz-0.6.5/setup.py` & `lbz-0.6.6/setup.py`

 * *Files identical despite different names*

