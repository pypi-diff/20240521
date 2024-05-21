# Comparing `tmp/streamback-0.2.1.tar.gz` & `tmp/streamback-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamback-0.2.1.tar", last modified: Tue May 21 09:48:15 2024, max compression
+gzip compressed data, was "streamback-0.2.2.tar", last modified: Tue May 21 09:50:06 2024, max compression
```

## Comparing `streamback-0.2.1.tar` & `streamback-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:48:15.476879 streamback-0.2.1/
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)    11356 2023-09-17 21:12:43.000000 streamback-0.2.1/LICENCE.txt
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9850 2024-05-21 09:48:15.476879 streamback-0.2.1/PKG-INFO
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9522 2024-05-21 09:37:37.000000 streamback-0.2.1/README.md
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       38 2024-05-21 09:48:15.476879 streamback-0.2.1/setup.cfg
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      826 2024-05-21 09:47:09.000000 streamback-0.2.1/setup.py
-drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:48:15.476879 streamback-0.2.1/streamback/
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      542 2024-05-21 09:45:55.000000 streamback-0.2.1/streamback/__init__.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      409 2024-02-03 23:22:17.000000 streamback-0.2.1/streamback/callbacks.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      104 2023-09-17 21:22:51.000000 streamback-0.2.1/streamback/context.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      220 2023-11-21 12:26:15.000000 streamback-0.2.1/streamback/events.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1057 2024-01-10 09:28:47.000000 streamback-0.2.1/streamback/exceptions.py
-drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:48:15.476879 streamback-0.2.1/streamback/extensions/
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)        0 2024-01-30 21:53:20.000000 streamback-0.2.1/streamback/extensions/__init__.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2001 2024-05-21 09:46:47.000000 streamback-0.2.1/streamback/extensions/auto_restart.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2340 2024-05-21 09:03:20.000000 streamback-0.2.1/streamback/extensions/stats.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2583 2024-01-30 21:13:28.000000 streamback-0.2.1/streamback/feedback_lane.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     3337 2024-05-21 08:31:00.000000 streamback-0.2.1/streamback/listener.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1339 2024-01-10 11:11:57.000000 streamback-0.2.1/streamback/message.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     4591 2024-05-21 09:46:47.000000 streamback-0.2.1/streamback/process_manager.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      641 2023-10-14 23:34:10.000000 streamback-0.2.1/streamback/retry_strategy.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      752 2024-02-03 23:04:57.000000 streamback-0.2.1/streamback/router.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)    13267 2024-05-21 09:13:06.000000 streamback-0.2.1/streamback/streamback.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9382 2024-05-21 09:30:50.000000 streamback-0.2.1/streamback/streams.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       64 2024-05-21 09:45:29.000000 streamback-0.2.1/streamback/topic_process_messages.py
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1102 2024-05-21 08:59:42.000000 streamback-0.2.1/streamback/utils.py
-drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:48:15.476879 streamback-0.2.1/streamback.egg-info/
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9850 2024-05-21 09:48:15.000000 streamback-0.2.1/streamback.egg-info/PKG-INFO
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      674 2024-05-21 09:48:15.000000 streamback-0.2.1/streamback.egg-info/SOURCES.txt
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)        1 2024-05-21 09:48:15.000000 streamback-0.2.1/streamback.egg-info/dependency_links.txt
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       51 2024-05-21 09:48:15.000000 streamback-0.2.1/streamback.egg-info/requires.txt
--rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       11 2024-05-21 09:48:15.000000 streamback-0.2.1/streamback.egg-info/top_level.txt
+drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:50:06.987643 streamback-0.2.2/
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)    11356 2023-09-17 21:12:43.000000 streamback-0.2.2/LICENCE.txt
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9850 2024-05-21 09:50:06.987643 streamback-0.2.2/PKG-INFO
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9522 2024-05-21 09:37:37.000000 streamback-0.2.2/README.md
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       38 2024-05-21 09:50:06.987643 streamback-0.2.2/setup.cfg
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      826 2024-05-21 09:50:05.000000 streamback-0.2.2/setup.py
+drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:50:06.987643 streamback-0.2.2/streamback/
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      542 2024-05-21 09:45:55.000000 streamback-0.2.2/streamback/__init__.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      409 2024-02-03 23:22:17.000000 streamback-0.2.2/streamback/callbacks.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      104 2023-09-17 21:22:51.000000 streamback-0.2.2/streamback/context.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      220 2023-11-21 12:26:15.000000 streamback-0.2.2/streamback/events.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1057 2024-01-10 09:28:47.000000 streamback-0.2.2/streamback/exceptions.py
+drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:50:06.987643 streamback-0.2.2/streamback/extensions/
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)        0 2024-01-30 21:53:20.000000 streamback-0.2.2/streamback/extensions/__init__.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2001 2024-05-21 09:46:47.000000 streamback-0.2.2/streamback/extensions/auto_restart.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2340 2024-05-21 09:03:20.000000 streamback-0.2.2/streamback/extensions/stats.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     2583 2024-01-30 21:13:28.000000 streamback-0.2.2/streamback/feedback_lane.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     3337 2024-05-21 08:31:00.000000 streamback-0.2.2/streamback/listener.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1339 2024-01-10 11:11:57.000000 streamback-0.2.2/streamback/message.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     4609 2024-05-21 09:49:45.000000 streamback-0.2.2/streamback/process_manager.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      641 2023-10-14 23:34:10.000000 streamback-0.2.2/streamback/retry_strategy.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      752 2024-02-03 23:04:57.000000 streamback-0.2.2/streamback/router.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)    13267 2024-05-21 09:13:06.000000 streamback-0.2.2/streamback/streamback.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9382 2024-05-21 09:30:50.000000 streamback-0.2.2/streamback/streams.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       64 2024-05-21 09:45:29.000000 streamback-0.2.2/streamback/topic_process_messages.py
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     1102 2024-05-21 08:59:42.000000 streamback-0.2.2/streamback/utils.py
+drwxrwxr-x   0 stefanos  (1000) stefanos  (1000)        0 2024-05-21 09:50:06.987643 streamback-0.2.2/streamback.egg-info/
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)     9850 2024-05-21 09:50:06.000000 streamback-0.2.2/streamback.egg-info/PKG-INFO
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)      674 2024-05-21 09:50:06.000000 streamback-0.2.2/streamback.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)        1 2024-05-21 09:50:06.000000 streamback-0.2.2/streamback.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       51 2024-05-21 09:50:06.000000 streamback-0.2.2/streamback.egg-info/requires.txt
+-rw-rw-r--   0 stefanos  (1000) stefanos  (1000)       11 2024-05-21 09:50:06.000000 streamback-0.2.2/streamback.egg-info/top_level.txt
```

### Comparing `streamback-0.2.1/LICENCE.txt` & `streamback-0.2.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/PKG-INFO` & `streamback-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamback
-Version: 0.2.1
+Version: 0.2.2
 Summary: Two way streams for your microservices
 Author: Stefanos Liakis
 Author-email: stliakis@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `streamback-0.2.1/README.md` & `streamback-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/setup.py` & `streamback-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 else:
     REQUIRES = [
         "redis>=2.10.6", "confluent-kafka>=1.7.0", "psutil>=5.8.0"
     ]
 
 setup(
     name="streamback",
-    version="0.2.1",
+    version="0.2.2",
     author='Stefanos Liakis',
     author_email='stliakis@gmail.com',
     description="Two way streams for your microservices",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=REQUIRES,
```

### Comparing `streamback-0.2.1/streamback/__init__.py` & `streamback-0.2.2/streamback/__init__.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/exceptions.py` & `streamback-0.2.2/streamback/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/extensions/auto_restart.py` & `streamback-0.2.2/streamback/extensions/auto_restart.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/extensions/stats.py` & `streamback-0.2.2/streamback/extensions/stats.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/feedback_lane.py` & `streamback-0.2.2/streamback/feedback_lane.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/listener.py` & `streamback-0.2.2/streamback/listener.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/message.py` & `streamback-0.2.2/streamback/message.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/process_manager.py` & `streamback-0.2.2/streamback/process_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
                                                                                                topic),
                                                                                            ", ".join(str(listener) for
                                                                                                      listener in
                                                                                                      listeners))
                                                                                        for topic, listeners in
                                                                                        listeners.items()])))
 
-        for topic, listeners in listeners.items():
+        for topic, listeners_of_topic in listeners.items():
             for i in range(listener_procs_per_topic.get(topic)):
-                topic_process = TopicProcess(topic=topic, listeners=listeners, target=target)
+                topic_process = TopicProcess(topic=topic, listeners=listeners_of_topic, target=target)
                 self.add_topic_process(
                     topic_process
                 )
                 topic_process.spawn()
 
         def signal_handler(sig, frame):
             log(INFO, "PROCESS_MANAGER_MASTER_PROCESS_KILLED")
```

### Comparing `streamback-0.2.1/streamback/retry_strategy.py` & `streamback-0.2.2/streamback/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/router.py` & `streamback-0.2.2/streamback/router.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/streamback.py` & `streamback-0.2.2/streamback/streamback.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/streams.py` & `streamback-0.2.2/streamback/streams.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback/utils.py` & `streamback-0.2.2/streamback/utils.py`

 * *Files identical despite different names*

### Comparing `streamback-0.2.1/streamback.egg-info/PKG-INFO` & `streamback-0.2.2/streamback.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamback
-Version: 0.2.1
+Version: 0.2.2
 Summary: Two way streams for your microservices
 Author: Stefanos Liakis
 Author-email: stliakis@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `streamback-0.2.1/streamback.egg-info/SOURCES.txt` & `streamback-0.2.2/streamback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

