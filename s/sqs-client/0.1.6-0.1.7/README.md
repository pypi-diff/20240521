# Comparing `tmp/sqs_client-0.1.6.tar.gz` & `tmp/sqs_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqs_client-0.1.6.tar", last modified: Tue May 14 04:13:32 2024, max compression
+gzip compressed data, was "sqs_client-0.1.7.tar", last modified: Tue May 21 07:04:14 2024, max compression
```

## Comparing `sqs_client-0.1.6.tar` & `sqs_client-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:13:32.464771 sqs_client-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 04:13:13.000000 sqs_client-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-14 04:13:32.464771 sqs_client-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-14 04:13:13.000000 sqs_client-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 04:13:13.000000 sqs_client-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 04:13:32.464771 sqs_client-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:13:32.464771 sqs_client-0.1.6/sqs_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 04:13:13.000000 sqs_client-0.1.6/sqs_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-14 04:13:13.000000 sqs_client-0.1.6/sqs_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-14 04:13:13.000000 sqs_client-0.1.6/sqs_client/publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-14 04:13:13.000000 sqs_client-0.1.6/sqs_client/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:13:32.464771 sqs_client-0.1.6/sqs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-14 04:13:32.000000 sqs_client-0.1.6/sqs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 04:13:32.000000 sqs_client-0.1.6/sqs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 04:13:32.000000 sqs_client-0.1.6/sqs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 04:13:32.000000 sqs_client-0.1.6/sqs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:04:14.841814 sqs_client-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 07:04:01.000000 sqs_client-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-21 07:04:14.841814 sqs_client-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-21 07:04:01.000000 sqs_client-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-21 07:04:01.000000 sqs_client-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-21 07:04:14.841814 sqs_client-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:04:14.841814 sqs_client-0.1.7/sqs_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:04:01.000000 sqs_client-0.1.7/sqs_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-21 07:04:01.000000 sqs_client-0.1.7/sqs_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-21 07:04:01.000000 sqs_client-0.1.7/sqs_client/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-21 07:04:01.000000 sqs_client-0.1.7/sqs_client/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:04:14.841814 sqs_client-0.1.7/sqs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-21 07:04:14.000000 sqs_client-0.1.7/sqs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-21 07:04:14.000000 sqs_client-0.1.7/sqs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:04:14.000000 sqs_client-0.1.7/sqs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 07:04:14.000000 sqs_client-0.1.7/sqs_client.egg-info/top_level.txt
```

### Comparing `sqs_client-0.1.6/LICENSE` & `sqs_client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sqs_client-0.1.6/PKG-INFO` & `sqs_client-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqs-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: SQS client
 Author-email: Digital Fortress <hai.huynh@digitalfortress.dev>
 Project-URL: Homepage, https://github.com/digitalfortress-dev/python-sqs-client
 Project-URL: Issues, https://github.com/digitalfortress-dev/python-sqs-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sqs_client-0.1.6/README.md` & `sqs_client-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sqs_client-0.1.6/pyproject.toml` & `sqs_client-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqs-client"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Digital Fortress", email="hai.huynh@digitalfortress.dev" },
 ]
 description = "SQS client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sqs_client-0.1.6/sqs_client/client.py` & `sqs_client-0.1.7/sqs_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from logging import exception
 
 import boto3
+from botocore.config import Config
 
 from sqs_client.task import Task
 
 
 class SQSClient:
     """
     This class represents a client for interacting with the SQS service.
@@ -13,14 +14,15 @@
     """
 
     def __init__(
         self,
         region_name=None,
         aws_access_key_id=None,
         aws_secret_access_key=None,
+        max_pool_connections: int = 10,
     ):
         """
         Initializes the SQSClient class.
 
         Args:
             region_name: (string) The name of the region associated with the client.
             aws_access_key_id: (string) The access key to use when creating
@@ -30,19 +32,21 @@
                 to override the credentials used for this specific client.
             aws_access_key_id: (string) The access key to use when creating
                 the client.  This is entirely optional, and if not provided,
                 the credentials configured for the session will automatically
                 be used.  You only need to provide this argument if you want
                 to override the credentials used for this specific client.
         """
+        config = Config(max_pool_connections=max_pool_connections)
         self._boto3_client = boto3.client(
             "sqs",
             region_name=region_name,
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
+            config=config,
         )
         self._list_queue_urls = None
         self._task_list = {}
 
     def get_task_list(self):
         """
         This function retrieves the list of tasks currently
```

### Comparing `sqs_client-0.1.6/sqs_client/publisher.py` & `sqs_client-0.1.7/sqs_client/publisher.py`

 * *Files identical despite different names*

### Comparing `sqs_client-0.1.6/sqs_client/task.py` & `sqs_client-0.1.7/sqs_client/task.py`

 * *Files identical despite different names*

### Comparing `sqs_client-0.1.6/sqs_client.egg-info/PKG-INFO` & `sqs_client-0.1.7/sqs_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqs-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: SQS client
 Author-email: Digital Fortress <hai.huynh@digitalfortress.dev>
 Project-URL: Homepage, https://github.com/digitalfortress-dev/python-sqs-client
 Project-URL: Issues, https://github.com/digitalfortress-dev/python-sqs-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

