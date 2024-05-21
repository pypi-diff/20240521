# Comparing `tmp/everai-0.1.57-py3-none-any.whl.zip` & `tmp/everai-0.1.58-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 440628 bytes, number of entries: 424
+Zip file size: 440627 bytes, number of entries: 424
 -rw-r--r--  2.0 unx       66 b- defN 24-Apr-24 07:43 everai/__init__.py
 -rw-r--r--  2.0 unx     1214 b- defN 24-Apr-28 08:33 everai/constants.py
--rw-r--r--  2.0 unx       23 b- defN 24-May-21 04:27 everai/version.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-21 04:29 everai/version.py
 -rw-r--r--  2.0 unx       40 b- defN 24-Mar-15 10:09 everai/api/__init__.py
 -rw-r--r--  2.0 unx    15133 b- defN 24-May-09 07:21 everai/api/api.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-15 11:24 everai/app/__init__.py
 -rw-r--r--  2.0 unx     3732 b- defN 24-May-07 10:58 everai/app/app.py
--rw-r--r--  2.0 unx    12602 b- defN 24-May-21 04:26 everai/app/app_manager.py
+-rw-r--r--  2.0 unx    12594 b- defN 24-May-21 04:29 everai/app/app_manager.py
 -rw-r--r--  2.0 unx     1791 b- defN 24-Apr-24 07:37 everai/app/app_runner.py
 -rw-r--r--  2.0 unx     3486 b- defN 24-May-06 13:55 everai/app/app_runtime.py
 -rw-r--r--  2.0 unx     2568 b- defN 24-Apr-23 14:51 everai/app/app_setup.py
 -rw-r--r--  2.0 unx     1325 b- defN 24-May-13 12:03 everai/app/autocaling_handler.py
 -rw-r--r--  2.0 unx     2650 b- defN 24-May-16 11:25 everai/app/context.py
 -rw-r--r--  2.0 unx     3004 b- defN 24-Apr-28 08:38 everai/app/service.py
 -rw-r--r--  2.0 unx      210 b- defN 24-Mar-28 12:25 everai/app/typing.py
@@ -413,14 +413,14 @@
 -rw-r--r--  2.0 unx     1912 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body_file.py
 -rw-r--r--  2.0 unx     2548 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_revision_body.py
 -rw-r--r--  2.0 unx     2233 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1624 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_create_body.py
 -rw-r--r--  2.0 unx     2149 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1769 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1968 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 04:28 everai-0.1.57.dist-info/LICENSE
--rw-r--r--  2.0 unx     1985 b- defN 24-May-21 04:28 everai-0.1.57.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-21 04:28 everai-0.1.57.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 24-May-21 04:28 everai-0.1.57.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-May-21 04:28 everai-0.1.57.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    42349 b- defN 24-May-21 04:28 everai-0.1.57.dist-info/RECORD
-424 files, 1385000 bytes uncompressed, 371658 bytes compressed:  73.2%
+-rw-r--r--  2.0 unx        0 b- defN 24-May-21 04:29 everai-0.1.58.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1985 b- defN 24-May-21 04:29 everai-0.1.58.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 04:29 everai-0.1.58.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 24-May-21 04:29 everai-0.1.58.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-May-21 04:29 everai-0.1.58.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    42349 b- defN 24-May-21 04:29 everai-0.1.58.dist-info/RECORD
+424 files, 1384992 bytes uncompressed, 371657 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -1248,26 +1248,26 @@
 
 Filename: generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_sign_upload_body.py
 Comment: 
 
-Filename: everai-0.1.57.dist-info/LICENSE
+Filename: everai-0.1.58.dist-info/LICENSE
 Comment: 
 
-Filename: everai-0.1.57.dist-info/METADATA
+Filename: everai-0.1.58.dist-info/METADATA
 Comment: 
 
-Filename: everai-0.1.57.dist-info/WHEEL
+Filename: everai-0.1.58.dist-info/WHEEL
 Comment: 
 
-Filename: everai-0.1.57.dist-info/entry_points.txt
+Filename: everai-0.1.58.dist-info/entry_points.txt
 Comment: 
 
-Filename: everai-0.1.57.dist-info/top_level.txt
+Filename: everai-0.1.58.dist-info/top_level.txt
 Comment: 
 
-Filename: everai-0.1.57.dist-info/RECORD
+Filename: everai-0.1.58.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## everai/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.57"
+__version__ = "0.1.58"
```

## everai/app/app_manager.py

```diff
@@ -151,24 +151,24 @@
 
         http_server.serve_forever()
         # flask_app.run(host=listen, port=port, debug=False)
 
     def run(self, app: typing.Optional[App] = None, *args, **kwargs):
         app = app or must_find_target(target_type=App)
         app.runtime = AppRuntime()
-        # # start prepare thread
-        # prepare_thread = threading.Thread(target=self.prepare,
-        #                                   args=(app,),
-        #                                   kwargs=dict(
-        #                                       is_prepare_mode=False,
-        #                                   ))
-        # prepare_thread.start()
+        # start prepare thread
+        prepare_thread = threading.Thread(target=self.prepare,
+                                          args=(app,),
+                                          kwargs=dict(
+                                              is_prepare_mode=False,
+                                          ))
+        prepare_thread.start()
 
-        self.prepare(app, False)
-        print('prepare finished')
+        # self.prepare(app, False)
+        # print('prepare finished')
 
         flask_app = Flask(app.name)
         self.everai_handler(flask_app)
         app.service.create_handler(flask_app)
 
         def final_clear():
             app.do_clear()
@@ -192,15 +192,15 @@
         app.runtime = runtime
         return app, runtime
 
     def prepare(self,
                 app: typing.Optional[App] = None,
                 is_prepare_mode: bool = True,
                 *args, **kwargs):
-        traceback.print_stack()
+        # traceback.print_stack()
         try:
             app, runtime = self.prepare_secrets_configmaps(app)
 
             runtime.is_prepare_mode = is_prepare_mode
             self.prepare_volumes(app, runtime)
 
             app.do_prepare()
```

## Comparing `everai-0.1.57.dist-info/METADATA` & `everai-0.1.58.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everai
-Version: 0.1.57
+Version: 0.1.58
 Summary: Client library to manage everai infrastructure
 Author-email: mc <mc@expvent.com>
 Maintainer-email: mc <mc@expvent.com>
 Project-URL: Homepage, https://everai.expvent.com
 Project-URL: Documentation, https://everai.expvent.com
 Project-URL: Repository, https://github.com/expvent/everai
 Project-URL: Issues, https://github.com/expvent/everai/issues
```

## Comparing `everai-0.1.57.dist-info/RECORD` & `everai-0.1.58.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 everai/__init__.py,sha256=AbgR3tVRy6TETgwXyJITEnET1TSFpEAEqQJJqzReYqQ,66
 everai/constants.py,sha256=6tvPKHYvL1H5ippD2YkwCerLhKftIiOg-SVtFLtVYN4,1214
-everai/version.py,sha256=4_3hAGEogvYbOy6vn6QDJpHwwyZfPSVQHAgrUMAMbLI,23
+everai/version.py,sha256=ujgZXX_cw13M2UkyXWVg5j1fgdE25Qb3rUzLZVokSKg,23
 everai/api/__init__.py,sha256=2WLrQ_PpJ35__yOVHC89MhILujyGioyaGir-5n6hxCc,40
 everai/api/api.py,sha256=Fsa9IDVLNW26A8pcvEYpPCzRD5YBlCd005vqAHfVShM,15133
 everai/app/__init__.py,sha256=A-USWcj6TDAW_hxG6wT3Qb8m3d5Tq733WWC9McNhlGI,208
 everai/app/app.py,sha256=z9B48uwKAJHHW7OfF_rcVmhxR74Y2JAw4n5AApmMLEI,3732
-everai/app/app_manager.py,sha256=BI5zS9p4rdspjXZKqqKHKofa4xdzP-HZ2mkJveCS-88,12602
+everai/app/app_manager.py,sha256=wOcpSZ-iNquBDuQwqw_DEBXI-gvg6YGeLpUjQ1hM_VE,12594
 everai/app/app_runner.py,sha256=HVlOLweFX-C2kBbgyVwuDz4vfGzQ6uzHpNVzikQhRfA,1791
 everai/app/app_runtime.py,sha256=2wFrZLtfNgG6uPR5LP4ID6XlNTOOu0Cy7nHT0wbvWlQ,3486
 everai/app/app_setup.py,sha256=CLXAC83OyTqEjAEKNLHQaCT3UPhvw149mD1VQr-AEEg,2568
 everai/app/autocaling_handler.py,sha256=lWZcILpLX6eqEoiUCi7LtF0ZN_PNZyZh93aYiXWe0us,1325
 everai/app/context.py,sha256=uguFr1Kmw9jMKh0XYW38lumKsoyOdMNao1gqEM9zIn8,2650
 everai/app/service.py,sha256=vlyKTK0PBAMPvL06AbDKFedHA9hyxaCLVU-b-6RGYj0,3004
 everai/app/typing.py,sha256=d7tPA7VoDY771u-v0DLwD6TTMfPotg8u_PAshDcHRQo,210
@@ -412,13 +412,13 @@
 generated/volumes/test/test_volume_service_commit_file_body_file.py,sha256=F4jWVTlpo82x5j68w3hYpaHvaUZhCiFrmBSo1SVZOu0,1912
 generated/volumes/test/test_volume_service_commit_revision_body.py,sha256=UizO6O0rY4b9isgc_d2lKBUwTlCn0kiefccAD86nCcs,2548
 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py,sha256=Ek6ZP78kDn1ol-guEmhm2zA42c_6XkArQf8G-_L5MgI,2233
 generated/volumes/test/test_volume_service_create_body.py,sha256=2MA4PEVNwPpMGuvpwMu4qeYvDAjrZjyUaeuo9p3qJ1c,1624
 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py,sha256=G58739S9489bMEXfaefcWch_GqgV-PTw4QCewOzxhSs,2149
 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py,sha256=3b5ULrWgH38nEWU0s_MISEyj4j6LV8doFAx3CfQ6XjY,1769
 generated/volumes/test/test_volume_service_sign_upload_body.py,sha256=xX2B1LCvIu0OHX0AkyL8dXPClBTDgmZwmgPJOjjz96g,1968
-everai-0.1.57.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-everai-0.1.57.dist-info/METADATA,sha256=n-bBcm3LqKZR3Z_auqKvtBsyIc9pCKUQU9wRwbGY6tQ,1985
-everai-0.1.57.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-everai-0.1.57.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
-everai-0.1.57.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
-everai-0.1.57.dist-info/RECORD,,
+everai-0.1.58.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+everai-0.1.58.dist-info/METADATA,sha256=0bdpz-FX_hd0pVvq3qw-7AzeUVWUvdbO0mm3yo1-MU0,1985
+everai-0.1.58.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+everai-0.1.58.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
+everai-0.1.58.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
+everai-0.1.58.dist-info/RECORD,,
```

