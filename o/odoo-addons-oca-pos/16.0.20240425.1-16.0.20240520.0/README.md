# Comparing `tmp/odoo_addons_oca_pos-16.0.20240425.1-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_pos-16.0.20240520.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1754 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3576 b- defN 24-Apr-26 05:10 odoo_addons_oca_pos-16.0.20240425.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 05:10 odoo_addons_oca_pos-16.0.20240425.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-26 05:10 odoo_addons_oca_pos-16.0.20240425.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-Apr-26 05:10 odoo_addons_oca_pos-16.0.20240425.1.dist-info/RECORD
-4 files, 4054 bytes uncompressed, 996 bytes compressed:  75.4%
+Zip file size: 1768 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3654 b- defN 24-May-21 05:55 odoo_addons_oca_pos-16.0.20240520.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 05:55 odoo_addons_oca_pos-16.0.20240520.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-21 05:55 odoo_addons_oca_pos-16.0.20240520.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-May-21 05:55 odoo_addons_oca_pos-16.0.20240520.0.dist-info/RECORD
+4 files, 4132 bytes uncompressed, 1010 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_pos-16.0.20240425.1.dist-info/METADATA
+Filename: odoo_addons_oca_pos-16.0.20240520.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240425.1.dist-info/WHEEL
+Filename: odoo_addons_oca_pos-16.0.20240520.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240425.1.dist-info/top_level.txt
+Filename: odoo_addons_oca_pos-16.0.20240520.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240425.1.dist-info/RECORD
+Filename: odoo_addons_oca_pos-16.0.20240520.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_pos-16.0.20240425.1.dist-info/METADATA` & `odoo_addons_oca_pos-16.0.20240520.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-pos
-Version: 16.0.20240425.1
+Version: 16.0.20240520.0
 Summary: Meta package for oca-pos Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -34,14 +34,15 @@
 Requires-Dist: odoo-addon-pos-partner-birthdate <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-partner-firstname <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-partner-location-abstract <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-partner-location-google-map <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-partner-sale-warning <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-change <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-method-cashdro <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-pos-payment-method-change-policy <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-method-image <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-terminal <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-display-default-code <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-label <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-multi-barcode <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-packaging-container-deposit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-packaging-multi-barcode <16.1dev,>=16.0dev
```

