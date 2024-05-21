# Comparing `tmp/odoo_addons_oca_server_backend-16.0.20240415.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_server_backend-16.0.20240520.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1504 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1188 b- defN 24-Apr-16 07:17 odoo_addons_oca_server_backend-16.0.20240415.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 07:17 odoo_addons_oca_server_backend-16.0.20240415.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-16 07:17 odoo_addons_oca_server_backend-16.0.20240415.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      429 b- defN 24-Apr-16 07:17 odoo_addons_oca_server_backend-16.0.20240415.0.dist-info/RECORD
-4 files, 1710 bytes uncompressed, 658 bytes compressed:  61.5%
+Zip file size: 1513 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1256 b- defN 24-May-21 06:45 odoo_addons_oca_server_backend-16.0.20240520.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 06:45 odoo_addons_oca_server_backend-16.0.20240520.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-21 06:45 odoo_addons_oca_server_backend-16.0.20240520.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      429 b- defN 24-May-21 06:45 odoo_addons_oca_server_backend-16.0.20240520.0.dist-info/RECORD
+4 files, 1778 bytes uncompressed, 667 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_server_backend-16.0.20240415.0.dist-info/METADATA
+Filename: odoo_addons_oca_server_backend-16.0.20240520.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_server_backend-16.0.20240415.0.dist-info/WHEEL
+Filename: odoo_addons_oca_server_backend-16.0.20240520.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_server_backend-16.0.20240415.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_server_backend-16.0.20240520.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_server_backend-16.0.20240415.0.dist-info/RECORD
+Filename: odoo_addons_oca_server_backend-16.0.20240520.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_server_backend-16.0.20240415.0.dist-info/METADATA` & `odoo_addons_oca_server_backend-16.0.20240520.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-server-backend
-Version: 16.0.20240415.0
+Version: 16.0.20240520.0
 Summary: Meta package for oca-server-backend Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -16,11 +16,12 @@
 Requires-Dist: odoo-addon-base-global-discount <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-group-backend <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-import-match <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-portal-type <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-user-role <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-user-role-company <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-user-role-history <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-server-action-navigate <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-server-action-sort <16.1dev,>=16.0dev
 
 UNKNOWN
```

