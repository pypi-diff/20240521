# Comparing `tmp/autogencap_rajan_jedi-0.0.7.tar.gz` & `tmp/autogencap_rajan_jedi-0.0.8.tar.gz`

## Comparing `autogencap_rajan_jedi-0.0.7.tar` & `autogencap_rajan_jedi-0.0.8.tar`

### file list

```diff
@@ -1,38 +1,36 @@
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/Actor.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ActorConnector.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/Broker.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/Config.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/Constants.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/DebugLog.py
--rw-r--r--   0        0        0     8917 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/DirectorySvc.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/LocalActorNetwork.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/requirements.txt
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/setup.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/utility.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AG2CAP.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AGActor.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AutoGenConnector.py
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAP2AG.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPGroupChat.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPGroupChatManager.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPPair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/agent.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen.proto
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen_pb2.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen_pb2.pyi
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP.proto
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAPAgents_pb2.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAPAgents_pb2.pyi
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP_pb2.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP_pb2.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/proto-instructions.txt
--rwxr-xr-x   0        0        0 11783121 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/protoc.exe
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/test.seqdiag
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/.gitignore
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/README.md
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/Actor.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ActorConnector.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/Broker.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/Config.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/Constants.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/DebugLog.py
+-rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/DirectorySvc.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/LocalActorNetwork.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/requirements.txt
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/setup.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/utility.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AG2CAP.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AGActor.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AutoGenConnector.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAP2AG.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPGroupChat.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPGroupChatManager.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPPair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/agent.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen.proto
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen_pb2.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen_pb2.pyi
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP.proto
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP_pb2.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP_pb2.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/proto-instructions.txt
+-rwxr-xr-x   0        0        0 11783121 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/protoc.exe
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/test.seqdiag
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/README.md
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/PKG-INFO
```

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/Actor.py` & `autogencap_rajan_jedi-0.0.8/autogencap/Actor.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/ActorConnector.py` & `autogencap_rajan_jedi-0.0.8/autogencap/ActorConnector.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,9 +144,9 @@
             if num_attempts == -1:
                 self._resp_socket.setsockopt(zmq.RCVTIMEO, original_timeout)
 
         Error("ActorConnector", f"{self._topic}: No response received. Giving up.")
         return None, None, None
 
     def close(self):
-        self._pub_socket.close()
+        self._sender.close()
         self._resp_socket.close()
```

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/Broker.py` & `autogencap_rajan_jedi-0.0.8/autogencap/Broker.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/DebugLog.py` & `autogencap_rajan_jedi-0.0.8/autogencap/DebugLog.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 class ConsoleLogger(BaseLogger):
     def __init__(self):
         super().__init__()
 
     def WriteLog(self, level, context, msg):
-        timestamp = colored(datetime.datetime.now().strftime("%m/%d/%y %H:%M:%S"), "pink")
+        timestamp = colored(datetime.datetime.now().strftime("%m/%d/%y %H:%M:%S"), "dark_grey")
         # Translate level number to name and color
         level_name = colored(LEVEL_NAMES[level], LEVEL_COLOR[level])
         # Left justify the context and color it blue
         context = colored(context.ljust(14), "blue")
         # Left justify the threadid and color it blue
         thread_id = colored(str(threading.get_ident()).ljust(5), "blue")
         # color the msg based on the level
```

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/DirectorySvc.py` & `autogencap_rajan_jedi-0.0.8/autogencap/DirectorySvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self._directory_connector: ActorConnector = None
         self._directory_actor: DirectoryActor = None
 
     def _no_other_directory(self) -> bool:
         Debug("DirectorySvc", "Pinging existing DirectorySvc")
         ping = Ping()
         serialized_msg = ping.SerializeToString()
-        _, _, resp = self._directory_connector.binary_request(Ping.__name__, serialized_msg, retry=1)
+        _, _, resp = self._directory_connector.binary_request(Ping.__name__, serialized_msg, num_attempts=1)
         if resp is None:
             return True
         return False
 
     def start(self):
         Debug("DirectorySvc", "Starting.")
         self._directory_connector = ActorConnector(self._context, Directory_Svc_Topic)
```

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/LocalActorNetwork.py` & `autogencap_rajan_jedi-0.0.8/autogencap/LocalActorNetwork.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/test.py` & `autogencap_rajan_jedi-0.0.8/autogencap/test.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AG2CAP.py` & `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AG2CAP.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AutoGenConnector.py` & `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AutoGenConnector.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAP2AG.py` & `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAP2AG.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPGroupChat.py` & `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPGroupChat.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPGroupChatManager.py` & `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPGroupChatManager.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPPair.py` & `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPPair.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/agent.py` & `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/agent.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen.proto` & `autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen.proto`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen_pb2.py` & `autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen_pb2.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen_pb2.pyi` & `autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen_pb2.pyi`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP.proto` & `autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP.proto`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP_pb2.py` & `autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP_pb2.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP_pb2.pyi` & `autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP_pb2.pyi`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/autogencap/proto/protoc.exe` & `autogencap_rajan_jedi-0.0.8/autogencap/proto/protoc.exe`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/.gitignore` & `autogencap_rajan_jedi-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/README.md` & `autogencap_rajan_jedi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.7/pyproject.toml` & `autogencap_rajan_jedi-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autogencap_rajan.jedi"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Rajan Chari", email="rajan.jedi@gmail.com" },
 ]
 dependencies = [
     "pyzmq >= 25.1.2",
     "protobuf >= 4.25.3",
     "termcolor >= 2.4.0",
```

### Comparing `autogencap_rajan_jedi-0.0.7/PKG-INFO` & `autogencap_rajan_jedi-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autogencap_rajan.jedi
-Version: 0.0.7
+Version: 0.0.8
 Summary: CAP w/ autogen bindings
 Project-URL: Homepage, https://github.com/microsoft/autogen
 Project-URL: Bug Tracker, https://github.com/microsoft/autogen/issues
 Author-email: Rajan Chari <rajan.jedi@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

