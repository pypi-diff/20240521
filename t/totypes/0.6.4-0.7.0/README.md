# Comparing `tmp/totypes-0.6.4.tar.gz` & `tmp/totypes-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totypes-0.6.4.tar", last modified: Tue Mar  5 03:45:03 2024, max compression
+gzip compressed data, was "totypes-0.7.0.tar", last modified: Tue May 21 19:13:48 2024, max compression
```

## Comparing `totypes-0.6.4.tar` & `totypes-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 03:45:03.305422 totypes-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-05 03:44:53.000000 totypes-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-05 03:45:03.305422 totypes-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-05 03:44:53.000000 totypes-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-05 03:44:53.000000 totypes-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 03:45:03.305422 totypes-0.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 03:45:03.301422 totypes-0.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 03:45:03.301422 totypes-0.6.4/src/totypes/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-05 03:44:53.000000 totypes-0.6.4/src/totypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-03-05 03:44:53.000000 totypes-0.6.4/src/totypes/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-05 03:44:53.000000 totypes-0.6.4/src/totypes/partition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 03:44:53.000000 totypes-0.6.4/src/totypes/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-05 03:44:53.000000 totypes-0.6.4/src/totypes/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14918 2024-03-05 03:44:53.000000 totypes-0.6.4/src/totypes/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 03:45:03.305422 totypes-0.6.4/src/totypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-05 03:45:03.000000 totypes-0.6.4/src/totypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-05 03:45:03.000000 totypes-0.6.4/src/totypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 03:45:03.000000 totypes-0.6.4/src/totypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-05 03:45:03.000000 totypes-0.6.4/src/totypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-05 03:45:03.000000 totypes-0.6.4/src/totypes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 03:45:03.305422 totypes-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-03-05 03:44:53.000000 totypes-0.6.4/tests/test_json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-05 03:44:53.000000 totypes-0.6.4/tests/test_json_utils_server_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-03-05 03:44:53.000000 totypes-0.6.4/tests/test_partition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-03-05 03:44:53.000000 totypes-0.6.4/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10783 2024-03-05 03:44:53.000000 totypes-0.6.4/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.047429 totypes-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-21 19:13:37.000000 totypes-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-21 19:13:48.047429 totypes-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-21 19:13:37.000000 totypes-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-21 19:13:37.000000 totypes-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:13:48.047429 totypes-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.043429 totypes-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.043429 totypes-0.7.0/src/totypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/partition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.047429 totypes-0.7.0/src/totypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.047429 totypes-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_json_utils_server_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_partition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10783 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_types.py
```

### Comparing `totypes-0.6.4/LICENSE` & `totypes-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `totypes-0.6.4/PKG-INFO` & `totypes-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totypes
-Version: 0.6.4
+Version: 0.7.0
 Summary: Custom datatypes useful in a topology optimization context
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -42,15 +42,15 @@
 Provides-Extra: dev
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: totypes[tests]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # totypes - Custom types for topology optimization
-`v0.6.4`
+`v0.7.0`
 
 ## Overview
 
 The `totypes` package defines custom jax-compatible datatypes for use in a topology optimization, inverse design, or AI-guided design context. The custom types are pytree nodes consisting of standard jax arrays along with metadata that describe the desired characteristics of the arrays.
 - `BoundedArray`, an array with optional lower and/or upper bounds, used e.g. for representing layer thicknesses.
 - `Density2DArray`, an array with lower and upper bounds and characteristics such as fixed pixels, minimum feature size, or symmetry, used for representing layer density as is common in topology optimization.
```

### Comparing `totypes-0.6.4/README.md` & `totypes-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # totypes - Custom types for topology optimization
-`v0.6.4`
+`v0.7.0`
 
 ## Overview
 
 The `totypes` package defines custom jax-compatible datatypes for use in a topology optimization, inverse design, or AI-guided design context. The custom types are pytree nodes consisting of standard jax arrays along with metadata that describe the desired characteristics of the arrays.
 - `BoundedArray`, an array with optional lower and/or upper bounds, used e.g. for representing layer thicknesses.
 - `Density2DArray`, an array with lower and upper bounds and characteristics such as fixed pixels, minimum feature size, or symmetry, used for representing layer density as is common in topology optimization.
```

### Comparing `totypes-0.6.4/pyproject.toml` & `totypes-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "totypes"
-version = "v0.6.4"
+version = "v0.7.0"
 description = "Custom datatypes useful in a topology optimization context"
 keywords = ["topology", "optimization", "jax", "inverse design"]
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 
 authors = [
```

### Comparing `totypes-0.6.4/src/totypes/json_utils.py` & `totypes-0.7.0/src/totypes/json_utils.py`

 * *Files identical despite different names*

### Comparing `totypes-0.6.4/src/totypes/partition_utils.py` & `totypes-0.7.0/src/totypes/partition_utils.py`

 * *Files identical despite different names*

### Comparing `totypes-0.6.4/src/totypes/symmetry.py` & `totypes-0.7.0/src/totypes/symmetry.py`

 * *Files identical despite different names*

### Comparing `totypes-0.6.4/src/totypes/types.py` & `totypes-0.7.0/src/totypes/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,22 @@
                 ):
                     raise ValueError(
                         "`upper_bound` must be strictly greater than `lower_bound`."
                     )
 
     @property
     def shape(self) -> Tuple[int, ...]:
-        """Returns the shape of the array."""
+        """Return the shape of the array."""
         return jnp.shape(self.array)  # type: ignore[no-any-return]
 
+    @property
+    def ndim(self) -> int:
+        """Return the number of dimensions of the array."""
+        return int(jnp.ndim(self.array))
+
 
 def _flatten_bounded_array(
     bounded_array: BoundedArray,
 ) -> Tuple[Tuple[ArrayOrScalar], Tuple["_HashableWrapper", "_HashableWrapper"]]:
     """Flattens a `BoundedArray` into children and auxilliary data."""
     return (
         (bounded_array.array,),
@@ -248,17 +253,22 @@
             raise ValueError(
                 f"Some specified symmetries require a square array shape, but got a "
                 f"shape of {self.array.shape} for symmetries {self.symmetries}."
             )
 
     @property
     def shape(self) -> Tuple[int, ...]:
-        """Returns the shape of the array."""
+        """Return the shape of the array."""
         return jnp.shape(self.array)  # type: ignore[no-any-return]
 
+    @property
+    def ndim(self) -> int:
+        """Return the number of dimensions of the array."""
+        return int(jnp.ndim(self.array))
+
 
 def _flatten_density_2d(
     density: Density2DArray,
 ) -> Tuple[
     Tuple[Array],
     Tuple[
         float,
```

### Comparing `totypes-0.6.4/src/totypes.egg-info/PKG-INFO` & `totypes-0.7.0/src/totypes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totypes
-Version: 0.6.4
+Version: 0.7.0
 Summary: Custom datatypes useful in a topology optimization context
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -42,15 +42,15 @@
 Provides-Extra: dev
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: totypes[tests]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # totypes - Custom types for topology optimization
-`v0.6.4`
+`v0.7.0`
 
 ## Overview
 
 The `totypes` package defines custom jax-compatible datatypes for use in a topology optimization, inverse design, or AI-guided design context. The custom types are pytree nodes consisting of standard jax arrays along with metadata that describe the desired characteristics of the arrays.
 - `BoundedArray`, an array with optional lower and/or upper bounds, used e.g. for representing layer thicknesses.
 - `Density2DArray`, an array with lower and upper bounds and characteristics such as fixed pixels, minimum feature size, or symmetry, used for representing layer density as is common in topology optimization.
```

### Comparing `totypes-0.6.4/tests/test_json_utils.py` & `totypes-0.7.0/tests/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `totypes-0.6.4/tests/test_json_utils_server_client.py` & `totypes-0.7.0/tests/test_json_utils_server_client.py`

 * *Files identical despite different names*

### Comparing `totypes-0.6.4/tests/test_partition_utils.py` & `totypes-0.7.0/tests/test_partition_utils.py`

 * *Files identical despite different names*

### Comparing `totypes-0.6.4/tests/test_symmetry.py` & `totypes-0.7.0/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `totypes-0.6.4/tests/test_types.py` & `totypes-0.7.0/tests/test_types.py`

 * *Files identical despite different names*

