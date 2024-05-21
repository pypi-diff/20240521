# Comparing `tmp/ovos_solver_hivemind_plugin-0.0.0a4-py3-none-any.whl.zip` & `tmp/ovos_solver_hivemind_plugin-0.0.0a5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4149 bytes, number of entries: 8
--rw-r--r--  2.0 unx     2004 b- defN 24-May-21 01:10 ovos_hivemind_solver/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 24-May-21 01:10 ovos_hivemind_solver/version.py
--rw-r--r--  2.0 unx     2451 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/WHEEL
--rw-r--r--  2.0 unx       86 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/zip-safe
--rw-rw-r--  2.0 unx      787 b- defN 24-May-21 01:10 ovos_solver_hivemind_plugin-0.0.0a4.dist-info/RECORD
-8 files, 5619 bytes uncompressed, 2729 bytes compressed:  51.4%
+Zip file size: 4222 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     2004 b- defN 24-May-21 02:02 ovos_hivemind_solver/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-May-21 02:02 ovos_hivemind_solver/version.py
+-rw-r--r--  2.0 unx     2633 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      787 b- defN 24-May-21 02:02 ovos_solver_hivemind_plugin-0.0.0a5.dist-info/RECORD
+8 files, 5801 bytes uncompressed, 2802 bytes compressed:  51.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_hivemind_solver/__init__.py
 Comment: 
 
 Filename: ovos_hivemind_solver/version.py
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/METADATA
+Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/METADATA
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/WHEEL
+Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/entry_points.txt
+Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/top_level.txt
+Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/zip-safe
+Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a4.dist-info/RECORD
+Filename: ovos_solver_hivemind_plugin-0.0.0a5.dist-info/RECORD
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
-VERSION_ALPHA = 4
+VERSION_ALPHA = 5
 # END_VERSION_BLOCK
```

## Comparing `ovos_solver_hivemind_plugin-0.0.0a4.dist-info/METADATA` & `ovos_solver_hivemind_plugin-0.0.0a5.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-solver-hivemind-plugin
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: A question solver plugin for OVOS
 Home-page: https://github.com/JarbasHiveMind/ovos-solver-hivemind-plugin
 Author: jarbasai
 Author-email: jarbasai@mailfence.com
 License: MIT
 Keywords: OVOS openvoiceos plugin utterance fallback query
 Platform: UNKNOWN
@@ -18,14 +18,18 @@
 exposes a hivemind connection as a solver plugin
 
 use cases:
 - allow your OVOS device to get responses from a remote HiveMind, via [companion skill](https://github.com/JarbasHiveMind/ovos-skill-fallback-hivemind)
 - expose HiveMind to any OpenAI compatible UI, via [ovos-persona-server](https://github.com/OpenVoiceOS/ovos-persona-server)
 - Integrate HiveMind/OVOS into a [MOS (Mixture Of Solvers)](https://github.com/TigreGotico/ovos-MoS)
 
+## Install
+
+`pip install ovos-solver-hivemind-plugin`
+
 ## Setup
 
 You need to register the solver in the HiveMind server
 ```bash
 $ hivemind-core add-client
 Credentials added to database!
 
@@ -62,14 +66,18 @@
 2024-05-20 21:22:28.003 - OVOS - hivemind_bus_client.client:__init__:112 - INFO - Session ID: 34d75c93-4e65-4ea9-b5f4-87169dcfda01
 (...)
 == Identity successfully connected to HiveMind!
 ```
 
 ## Usage
 
+For usage with any solver framework, such as persona, use `"ovos-solver-hivemind-plugin"` for the solver id
+
+Standalone usage
+
 ```python
 from ovos_hivemind_solver import HiveMindSolver
 
 bot = HiveMindSolver()
 bot.connect()  # connection info from identity file
 print(bot.spoken_answer("what is the speed of light?"))
 ```
```

## Comparing `ovos_solver_hivemind_plugin-0.0.0a4.dist-info/RECORD` & `ovos_solver_hivemind_plugin-0.0.0a5.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 ovos_hivemind_solver/__init__.py,sha256=U1Z1qAmkgYCCL1J7MzQqwr5J-elJqM044u1--oQMY68,2004
-ovos_hivemind_solver/version.py,sha256=JN7aD_TugTLEaBIwM5kbDnKdd-QQQx3WIIaO6M_RM2s,177
-ovos_solver_hivemind_plugin-0.0.0a4.dist-info/METADATA,sha256=J_LHzF2IYCj3z0it-KkNVw7r5b4ICdjWz-nZGCBQfaU,2451
-ovos_solver_hivemind_plugin-0.0.0a4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ovos_solver_hivemind_plugin-0.0.0a4.dist-info/entry_points.txt,sha256=JVeOkEId-_bpe2JqMZKWvEKGxlSthx0UHAqGCCF1Wf8,86
-ovos_solver_hivemind_plugin-0.0.0a4.dist-info/top_level.txt,sha256=14OLHqYSDQpRdotikZA0s3orZiUR-YKWXjKjPx77dFY,21
-ovos_solver_hivemind_plugin-0.0.0a4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_solver_hivemind_plugin-0.0.0a4.dist-info/RECORD,,
+ovos_hivemind_solver/version.py,sha256=hDOolhK88hLPyvV5m7E3osBHrG_NBU03rdk3-5YAKCA,177
+ovos_solver_hivemind_plugin-0.0.0a5.dist-info/METADATA,sha256=EtUhh1aZ9DU2-Utv6ahgj1yJdakNKLn-lCOqv__pVRI,2633
+ovos_solver_hivemind_plugin-0.0.0a5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ovos_solver_hivemind_plugin-0.0.0a5.dist-info/entry_points.txt,sha256=JVeOkEId-_bpe2JqMZKWvEKGxlSthx0UHAqGCCF1Wf8,86
+ovos_solver_hivemind_plugin-0.0.0a5.dist-info/top_level.txt,sha256=14OLHqYSDQpRdotikZA0s3orZiUR-YKWXjKjPx77dFY,21
+ovos_solver_hivemind_plugin-0.0.0a5.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_solver_hivemind_plugin-0.0.0a5.dist-info/RECORD,,
```

