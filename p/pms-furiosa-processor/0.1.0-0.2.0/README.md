# Comparing `tmp/pms_furiosa_processor-0.1.0.tar.gz` & `tmp/pms_furiosa_processor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pms_furiosa_processor-0.1.0.tar", max compression
+gzip compressed data, was "pms_furiosa_processor-0.2.0.tar", max compression
```

## Comparing `pms_furiosa_processor-0.1.0.tar` & `pms_furiosa_processor-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       57 2024-04-30 09:22:40.890819 pms_furiosa_processor-0.1.0/README.md
--rw-r--r--   0        0        0      173 2024-04-30 09:22:42.870841 pms_furiosa_processor-0.1.0/pms_furiosa_processor/__init__.py
--rw-r--r--   0        0        0      802 2024-04-30 09:22:40.890819 pms_furiosa_processor-0.1.0/pms_furiosa_processor/_const.py
--rw-r--r--   0        0        0     4161 2024-04-30 09:22:40.890819 pms_furiosa_processor-0.1.0/pms_furiosa_processor/_dpir_processor.py
--rw-r--r--   0        0        0     5662 2024-04-30 09:22:40.890819 pms_furiosa_processor-0.1.0/pms_furiosa_processor/_dru_rbpn_sr_f3_processor.py
--rw-r--r--   0        0        0      471 2024-04-30 09:22:42.870841 pms_furiosa_processor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 pms_furiosa_processor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-04-30 09:22:40.890819 pms_furiosa_processor-0.2.0/README.md
+-rw-r--r--   0        0        0      173 2024-05-21 07:27:08.040351 pms_furiosa_processor-0.2.0/pms_furiosa_processor/__init__.py
+-rw-r--r--   0        0        0      802 2024-04-30 09:22:40.890819 pms_furiosa_processor-0.2.0/pms_furiosa_processor/_const.py
+-rw-r--r--   0        0        0     4161 2024-04-30 09:22:40.890819 pms_furiosa_processor-0.2.0/pms_furiosa_processor/_dpir_processor.py
+-rw-r--r--   0        0        0     5684 2024-05-21 07:27:06.020278 pms_furiosa_processor-0.2.0/pms_furiosa_processor/_dru_rbpn_sr_f3_processor.py
+-rw-r--r--   0        0        0      471 2024-05-21 07:27:08.040351 pms_furiosa_processor-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 pms_furiosa_processor-0.2.0/PKG-INFO
```

### Comparing `pms_furiosa_processor-0.1.0/pms_furiosa_processor/_const.py` & `pms_furiosa_processor-0.2.0/pms_furiosa_processor/_const.py`

 * *Files identical despite different names*

### Comparing `pms_furiosa_processor-0.1.0/pms_furiosa_processor/_dpir_processor.py` & `pms_furiosa_processor-0.2.0/pms_furiosa_processor/_dpir_processor.py`

 * *Files identical despite different names*

### Comparing `pms_furiosa_processor-0.1.0/pms_furiosa_processor/_dru_rbpn_sr_f3_processor.py` & `pms_furiosa_processor-0.2.0/pms_furiosa_processor/_dru_rbpn_sr_f3_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,16 @@
 
         prediction = np.empty(
             (
                 1,
                 3,
                 height * upscale_ratio,
                 width * upscale_ratio,
-            )
+            ),
+            np.uint8,
         )
 
         for output, index_row, index_col in data:
             cut_output = output[0]
             prediction[
                 :,
                 :,
@@ -106,15 +107,14 @@
                 index_col * upscale_ratio : (index_col + col_size) * upscale_ratio,
             ] = cut_output[
                 :,
                 :,
                 pad_size * upscale_ratio : (pad_size + row_size) * upscale_ratio,
                 pad_size * upscale_ratio : (pad_size + col_size) * upscale_ratio,
             ]
-
         img = np.squeeze(prediction, axis=0)  # Remove batch dimension
         img = np.transpose(img, (1, 2, 0))
 
         return img
 
     @staticmethod
     async def predict(
```

### Comparing `pms_furiosa_processor-0.1.0/PKG-INFO` & `pms_furiosa_processor-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pms-furiosa-processor
-Version: 0.1.0
+Version: 0.2.0
 Summary: package for pms furiosa(NPU) processor
 Author: HyeongSeok Kim
 Author-email: tiryul@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

