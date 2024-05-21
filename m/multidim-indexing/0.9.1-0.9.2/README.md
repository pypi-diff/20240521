# Comparing `tmp/multidim_indexing-0.9.1.tar.gz` & `tmp/multidim_indexing-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidim_indexing-0.9.1.tar", last modified: Wed Sep 27 21:32:41 2023, max compression
+gzip compressed data, was "multidim_indexing-0.9.2.tar", last modified: Tue May 21 01:12:50 2024, max compression
```

## Comparing `multidim_indexing-0.9.1.tar` & `multidim_indexing-0.9.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-09-27 21:32:41.565855 multidim_indexing-0.9.1/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1056 2023-02-10 03:56:21.000000 multidim_indexing-0.9.1/LICENSE.txt
--rw-r--r--   0 zhsh      (1001) zhsh      (1001)     9051 2023-09-27 21:32:41.565855 multidim_indexing-0.9.1/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     6744 2023-08-23 20:54:21.000000 multidim_indexing-0.9.1/README.md
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4172 2023-09-27 21:32:01.000000 multidim_indexing-0.9.1/pyproject.toml
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2023-09-27 21:32:41.565855 multidim_indexing-0.9.1/setup.cfg
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-09-27 21:32:41.561855 multidim_indexing-0.9.1/src/
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-09-27 21:32:41.561855 multidim_indexing-0.9.1/src/multidim_indexing/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        0 2023-02-10 04:00:36.000000 multidim_indexing-0.9.1/src/multidim_indexing/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1382 2023-02-10 04:00:36.000000 multidim_indexing-0.9.1/src/multidim_indexing/numpy_view.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     2675 2023-02-10 04:00:36.000000 multidim_indexing-0.9.1/src/multidim_indexing/torch_view.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     9876 2023-09-27 21:28:43.000000 multidim_indexing-0.9.1/src/multidim_indexing/view.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-09-27 21:32:41.565855 multidim_indexing-0.9.1/src/multidim_indexing.egg-info/
--rw-r--r--   0 zhsh      (1001) zhsh      (1001)     9051 2023-09-27 21:32:41.000000 multidim_indexing-0.9.1/src/multidim_indexing.egg-info/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      446 2023-09-27 21:32:41.000000 multidim_indexing-0.9.1/src/multidim_indexing.egg-info/SOURCES.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2023-09-27 21:32:41.000000 multidim_indexing-0.9.1/src/multidim_indexing.egg-info/dependency_links.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       64 2023-09-27 21:32:41.000000 multidim_indexing-0.9.1/src/multidim_indexing.egg-info/requires.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       18 2023-09-27 21:32:41.000000 multidim_indexing-0.9.1/src/multidim_indexing.egg-info/top_level.txt
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-09-27 21:32:41.565855 multidim_indexing-0.9.1/tests/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     6859 2023-01-14 23:14:02.000000 multidim_indexing-0.9.1/tests/test_numpy_view.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     9498 2023-08-23 20:50:05.000000 multidim_indexing-0.9.1/tests/test_torch_view.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.772292 multidim_indexing-0.9.2/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1056 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/LICENSE.txt
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-21 01:12:50.772292 multidim_indexing-0.9.2/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6744 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/README.md
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     4172 2024-05-17 02:36:21.000000 multidim_indexing-0.9.2/pyproject.toml
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       38 2024-05-21 01:12:50.772292 multidim_indexing-0.9.2/setup.cfg
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.768292 multidim_indexing-0.9.2/src/
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.768292 multidim_indexing-0.9.2/src/multidim_indexing/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        0 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/src/multidim_indexing/__init__.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1547 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/src/multidim_indexing/numpy_view.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     2851 2024-05-17 02:30:54.000000 multidim_indexing-0.9.2/src/multidim_indexing/torch_view.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    11208 2024-05-17 02:35:21.000000 multidim_indexing-0.9.2/src/multidim_indexing/view.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.768292 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      472 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        1 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       64 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/requires.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       18 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/top_level.txt
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.768292 multidim_indexing-0.9.2/tests/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6859 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/tests/test_numpy_view.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      893 2024-05-17 01:24:04.000000 multidim_indexing-0.9.2/tests/test_performance.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     9498 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/tests/test_torch_view.py
```

### Comparing `multidim_indexing-0.9.1/LICENSE.txt` & `multidim_indexing-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multidim_indexing-0.9.1/PKG-INFO` & `multidim_indexing-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidim_indexing
-Version: 0.9.1
+Version: 0.9.2
 Summary: Multidimensional batch indexing of pytorch tensors and numpy arrays
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 Sheng Zhong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `multidim_indexing-0.9.1/README.md` & `multidim_indexing-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `multidim_indexing-0.9.1/pyproject.toml` & `multidim_indexing-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multidim_indexing"
-version = "0.9.1"
+version = "0.9.2"
 description = "Multidimensional batch indexing of pytorch tensors and numpy arrays"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `multidim_indexing-0.9.1/src/multidim_indexing/numpy_view.py` & `multidim_indexing-0.9.2/src/multidim_indexing/numpy_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from multidim_indexing.view import MultidimView, classproperty
 import numpy as np
 
 
 class NumpyMultidimView(MultidimView):
     @classproperty
+    def default_coordinate_dtype(cls):
+        return float
+
+    @classproperty
     def lib(cls):
         return np
 
     @property
     def int(self):
         return int
 
@@ -22,14 +26,18 @@
         return arr.astype(dtype)
 
     @classmethod
     def all(cls, arr, dim=0):
         return np.all(arr, axis=dim)
 
     @classmethod
+    def any(cls, arr, dim=0):
+        return np.any(arr, axis=dim)
+
+    @classmethod
     def is_valid_arr_value(cls, val, valid):
         return not np.isscalar(val) and val.size == valid.size
 
     @classmethod
     def ravel_multi_index(cls, key, shape):
         if len(key.shape) == 2:
             key = key.T
```

### Comparing `multidim_indexing-0.9.1/src/multidim_indexing/torch_view.py` & `multidim_indexing-0.9.2/src/multidim_indexing/torch_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 class TorchMultidimView(MultidimView):
     def __init__(self, source, *args, **kwargs):
         self.device = source.device
         super(TorchMultidimView, self).__init__(source, *args, **kwargs)
 
     @classproperty
+    def default_coordinate_dtype(cls):
+        return torch.float32
+
+    @classproperty
     def lib(cls):
         return torch
 
     @property
     def int(self):
         return torch.long
 
@@ -27,14 +31,18 @@
         return arr.to(dtype=dtype)
 
     @classmethod
     def all(cls, arr, dim=0):
         return torch.all(arr, dim=dim)
 
     @classmethod
+    def any(cls, arr, dim=0):
+        return torch.any(arr, dim=dim)
+
+    @classmethod
     def is_valid_arr_value(cls, val, valid):
         return torch.is_tensor(val) and torch.numel(val) == torch.numel(valid)
 
     @classmethod
     def ravel_multi_index(cls, key, shape):
         return ravel_multi_index(key, shape)
 
@@ -53,14 +61,15 @@
     def cat(cls, arrs, dim=0):
         return torch.cat(arrs, dim=dim)
 
     @classmethod
     def stack(cls, arrs, dim=0):
         return torch.stack(arrs, dim=dim)
 
+
 # filling in functions from numpy from francois-rozet
 Shape = Union[List[int], Tuple[int, ...], torch.Size]
 
 
 def ravel_multi_index(coords: torch.Tensor, shape: Shape) -> torch.Tensor:
     r"""Converts a tensor of coordinate vectors into a tensor of flat indices.
     This is a `torch` implementation of `numpy.ravel_multi_index`.
```

### Comparing `multidim_indexing-0.9.1/src/multidim_indexing/view.py` & `multidim_indexing-0.9.2/src/multidim_indexing/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,52 +7,69 @@
         self.f = f
 
     def __get__(self, obj, owner):
         return self.f(owner)
 
 
 class MultidimView(abc.ABC):
-    def __init__(self, source, value_ranges=None, invalid_value=-1, check_safety=True, method='nearest'):
+    def __init__(self, source, value_ranges=None, invalid_value=-1, check_safety=True, method='nearest',
+                 coord_dtype=None):
         """
         View into a tensor or numpy array that is convenient to index using a batch of indices.
         Intended for use on a cache of a function that needs to be indexed into with coordinates
         rather than integer indices.
 
         :param source: d dimensional underlying tensor or numpy array
         :param value_ranges: d pairs of [min, max] (or an otherwise sequence) coordinate keys for each of the
             d dimensions. It is an inclusive range, so indexing with the boundary values of either min or max is valid
         :param invalid_value: when check_safety is True, querying with out of range coordinates returns this value
             rather than raising an error. Needs to be the same dtype as source
         :param check_safety: whether to check if the keys are within bound; turn off to get about 40% speedup in
             indexing
         :param method: interpolation method when querying with value ranges, can be 'nearest' or 'linear'
+        :param coord_dtype: dtype of the coordinate keys, defaults to float of the appropriate type
         """
         self.dtype = source.dtype
         self.shape = source.shape
         self.dim = len(source.shape)
         self.invalid_value = invalid_value
         self.check_safety = check_safety
         self.method = method
+        self.coordinate_dtype = coord_dtype or self.default_coordinate_dtype
 
         if value_ranges is not None:
             self._min = self.arr([min(range) for range in value_ranges])
             self._max = self.arr([max(range) for range in value_ranges])
             self._is_value_range = True
             # want an inclusive range on the min and max, so indexing with max should be valid
-            self._resolution = (self._max - self._min) / (self.arr(self.shape) - 1)
+            shape = self.arr(self.shape)
+            self._resolution = (self._max - self._min) / (shape - 1)
+            # if some dim of shape is 1, then resolution for it is undefined
+            invalid_resolution = self.lib.isnan(self._resolution)
+            valid_resolution_val = self._resolution[~invalid_resolution]
+            if len(shape) != len(self._resolution):
+                raise RuntimeError(f"Shape {shape} of source is not compatible with value_ranges {value_ranges}")
+            if self.any(invalid_resolution) and len(valid_resolution_val) > 0:
+                # we assume that it'll have the same resolution as the first non-1 dim
+                self._resolution[invalid_resolution] = valid_resolution_val[0]
         else:
             self._min = self.lib.zeros(self.dim, dtype=self.int)
             self._max = self.arr(source.shape, dtype=self.int) - 1
             self._is_value_range = False
 
         # flattened view of the source data
         self._d = source.reshape(-1)
 
     @classproperty
     @abc.abstractmethod
+    def default_coordinate_dtype(cls):
+        """Return the default coordinate type for coordinate keys"""
+
+    @classproperty
+    @abc.abstractmethod
     def lib(cls):
         """Tensor/array library e.g. numpy and torch"""
 
     @property
     @abc.abstractmethod
     def int(self):
         """Return the integer type"""
@@ -77,14 +94,19 @@
     @classmethod
     @abc.abstractmethod
     def all(cls, arr, dim=0):
         """Logically evaluate to true iff all elements of arr is true"""
 
     @classmethod
     @abc.abstractmethod
+    def any(cls, arr, dim=0):
+        """Logically evaluate to true if any elements of arr is true"""
+
+    @classmethod
+    @abc.abstractmethod
     def is_valid_arr_value(cls, val, valid):
         """Evaluate if the value is an array of compatible size with valid mask"""
 
     @classmethod
     @abc.abstractmethod
     def ravel_multi_index(cls, key, shape):
         """Flatten keys from N x d to N"""
@@ -115,38 +137,45 @@
 
     def is_key_ravelled(self, key):
         return len(key.shape) == 1 or (key.shape[-1] == 1 and self.dim != 1)
 
     def ensure_index_key(self, key, force=False):
         if self.is_key_ravelled(key):
             key = self.unravel_key(key.reshape(-1))
-        # convert key from value ranges to indices if necessary
+
         if self._is_value_range and (force or key.dtype != self.int):
-            index_key = self.stack(
-                [self.cast(self.lib.round((key[..., i] - self._min[i]) / self._resolution[i]), self.int) for i in
-                 range(self.dim)],
-                dim=-1)
+            offsets = (key - self._min) / self._resolution
+            index_key = self.cast(offsets.round(), self.int)
             key = index_key
+
         return key
 
     def ensure_value_key(self, key, force=False):
         if self.is_key_ravelled(key):
             key = self.unravel_key(key.reshape(-1))
         # convert key from indices to value ranges if necessary
-        if self._is_value_range and (force or key.dtype != self.dtype):
-            value_key = self.stack(
-                [self.cast(key[..., i] * self._resolution[i] + self._min[i], self.dtype) for i in range(self.dim)],
-                dim=-1)
+        if self._is_value_range and (force or key.dtype != self.coordinate_dtype):
+            # scales = torch.tensor(self._resolution, device=key.device, dtype=self.coordinate_dtype)
+            scales = self._resolution
+            # offsets = torch.tensor(self._min, device=key.device, dtype=self.coordinate_dtype)
+            offsets = self.cast(self._min, self.coordinate_dtype)
+
+            # Broadcasting the scales and offsets across the last dimension
+            value_key = key * scales + offsets
+
+            if key.dtype != self.coordinate_dtype:
+                value_key = value_key.to(self.coordinate_dtype)
+
             key = value_key
+
         return key
 
     def get_valid_values(self, key):
-        return self.all(
-            self.stack([(self._min[i] <= key[..., i]) & (key[..., i] <= self._max[i]) for i in range(self.dim)]),
-            dim=0)
+        is_valid = (self._min <= key) & (key <= self._max)
+        return self.all(is_valid, dim=-1)
 
     def _check_and_flatten_key(self, key):
         """Flatten batch dimensions of key to ensure it is N x d"""
         # check if shorthand is used where batch indices are not specified
         if key.shape[-1] == self.dim - 1:
             B = key.shape[0]
             batch_index = self.repeat(self.lib.arange(B).reshape(B, 1, 1), (1, key.shape[-2], 1))
```

### Comparing `multidim_indexing-0.9.1/src/multidim_indexing.egg-info/PKG-INFO` & `multidim_indexing-0.9.2/src/multidim_indexing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: multidim-indexing
-Version: 0.9.1
+Name: multidim_indexing
+Version: 0.9.2
 Summary: Multidimensional batch indexing of pytorch tensors and numpy arrays
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 Sheng Zhong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `multidim_indexing-0.9.1/tests/test_numpy_view.py` & `multidim_indexing-0.9.2/tests/test_numpy_view.py`

 * *Files identical despite different names*

### Comparing `multidim_indexing-0.9.1/tests/test_torch_view.py` & `multidim_indexing-0.9.2/tests/test_torch_view.py`

 * *Files identical despite different names*

