# Comparing `tmp/udata_metrics-2.0.3.dev25-py2.py3-none-any.whl.zip` & `tmp/udata_metrics-2.0.3.dev27-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3407 bytes, number of entries: 9
--rw-r--r--  2.0 unx      248 b- defN 20-Apr-14 13:03 udata_metrics/__init__.py
--rw-r--r--  2.0 unx     1461 b- defN 20-Apr-14 13:03 udata_metrics/client.py
--rw-r--r--  2.0 unx        0 b- defN 20-Apr-14 13:03 udata_metrics/models.py
--rw-r--r--  2.0 unx      551 b- defN 20-Apr-14 13:03 udata_metrics/tasks.py
--rw-r--r--  2.0 unx     1430 b- defN 20-Apr-14 13:04 udata_metrics-2.0.3.dev25.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-Apr-14 13:04 udata_metrics-2.0.3.dev25.dist-info/WHEEL
--rw-r--r--  2.0 unx      133 b- defN 20-Apr-14 13:04 udata_metrics-2.0.3.dev25.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 20-Apr-14 13:04 udata_metrics-2.0.3.dev25.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      771 b- defN 20-Apr-14 13:04 udata_metrics-2.0.3.dev25.dist-info/RECORD
-9 files, 4718 bytes uncompressed, 2059 bytes compressed:  56.4%
+Zip file size: 3486 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      248 b- defN 20-Apr-15 14:10 udata_metrics/__init__.py
+-rw-r--r--  2.0 unx     2140 b- defN 20-Apr-15 14:10 udata_metrics/client.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Apr-15 14:10 udata_metrics/models.py
+-rw-r--r--  2.0 unx      551 b- defN 20-Apr-15 14:10 udata_metrics/tasks.py
+-rw-r--r--  2.0 unx     1430 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/WHEEL
+-rw-r--r--  2.0 unx      133 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      771 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/RECORD
+9 files, 5397 bytes uncompressed, 2138 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: udata_metrics/models.py
 Comment: 
 
 Filename: udata_metrics/tasks.py
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev25.dist-info/METADATA
+Filename: udata_metrics-2.0.3.dev27.dist-info/METADATA
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev25.dist-info/WHEEL
+Filename: udata_metrics-2.0.3.dev27.dist-info/WHEEL
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev25.dist-info/entry_points.txt
+Filename: udata_metrics-2.0.3.dev27.dist-info/entry_points.txt
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev25.dist-info/top_level.txt
+Filename: udata_metrics-2.0.3.dev27.dist-info/top_level.txt
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev25.dist-info/RECORD
+Filename: udata_metrics-2.0.3.dev27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## udata_metrics/client.py

```diff
@@ -9,15 +9,20 @@
 
     def get_views_from_all_datasets(self):
         query = 'select sum(*) from dataset_views group by dataset;'
         result = self.client.query(query)
         return result
     
     def get_views_from_all_resources(self):
-        query = 'select sum(*) from resource_views group by dataset;'
+        query = 'select sum(*) from resource_views group by resource;'
+        result = self.client.query(query)
+        return result
+    
+    def get_views_from_all_community_resources(self):
+        query = 'select sum(*) from community_resource_views group by communityresource;'
         result = self.client.query(query)
         return result
     
     def get_views_from_all_reuses(self):
         query = 'select sum(*) from reuse_views group by reuse;'
         result = self.client.query(query)
         return result
@@ -32,14 +37,24 @@
         result = self.client.query(query)
         return result
     
     def get_views_from_specific_model(self, model_name, model_id):
         query = f"select * from {model_name}_views where {model_name}='{model_id}';"
         result = self.client.query(query)
         return result
+    
+    def sum_views_from_specific_ressources(self, resource_id):
+        query = f"select sum(*) from resource_views where resource='{resource_id}';"
+        result = self.client.query(query)
+        return result
+    
+    def sum_views_from_specific_com_ressources(self, com_resource_id):
+        query = f"select sum(*) from community_resource_views where communityresource='{com_resource_id}';"
+        result = self.client.query(query)
+        return result
 
     def insert(self, body):
         self.client.write_points([body])
 
 
 def metrics_client_factory():
     dsn = current_app.config['METRICS_DSN']
```

## Comparing `udata_metrics-2.0.3.dev25.dist-info/METADATA` & `udata_metrics-2.0.3.dev27.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udata-metrics
-Version: 2.0.3.dev25
+Version: 2.0.3.dev27
 Summary: Open data portal
 Home-page: https://github.com/opendatateam/udata-metrics
 Author: Open Data Team
 Author-email: contact@opendata.team
 License: AGPL
 Keywords: udata metrics
 Platform: UNKNOWN
@@ -15,15 +15,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Software Distribution
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: udata (>=2.0.0.dev)
+Requires-Dist: udata (>=2.0.2.dev)
 Requires-Dist: influxdb (==5.2.3)
 Provides-Extra: test
 Requires-Dist: httpretty (==0.9.7) ; extra == 'test'
 Requires-Dist: mock (==3.0.5) ; extra == 'test'
 Requires-Dist: pytest-flask (==0.15.0) ; extra == 'test'
 Requires-Dist: pytest-sugar (==0.9.2) ; extra == 'test'
 Requires-Dist: pytest (==4.6.3) ; extra == 'test'
```

## Comparing `udata_metrics-2.0.3.dev25.dist-info/RECORD` & `udata_metrics-2.0.3.dev27.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 udata_metrics/__init__.py,sha256=KWgBsbrTXZE9HLIroz91vSRVVmWMOM_0bePBTlW5JKg,248
-udata_metrics/client.py,sha256=Y95wiiCng331x26j2fI-Zvpy_pxFgg6corI5hp0gges,1461
+udata_metrics/client.py,sha256=AaCuquLLikltf9gh8bwMxlj1TpKxRGHoc7x-mDtmcfk,2140
 udata_metrics/models.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 udata_metrics/tasks.py,sha256=2QllmBB0qbJZZ0FXTJA9ogutQrt30eDabixtSaB2x2w,551
-udata_metrics-2.0.3.dev25.dist-info/METADATA,sha256=wSd_etDWnzmvejMcDuhssw_FwHMCHRDnFNekhDTDRYQ,1430
-udata_metrics-2.0.3.dev25.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
-udata_metrics-2.0.3.dev25.dist-info/entry_points.txt,sha256=yFXGBbbQNOyAOY6twoAsxTEccnn__Ab8f9GomEuOq3E,133
-udata_metrics-2.0.3.dev25.dist-info/top_level.txt,sha256=o6Ie2ExH6IjYYrl7G_pHkdzPqLDrvV20mp7kDfDwh54,14
-udata_metrics-2.0.3.dev25.dist-info/RECORD,,
+udata_metrics-2.0.3.dev27.dist-info/METADATA,sha256=lMw6sAuL17uEEwkReCNtk-YzujzN_QlGwTGReBD8QK4,1430
+udata_metrics-2.0.3.dev27.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
+udata_metrics-2.0.3.dev27.dist-info/entry_points.txt,sha256=yFXGBbbQNOyAOY6twoAsxTEccnn__Ab8f9GomEuOq3E,133
+udata_metrics-2.0.3.dev27.dist-info/top_level.txt,sha256=o6Ie2ExH6IjYYrl7G_pHkdzPqLDrvV20mp7kDfDwh54,14
+udata_metrics-2.0.3.dev27.dist-info/RECORD,,
```

