# Comparing `tmp/dig_ass_critic_protos-1.0.6.tar.gz` & `tmp/dig_ass_critic_protos-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_critic_protos-1.0.6.tar", last modified: Mon May 20 11:51:35 2024, max compression
+gzip compressed data, was "dig_ass_critic_protos-1.0.7.tar", last modified: Tue May 21 11:29:32 2024, max compression
```

## Comparing `dig_ass_critic_protos-1.0.6.tar` & `dig_ass_critic_protos-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:35.366754 dig_ass_critic_protos-1.0.6/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-1.0.6/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      375 2024-05-20 11:51:35.366754 dig_ass_critic_protos-1.0.6/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-1.0.6/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:35.362754 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2874 2024-05-20 11:51:33.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2610 2024-05-20 11:51:33.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-05-20 11:51:33.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-20 11:50:51.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1761 2024-05-14 12:40:02.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:35.366754 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      375 2024-05-20 11:51:35.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      540 2024-05-20 11:51:35.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-20 11:51:35.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-20 11:51:35.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-20 11:51:35.000000 dig_ass_critic_protos-1.0.6/dig_ass_critic_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-20 11:47:49.000000 dig_ass_critic_protos-1.0.6/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-20 11:51:35.366754 dig_ass_critic_protos-1.0.6/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.6/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 11:29:32.512079 dig_ass_critic_protos-1.0.7/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-1.0.7/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      376 2024-05-21 11:29:32.512079 dig_ass_critic_protos-1.0.7/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-1.0.7/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 11:29:32.512079 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2874 2024-05-21 11:29:31.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2610 2024-05-21 11:29:31.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-05-21 11:29:31.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-21 11:28:08.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1762 2024-05-21 11:12:09.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 11:29:32.512079 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      376 2024-05-21 11:29:32.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      540 2024-05-21 11:29:32.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-21 11:29:32.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       58 2024-05-21 11:29:32.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-21 11:29:32.000000 dig_ass_critic_protos-1.0.7/dig_ass_critic_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       58 2024-05-21 11:15:21.000000 dig_ass_critic_protos-1.0.7/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-21 11:29:32.512079 dig_ass_critic_protos-1.0.7/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.7/setup.py
```

### Comparing `dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py` & `dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi` & `dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py` & `dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.6/dig_ass_critic_protos/client.py` & `dig_ass_critic_protos-1.0.7/dig_ass_critic_protos/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     DigitalAssistantCriticResponse,
     ChatItem,
     OuterContextItem,
     InnerContextItem,
     ReplicaItem,
 )
 
-from agi_med_utils.abstract_client import AbstractClient
+from agi_med_protos.abstract_client import AbstractClient
 
 
 class CriticClient(AbstractClient):
     def __init__(self, address) -> None:
         super().__init__(address)
         self._stub = DigitalAssistantCriticStub(self._channel)
```

### Comparing `dig_ass_critic_protos-1.0.6/dig_ass_critic_protos.egg-info/SOURCES.txt` & `dig_ass_critic_protos-1.0.7/dig_ass_critic_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.6/setup.py` & `dig_ass_critic_protos-1.0.7/setup.py`

 * *Files identical despite different names*

