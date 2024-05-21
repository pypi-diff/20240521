# Comparing `tmp/cirq-1.4.0.dev20240518010119-py3-none-any.whl.zip` & `tmp/cirq-1.4.0.dev20240521175101-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 8320 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 24-May-18 01:01 cirq-1.4.0.dev20240518010119.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 24-May-18 01:01 cirq-1.4.0.dev20240518010119.dist-info/LICENSE
--rw-r--r--  2.0 unx     7712 b- defN 24-May-18 01:01 cirq-1.4.0.dev20240518010119.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-18 01:01 cirq-1.4.0.dev20240518010119.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-18 01:01 cirq-1.4.0.dev20240518010119.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 24-May-18 01:01 cirq-1.4.0.dev20240518010119.dist-info/RECORD
+-rw-r--r--  2.0 unx      292 b- defN 24-May-21 17:51 cirq-1.4.0.dev20240521175101.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-21 17:51 cirq-1.4.0.dev20240521175101.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7712 b- defN 24-May-21 17:51 cirq-1.4.0.dev20240521175101.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 17:51 cirq-1.4.0.dev20240521175101.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-21 17:51 cirq-1.4.0.dev20240521175101.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 24-May-21 17:51 cirq-1.4.0.dev20240521175101.dist-info/RECORD
 6 files, 20017 bytes uncompressed, 7282 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.4.0.dev20240518010119.dist-info/AUTHORS
+Filename: cirq-1.4.0.dev20240521175101.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.4.0.dev20240518010119.dist-info/LICENSE
+Filename: cirq-1.4.0.dev20240521175101.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.4.0.dev20240518010119.dist-info/METADATA
+Filename: cirq-1.4.0.dev20240521175101.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.4.0.dev20240518010119.dist-info/WHEEL
+Filename: cirq-1.4.0.dev20240521175101.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.4.0.dev20240518010119.dist-info/top_level.txt
+Filename: cirq-1.4.0.dev20240521175101.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.4.0.dev20240518010119.dist-info/RECORD
+Filename: cirq-1.4.0.dev20240521175101.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.4.0.dev20240518010119.dist-info/LICENSE` & `cirq-1.4.0.dev20240521175101.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.4.0.dev20240518010119.dist-info/METADATA` & `cirq-1.4.0.dev20240521175101.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.4.0.dev20240518010119
+Version: 1.4.0.dev20240521175101
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Requires-Python: >=3.10.0
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: cirq-aqt ==1.4.0.dev20240518010119
-Requires-Dist: cirq-core ==1.4.0.dev20240518010119
-Requires-Dist: cirq-google ==1.4.0.dev20240518010119
-Requires-Dist: cirq-ionq ==1.4.0.dev20240518010119
-Requires-Dist: cirq-pasqal ==1.4.0.dev20240518010119
-Requires-Dist: cirq-rigetti ==1.4.0.dev20240518010119
-Requires-Dist: cirq-web ==1.4.0.dev20240518010119
+Requires-Dist: cirq-aqt ==1.4.0.dev20240521175101
+Requires-Dist: cirq-core ==1.4.0.dev20240521175101
+Requires-Dist: cirq-google ==1.4.0.dev20240521175101
+Requires-Dist: cirq-ionq ==1.4.0.dev20240521175101
+Requires-Dist: cirq-pasqal ==1.4.0.dev20240521175101
+Requires-Dist: cirq-rigetti ==1.4.0.dev20240521175101
+Requires-Dist: cirq-web ==1.4.0.dev20240521175101
 Provides-Extra: dev_env
 Requires-Dist: mypy ==1.2.0 ; extra == 'dev_env'
 Requires-Dist: types-backports ==0.1.3 ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf ~=3.20 ; extra == 'dev_env'
 Requires-Dist: types-requests ==2.28.1 ; extra == 'dev_env'
 Requires-Dist: types-setuptools ==62.6.1 ; extra == 'dev_env'
```

