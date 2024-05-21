# Comparing `tmp/views_tensor_utilities-0.8.6.tar.gz` & `tmp/views_tensor_utilities-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "views_tensor_utilities-0.8.6.tar", max compression
+gzip compressed data, was "views_tensor_utilities-0.8.7.tar", max compression
```

## Comparing `views_tensor_utilities-0.8.6.tar` & `views_tensor_utilities-0.8.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.6/README.md
--rw-r--r--   0        0        0      456 2024-05-21 08:02:38.846994 views_tensor_utilities-0.8.6/pyproject.toml
--rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.6/views_tensor_utilities/__init__.py
--rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.6/views_tensor_utilities/defaults.py
--rw-r--r--   0        0        0    17579 2024-05-07 11:30:35.990360 views_tensor_utilities-0.8.6/views_tensor_utilities/mappings.py
--rw-r--r--   0        0        0    11182 2024-05-21 08:01:33.067795 views_tensor_utilities-0.8.6/views_tensor_utilities/objects.py
--rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.7/README.md
+-rw-r--r--   0        0        0      456 2024-05-21 08:20:00.494352 views_tensor_utilities-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.7/views_tensor_utilities/__init__.py
+-rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.7/views_tensor_utilities/defaults.py
+-rw-r--r--   0        0        0    17121 2024-05-21 08:19:55.012374 views_tensor_utilities-0.8.7/views_tensor_utilities/mappings.py
+-rw-r--r--   0        0        0    11182 2024-05-21 08:01:33.067795 views_tensor_utilities-0.8.7/views_tensor_utilities/objects.py
+-rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.7/PKG-INFO
```

### Comparing `views_tensor_utilities-0.8.6/README.md` & `views_tensor_utilities-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `views_tensor_utilities-0.8.6/views_tensor_utilities/mappings.py` & `views_tensor_utilities-0.8.7/views_tensor_utilities/mappings.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,16 @@
     def __init__(self, times, index_to_time, time_to_index):
         self.times = times
         self.index_to_time = index_to_time
         self.time_to_index = time_to_index
 
     @classmethod
     def from_pandas(cls, pandas_object):
-        if isinstance(pandas_object, pd.DataFrame):
-            index = pandas_object.index
-        elif isinstance(pandas_object, pd.MultiIndex):
-            index = pandas_object
-        else:
-            raise RuntimeError(f'Input is not a df or a df index')
+
+        index = get_index(pandas_object)
 
         # get unique times
 
         times = np.array(list({idx[0] for idx in index.values}))
         times = list(np.sort(times))
 
         # make dicts to transform between times and the index of a time in the list
@@ -62,20 +58,16 @@
     def __init__(self, spaces, index_to_space, space_to_index):
         self.spaces = spaces
         self.index_to_space = index_to_space
         self.space_to_index = space_to_index
 
     @classmethod
     def from_pandas(cls, pandas_object):
-        if isinstance(pandas_object, pd.DataFrame):
-            index = pandas_object.index
-        elif isinstance(pandas_object, pd.MultiIndex):
-            index = pandas_object
-        else:
-            raise RuntimeError(f'Input is not a df or a df index')
+
+        index = get_index(pandas_object)
 
         spaces = np.array(list({idx[1] for idx in index.values}))
 
         spaces = np.sort(spaces)
 
         space_to_index = {}
         index_to_space = {}
@@ -126,20 +118,15 @@
         """
         from_pandas
 
         Factory method which builds class instances from pandas dataframes or multiindexes
 
         """
 
-        if isinstance(pandas_object, pd.DataFrame):
-            index = pandas_object.index
-        elif isinstance(pandas_object, pd.MultiIndex):
-            index = pandas_object
-        else:
-            raise RuntimeError(f'Input is not a df or a df index')
+        index = get_index(pandas_object)
 
         pgids = np.array(list({idx[1] for idx in index.values}))
         pgids = np.sort(pgids)
 
         # convert pgids to longitudes and latitudes
 
         longitudes = pgids % defaults.pg_stride
@@ -229,20 +216,15 @@
         """
         from_pandas
 
         Factory method which builds class instances from pandas dataframes or multiindexes
 
         """
 
-        if isinstance(pandas_object, pd.DataFrame):
-            index = pandas_object.index
-        elif isinstance(pandas_object, pd.MultiIndex):
-            index = pandas_object
-        else:
-            raise RuntimeError(f'Input is not a df or a df index')
+        index = get_index(pandas_object)
 
         time_indices = index.levels[0].to_list()
         space_indices = index.levels[1].to_list()
 
         index_tuples = index.to_list()
 
         time_space_indices = cls(time_indices=time_indices, space_indices=space_indices,
@@ -266,14 +248,36 @@
 
     if time_space.nrow == time_space.ntime * time_space.nspace:
         return True
     else:
         return False
 
 
+def get_index(pandas_object):
+
+    """
+    get_index
+
+    Given either a df or a df index, return the index
+
+    :param pandas_object:
+    :return: index
+
+    """
+
+    if isinstance(pandas_object, pd.DataFrame):
+        index = pandas_object.index
+    elif isinstance(pandas_object, pd.MultiIndex):
+        index = pandas_object
+    else:
+        raise RuntimeError(f'Input is not a df or a df index')
+
+    return index
+
+
 def __check_df_data_types(df):
     """
     check_df_data_types
 
     Check that there is only one data type in the input dataframe, and that it is in the set of allowed
     data types
     """
@@ -384,16 +388,16 @@
 
     if cast_to_dtype is None:
         dtype = __get_dtype(df)
     else:
         __check_cast_to_dtypes(cast_to_dtype)
         dtype = cast_to_dtype
 
-    if override_dne is not None:
-        raise RuntimeError(f'no dne tokens to override in strideable dataframe')
+#    if override_dne is not None:
+#        raise RuntimeError(f'no dne tokens to override in strideable dataframe')
 
     # get shape of dataframe
 
     dim0, dim1 = df.index.levshape
 
     dim2 = df.shape[1]
```

### Comparing `views_tensor_utilities-0.8.6/views_tensor_utilities/objects.py` & `views_tensor_utilities-0.8.7/views_tensor_utilities/objects.py`

 * *Files identical despite different names*

### Comparing `views_tensor_utilities-0.8.6/PKG-INFO` & `views_tensor_utilities-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: views-tensor-utilities
-Version: 0.8.6
+Version: 0.8.7
 Summary: Classes and functions for transforming between VIEWS-compliant dfs and tensors
 Author: jimdale
 Author-email: jimdale@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

