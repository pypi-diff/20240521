# Comparing `tmp/ovos_solver_hivemind_plugin-0.0.0a5-py3-none-any.whl.zip` & `tmp/ovos_solver_hivemind_plugin-0.0.0a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4222 bytes, number of entries: 8
--rw-r--r--  2.0 unx     2004 b- defN 24-May-21 02:02 ovos_hivemind_solver/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 24-May-21 02:02 ovos_hivemind_solver/version.py
--rw-r--r--  2.0 unx     2633 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       86 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/zip-safe
--rw-rw-r--  2.0 unx      787 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/RECORD
-8 files, 5801 bytes uncompressed, 2802 bytes compressed:  51.7%
+Zip file size: 4607 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3292 b- defN 24-May-21 17:57 ovos_hivemind_solver/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-May-21 17:57 ovos_hivemind_solver/version.py
+-rw-r--r--  2.0 unx     2633 b- defN 24-May-21 17:57 ovos_solver_hivemind_plugin-0.0.0a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 17:57 ovos_solver_hivemind_plugin-0.0.0a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 24-May-21 17:57 ovos_solver_hivemind_plugin-0.0.0a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 24-May-21 17:57 ovos_solver_hivemind_plugin-0.0.0a6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-21 17:57 ovos_solver_hivemind_plugin-0.0.0a6.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      787 b- defN 24-May-21 17:57 ovos_solver_hivemind_plugin-0.0.0a6.dist-info/RECORD
+8 files, 7089 bytes uncompressed, 3187 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_hivemind_solver/__init__.py
 Comment: 
 
 Filename: ovos_hivemind_solver/version.py
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/METADATA
+Filename: ovos_solver_hivemind_plugin-0.0.0a6.dist-info/METADATA
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/WHEEL
+Filename: ovos_solver_hivemind_plugin-0.0.0a6.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/entry_points.txt
+Filename: ovos_solver_hivemind_plugin-0.0.0a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/top_level.txt
+Filename: ovos_solver_hivemind_plugin-0.0.0a6.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/zip-safe
+Filename: ovos_solver_hivemind_plugin-0.0.0a6.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/RECORD
+Filename: ovos_solver_hivemind_plugin-0.0.0a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_hivemind_solver/__init__.py

```diff
@@ -1,58 +1,88 @@
-from hivemind_bus_client import HiveMessageBusClient, HiveMessage, \
-    HiveMessageType
+from hivemind_bus_client import HiveMessageBusClient
 from ovos_bus_client.message import Message
 from ovos_plugin_manager.templates.solvers import QuestionSolver
 from ovos_utils.log import LOG
+from threading import Event
 
 
 class HiveMindSolver(QuestionSolver):
     enable_tx = False
     priority = 70
 
     def __init__(self, config=None):
         config = config or {}
         super().__init__(config)
         self.hm = None
+        self._response = Event()
+        self._responses = []
         if self.config.get("autoconnect"):
             self.connect()
 
     def bind(self, hm: HiveMessageBusClient):
         """if you want to re-use a open connection"""
         self.hm = hm
 
     def connect(self):
         """assume identity set beforehand, eg via `hivemind-client set-identity`
         """
         self.hm = HiveMessageBusClient(useragent="ovos-hivemind-solver")
         self.hm.run_in_thread()
+        self.hm.on_mycroft("speak", self._receive_answer)
+        # NOTE: this message not yet introduced in ovos-core
+        self.hm.on_mycroft("ovos.utterance.handled", self._end_of_response)
+
+        ##############
+        # HACK - waiting for https://github.com/OpenVoiceOS/ovos-core/pull/478
+        # TODO - new bus message in ovos-core
+        #  to unambiguosly identify end of utterance parsing
+        #  currently these are 4 possible outcomes for any request
+        #  does not account for OCP pipeline requests
+        self.hm.on_mycroft("ovos.utterance.cancelled",
+                           self._end_of_response)
+        self.hm.on_mycroft("complete_intent_failure",
+                           self._end_of_response)
+        self.hm.on_mycroft("mycroft.skill.handler.complete",
+                           self._end_of_response)
+        self.hm.on_mycroft( "skill.converse.response",
+                           self._end_of_response)
+
+    def _end_of_response(self, message):
+        if message.type == "skill.converse.response":
+            if not message.data.get("result"):
+                return
+        self._response.set()
+
+    def _receive_answer(self, message):
+        utt = message.data["utterance"]
+        self._responses.append(utt)
 
     # abstract Solver methods
     def get_data(self, query, context=None):
         return {"answer": self.get_spoken_answer(query, context)}
 
-    def get_spoken_answer(self, query, context=None):
+    def get_spoken_answer(self, query, context=None, timeout=10):
         if self.hm is None:
             LOG.error("not connected to HiveMind")
             return
+        self._response.clear()
+        self._responses = []
+
         context = context or {}
         if "session" in context:
             lang = context["session"]["lang"]
         else:
             lang = context.get("lang") or self.config.get("lang", "en-us")
         mycroft_msg = Message("recognizer_loop:utterance",
                               {"utterances": [query], "lang": lang})
-        msg = HiveMessage(HiveMessageType.BUS, mycroft_msg)
-        response = self.hm.wait_for_payload_response(
-            message=msg,
-            reply_type=HiveMessageType.BUS,
-            payload_type="speak",
-            timeout=20)
-        if response:
-            return response.payload.data["utterance"]
+        self.hm.emit_mycroft(mycroft_msg)
+        self._response.wait(timeout=timeout)
+        if self._responses:
+            # merge multiple speak messages into one
+            return "\n".join(self._responses)
         return None  # let next solver attempt
 
 
 if __name__ == "__main__":
     cfg = {
         "autoconnect": True
     }
```

## ovos_hivemind_solver/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 5
+VERSION_ALPHA = 6
 # END_VERSION_BLOCK
```

## Comparing `ovos_solver_hivemind_plugin-0.0.0a5.dist-info/METADATA` & `ovos_solver_hivemind_plugin-0.0.0a6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-solver-hivemind-plugin
-Version: 0.0.0a5
+Version: 0.0.0a6
 Summary: A question solver plugin for OVOS
 Home-page: https://github.com/JarbasHiveMind/ovos-solver-hivemind-plugin
 Author: jarbasai
 Author-email: jarbasai@mailfence.com
 License: MIT
 Keywords: OVOS openvoiceos plugin utterance fallback query
 Platform: UNKNOWN
```

