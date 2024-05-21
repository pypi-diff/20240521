# Comparing `tmp/taskiq_sqs-0.0.3.tar.gz` & `tmp/taskiq_sqs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_sqs-0.0.3.tar", last modified: Thu May 16 02:45:06 2024, max compression
+gzip compressed data, was "taskiq_sqs-0.0.4.tar", last modified: Tue May 21 19:21:25 2024, max compression
```

## Comparing `taskiq_sqs-0.0.3.tar` & `taskiq_sqs-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.840353 taskiq_sqs-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.840353 taskiq_sqs-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.840353 taskiq_sqs-0.0.3/taskiq_sqs/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/taskiq_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/taskiq_sqs/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/tests/test_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:21:25.902192 taskiq_sqs-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:21:25.898192 taskiq_sqs-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:21:25.898192 taskiq_sqs-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-21 19:21:25.902192 taskiq_sqs-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-21 19:21:25.902192 taskiq_sqs-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:21:25.898192 taskiq_sqs-0.0.4/taskiq_sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/taskiq_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/taskiq_sqs/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:21:25.902192 taskiq_sqs-0.0.4/taskiq_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-21 19:21:25.000000 taskiq_sqs-0.0.4/taskiq_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-21 19:21:25.000000 taskiq_sqs-0.0.4/taskiq_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:21:25.000000 taskiq_sqs-0.0.4/taskiq_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-21 19:21:25.000000 taskiq_sqs-0.0.4/taskiq_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 19:21:25.000000 taskiq_sqs-0.0.4/taskiq_sqs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:21:25.902192 taskiq_sqs-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-21 19:20:54.000000 taskiq_sqs-0.0.4/tests/test_broker.py
```

### Comparing `taskiq_sqs-0.0.3/.github/workflows/release.yaml` & `taskiq_sqs-0.0.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `taskiq_sqs-0.0.3/.github/workflows/test.yaml` & `taskiq_sqs-0.0.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `taskiq_sqs-0.0.3/.gitignore` & `taskiq_sqs-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `taskiq_sqs-0.0.3/LICENSE` & `taskiq_sqs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_sqs-0.0.3/PKG-INFO` & `taskiq_sqs-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-sqs
-Version: 0.0.3
+Version: 0.0.4
 Summary: SQS Broker for TaskIQ
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `taskiq_sqs-0.0.3/README.md` & `taskiq_sqs-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_sqs-0.0.3/pyproject.toml` & `taskiq_sqs-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskiq_sqs-0.0.3/taskiq_sqs/broker.py` & `taskiq_sqs-0.0.4/taskiq_sqs/broker.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import boto3
 from asyncer import asyncify
 from mypy_boto3_sqs.service_resource import Queue
 from taskiq import AsyncBroker
 from taskiq.abc.result_backend import AsyncResultBackend
 from taskiq.acks import AckableMessage
+from taskiq.exceptions import BrokerError
 from taskiq.message import BrokerMessage
 
 logger = logging.getLogger(__name__)
 
 
 def stamp() -> int:
     return int(datetime.now(tz=timezone.utc).timestamp())
@@ -20,22 +21,30 @@
 
 class SQSBroker(AsyncBroker):
     """AWS SQS TaskIQ broker."""
 
     def __init__(
         self,
         sqs_queue_url: str,
+        wait_time_seconds: int = 0,  # Used for long polling
+        max_number_of_messages: int = 1,  # size of batch to receive from the queue
         result_backend: Optional[AsyncResultBackend] = None,
         task_id_generator: Optional[Callable[[], str]] = None,
     ) -> None:
         super().__init__(result_backend, task_id_generator)
         self.sqs_queue_url = sqs_queue_url
         self._sqs = boto3.resource("sqs")
         self._sqs_queue: Optional[Queue] = None
 
+        if max_number_of_messages > 10:
+            raise BrokerError("MaxNumberOfMessages can be no greater than 10")
+
+        self.wait_time_seconds = max(wait_time_seconds, 0)
+        self.max_number_of_messages = max(max_number_of_messages, 1)
+
     async def _get_queue(self) -> Queue:
         queue_name = self.sqs_queue_url.split("/")[-1]
 
         if not self._sqs_queue:
             self._sqs_queue = await asyncify(self._sqs.get_queue_by_name)(
                 QueueName=queue_name
             )
@@ -93,36 +102,43 @@
         :return: nothing.
         """
 
         queue = await self._get_queue()
 
         # TODO: Consider using AckableMessage and confirm with the queue to reduce lost messages
         while True:
-            last_had_message = False
+            no_backoff = False
 
             for message in await asyncify(queue.receive_messages)(
-                MessageAttributeNames=[".*"]
+                MessageAttributeNames=[".*"],
+                # If there's competition on this queue (multiple processes of workers pulling from
+                # the same queue), and processing takes longer than the visibility timeout, multiple
+                # workers may end up processing the same message.
+                MaxNumberOfMessages=self.max_number_of_messages,
+                # Use long poling.
+                WaitTimeSeconds=self.wait_time_seconds,
             ):
                 try:
                     if message.message_attributes:
                         # if expiry was set as a message attribute, respect it
                         if expiry_typed := message.message_attributes.get("expiry"):
                             expiry = int(expiry_typed.get("StringValue", 0))
                             now = stamp()
                             if 0 < expiry < now:
                                 logger.warn(
                                     f"Message expired {now - expiry} seconds ago. Skipping."
                                 )
                                 await asyncify(message.delete)()
+                                no_backoff = True
                                 continue
                 except TypeError:
                     # Ignore weird expiries.  Not critical.
                     pass
 
                 yield message.body.encode("utf-8")
                 await asyncify(message.delete)()
-                last_had_message = True
+                no_backoff = True
 
-            sleepdur = 0.1 if last_had_message else 1
+            sleepdur = 0.01 if no_backoff else 1
             logger.debug(f"No messages on queue. Broker is sleeping for {sleepdur}s...")
             await asyncio.sleep(sleepdur)
-            last_had_message = False
+            no_backoff = False
```

### Comparing `taskiq_sqs-0.0.3/taskiq_sqs.egg-info/PKG-INFO` & `taskiq_sqs-0.0.4/taskiq_sqs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-sqs
-Version: 0.0.3
+Version: 0.0.4
 Summary: SQS Broker for TaskIQ
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

