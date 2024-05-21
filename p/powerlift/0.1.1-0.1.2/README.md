# Comparing `tmp/powerlift-0.1.1-py3-none-any.whl.zip` & `tmp/powerlift-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 27878 bytes, number of entries: 20
+Zip file size: 27930 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      712 b- defN 24-May-17 18:23 powerlift/bench/__init__.py
 -rw-r--r--  2.0 unx     6431 b- defN 24-May-12 23:47 powerlift/bench/benchmark.py
 -rw-r--r--  2.0 unx     5888 b- defN 24-May-10 19:49 powerlift/bench/experiment.py
--rw-r--r--  2.0 unx    36279 b- defN 24-May-20 19:08 powerlift/bench/store.py
+-rw-r--r--  2.0 unx    36619 b- defN 24-May-20 21:19 powerlift/bench/store.py
 -rw-r--r--  2.0 unx      856 b- defN 24-May-07 19:14 powerlift/db/__init__.py
 -rw-r--r--  2.0 unx     1364 b- defN 24-May-10 18:52 powerlift/db/actions.py
 -rw-r--r--  2.0 unx     6971 b- defN 24-May-10 18:52 powerlift/db/schema.py
 -rw-r--r--  2.0 unx      233 b- defN 24-May-07 19:14 powerlift/executors/__init__.py
 -rw-r--r--  2.0 unx     7639 b- defN 24-May-07 19:14 powerlift/executors/azure_ci.py
 -rw-r--r--  2.0 unx     2275 b- defN 24-May-07 19:14 powerlift/executors/base.py
 -rw-r--r--  2.0 unx     3041 b- defN 24-May-07 19:14 powerlift/executors/docker.py
 -rw-r--r--  2.0 unx     3069 b- defN 24-May-14 00:02 powerlift/executors/localmachine.py
 -rw-r--r--  2.0 unx      136 b- defN 24-May-07 19:14 powerlift/measures/__init__.py
 -rw-r--r--  2.0 unx     4500 b- defN 24-May-07 19:14 powerlift/measures/task_measures.py
 -rw-r--r--  2.0 unx     2639 b- defN 24-May-14 00:03 powerlift/run/__main__.py
--rw-r--r--  2.0 unx     1085 b- defN 24-May-20 20:20 powerlift-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5740 b- defN 24-May-20 20:20 powerlift-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-20 20:20 powerlift-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-20 20:20 powerlift-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1668 b- defN 24-May-20 20:20 powerlift-0.1.1.dist-info/RECORD
-20 files, 90628 bytes uncompressed, 25158 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx     1085 b- defN 24-May-20 22:21 powerlift-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5740 b- defN 24-May-20 22:21 powerlift-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 22:21 powerlift-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-20 22:21 powerlift-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1668 b- defN 24-May-20 22:21 powerlift-0.1.2.dist-info/RECORD
+20 files, 90968 bytes uncompressed, 25210 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: powerlift/measures/task_measures.py
 Comment: 
 
 Filename: powerlift/run/__main__.py
 Comment: 
 
-Filename: powerlift-0.1.1.dist-info/LICENSE
+Filename: powerlift-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: powerlift-0.1.1.dist-info/METADATA
+Filename: powerlift-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: powerlift-0.1.1.dist-info/WHEEL
+Filename: powerlift-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: powerlift-0.1.1.dist-info/top_level.txt
+Filename: powerlift-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: powerlift-0.1.1.dist-info/RECORD
+Filename: powerlift-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## powerlift/bench/store.py

```diff
@@ -108,18 +108,28 @@
         import pandas as pd
         from types import FunctionType
         import inspect
 
         bstream = io.BytesIO()
         mimetype = None
         if isinstance(obj, pd.Series):
-            obj.astype(dtype=object).to_frame(name="Target").to_parquet(bstream)
+            orig_close = bstream.close
+            bstream.close = lambda: None
+            try:
+                obj.astype(dtype=object).to_frame(name="Target").to_parquet(bstream)
+            finally:
+                bstream.close = orig_close
             mimetype = MIMETYPE_SERIES
         elif isinstance(obj, pd.DataFrame):
-            obj.to_parquet(bstream)
+            orig_close = bstream.close
+            bstream.close = lambda: None
+            try:
+                obj.to_parquet(bstream)
+            finally:
+                bstream.close = orig_close
             mimetype = MIMETYPE_DF
         elif isinstance(obj, dict):
             bstream.write(json.dumps(obj).encode())
             mimetype = MIMETYPE_JSON
         elif isinstance(obj, FunctionType):
             src = inspect.getsource(obj)
             src_ast = _parse_function(src)
@@ -133,14 +143,16 @@
                 "name": obj.name,
                 "content": content,
             }
             bstream.write(json.dumps(json_record).encode())
             mimetype = MIMETYPE_WHEEL
         else:
             return None, None
+        
+
         return mimetype, bstream
 
 
 class Store:
     """Store that represents persistent state for experiments.
 
     Apart from initialization, the user should not be using its methods normally.
```

## Comparing `powerlift-0.1.1.dist-info/LICENSE` & `powerlift-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `powerlift-0.1.1.dist-info/METADATA` & `powerlift-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerlift
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interactive Benchmarking for Machine Learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Project-URL: Bug Tracker, https://github.com/interpretml/interpret/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `powerlift-0.1.1.dist-info/RECORD` & `powerlift-0.1.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 powerlift/bench/__init__.py,sha256=HqW1l4O5fLWgPdfdCxQCYGYhDOPNiUhAMEyIKvjHEFo,712
 powerlift/bench/benchmark.py,sha256=QHNyfwsOCAac9pXrXSq2O3GI2VB20Rs6i3_3DDH240I,6431
 powerlift/bench/experiment.py,sha256=LCjzoJVSBa96XvFbwYvk1obMbKJHal2NU4fzL0r64PI,5888
-powerlift/bench/store.py,sha256=hhQumyqY9KSO8cmoXuFFc7wFeuZf2SYJyN8RE1AC5ec,36279
+powerlift/bench/store.py,sha256=E5c5DqmZ2jlb-2VsQ9G9M-knDZ_kaimYj3GR1QQFkwo,36619
 powerlift/db/__init__.py,sha256=f0S6DsKHCEB8iZ6cVh7MX-1kl4KHtgVsmJcbtfEknEU,856
 powerlift/db/actions.py,sha256=qc9NxS9TLNfx9qYaPlpS4KpJhuGfSoKe3andHYJI32g,1364
 powerlift/db/schema.py,sha256=T1pCXaiLew_04Oadpg5IE6aYmwRokh-kU5m68lutMKI,6971
 powerlift/executors/__init__.py,sha256=Xxy4Qzjfe-hFY1ZarMYBEjH076CKHuHOTxqszoPYvuw,233
 powerlift/executors/azure_ci.py,sha256=hpjuyDlNFBFHwqiaVR6ZzHn7upN0NI7xJUHkJiFJN3A,7639
 powerlift/executors/base.py,sha256=Blhm0ZiF6u0_wqw8NjYKmF70fdkZsyL61zX5DfBdZoY,2275
 powerlift/executors/docker.py,sha256=1g-hphvh-g5-QuG_xyo7bhBp0SMdYIzY8EHz0D27Ixc,3041
 powerlift/executors/localmachine.py,sha256=8dYImIq5cQPVk0H4B_AiPpVGZKIhdbB05s46f717TOA,3069
 powerlift/measures/__init__.py,sha256=br7A9iJgQl7cPcPFnnJkRGEDRn_IBJMj24rVZFaSF44,136
 powerlift/measures/task_measures.py,sha256=23zwd25L_KB9Xe6LuWtBS4QBuv1F0mKnCR4HAKjsmg0,4500
 powerlift/run/__main__.py,sha256=YbXDeF33dehQgEEEFfuCctGlr2dTmNNhKjCibEg-EuE,2639
-powerlift-0.1.1.dist-info/LICENSE,sha256=7vlTCQ2WSK8wDjuX9Rv36FpE_bEP1FkMVxceVw-VTGs,1085
-powerlift-0.1.1.dist-info/METADATA,sha256=TTQeBg6P90KVXAirIukD_SuMmxXqFomozzGP7MqpQUU,5740
-powerlift-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-powerlift-0.1.1.dist-info/top_level.txt,sha256=PqZeILUPLCstbaDfaAG14A4rCLPYynR_EKCJjGGW88s,10
-powerlift-0.1.1.dist-info/RECORD,,
+powerlift-0.1.2.dist-info/LICENSE,sha256=7vlTCQ2WSK8wDjuX9Rv36FpE_bEP1FkMVxceVw-VTGs,1085
+powerlift-0.1.2.dist-info/METADATA,sha256=gEnReL7Ymye7W09Gm84gZvcsBBazVU3S6zYD5L32laM,5740
+powerlift-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+powerlift-0.1.2.dist-info/top_level.txt,sha256=PqZeILUPLCstbaDfaAG14A4rCLPYynR_EKCJjGGW88s,10
+powerlift-0.1.2.dist-info/RECORD,,
```

