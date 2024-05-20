# Comparing `tmp/cocorum-1.2.0.tar.gz` & `tmp/cocorum-1.3.1.tar.gz`

## Comparing `cocorum-1.2.0.tar` & `cocorum-1.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-1.2.0/cocorum_icon.png
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-1.2.0/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-1.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    21108 2020-02-02 00:00:00.000000 cocorum-1.2.0/src/cocorum/__init__.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-1.2.0/src/cocorum/localvars.py
--rw-r--r--   0        0        0    13245 2020-02-02 00:00:00.000000 cocorum-1.2.0/src/cocorum/ssechat.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 cocorum-1.2.0/src/cocorum/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 cocorum-1.2.0/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 cocorum-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 cocorum-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-1.3.1/cocorum_icon.png
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-1.3.1/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    21108 2020-02-02 00:00:00.000000 cocorum-1.3.1/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-1.3.1/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    13591 2020-02-02 00:00:00.000000 cocorum-1.3.1/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 cocorum-1.3.1/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cocorum-1.3.1/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 cocorum-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 cocorum-1.3.1/PKG-INFO
```

### Comparing `cocorum-1.2.0/cocorum_icon.png` & `cocorum-1.3.1/cocorum_icon.png`

 * *Files identical despite different names*

### Comparing `cocorum-1.2.0/.github/workflows/python-publish.yml` & `cocorum-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-1.2.0/src/cocorum/__init__.py` & `cocorum-1.3.1/src/cocorum/__init__.py`

 * *Files identical despite different names*

### Comparing `cocorum-1.2.0/src/cocorum/localvars.py` & `cocorum-1.3.1/src/cocorum/localvars.py`

 * *Files identical despite different names*

### Comparing `cocorum-1.2.0/src/cocorum/ssechat.py` & `cocorum-1.3.1/src/cocorum/ssechat.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,15 @@
 class SSEChat():
     """Access the Rumble SSE chat api"""
     def __init__(self, stream_id):
         self.stream_id = utils.stream_id_ensure_b36(stream_id)
 
         self.__mailbox = [] #A mailbox if you will
         self.deleted_message_ids = [] #IDs of messages that were deleted, as reported by the client
+        self.pinned_message = None #If a message is pinned, it is assigned to this
         self.users = {} #Dictionary of users by user ID
         self.channels = {} #Dictionary of channels by channel ID
         self.badges = {}
 
         #Connect to the API
         self.url = SSE_CHAT_URL.format(stream_id_b10 = self.stream_id_b10)
         self.client = sseclient.SSEClient(self.url)
@@ -264,20 +265,24 @@
         self.parse_init_data(self.next_jsondata())
 
     def next_jsondata(self):
         """Wait for the next message from the SSE and parse the JSON"""
         if not self.chat_running: #Do not try to query a new message if chat is closed
             return
 
-        message = next(self.client, None)
+        try:
+            message = next(self.client, None)
+        except requests.exceptions.ReadTimeout:
+            message = None
+
         if not message:
             self.chat_running = False #Chat has been closed
             return
         if not message.data: #Blank SSE event
-            print("Blank SSE event:", message)
+            print("Blank SSE event:>", message, "<:")
             #Self recursion should work so long as we don't get dozens of blank events in a row
             return self.next_jsondata()
 
         return json.loads(message.data)
 
     def parse_init_data(self, jsondata):
         """Extract initial chat data from the SSE init message JSON"""
@@ -352,14 +357,18 @@
             if jsondata["type"] in ("delete_messages", "delete_non_rant_messages"):
                 self.deleted_message_ids += jsondata["data"]["message_ids"]
 
             #Re-initialize (could contain new messages)
             elif jsondata["type"] == "init":
                 self.parse_init_data(jsondata)
 
+            #Pinned message
+            elif jsondata["type"] == "pin_message":
+                self.pinned_message = SSEChatMessage(jsondata["data"]["message"])
+
             #New messages
             elif jsondata["type"] == "messages":
                 #Parse messages, users, and channels
                 self.update_mailbox(jsondata)
                 self.update_users(jsondata)
                 self.update_channels(jsondata)
```

### Comparing `cocorum-1.2.0/src/cocorum/utils.py` & `cocorum-1.3.1/src/cocorum/utils.py`

 * *Files identical despite different names*

### Comparing `cocorum-1.2.0/LICENSE.txt` & `cocorum-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-1.2.0/README.md` & `cocorum-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 Most attributes that are not added features have the same name as the direct JSON counterparts, with the exception of adding prefixes to some things that have the same name in the JSON as Python builtin functions. For example, thing/id in JSON is thing.thing_id in this Python wrapper.
 
 ```
 from cocorum import RumbleAPI
 from cocorum.localvars import *
 
+#API_URL is either your Rumble Live Stream API URL with key,
+#or if you are also running GlobalGamer2015's RumBot, use http://localhost:9843/api/ls
+#to use RumBot's API passthrough and reduce unnecessary API traffic.
 api = RumbleAPI(API_URL, refresh_rate = 10)
 
 print(api.username)
 print(api.latest_follower)
 
 if api.latest_subscriber:
     print(api.latest_subscriber, "subscribed for $" + str(api.latest_subscriber.amount_dollars))
```

### Comparing `cocorum-1.2.0/pyproject.toml` & `cocorum-1.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "1.2.0"
+version = "1.3.1"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cocorum-1.2.0/PKG-INFO` & `cocorum-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 1.2.0
+Version: 1.3.1
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
@@ -28,14 +28,17 @@
 
 Most attributes that are not added features have the same name as the direct JSON counterparts, with the exception of adding prefixes to some things that have the same name in the JSON as Python builtin functions. For example, thing/id in JSON is thing.thing_id in this Python wrapper.
 
 ```
 from cocorum import RumbleAPI
 from cocorum.localvars import *
 
+#API_URL is either your Rumble Live Stream API URL with key,
+#or if you are also running GlobalGamer2015's RumBot, use http://localhost:9843/api/ls
+#to use RumBot's API passthrough and reduce unnecessary API traffic.
 api = RumbleAPI(API_URL, refresh_rate = 10)
 
 print(api.username)
 print(api.latest_follower)
 
 if api.latest_subscriber:
     print(api.latest_subscriber, "subscribed for $" + str(api.latest_subscriber.amount_dollars))
```

