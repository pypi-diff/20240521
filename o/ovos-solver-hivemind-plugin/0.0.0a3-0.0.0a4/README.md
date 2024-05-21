# Comparing `tmp/ovos_solver_hivemind_plugin-0.0.0a3-py3-none-any.whl.zip` & `tmp/ovos_solver_hivemind_plugin-0.0.0a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4156 bytes, number of entries: 8
--rw-r--r--  2.0 unx     2004 b- defN 24-May-20 20:51 ovos_hivemind_solver/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 24-May-20 20:51 ovos_hivemind_solver/version.py
--rw-r--r--  2.0 unx     2419 b- defN 24-May-20 20:51 ovos_solver_hivemind_plugin-0.0.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-20 20:51 ovos_solver_hivemind_plugin-0.0.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       86 b- defN 24-May-20 20:51 ovos_solver_hivemind_plugin-0.0.0a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 24-May-20 20:51 ovos_solver_hivemind_plugin-0.0.0a3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-20 20:51 ovos_solver_hivemind_plugin-0.0.0a3.dist-info/zip-safe
--rw-rw-r--  2.0 unx      787 b- defN 24-May-20 20:51 ovos_solver_hivemind_plugin-0.0.0a3.dist-info/RECORD
-8 files, 5587 bytes uncompressed, 2736 bytes compressed:  51.0%
+Zip file size: 4149 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     2004 b- defN 24-May-21 01:10 ovos_hivemind_solver/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-May-21 01:10 ovos_hivemind_solver/version.py
+-rw-r--r--  2.0 unx     2451 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      787 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/RECORD
+8 files, 5619 bytes uncompressed, 2729 bytes compressed:  51.4%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_hivemind_solver/__init__.py
 Comment: 
 
 Filename: ovos_hivemind_solver/version.py
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a3.dist-info/METADATA
+Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/METADATA
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a3.dist-info/WHEEL
+Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a3.dist-info/entry_points.txt
+Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a3.dist-info/top_level.txt
+Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a3.dist-info/zip-safe
+Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a3.dist-info/RECORD
+Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_hivemind_solver/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 3
+VERSION_ALPHA = 4
 # END_VERSION_BLOCK
```

## Comparing `ovos_solver_hivemind_plugin-0.0.0a3.dist-info/METADATA` & `ovos_solver_hivemind_plugin-0.0.0a4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-solver-hivemind-plugin
-Version: 0.0.0a3
+Version: 0.0.0a4
 Summary: A question solver plugin for OVOS
 Home-page: https://github.com/JarbasHiveMind/ovos-solver-hivemind-plugin
 Author: jarbasai
 Author-email: jarbasai@mailfence.com
 License: MIT
 Keywords: OVOS openvoiceos plugin utterance fallback query
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Requires-Dist: hivemind-bus-client >=0.0.4a21
 
 # HiveMind solver
 
 exposes a hivemind connection as a solver plugin
 
 use cases:
-- allow your OVOS device to get responses from HiveMind, via dedicated skill or pipeline (TODO - companion integrations)
+- allow your OVOS device to get responses from a remote HiveMind, via [companion skill](https://github.com/JarbasHiveMind/ovos-skill-fallback-hivemind)
 - expose HiveMind to any OpenAI compatible UI, via [ovos-persona-server](https://github.com/OpenVoiceOS/ovos-persona-server)
 - Integrate HiveMind/OVOS into a [MOS (Mixture Of Solvers)](https://github.com/TigreGotico/ovos-MoS)
 
 ## Setup
 
 You need to register the solver in the HiveMind server
 ```bash
@@ -70,7 +70,8 @@
 from ovos_hivemind_solver import HiveMindSolver
 
 bot = HiveMindSolver()
 bot.connect()  # connection info from identity file
 print(bot.spoken_answer("what is the speed of light?"))
 ```
 
+
```

