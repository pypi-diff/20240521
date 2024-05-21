# Comparing `tmp/views_tensor_utilities-0.8.5.tar.gz` & `tmp/views_tensor_utilities-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "views_tensor_utilities-0.8.5.tar", max compression
+gzip compressed data, was "views_tensor_utilities-0.8.6.tar", max compression
```

## Comparing `views_tensor_utilities-0.8.5.tar` & `views_tensor_utilities-0.8.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.5/README.md
--rw-r--r--   0        0        0      456 2024-05-07 11:30:35.989947 views_tensor_utilities-0.8.5/pyproject.toml
--rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.5/views_tensor_utilities/__init__.py
--rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.5/views_tensor_utilities/defaults.py
--rw-r--r--   0        0        0    17579 2024-05-07 11:30:35.990360 views_tensor_utilities-0.8.5/views_tensor_utilities/mappings.py
--rw-r--r--   0        0        0    11099 2024-04-23 11:49:43.048800 views_tensor_utilities-0.8.5/views_tensor_utilities/objects.py
--rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.6/README.md
+-rw-r--r--   0        0        0      456 2024-05-21 08:02:38.846994 views_tensor_utilities-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.6/views_tensor_utilities/__init__.py
+-rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.6/views_tensor_utilities/defaults.py
+-rw-r--r--   0        0        0    17579 2024-05-07 11:30:35.990360 views_tensor_utilities-0.8.6/views_tensor_utilities/mappings.py
+-rw-r--r--   0        0        0    11182 2024-05-21 08:01:33.067795 views_tensor_utilities-0.8.6/views_tensor_utilities/objects.py
+-rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.6/PKG-INFO
```

### Comparing `views_tensor_utilities-0.8.5/README.md` & `views_tensor_utilities-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `views_tensor_utilities-0.8.5/views_tensor_utilities/mappings.py` & `views_tensor_utilities-0.8.6/views_tensor_utilities/mappings.py`

 * *Files identical despite different names*

### Comparing `views_tensor_utilities-0.8.5/views_tensor_utilities/objects.py` & `views_tensor_utilities-0.8.6/views_tensor_utilities/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,16 @@
                 missing = mappings.get_missing(split_df)
 
                 try:
 
                     tensor_time_space = self.transformer(split_df, self.cast_to_dtype, self.override_dne,
                                                          self.override_missing)
                 except:
-
-                    tensor_time_space = self.transformer(split_df)
+                    raise RuntimeError('failed to cast at least one df to tensor')
+#                    tensor_time_space = self.transformer(split_df)
 
                 vnt = ViewsNumpy(tensor_time_space, split_df.columns, dne, missing)
 
                 if broadcast_index:
                     vnt.index = split_df.index
 
                 tensors.append(vnt)
```

### Comparing `views_tensor_utilities-0.8.5/PKG-INFO` & `views_tensor_utilities-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: views-tensor-utilities
-Version: 0.8.5
+Version: 0.8.6
 Summary: Classes and functions for transforming between VIEWS-compliant dfs and tensors
 Author: jimdale
 Author-email: jimdale@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

