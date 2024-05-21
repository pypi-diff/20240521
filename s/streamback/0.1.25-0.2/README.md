# Comparing `tmp/streamback-0.1.25.tar.gz` & `tmp/streamback-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamback-0.1.25.tar", last modified: Mon Mar 11 12:49:33 2024, max compression
+gzip compressed data, was "streamback-0.2.tar", last modified: Tue May 21 09:38:05 2024, max compression
```

## Comparing `streamback-0.1.25.tar` & `streamback-0.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-03-11 12:49:33.678433 streamback-0.1.25/
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)    11356 2023-09-17 21:12:43.000000 streamback-0.1.25/LICENCE.txt
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9438 2024-03-11 12:49:33.678433 streamback-0.1.25/PKG-INFO
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9109 2024-01-30 22:15:43.000000 streamback-0.1.25/README.md
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       38 2024-03-11 12:49:33.678433 streamback-0.1.25/setup.cfg
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      827 2024-03-11 12:49:22.000000 streamback-0.1.25/setup.py
-drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-03-11 12:49:33.678433 streamback-0.1.25/streamback/
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      474 2024-01-30 21:54:32.000000 streamback-0.1.25/streamback/__init__.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      409 2024-02-03 23:22:17.000000 streamback-0.1.25/streamback/callbacks.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      104 2023-09-17 21:22:51.000000 streamback-0.1.25/streamback/context.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      220 2023-11-21 12:26:15.000000 streamback-0.1.25/streamback/events.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1057 2024-01-10 09:28:47.000000 streamback-0.1.25/streamback/exceptions.py
-drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-03-11 12:49:33.678433 streamback-0.1.25/streamback/extensions/
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)        0 2024-01-30 21:53:20.000000 streamback-0.1.25/streamback/extensions/__init__.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2167 2024-02-03 23:37:42.000000 streamback-0.1.25/streamback/extensions/stats.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2583 2024-01-30 21:13:28.000000 streamback-0.1.25/streamback/feedback_lane.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     3285 2024-02-03 23:05:52.000000 streamback-0.1.25/streamback/listener.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1339 2024-01-10 11:11:57.000000 streamback-0.1.25/streamback/message.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     3269 2024-02-03 23:35:15.000000 streamback-0.1.25/streamback/process_manager.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      641 2023-10-14 23:34:10.000000 streamback-0.1.25/streamback/retry_strategy.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      752 2024-02-03 23:04:57.000000 streamback-0.1.25/streamback/router.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)    12519 2024-03-11 12:49:01.000000 streamback-0.1.25/streamback/streamback.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9288 2024-01-31 12:11:50.000000 streamback-0.1.25/streamback/streams.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      757 2024-01-30 21:29:55.000000 streamback-0.1.25/streamback/utils.py
-drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-03-11 12:49:33.678433 streamback-0.1.25/streamback.egg-info/
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9438 2024-03-11 12:49:33.000000 streamback-0.1.25/streamback.egg-info/PKG-INFO
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      599 2024-03-11 12:49:33.000000 streamback-0.1.25/streamback.egg-info/SOURCES.txt
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)        1 2024-03-11 12:49:33.000000 streamback-0.1.25/streamback.egg-info/dependency_links.txt
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       51 2024-03-11 12:49:33.000000 streamback-0.1.25/streamback.egg-info/requires.txt
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       11 2024-03-11 12:49:33.000000 streamback-0.1.25/streamback.egg-info/top_level.txt
+drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:38:05.163991 streamback-0.2/
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)    11356 2023-09-17 21:12:43.000000 streamback-0.2/LICENCE.txt
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9848 2024-05-21 09:38:05.163991 streamback-0.2/PKG-INFO
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9522 2024-05-21 09:37:37.000000 streamback-0.2/README.md
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       38 2024-05-21 09:38:05.163991 streamback-0.2/setup.cfg
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      824 2024-05-21 09:27:38.000000 streamback-0.2/setup.py
+drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:38:05.163991 streamback-0.2/streamback/
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      620 2024-05-21 09:35:31.000000 streamback-0.2/streamback/__init__.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      409 2024-02-03 23:22:17.000000 streamback-0.2/streamback/callbacks.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      104 2023-09-17 21:22:51.000000 streamback-0.2/streamback/context.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      220 2023-11-21 12:26:15.000000 streamback-0.2/streamback/events.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1057 2024-01-10 09:28:47.000000 streamback-0.2/streamback/exceptions.py
+drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:38:05.163991 streamback-0.2/streamback/extensions/
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)        0 2024-01-30 21:53:20.000000 streamback-0.2/streamback/extensions/__init__.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1956 2024-05-21 09:26:20.000000 streamback-0.2/streamback/extensions/auto_restart.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2340 2024-05-21 09:03:20.000000 streamback-0.2/streamback/extensions/stats.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2583 2024-01-30 21:13:28.000000 streamback-0.2/streamback/feedback_lane.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     3337 2024-05-21 08:31:00.000000 streamback-0.2/streamback/listener.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1339 2024-01-10 11:11:57.000000 streamback-0.2/streamback/message.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     4600 2024-05-21 09:08:30.000000 streamback-0.2/streamback/process_manager.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      641 2023-10-14 23:34:10.000000 streamback-0.2/streamback/retry_strategy.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      752 2024-02-03 23:04:57.000000 streamback-0.2/streamback/router.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)    13267 2024-05-21 09:13:06.000000 streamback-0.2/streamback/streamback.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9382 2024-05-21 09:30:50.000000 streamback-0.2/streamback/streams.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1102 2024-05-21 08:59:42.000000 streamback-0.2/streamback/utils.py
+drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:38:05.163991 streamback-0.2/streamback.egg-info/
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9848 2024-05-21 09:38:05.000000 streamback-0.2/streamback.egg-info/PKG-INFO
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      637 2024-05-21 09:38:05.000000 streamback-0.2/streamback.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)        1 2024-05-21 09:38:05.000000 streamback-0.2/streamback.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       51 2024-05-21 09:38:05.000000 streamback-0.2/streamback.egg-info/requires.txt
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       11 2024-05-21 09:38:05.000000 streamback-0.2/streamback.egg-info/top_level.txt
```

### Comparing `streamback-0.1.25/LICENCE.txt` & `streamback-0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `streamback-0.1.25/PKG-INFO` & `streamback-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: streamback
-Version: 0.1.25
-Summary: Two way streams for your microservices
-Author: Stefanos Liakis
-Author-email: stliakis@gmail.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
 ## 2-way streams for your microservices
 
 ### What is a stream with feedbacks?
 
 ----
 
 With Streamback you can implement the producer-consumer model but with a twist. The consumer can
@@ -337,28 +326,46 @@
     streams="main=kafka://kafka:9092&feedback=redis://redis:6379",
 ).add_callback(StreambackCallbacks())
 ```
 
 ## Extensions
 
 By using the callbacks mechanism new extensions can be created to inject custom logic into the lifecycle of Streamback.
-For example
-the ListenerStats extension can be used to log the memory usage of each listener.
+
+### Stats extension
+
+The ListenerStats extension can be used to log the memory usage of each listener.
 
 ```python
 from streamback import Streamback, ListenerStats
 
 streamback = Streamback(
     "example_consumer_app",
     streams="main=kafka://kafka:9092&feedback=redis://redis:6379",
 ).add_callback(ListenerStats(interval=10))
 ```
 
-The above will log the memory usage of the listeners every 10 seconds, you can extend the ListenerStats class to add
-custom
+The above will log the memory usage of the listeners every 10 seconds
+
+### AutoRestart extension
+
+```python
+from streamback import Streamback, AutoRestart
+
+streamback = Streamback(
+    "example_consumer_app",
+    streams="main=kafka://kafka:9092&feedback=redis://redis:6379",
+).add_callback(AutoRestart(max_seconds=10, max_memory_mb=100))
+```
+
+The above will restart the child processes every 10 seconds or when it reaches 100mb of rss memory usage.
+
+### Custom extensions
+
+You can extend the ListenerStats class to add custom
 logic like reporting the memory usage to a monitoring service.
 
 ```python
 from streamback import Streamback, ListenerStats
 
 
 class MyListenerStats(ListenerStats):
@@ -372,8 +379,8 @@
 ).add_callback(MyListenerStats(interval=10))
 ```
 
 ### Why python 2.7 compatible?
 
 Streamback has been created for usage in car.gr's systems which has some legacy python 2.7 services. We are are planing
 to move Streamback to python >3.7 in some later version but for now the python 2.7 support was crucial and thus the
-async/await support was sacrificed. Currently it is used in production to handle millions of messages per day.
+async/await support was sacrificed. Currently it is used in production to handle millions of messages per day.
```

### Comparing `streamback-0.1.25/README.md` & `streamback-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: streamback
+Version: 0.2
+Summary: Two way streams for your microservices
+Author: Stefanos Liakis
+Author-email: stliakis@gmail.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
 ## 2-way streams for your microservices
 
 ### What is a stream with feedbacks?
 
 ----
 
 With Streamback you can implement the producer-consumer model but with a twist. The consumer can
@@ -326,28 +337,46 @@
     streams="main=kafka://kafka:9092&feedback=redis://redis:6379",
 ).add_callback(StreambackCallbacks())
 ```
 
 ## Extensions
 
 By using the callbacks mechanism new extensions can be created to inject custom logic into the lifecycle of Streamback.
-For example
-the ListenerStats extension can be used to log the memory usage of each listener.
+
+### Stats extension
+
+The ListenerStats extension can be used to log the memory usage of each listener.
 
 ```python
 from streamback import Streamback, ListenerStats
 
 streamback = Streamback(
     "example_consumer_app",
     streams="main=kafka://kafka:9092&feedback=redis://redis:6379",
 ).add_callback(ListenerStats(interval=10))
 ```
 
-The above will log the memory usage of the listeners every 10 seconds, you can extend the ListenerStats class to add
-custom
+The above will log the memory usage of the listeners every 10 seconds
+
+### AutoRestart extension
+
+```python
+from streamback import Streamback, AutoRestart
+
+streamback = Streamback(
+    "example_consumer_app",
+    streams="main=kafka://kafka:9092&feedback=redis://redis:6379",
+).add_callback(AutoRestart(max_seconds=10, max_memory_mb=100))
+```
+
+The above will restart the child processes every 10 seconds or when it reaches 100mb of rss memory usage.
+
+### Custom extensions
+
+You can extend the ListenerStats class to add custom
 logic like reporting the memory usage to a monitoring service.
 
 ```python
 from streamback import Streamback, ListenerStats
 
 
 class MyListenerStats(ListenerStats):
@@ -361,8 +390,8 @@
 ).add_callback(MyListenerStats(interval=10))
 ```
 
 ### Why python 2.7 compatible?
 
 Streamback has been created for usage in car.gr's systems which has some legacy python 2.7 services. We are are planing
 to move Streamback to python >3.7 in some later version but for now the python 2.7 support was crucial and thus the
-async/await support was sacrificed. Currently it is used in production to handle millions of messages per day.
+async/await support was sacrificed. Currently it is used in production to handle millions of messages per day.
```

### Comparing `streamback-0.1.25/setup.py` & `streamback-0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 else:
     REQUIRES = [
         "redis>=2.10.6", "confluent-kafka>=1.7.0", "psutil>=5.8.0"
     ]
 
 setup(
     name="streamback",
-    version="0.1.25",
+    version="0.2",
     author='Stefanos Liakis',
     author_email='stliakis@gmail.com',
     description="Two way streams for your microservices",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=REQUIRES,
```

### Comparing `streamback-0.1.25/streamback/exceptions.py` & `streamback-0.2/streamback/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamback-0.1.25/streamback/extensions/stats.py` & `streamback-0.2/streamback/extensions/stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,18 @@
             if time.time() - self.last_tick < self.interval:
                 return
 
         total_rss, total_vms = 0, 0
 
         memory_per_topic = {}
         for topic_process in process_manager.topic_processes:
+            if not topic_process.is_process_alive():
+                log(INFO, "PROCESS_IS_DEAD[topic={topic}]".format(topic=topic_process.topic))
+                continue
+
             process = psutil.Process(topic_process.process.pid)
             memory_info = process.memory_info()
             total_rss += memory_info.rss
             topic_name = str(topic_process.topic)
             memory_per_topic.setdefault(topic_name, {
                 "rss": 0,
                 "vms": 0,
```

### Comparing `streamback-0.1.25/streamback/feedback_lane.py` & `streamback-0.2/streamback/feedback_lane.py`

 * *Files identical despite different names*

### Comparing `streamback-0.1.25/streamback/listener.py` & `streamback-0.2/streamback/listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,17 @@
             args = []
             if "context" in valid_arguments:
                 args.append(context)
             args.append(message)
 
             self.function(*args)
 
+    def flush(self, *args, **kwargs):
+        pass
+
     def consume_input(self, *args, **kwargs):
         if self.function:
             self.function(*args, **kwargs)
 
     def __repr__(self):
         if self.function:
             return "Listener[topic=%s,function=%s]" % (self.topic, self.function.__name__)
```

### Comparing `streamback-0.1.25/streamback/message.py` & `streamback-0.2/streamback/message.py`

 * *Files identical despite different names*

### Comparing `streamback-0.1.25/streamback/retry_strategy.py` & `streamback-0.2/streamback/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `streamback-0.1.25/streamback/router.py` & `streamback-0.2/streamback/router.py`

 * *Files identical despite different names*

### Comparing `streamback-0.1.25/streamback/streamback.py` & `streamback-0.2/streamback/streamback.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import time
 import traceback
 from logging import INFO, ERROR, WARNING, DEBUG
 import uuid
 import signal
 import sys
-from .process_manager import ProcessManager
+from .process_manager import ProcessManager, TopicProcessMessages
 from .feedback_lane import FeedbackLane
 from .exceptions import InvalidMessageType
 from .context import ConsumerContext
 from .events import Events
 from .listener import Listener
 from .streams import KafkaStream, ParsedStreams
 from .utils import log
@@ -268,21 +268,32 @@
         return decorator
 
     def include_router(self, router):
         self.routers.append(router)
         for listener in router.listeners:
             self.add_listener(listener)
 
-    def start_listeners(self, topic, listeners):
+    def on_message_from_master_process(self, message, topic, listeners):
+        log(INFO, "RECEIVED_MESSAGE_FROM_MASTER_PROCESS[message={message}]".format(message=message))
+        if message == TopicProcessMessages.TERMINATE:
+            log(INFO, "LISTENER_PROCESS_KILLED[topic={topic}]".format(topic=topic))
+            self.close(listeners)
+            sys.exit(0)
+
+    def start_listeners(self, pipe, topic, listeners):
         self.listeners = listeners
         self.initialize_streams()
         self.on_fork()
 
+        def on_tick():
+            if pipe.poll():
+                self.on_message_from_master_process(pipe.recv(), topic, listeners)
+
         for message in self.main_stream.read_stream(
-                streamback=self, topics=[topic], timeout=None
+                streamback=self, topics=[topic], timeout=None, on_tick=on_tick
         ):
             log(
                 INFO,
                 "RECEIVED[message={message}]".format(message=message),
             )
 
             context = ConsumerContext(streamback=self)
@@ -305,15 +316,14 @@
                     traceback.print_exc()
                     failed_listeners.append([listener, e, context, message])
                     for callback in self.get_callbacks():
                         callback.on_consume_end(
                             self, listener, context, message, exception=e
                         )
                 finally:
-
                     message.ack()
 
             if failed_listeners:
                 errors = []
                 for failed_listener in failed_listeners:
                     self.consume_exception(*failed_listener)
                     errors.append(repr(failed_listener[1]))
@@ -322,26 +332,26 @@
                     self.send_feedback_end(
                         message.feedback_topic, with_error=", ".join(errors)
                     )
             elif not failed_listeners:
                 if self.feedback_stream and message.feedback_topic:
                     self.send_feedback_end(message.feedback_topic)
 
-    def _start_listener(self, topic, listeners):
+    def _start_listener(self, pipe, topic, listeners):
         def signal_handler(sig, frame):
             log(INFO, "LISTENER_PROCESS_KILLED[topic={topic}]".format(topic=topic))
-            self.close()
+            self.close(listeners)
             sys.exit(0)
 
         signal.signal(signal.SIGTERM, signal_handler)
 
         try:
-            self.start_listeners(topic, listeners)
+            self.start_listeners(pipe, topic, listeners)
         except (KeyboardInterrupt, Exception):
-            self.close()
+            self.close(listeners)
 
     def start(self):
         process_manager = ProcessManager()
         process_manager.spin(self, self._start_listener, self.listeners)
 
     def get_callbacks(self):
         return self.callbacks
@@ -357,21 +367,25 @@
         self.listeners.setdefault(listener.topic, []).append(listener)
         return self
 
     def add_callback(self, *callback):
         self.callbacks.extend(callback)
         return self
 
-    def close(self):
-        log(INFO, "CLOSING_STREAMBACK")
+    def close(self, listeners):
+        for listener in listeners:
+            log(INFO, "FLUSHING_LISTENER[listener={listener}]".format(listener=listener))
+            listener.flush()
 
         if self.feedback_stream and self.feedback_stream.is_initialized():
             self.feedback_stream.close()
         if self.main_stream and self.main_stream.is_initialized():
             self.main_stream.close()
 
+        log(INFO, "CLOSING_STREAMBACK[]")
+
     def __repr__(self):
         return "Streamback[name={name},main_stream={main_stream},feedback_stream={feedback_stream}]".format(
             name=self.name,
             main_stream=self.main_stream,
             feedback_stream=self.feedback_stream,
         )
```

### Comparing `streamback-0.1.25/streamback/streams.py` & `streamback-0.2/streamback/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def initialize(self, group_name, timeout=10):
         raise NotImplementedError
 
     def send(self, topic, payload, key=None, flush=False):
         raise NotImplementedError
 
-    def read_stream(self, streamback, topics, timeout=None):
+    def read_stream(self, streamback, topics, timeout=None, on_tick=None):
         raise NotImplementedError
 
     def serialize_payload(self, data):
         return json.dumps(data).encode("utf-8")
 
     def deserialize_payload(self, data):
         return json.loads(data.decode("utf-8"))
@@ -145,26 +145,29 @@
             )
             return False
         else:
             log(INFO, "SUCCESSFULLY_FLUSHED_MESSAGES")
 
         return True
 
-    def read_stream(self, streamback, topics, timeout=None):
+    def read_stream(self, streamback, topics, timeout=None, on_tick=None):
         consumer = self.kafka_consumer
         consumer.subscribe(topics)
         begin = time.time()
 
         log(
             INFO,
             "MAIN_STREAM_LISTENING[topics={topics}]".format(topics=topics),
         )
 
         while True:
-            msg = consumer.poll(0.1)
+            if on_tick:
+                on_tick()
+
+            msg = consumer.poll(0.05)
 
             if timeout:
                 time_since_begin = time.time() - begin
                 if time_since_begin > timeout:
                     return
 
             if not msg:
@@ -219,15 +222,15 @@
     def send(self, topic, payload, key=None, flush=None):
         self.redis_client.lpush(topic, self.serialize_payload(payload))
         self.redis_client.expire(topic, 300)
 
     def get_pending_messages_count(self):
         return 0
 
-    def read_stream(self, streamback, topics, timeout=None):
+    def read_stream(self, streamback, topics, timeout=None, on_tick=None):
         while True:
             value = self.redis_client.brpop(topics, timeout=timeout)
 
             if value is None:
                 raise FeedbackTimeout(topics=topics, timeout=timeout)
 
             payload = self.deserialize_payload(value[1])
```

### Comparing `streamback-0.1.25/streamback.egg-info/PKG-INFO` & `streamback-0.2/streamback.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamback
-Version: 0.1.25
+Version: 0.2
 Summary: Two way streams for your microservices
 Author: Stefanos Liakis
 Author-email: stliakis@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
@@ -337,28 +337,46 @@
     streams="main=kafka://kafka:9092&feedback=redis://redis:6379",
 ).add_callback(StreambackCallbacks())
 ```
 
 ## Extensions
 
 By using the callbacks mechanism new extensions can be created to inject custom logic into the lifecycle of Streamback.
-For example
-the ListenerStats extension can be used to log the memory usage of each listener.
+
+### Stats extension
+
+The ListenerStats extension can be used to log the memory usage of each listener.
 
 ```python
 from streamback import Streamback, ListenerStats
 
 streamback = Streamback(
     "example_consumer_app",
     streams="main=kafka://kafka:9092&feedback=redis://redis:6379",
 ).add_callback(ListenerStats(interval=10))
 ```
 
-The above will log the memory usage of the listeners every 10 seconds, you can extend the ListenerStats class to add
-custom
+The above will log the memory usage of the listeners every 10 seconds
+
+### AutoRestart extension
+
+```python
+from streamback import Streamback, AutoRestart
+
+streamback = Streamback(
+    "example_consumer_app",
+    streams="main=kafka://kafka:9092&feedback=redis://redis:6379",
+).add_callback(AutoRestart(max_seconds=10, max_memory_mb=100))
+```
+
+The above will restart the child processes every 10 seconds or when it reaches 100mb of rss memory usage.
+
+### Custom extensions
+
+You can extend the ListenerStats class to add custom
 logic like reporting the memory usage to a monitoring service.
 
 ```python
 from streamback import Streamback, ListenerStats
 
 
 class MyListenerStats(ListenerStats):
```

### Comparing `streamback-0.1.25/streamback.egg-info/SOURCES.txt` & `streamback-0.2/streamback.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 streamback/utils.py
 streamback.egg-info/PKG-INFO
 streamback.egg-info/SOURCES.txt
 streamback.egg-info/dependency_links.txt
 streamback.egg-info/requires.txt
 streamback.egg-info/top_level.txt
 streamback/extensions/__init__.py
+streamback/extensions/auto_restart.py
 streamback/extensions/stats.py
```

