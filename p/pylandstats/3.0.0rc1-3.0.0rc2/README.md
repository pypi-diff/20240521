# Comparing `tmp/pylandstats-3.0.0rc1.tar.gz` & `tmp/pylandstats-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylandstats-3.0.0rc1.tar", last modified: Mon Nov 20 17:01:50 2023, max compression
+gzip compressed data, was "pylandstats-3.0.0rc2.tar", last modified: Tue May 21 12:57:25 2024, max compression
```

## Comparing `pylandstats-3.0.0rc1.tar` & `pylandstats-3.0.0rc2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:01:50.966253 pylandstats-3.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2023-11-20 17:01:50.966253 pylandstats-3.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:01:50.966253 pylandstats-3.0.0rc1/pylandstats/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/pylandstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:01:50.966253 pylandstats-3.0.0rc1/pylandstats/__pythran__/
--rw-------   0 runner    (1001) docker     (127)    25358 2023-11-20 17:01:50.000000 pylandstats-3.0.0rc1/pylandstats/__pythran__/landscape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2023-11-20 17:01:49.000000 pylandstats-3.0.0rc1/pylandstats/__pythran__/landscape.py
--rw-r--r--   0 runner    (1001) docker     (127)   145677 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/pylandstats/landscape.py
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/pylandstats/multilandscape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/pylandstats/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    29972 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/pylandstats/spatiotemporal.py
--rw-r--r--   0 runner    (1001) docker     (127)    23822 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/pylandstats/zonal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:01:50.966253 pylandstats-3.0.0rc1/pylandstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2023-11-20 17:01:50.000000 pylandstats-3.0.0rc1/pylandstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-20 17:01:50.000000 pylandstats-3.0.0rc1/pylandstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 17:01:50.000000 pylandstats-3.0.0rc1/pylandstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-11-20 17:01:50.000000 pylandstats-3.0.0rc1/pylandstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-20 17:01:50.000000 pylandstats-3.0.0rc1/pylandstats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 17:01:50.966253 pylandstats-3.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:01:50.966253 pylandstats-3.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    59304 2023-11-20 17:01:32.000000 pylandstats-3.0.0rc1/tests/test_pylandstats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:57:25.368181 pylandstats-3.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-21 12:57:25.368181 pylandstats-3.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:57:25.368181 pylandstats-3.0.0rc2/pylandstats/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/pylandstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:57:25.368181 pylandstats-3.0.0rc2/pylandstats/__pythran__/
+-rw-------   0 runner    (1001) docker     (127)    25243 2024-05-21 12:57:24.000000 pylandstats-3.0.0rc2/pylandstats/__pythran__/landscape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-21 12:57:23.000000 pylandstats-3.0.0rc2/pylandstats/__pythran__/landscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146235 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/pylandstats/landscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/pylandstats/multilandscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/pylandstats/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/pylandstats/spatiotemporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24455 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/pylandstats/zonal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:57:25.368181 pylandstats-3.0.0rc2/pylandstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-21 12:57:25.000000 pylandstats-3.0.0rc2/pylandstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-21 12:57:25.000000 pylandstats-3.0.0rc2/pylandstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:57:25.000000 pylandstats-3.0.0rc2/pylandstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-21 12:57:25.000000 pylandstats-3.0.0rc2/pylandstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 12:57:25.000000 pylandstats-3.0.0rc2/pylandstats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:57:25.368181 pylandstats-3.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:57:25.368181 pylandstats-3.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    61407 2024-05-21 12:57:12.000000 pylandstats-3.0.0rc2/tests/test_pylandstats.py
```

### Comparing `pylandstats-3.0.0rc1/LICENSE` & `pylandstats-3.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylandstats-3.0.0rc1/PKG-INFO` & `pylandstats-3.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pylandstats
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: Computing landscape metrics in the Python ecosystem.
 Author-email: Martí Bosch <marti.bosch@epfl.ch>
 License: GPL-3.0
 Project-URL: Repository, https://github.com/martibosch/pylandstats
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: black
+Requires-Dist: dask
 Requires-Dist: geopandas
 Requires-Dist: matplotlib>=2.2
 Requires-Dist: numba; platform_system == "Windows"
 Requires-Dist: numpy>=1.15
 Requires-Dist: pandas>=0.23
 Requires-Dist: rasterio>=1.0.0
 Requires-Dist: scipy>=1.0.0
```

### Comparing `pylandstats-3.0.0rc1/README.md` & `pylandstats-3.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `pylandstats-3.0.0rc1/pylandstats/__pythran__/landscape.cpp` & `pylandstats-3.0.0rc2/pylandstats/__pythran__/landscape.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 #include <pythonic/include/types/numpy_texpr.hpp>
-#include <pythonic/include/types/int.hpp>
 #include <pythonic/include/types/uint32.hpp>
+#include <pythonic/include/types/int.hpp>
 #include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/types/ndarray.hpp>
-#include <pythonic/types/numpy_texpr.hpp>
 #include <pythonic/types/int.hpp>
 #include <pythonic/types/uint32.hpp>
+#include <pythonic/types/numpy_texpr.hpp>
 #include <pythonic/include/builtins/getattr.hpp>
 #include <pythonic/include/builtins/len.hpp>
 #include <pythonic/include/builtins/list.hpp>
 #include <pythonic/include/builtins/range.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
 #include <pythonic/include/numpy/ndarray/reshape.hpp>
 #include <pythonic/include/numpy/ravel.hpp>
@@ -54,17 +54,16 @@
     struct __transonic__
     {
       typedef void callable;
       typedef void pure;
       struct type
       {
         typedef pythonic::types::str __type0;
-        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-        typedef typename pythonic::returnable<__type1>::type __type2;
-        typedef __type2 result_type;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
       }  ;
       inline
       typename type::result_type operator()() const;
       ;
     }  ;
     struct ADJ_ARR_DTYPE
     {
@@ -172,15 +171,15 @@
       typename type<argument_type0, argument_type1>::result_type operator()(argument_type0 padded_arr, argument_type1 num_classes) const
       ;
     }  ;
     inline
     typename __transonic__::type::result_type __transonic__::operator()() const
     {
       {
-        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.3"));
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::str("0.6.4");
         return tmp_global;
       }
     }
     inline
     typename ADJ_ARR_DTYPE::type::result_type ADJ_ARR_DTYPE::operator()() const
     {
       {
@@ -274,16 +273,16 @@
       __type85 vertical_adjacency_arr = pythonic::numpy::functor::zeros{}(pythonic::numpy::functor::square{}(num_cols_adjacency), ADJ_ARR_DTYPE()());
       __type86 num_cols_pixel = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, padded_arr)));
       __type87 flat_arr = pythonic::numpy::functor::ravel{}(padded_arr);
       typename pythonic::lazy<decltype(__type88({1L, -1L}))>::type horizontal_neighbors = __type88({1L, -1L});
       __type90 vertical_neighbors = __type89({num_cols_pixel, pythonic::operator_::neg(num_cols_pixel)});
       typename pythonic::lazy<decltype(pythonic::operator_::sub(pythonic::builtins::functor::len{}(flat_arr), pythonic::operator_::add(num_cols_pixel, 1L)))>::type end = pythonic::operator_::sub(pythonic::builtins::functor::len{}(flat_arr), pythonic::operator_::add(num_cols_pixel, 1L));
       {
-        long  __target140228695349552 = end;
-        for (long  i=pythonic::operator_::add(num_cols_pixel, 1L); i < __target140228695349552; i += 1L)
+        long  __target140045681642128 = end;
+        for (long  i=pythonic::operator_::add(num_cols_pixel, 1L); i < __target140045681642128; i += 1L)
         {
           typename pythonic::lazy<decltype(pythonic::types::as_const(flat_arr).fast(i))>::type class_i = pythonic::types::as_const(flat_arr).fast(i);
           {
             for (auto&& neighbor: horizontal_neighbors)
             {
               pythonic::types::as_const(horizontal_adjacency_arr)[pythonic::operator_::add(class_i, pythonic::operator_::mul(num_cols_adjacency, pythonic::types::as_const(flat_arr)[pythonic::operator_::add(i, neighbor)]))] += 1L;
             }
@@ -424,28 +423,29 @@
 #if defined(GNUC) && !defined(__clang__)
 __attribute__ ((externally_visible))
 #endif
 #endif
 ;
 PyMODINIT_FUNC
 PYTHRAN_MODULE_INIT(landscape)(void) {
-    import_array()
+    import_array();
+
     #if PY_MAJOR_VERSION >= 3
     PyObject* theModule = PyModule_Create(&moduledef);
     #else
     PyObject* theModule = Py_InitModule3("landscape",
                                          Methods,
                                          ""
     );
     #endif
     if(! theModule)
         PYTHRAN_RETURN;
     PyObject * theDoc = Py_BuildValue("(ss)",
-                                      "0.14.0",
-                                      "8c020df956122206354571a751342102e62061a2edc5ce5aff2daabbd8b872d9");
+                                      "0.16.0",
+                                      "c1cfc6bb43a3092a1c74399f5091b73f45874f56fc33a54908dbd847b0ad8d6f");
     if(! theDoc)
         PYTHRAN_RETURN;
     PyModule_AddObject(theModule,
                        "__pythran__",
                        theDoc);
 
     PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `pylandstats-3.0.0rc1/pylandstats/__pythran__/landscape.py` & `pylandstats-3.0.0rc2/pylandstats/__pythran__/landscape.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,8 +41,8 @@
         for neighbor in vertical_neighbors:
             # adjacency_arr[1, class_i, flat_arr[i + neighbor]] += 1
             vertical_adjacency_arr[class_i +
                                    num_cols_adjacency * flat_arr[i + neighbor]] += 1
     return np.stack((horizontal_adjacency_arr, vertical_adjacency_arr)).reshape((2, num_cols_adjacency, num_cols_adjacency))
 
 
-__transonic__ = ('0.5.3',)
+__transonic__ = "0.6.4"
```

### Comparing `pylandstats-3.0.0rc1/pylandstats/landscape.py` & `pylandstats-3.0.0rc2/pylandstats/landscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
         self.landscape_arr = landscape_arr
         self.cell_width, self.cell_height = res
         self.cell_area = res[0] * res[1]
         self.nodata = nodata
         self.transform = transform
 
-        # set the neigbhor adjacency rule
+        # set the neighbor adjacency rule
         if neighborhood_rule is None:
             neighborhood_rule = settings.DEFAULT_NEIGHBORHOOD_RULE
         elif isinstance(neighborhood_rule, int):
             neighborhood_rule = str(neighborhood_rule)
         if neighborhood_rule not in ("8", "4"):
             raise ValueError("`neighborhood_rule` is not among ('8', '4')")
         self.neighborhood_rule = neighborhood_rule
@@ -252,19 +252,23 @@
         "fractal_dimension",
         "core_area",
         "number_of_core_areas",
         "core_area_index",
         "euclidean_nearest_neighbor",
     ]  # 'contiguity_index', 'proximity'
 
-    # iterate all patch metrics except "number_of_core_areas"
+    # iterate all patch metrics except "number_of_core_areas", and add
+    # "disjunct_core_area"
     _PATCH_METRICS = PATCH_METRICS.copy()
     _PATCH_METRICS.remove("number_of_core_areas")
+    _PATCH_METRICS.append("disjunct_core_area")
+    # we could define the list of suffixes as a class-constant but using it in settings
+    # would cause a singular import
     DISTR_METRICS = [
-        patch_metric + "_" + suffix
+        f"{patch_metric}_{suffix}"
         for patch_metric in _PATCH_METRICS
         for suffix in ["mn", "am", "md", "ra", "sd", "cv"]
     ]
 
     CLASS_METRICS = [
         "total_area",
         "proportion_of_landscape",
@@ -764,90 +768,90 @@
 
     # metric distribution statistics
 
     def _metric_reduce(
         self,
         class_val,
         patch_metric_method,
-        patch_metric_method_kws,
+        patch_metric_method_kwargs,
         reduce_method,
     ):
-        if patch_metric_method_kws is None:
+        if patch_metric_method_kwargs is None:
             patch_metrics = patch_metric_method(class_val=class_val)
         else:
             patch_metrics = patch_metric_method(
-                class_val=class_val, **patch_metric_method_kws
+                class_val=class_val, **patch_metric_method_kwargs
             )
         if class_val is None:
             # ACHTUNG: dropping columns from a `pd.DataFrame` until leaving it with only
             # one column will still return a `pd.DataFrame`, so we must convert to
             # `pd.Series` manually (e.g., with `iloc`)
             patch_metrics = patch_metrics.drop("class_val", axis=1).iloc[:, 0]
 
         return reduce_method(patch_metrics)
 
     def _metric_mn(
-        self, class_val, patch_metric_method, *, patch_metric_method_kws=None
+        self, class_val, patch_metric_method, *, patch_metric_method_kwargs=None
     ):
         return self._metric_reduce(
-            class_val, patch_metric_method, patch_metric_method_kws, np.mean
+            class_val, patch_metric_method, patch_metric_method_kwargs, np.mean
         )
 
     def _metric_am(
-        self, class_val, patch_metric_method, *, patch_metric_method_kws=None
+        self, class_val, patch_metric_method, *, patch_metric_method_kwargs=None
     ):
         # `area` can be `pd.Series` or `pd.DataFrame`
         area = self.area(class_val=class_val)
 
         if class_val is None:
             area = area["area"]
 
         return self._metric_reduce(
             class_val,
             patch_metric_method,
-            patch_metric_method_kws,
+            patch_metric_method_kwargs,
             functools.partial(np.average, weights=area),
         )
 
     def _metric_md(
-        self, class_val, patch_metric_method, *, patch_metric_method_kws=None
+        self, class_val, patch_metric_method, *, patch_metric_method_kwargs=None
     ):
         return self._metric_reduce(
-            class_val, patch_metric_method, patch_metric_method_kws, np.median
+            class_val, patch_metric_method, patch_metric_method_kwargs, np.median
         )
 
     def _metric_ra(
-        self, class_val, patch_metric_method, *, patch_metric_method_kws=None
+        self, class_val, patch_metric_method, *, patch_metric_method_kwargs=None
     ):
         return self._metric_reduce(
             class_val,
             patch_metric_method,
-            patch_metric_method_kws,
-            lambda ser: ser.max() - ser.min(),
+            patch_metric_method_kwargs,
+            lambda metric_ser: metric_ser.max() - metric_ser.min(),
         )
 
     def _metric_sd(
-        self, class_val, patch_metric_method, *, patch_metric_method_kws=None
+        self, class_val, patch_metric_method, *, patch_metric_method_kwargs=None
     ):
         return self._metric_reduce(
-            class_val, patch_metric_method, patch_metric_method_kws, np.std
+            class_val, patch_metric_method, patch_metric_method_kwargs, np.std
         )
 
     def _metric_cv(
         self,
         class_val,
         patch_metric_method,
         *,
-        patch_metric_method_kws=None,
+        patch_metric_method_kwargs=None,
         percent=True,
     ):
         metric_cv = self._metric_reduce(
             class_val,
             patch_metric_method,
-            patch_metric_method_kws,
+            patch_metric_method_kwargs,
             stats.variation,
         )
         if percent:
             metric_cv *= 100
 
         return metric_cv
 
@@ -1608,15 +1612,15 @@
                     ]:
                         adjacency_arr = np.triu(
                             self._adjacency_df.loc[direction]
                             .drop(self.nodata)
                             .drop(self.nodata, axis=1)
                         )
                         # `np.fill_diagonal` acts inplace, however `np.triu` returns a
-                        # copy so we do not need to worry about inadvently modfying
+                        # copy so we do not need to worry about inadvently modifying
                         # `self._adjacency_df`
                         np.fill_diagonal(adjacency_arr, 0)
                         total_edge += np.sum(adjacency_arr) * length
         else:
             if count_boundary:
                 # then the total edge is just the sum of the perimeters of all the
                 # patches of the corresponding class
@@ -1704,15 +1708,15 @@
             more legible values).
 
         Returns
         -------
         AREA_MN : numeric
         """
         return self._metric_mn(
-            class_val, self.area, patch_metric_method_kws={"hectares": hectares}
+            class_val, self.area, patch_metric_method_kwargs={"hectares": hectares}
         )
 
     def area_am(self, *, class_val=None, hectares=True):
         """Area-weighted mean of the patch area distribution.
 
         See also the documentation of `area`.
 
@@ -1726,15 +1730,15 @@
             more legible values).
 
         Returns
         -------
         AREA_AM : numeric
         """
         return self._metric_am(
-            class_val, self.area, patch_metric_method_kws={"hectares": hectares}
+            class_val, self.area, patch_metric_method_kwargs={"hectares": hectares}
         )
 
     def area_md(self, *, class_val=None, hectares=True):
         """Median of the patch area distribution.
 
         See also the documentation of `area`.
 
@@ -1748,15 +1752,15 @@
             more legible values).
 
         Returns
         -------
         AREA_MD : numeric
         """
         return self._metric_md(
-            class_val, self.area, patch_metric_method_kws={"hectares": hectares}
+            class_val, self.area, patch_metric_method_kwargs={"hectares": hectares}
         )
 
     def area_ra(self, *, class_val=None, hectares=True):
         """Range of the patch area distribution.
 
         See also the documentation of `area`.
 
@@ -1770,15 +1774,15 @@
             more legible values).
 
         Returns
         -------
         AREA_RA : numeric
         """
         return self._metric_ra(
-            class_val, self.area, patch_metric_method_kws={"hectares": hectares}
+            class_val, self.area, patch_metric_method_kwargs={"hectares": hectares}
         )
 
     def area_sd(self, *, class_val=None, hectares=True):
         """Standard deviation of the patch area distribution.
 
         See also the documentation of `area`.
 
@@ -1792,15 +1796,15 @@
             more legible values).
 
         Returns
         -------
         AREA_SD : numeric
         """
         return self._metric_sd(
-            class_val, self.area, patch_metric_method_kws={"hectares": hectares}
+            class_val, self.area, patch_metric_method_kwargs={"hectares": hectares}
         )
 
     def area_cv(self, *, class_val=None, percent=True):
         """Coefficient of variation of the patch area distribution.
 
         See also the documentation of `area`.
 
@@ -1943,15 +1947,15 @@
         Returns
         -------
         PARA_MN : numeric
         """
         return self._metric_mn(
             class_val,
             self.perimeter_area_ratio,
-            patch_metric_method_kws={"hectares": hectares},
+            patch_metric_method_kwargs={"hectares": hectares},
         )
 
     def perimeter_area_ratio_am(self, *, class_val=None, hectares=True):
         """Area-weighted mean of the patch perimeter-area ratio distribution.
 
         See also the documentation of `perimeter_area_ratio`.
 
@@ -1967,15 +1971,15 @@
         Returns
         -------
         PARA_AM : numeric
         """
         return self._metric_am(
             class_val,
             self.perimeter_area_ratio,
-            patch_metric_method_kws={"hectares": hectares},
+            patch_metric_method_kwargs={"hectares": hectares},
         )
 
     def perimeter_area_ratio_md(self, *, class_val=None, hectares=True):
         """Median of the patch perimeter-area ratio distribution.
 
         See also the documentation of `perimeter_area_ratio`.
 
@@ -1991,15 +1995,15 @@
         Returns
         -------
         PARA_MD : numeric
         """
         return self._metric_md(
             class_val,
             self.perimeter_area_ratio,
-            patch_metric_method_kws={"hectares": hectares},
+            patch_metric_method_kwargs={"hectares": hectares},
         )
 
     def perimeter_area_ratio_ra(self, *, class_val=None, hectares=True):
         """Range of the patch perimeter-area ratio distribution.
 
         See also the documentation of `perimeter_area_ratio`.
 
@@ -2015,15 +2019,15 @@
         Returns
         -------
         PARA_RA : numeric
         """
         return self._metric_ra(
             class_val,
             self.perimeter_area_ratio,
-            patch_metric_method_kws={"hectares": hectares},
+            patch_metric_method_kwargs={"hectares": hectares},
         )
 
     def perimeter_area_ratio_sd(self, *, class_val=None, hectares=True):
         """Standard deviation of the patch perimeter-area ratio distribution.
 
         See also the documentation of `perimeter_area_ratio`.
 
@@ -2039,15 +2043,15 @@
         Returns
         -------
         PARA_SD : numeric
         """
         return self._metric_sd(
             class_val,
             self.perimeter_area_ratio,
-            patch_metric_method_kws={"hectares": hectares},
+            patch_metric_method_kwargs={"hectares": hectares},
         )
 
     def perimeter_area_ratio_cv(self, *, class_val=None, percent=True):
         """Coefficient of variation of the patch perimeter-area ratio distribution.
 
         See also the documentation of `perimeter_area_ratio`.
 
@@ -2601,15 +2605,15 @@
         Returns
         -------
         CORE_MN : numeric
         """
         return self._metric_mn(
             class_val,
             self.core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "hectares": hectares,
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_am(
@@ -2636,15 +2640,15 @@
         Returns
         -------
         CORE_AM : numeric
         """
         return self._metric_am(
             class_val,
             self.core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "hectares": hectares,
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_md(
@@ -2671,15 +2675,15 @@
         Returns
         -------
         CORE_MD : numeric
         """
         return self._metric_md(
             class_val,
             self.core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "hectares": hectares,
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_ra(
@@ -2706,15 +2710,15 @@
         Returns
         -------
         CORE_RA : numeric
         """
         return self._metric_ra(
             class_val,
             self.core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "hectares": hectares,
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_sd(
@@ -2741,15 +2745,15 @@
         Returns
         -------
         CORE_SD : numeric
         """
         return self._metric_sd(
             class_val,
             self.core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "hectares": hectares,
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_cv(
@@ -2776,15 +2780,15 @@
         Returns
         -------
         CORE_CV : numeric
         """
         return self._metric_cv(
             class_val,
             self.core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
             percent=percent,
         )
 
     def _disjunct_core_area(
@@ -2845,15 +2849,15 @@
         Returns
         -------
         CORE_MN : numeric
         """
         return self._metric_mn(
             class_val,
             self._disjunct_core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "hectares": hectares,
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def disjunct_core_area_am(
@@ -2885,15 +2889,18 @@
         # disjunct core area rather than the patch area, so we will not use `_metric_am`
         disjunct_core_area = self._disjunct_core_area(
             class_val=class_val,
             hectares=hectares,
             count_boundary=count_boundary,
             edge_depth=edge_depth,
         )
-        return np.average(disjunct_core_area, weights=disjunct_core_area)
+        try:
+            return np.average(disjunct_core_area, weights=disjunct_core_area)
+        except ZeroDivisionError:
+            return np.nan
 
     def disjunct_core_area_md(
         self, *, class_val=None, hectares=True, count_boundary=True, edge_depth=1
     ):
         """Median of the core area per disjunct core distribution.
 
         See also the documentation of `Landscape.core_area`.
@@ -2915,15 +2922,15 @@
         Returns
         -------
         CORE_MD : numeric
         """
         return self._metric_md(
             class_val,
             self._disjunct_core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "hectares": hectares,
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def disjunct_core_area_ra(
@@ -2950,15 +2957,15 @@
         Returns
         -------
         CORE_RA : numeric
         """
         return self._metric_ra(
             class_val,
             self._disjunct_core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "hectares": hectares,
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def disjunct_core_area_sd(
@@ -2985,15 +2992,15 @@
         Returns
         -------
         CORE_SD : numeric
         """
         return self._metric_sd(
             class_val,
             self._disjunct_core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "hectares": hectares,
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def disjunct_core_area_cv(
@@ -3020,15 +3027,15 @@
         Returns
         -------
         CORE_CV : numeric
         """
         return self._metric_cv(
             class_val,
             self._disjunct_core_area,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
             percent=percent,
         )
 
     def core_area_index_mn(self, *, class_val=None, count_boundary=True, edge_depth=1):
@@ -3050,15 +3057,15 @@
         Returns
         -------
         CAI_MN : numeric
         """
         return self._metric_mn(
             class_val,
             self.core_area_index,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_index_am(self, *, class_val=None, count_boundary=True, edge_depth=1):
         """Area-weighted mean of the core area index distribution.
@@ -3079,15 +3086,15 @@
         Returns
         -------
         CAI_AM : numeric
         """
         return self._metric_am(
             class_val,
             self.core_area_index,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_index_md(self, *, class_val=None, count_boundary=True, edge_depth=1):
         """Median of the core area index distribution.
@@ -3108,15 +3115,15 @@
         Returns
         -------
         CAI_MD : numeric
         """
         return self._metric_md(
             class_val,
             self.core_area_index,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_index_ra(self, *, class_val=None, count_boundary=True, edge_depth=1):
         """Range of the core area index distribution.
@@ -3137,15 +3144,15 @@
         Returns
         -------
         CAI_RA : numeric
         """
         return self._metric_ra(
             class_val,
             self.core_area_index,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_index_sd(self, *, class_val=None, count_boundary=True, edge_depth=1):
         """Standard deviation of the core area index distribution.
@@ -3166,15 +3173,15 @@
         Returns
         -------
         CAI_SD : numeric
         """
         return self._metric_sd(
             class_val,
             self.core_area_index,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
         )
 
     def core_area_index_cv(
         self, *, class_val=None, count_boundary=True, edge_depth=1, percent=True
@@ -3200,15 +3207,15 @@
         Returns
         -------
         CAI_CV : numeric
         """
         return self._metric_cv(
             class_val,
             self.core_area_index,
-            patch_metric_method_kws={
+            patch_metric_method_kwargs={
                 "count_boundary": count_boundary,
                 "edge_depth": edge_depth,
             },
             percent=percent,
         )
 
     # isolation, proximity
@@ -3318,15 +3325,15 @@
         -------
         PROX_CV : numeric
         """
         # TODO
         raise NotImplementedError
 
     def euclidean_nearest_neighbor_mn(self, *, class_val=None):
-        """Mean of the Euclidean nearest neigbhor distribution.
+        """Mean of the Euclidean nearest neighbor distribution.
 
         See also the documentation of `Landscape.euclidean_nearest_neighbor`.
 
         Parameters
         ----------
         class_val : int, optional
             If provided, the metric will be computed at the level of the corresponding
@@ -3573,16 +3580,16 @@
         ENT : numeric
             0 <= ENT <= log_b(m) ; ENT approaches 0 when the entire landscape consists
             of a single patch, and approaches its maximum value, i.e., log_b(m), as the
             distribution of area among classes becomes more equitable.
         """
         if len(self.classes) < 2:
             warnings.warn(
-                "Entropy-based metrics can only be computed in landscapes with more "
-                "than two classes of patches. Returning nan",
+                "Entropy-based metrics can only be computed in landscapes with at least"
+                " two classes of patches. Returning nan",
                 RuntimeWarning,
             )
             return np.nan
 
         # sum along column to get counts of each class
         counts = self.compute_total_adjacency_df().sum()
 
@@ -3637,16 +3644,16 @@
             0 < JOINENT <= 2 log_b(m) ; JOINENT approaches 0 when the landscape consists
             of a single patch, and approaches its maximum value when the classes are
             maximally disaggregated (i.e., every cell is a patch of a different class)
             and interspersed (i.e., equal proportions of all pairwise adjacencies).
         """
         if len(self.classes) < 2:
             warnings.warn(
-                "Entropy-based metrics can only be computed in landscapes with more "
-                "than two classes of patches. Returning nan",
+                "Entropy-based metrics can only be computed in landscapes with at least"
+                " two classes of patches. Returning nan",
                 RuntimeWarning,
             )
             return np.nan
 
         # this would be the "adjacency vector"
         adjacencies = self.compute_total_adjacency_df().values.flatten()
 
@@ -3755,50 +3762,50 @@
             contag *= 100
 
         return contag
 
     ###########################################################################
     # compute metrics data frames
 
-    def compute_patch_metrics_df(self, *, metrics=None, metrics_kws=None):
+    def compute_patch_metrics_df(self, *, metrics=None, metrics_kwargs=None):
         """Compute patch-level metrics.
 
         Parameters
         ----------
         metrics : list-like, optional
             A list-like of strings with the names of the metrics that should be
             computed. If `None`, all the implemented patch-level metrics will be
             computed.
-        metrics_kws : dict, default None
+        metrics_kwargs : dict, default None
             Dictionary mapping the keyword arguments (values) that should be passed to
             each metric method (key), e.g., to compute `area` in meters instead of
-            hectares, metric_kws should map the string 'area' (method name) to
+            hectares, metric_kwargs should map the string 'area' (method name) to
             {'hectares': False}. If `None`, each metric will be computed according to
             FRAGSTATS defaults.
 
         Returns
         -------
         df : pandas.DataFrame
             Dataframe with the values computed for each patch (index) and metric
             (columns).
         """
         if metrics is None:
             metrics = Landscape.PATCH_METRICS
 
-        if metrics_kws is None:
-            metrics_kws = {}
+        if metrics_kwargs is None:
+            metrics_kwargs = {}
 
         metrics_dfs = [self._patch_class_ser]
         for metric in metrics:
-            if metric in metrics_kws:
-                metric_kws = metrics_kws[metric]
+            if metric in metrics_kwargs:
+                metric_kwargs = metrics_kwargs[metric]
             else:
-                metric_kws = {}
+                metric_kwargs = {}
             try:
-                metric_val = getattr(self, metric)(**metric_kws)
+                metric_val = getattr(self, metric)(**metric_kwargs)
             except AttributeError as getattr_e:
                 raise ValueError(
                     "{metric} is not among {Landscape.PATCH_METRICS}"
                 ) from getattr_e
             except TypeError as metric_args_e:
                 raise ValueError(
                     "{metric} cannot be computed at the patch level".format(
@@ -3815,31 +3822,33 @@
                 ) from drop_e
 
         df = pd.concat(metrics_dfs, axis=1)  # [['class_val'] + patch_metrics]
         df.index.name = "patch_id"
 
         return df
 
-    def compute_class_metrics_df(self, *, metrics=None, classes=None, metrics_kws=None):
+    def compute_class_metrics_df(
+        self, *, metrics=None, classes=None, metrics_kwargs=None
+    ):
         """Compute class-level metrics.
 
         Parameters
         ----------
         metrics : list-like, optional
             A list-like of strings with the names of the metrics that should be
             computed. If `None`, all the implemented class-level metrics will be
             computed.
         classes : list-like, optional
             A list-like of ints or strings with the class values that should be
             considered in the context of this analysis case.
-        metrics_kws : dict, optional
+        metrics_kwargs : dict, optional
             Dictionary mapping the keyword arguments (values) that should be passed to
             each metric method (key), e.g., to exclude the boundary from the computation
-            of `total_edge`, metric_kws should map the string 'total_edge' (method name)
-            to {'count_boundary': False}. If `None`, each metric will be computed
+            of `total_edge`, metric_kwargs should map the string 'total_edge' (method
+            name) to {'count_boundary': False}. If `None`, each metric will be computed
             according to FRAGSTATS defaults.
 
         Returns
         -------
         df : pandas.DataFrame
             Dataframe with the values computed for each class (index) and metric
             (columns).
@@ -3860,30 +3869,30 @@
                             metric=metric
                         )
                     )
 
         if classes is None:
             classes = self.classes
 
-        if metrics_kws is None:
-            metrics_kws = {}
+        if metrics_kwargs is None:
+            metrics_kwargs = {}
 
         try:
             metrics_sers = []
             for metric in metrics:
-                if metric in metrics_kws:
-                    metric_kws = metrics_kws[metric]
+                if metric in metrics_kwargs:
+                    metric_kwargs = metrics_kwargs[metric]
                 else:
-                    metric_kws = {}
+                    metric_kwargs = {}
 
                 metrics_sers.append(
                     pd.Series(
                         {
                             class_val: getattr(self, metric)(
-                                class_val=class_val, **metric_kws
+                                class_val=class_val, **metric_kwargs
                             )
                             for class_val in classes
                         },
                         name=metric,
                     )
                 )
 
@@ -3899,51 +3908,51 @@
             ) from metric_args_e
 
         df = pd.concat(metrics_sers, axis=1)
         df.index.name = "class_val"
 
         return df
 
-    def compute_landscape_metrics_df(self, *, metrics=None, metrics_kws=None):
+    def compute_landscape_metrics_df(self, *, metrics=None, metrics_kwargs=None):
         """Compute landscape-level metrics.
 
         Parameters
         ----------
         metrics : list-like, optional
             A list-like of strings with the names of the metrics that should be
             computed. If `None`, all the implemented landscape-level metrics will be
             computed.
-        metrics_kws : dict, optional
+        metrics_kwargs : dict, optional
             Dictionary mapping the keyword arguments (values) that should be passed to
             each metric method (key), e.g., to exclude the boundary from the computation
-            of `total_edge`, metric_kws should map the string 'total_edge' (method name)
-            to {'count_boundary': False}. If `None`, each metric will be computed
+            of `total_edge`, metric_kwargs should map the string 'total_edge' (method
+            name) to {'count_boundary': False}. If `None`, each metric will be computed
             according to FRAGSTATS defaults.
 
         Returns
         -------
         df : pandas.DataFrame
             Dataframe with the values computed at the landscape level (one row only) for
             each metric (columns).
         """
         if metrics is None:
             metrics = Landscape.LANDSCAPE_METRICS
 
-        if metrics_kws is None:
-            metrics_kws = {}
+        if metrics_kwargs is None:
+            metrics_kwargs = {}
 
         try:
             metrics_dict = {}
             for metric in metrics:
-                if metric in metrics_kws:
-                    metric_kws = metrics_kws[metric]
+                if metric in metrics_kwargs:
+                    metric_kwargs = metrics_kwargs[metric]
                 else:
-                    metric_kws = {}
+                    metric_kwargs = {}
 
-                metrics_dict[metric] = getattr(self, metric)(**metric_kws)
+                metrics_dict[metric] = getattr(self, metric)(**metric_kwargs)
 
         except AttributeError:
             raise ValueError(
                 "{metric} is not among {metrics}".format(
                     metric=metric, metrics=Landscape.LANDSCAPE_METRICS
                 )
             )
@@ -3972,16 +3981,16 @@
     def plot_landscape(
         self,
         *,
         cmap=None,
         ax=None,
         legend=False,
         figsize=None,
-        legend_kws=None,
-        **show_kws,
+        legend_kwargs=None,
+        **show_kwargs,
     ):
         """Plot the landscape with a categorical legend.
 
         Uses `rasterio.plot.show`.
 
         Parameters
         ----------
@@ -3989,17 +3998,17 @@
             A Colormap instance.
         ax : axis object, optional
             Plot in given axis; if `None` creates a new figure.
         legend : bool, optional
             If `True`, display the legend.
         figsize : tuple of two numeric types, optional
             Size of the figure to create. Ignored if axis `ax` is provided.
-        legend_kws : optional
+        legend_kwargs : optional
             Keyword arguments to be passed to `matplotlib.axes.Axes.legend`.
-        **show_kws : optional
+        **show_kwargs : optional
             Keyword arguments to be passed to `rasterio.plot.show`.
 
         Returns
         -------
         ax : matplotlib.axes.Axes
             Returns the `Axes` object with the plot drawn onto it.
         """
@@ -4018,25 +4027,25 @@
                 self.landscape_arr != self.nodata,
                 self.landscape_arr,
                 self.nodata,
             ),
             ax=ax,
             transform=self.transform,
             cmap=cmap,
-            **show_kws,
+            **show_kwargs,
         )
 
         if legend:
             im = ax.get_images()[0]
             # get the colors of the values, according to the colormap used by imshow
             colors = [im.cmap(im.norm(class_val)) for class_val in self.classes]
             # create a patch (proxy artist) for every color
             patches = [
                 mpatches.Patch(color=colors[i], label=f"{class_val}")
                 for i, class_val in enumerate(self.classes)
             ]
             # put those patched as legend-handles into the legend
-            if legend_kws is None:
-                legend_kws = {}
-            ax.legend(handles=patches, **legend_kws)
+            if legend_kwargs is None:
+                legend_kwargs = {}
+            ax.legend(handles=patches, **legend_kwargs)
 
         return ax
```

### Comparing `pylandstats-3.0.0rc1/pylandstats/multilandscape.py` & `pylandstats-3.0.0rc2/pylandstats/multilandscape.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Multi-landscape analysis."""
+
 import abc
 import functools
 
+import dask
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from dask import diagnostics
 
 from . import settings
 from .landscape import Landscape
 
 _compute_class_metrics_df_doc = """
 Compute the data frame of class-level metrics, which is {index_descr}.
 
@@ -16,24 +19,24 @@
 ----------
 metrics : list-like, optional
     A list-like of strings with the names of the metrics that should be computed in the
     context of this analysis case.
 classes : list-like, optional
     A list-like of ints or strings with the class values that should be considered in
     the context of this analysis case.
-metrics_kws : dict, optional
+metrics_kwargs : dict, optional
     Dictionary mapping the keyword arguments (values) that should be passed to each
     metric method (key), e.g., to exclude the boundary from the computation of
-    `total_edge`, metric_kws should map the string 'total_edge' (method name) to
+    `total_edge`, metric_kwargs should map the string 'total_edge' (method name) to
     {{'count_boundary': False}}. The default empty dictionary will compute each metric
     according to FRAGSTATS defaults.
 fillna : bool, optional
     Whether `NaN` values representing landscapes with no occurrences of patches of the
     provided class should be replaced by zero when appropriate, e.g., area and edge
-    metrics (no ocurrences mean zero area/edge). If the provided value is `None`
+    metrics (no occurrences mean zero area/edge). If the provided value is `None`
     (default), the value will be taken from `settings.CLASS_METRICS_DF_FILLNA`.
 
 Returns
 -------
 df : pandas.DataFrame
     Dataframe with the values computed for each {index_return} and metric (columns).
 """
@@ -42,18 +45,18 @@
 Computes the data frame of landscape-level metrics, which is {index_descr}.
 
 Parameters
 ----------
 metrics : list-like, optional
     A list-like of strings with the names of the metrics that should be computed. If
     `None`, all the implemented landscape-level metrics will be computed.
-metrics_kws : dict, optional
+metrics_kwargs : dict, optional
     Dictionary mapping the keyword arguments (values) that should be passed to each
     metric method (key), e.g., to exclude the boundary from the computation of
-    `total_edge`, metric_kws should map the string 'total_edge' (method name) to
+    `total_edge`, metric_kwargs should map the string 'total_edge' (method name) to
     {{'count_boundary': False}}. The default empty dictionary will compute each metric
     according to FRAGSTATS defaults.
 
 Returns
 -------
 df : pandas.DataFrame
     Dataframe with the values computed at the landscape level for each {index_return}
@@ -61,63 +64,59 @@
 """
 
 
 class MultiLandscape(abc.ABC):
     """Multi-landscape base abstract class."""
 
     @abc.abstractmethod
-    def __init__(self, landscapes, attribute_name, attribute_values, **landscape_kws):
+    def __init__(
+        self, landscapes, attribute_name, attribute_values, **landscape_kwargs
+    ):
         """Initialize the multi-landscape instance.
 
         Parameters
         ----------
         landscapes : list-like
             A list-like of `Landscape` instances or of strings/file-like/pathlib.Path
             objects so that each is passed as the `landscape` argument of
             `Landscape.__init__`.
         attribute_name : str
             Name of the attribute that will distinguish each landscape.
         attribute_values : list-like
             Values of the attribute that are characteristic to each landscape.
-        landscape_kws : dict, optional
+        landscape_kwargs : dict, optional
             Keyword arguments to be passed to the instantiation of
             `pylandstats.Landscape` for each element of `landscapes`. Ignored if the
             elements of `landscapes` are already instances of `pylandstats.Landcape`.
         """
-        if isinstance(landscapes[0], Landscape):
-            self.landscapes = landscapes
-        else:
-            self.landscapes = [
-                Landscape(landscape, **landscape_kws) for landscape in landscapes
+        if not isinstance(landscapes[0], Landscape):
+            # we assume that landscapes is a list of strings/file-like/path-like objects
+            landscapes = [
+                Landscape(landscape, **landscape_kwargs) for landscape in landscapes
             ]
-
-        if len(self.landscapes) != len(attribute_values):
+        if len(landscapes) != len(attribute_values):
             raise ValueError(
                 "The lengths of `landscapes` and `{}` must coincide".format(
                     attribute_name
                 )
             )
 
-        # set a `attribute_name` attribute with the value `attribute_values`, so that
-        # children classes can access it (e.g., for `SpatioTemporalAnalysis`,
-        # `attribute_name` will be 'dates' and `attribute_values` will be a list of
-        # dates that will therefore be accessible as an attribute as in `instance.dates`
-        setattr(self, attribute_name, attribute_values)
-        # also set a `attribute_name` attribute so that the methods of this class know
-        # how to access such attribute, i.e., as in `getattr(self, self.attribute_name)`
-        setattr(self, "attribute_name", attribute_name)
+        # at this point, landscapes is a list of pylandstats.Landscape instances
+        self.landscape_ser = pd.Series(landscapes, index=attribute_values).rename_axis(
+            attribute_name
+        )
 
         # get the all classes present in the provided landscapes
         self.present_classes = functools.reduce(
             np.union1d,
-            tuple(landscape.classes for landscape in self.landscapes),
+            tuple(landscape.classes for landscape in self.landscape_ser),
         )
 
     # fillna for metrics in class metrics dataframes. Since some classes might not
-    # apprear in some of the landscapes (e.g., zones or temporal snapshots without any
+    # appear in some of the landscapes (e.g., zones or temporal snapshots without any
     # pixel of a particular class type), they will appear as `NaN` in the data frame. We
     # can, however, infer the meaning of this situation for certain metrics, e.g,
     # non-occurence of a given class in a landscape means a number of patches, total
     # area, proportion of landscape, total edge... of the class of 0
     METRIC_FILLNA_DICT = {
         metric: 0
         for metric in [
@@ -134,111 +133,124 @@
             "total_edge",
             "edge_density",
             "total_core_area",
         ]
     }
 
     def __len__(self):  # noqa: D105
-        return len(self.landscapes)
+        return len(self.landscape_ser)
 
     def compute_class_metrics_df(  # noqa: D102
-        self, *, metrics=None, classes=None, metrics_kws=None, fillna=None
+        self, *, metrics=None, classes=None, metrics_kwargs=None, fillna=None
     ):
-        attribute_values = getattr(self, self.attribute_name)
-
-        # get the columns to init the data frame
-        if metrics is None:
-            columns = Landscape.CLASS_METRICS
-        else:
-            columns = metrics
         # if the classes kwarg is not provided, get the classes present in the
         # landscapes
         if classes is None:
             classes = self.present_classes
         # to avoid issues with mutable defaults
-        if metrics_kws is None:
-            metrics_kws = {}
+        if metrics_kwargs is None:
+            metrics_kwargs = {}
         # to avoid setting the same default keyword argument in multiple methods, use
         # the settings module
         if fillna is None:
             fillna = settings.CLASS_METRICS_DF_FILLNA
 
-        # IMPORTANT: here we need this approach (uglier when compared to the
-        # `compute_landscape_metrics_df` method below) because we need to filter each
-        # class metrics data frame so that we only include the classes considered in
-        # this `MultiLandscape` instance. We need to do it like this because the
-        # `Landcape.compute_class_metrics_df` does not have a `classes` argument that
-        # allows computing the data frame only for a custom set of classes. Should such
-        # `classes` argument be added at some point, we could use the approach of the
-        # `compute_landscape_metrics_df` method below.
-        # TODO: one-level index if only one class?
-        class_metrics_df = pd.DataFrame(
-            index=pd.MultiIndex.from_product([classes, attribute_values]),
-            columns=columns,
-        )
-
-        class_metrics_df.index.names = "class_val", self.attribute_name
-        class_metrics_df.columns.name = "metric"
+        tasks = [
+            dask.delayed(landscape.compute_class_metrics_df)(
+                metrics=metrics,
+                classes=np.intersect1d(classes, landscape.classes),
+                metrics_kwargs=metrics_kwargs,
+            )
+            for landscape in self.landscape_ser
+        ]
+        with diagnostics.ProgressBar():
+            dfs = dask.compute(*tasks)
 
-        for attribute_value, landscape in zip(attribute_values, self.landscapes):
-            # get the class metrics DataFrame for the landscape that corresponds to this
-            # attribute value
-            df = landscape.compute_class_metrics_df(
-                metrics=metrics, metrics_kws=metrics_kws
+        names = self.landscape_ser.index.names
+        # get the landscape series index and if not a multi-index, reshape it so that it
+        # the list comprehensions below work for both one-dimensional and multi index
+        landscape_index = self.landscape_ser.index.values
+        if len(names) == 1:
+            landscape_index = landscape_index.reshape(-1, 1)
+        class_metrics_df = (
+            pd.concat(
+                [
+                    df.assign(
+                        **{
+                            name: val if isinstance(i, tuple) else i[0]
+                            for name, val in zip(names, i)
+                        }
+                    )
+                    for i, df in zip(landscape_index, dfs)
+                ]
+            )
+            .set_index(names, append=True)
+            # only sort the first level, i.e., class val
+            .sort_index(level="class_val")
+        )
+        # then reindex to sort the other indices as they were originally sorted
+        # TODO: this is probably only needed for "zones" - not for dates, since we
+        # probably do not want to alphabetically sort zone labels but we probably want
+        # to sort dates. In any case, avoid premature optimization: we assume that the
+        # costs of sorting the metrics data frames are negligible
+        for name in self.landscape_ser.index.names:
+            class_metrics_df = class_metrics_df.reindex(
+                self.landscape_ser.index.get_level_values(name).unique(), level=name
             )
-            # filter so we only check the classes considered in this `MultiLandscape`
-            # instance
-            df = df.loc[df.index.intersection(classes)]
-            # put every row of the filtered DataFrame of this particular attribute value
-            for class_val, row in df.iterrows():
-                class_metrics_df.loc[(class_val, attribute_value), columns] = row
 
+        # ensure numeric types and fillna
         class_metrics_df = class_metrics_df.apply(pd.to_numeric)
         if fillna:
             class_metrics_df = class_metrics_df.fillna(
                 MultiLandscape.METRIC_FILLNA_DICT
             )
         return class_metrics_df
 
     compute_class_metrics_df.__doc__ = _compute_class_metrics_df_doc.format(
         index_descr="multi-indexed by the class and attribute value",
         index_return="class, attribute value (multi-index)",
     )
 
     def compute_landscape_metrics_df(  # noqa: D102
-        self, *, metrics=None, metrics_kws=None
+        self, *, metrics=None, metrics_kwargs=None
     ):
-        attribute_values = getattr(self, self.attribute_name)
-
-        # get the columns to init the data frame
-        if metrics is None:
-            columns = Landscape.LANDSCAPE_METRICS
-        else:
-            columns = metrics
         # to avoid issues with mutable defaults
-        if metrics_kws is None:
-            metrics_kws = {}
+        if metrics_kwargs is None:
+            metrics_kwargs = {}
 
-        if isinstance(attribute_values[0], tuple):
-            # for the zonal statistics analysis mainly
-            index = pd.MultiIndex.from_tuples(attribute_values)
-        else:
-            index = attribute_values
-        landscape_metrics_df = pd.DataFrame(index=index, columns=columns)
-        landscape_metrics_df.index.name = self.attribute_name
-        landscape_metrics_df.columns.name = "metric"
-
-        for attribute_value, landscape in zip(attribute_values, self.landscapes):
-            landscape_metrics_df.loc[
-                attribute_value, columns
-            ] = landscape.compute_landscape_metrics_df(
-                metrics=metrics, metrics_kws=metrics_kws
-            ).iloc[
-                0
-            ]
+        tasks = [
+            dask.delayed(landscape.compute_landscape_metrics_df)(
+                metrics=metrics, metrics_kwargs=metrics_kwargs
+            )
+            for landscape in self.landscape_ser
+        ]
+        with diagnostics.ProgressBar():
+            dfs = dask.compute(*tasks)
+
+        names = self.landscape_ser.index.names
+        # get the landscape series index and if not a multi-index, reshape it so that it
+        # the list comprehensions below work for both one-dimensional and multi index
+        landscape_index = self.landscape_ser.index.values
+        if len(names) == 1:
+            landscape_index = landscape_index.reshape(-1, 1)
+        landscape_metrics_df = (
+            pd.concat(
+                [
+                    df.assign(
+                        **{
+                            name: val if isinstance(i, tuple) else i[0]
+                            for name, val in zip(names, i)
+                        }
+                    )
+                    for i, df in zip(landscape_index, dfs)
+                ]
+            ).set_index(names)
+            # there is no need to sort here
+            # .sort_index()
+        )
 
         return landscape_metrics_df.apply(pd.to_numeric)
 
     compute_landscape_metrics_df.__doc__ = _compute_landscape_metrics_df_doc.format(
         index_descr="indexed by the attribute value",
         index_return="attribute value (index)",
     )
@@ -248,17 +260,17 @@
         metric,
         *,
         class_val=None,
         ax=None,
         metric_legend=True,
         metric_label=None,
         fmt="--o",
-        plot_kws=None,
-        subplots_kws=None,
-        metric_kws=None,
+        plot_kwargs=None,
+        subplots_kwargs=None,
+        metric_kwargs=None,
     ):
         """Plot the metric.
 
         Parameters
         ----------
         metric : str
             A string indicating the name of the metric to plot.
@@ -272,62 +284,58 @@
             the y-axis).
         metric_label : str, optional
             Label of the y-axis to be displayed if `metric_legend` is `True`. If the
             provided value is `None`, the label will be taken from the `settings`
             module.
         fmt : str, default '--o'
             A format string for `matplotlib.pyplot.plot`.
-        plot_kws : dict, default None
+        plot_kwargs : dict, default None
             Keyword arguments to be passed to `matplotlib.pyplot.plot`.
-        subplots_kws : dict, default None
+        subplots_kwargs : dict, default None
             Keyword arguments to be passed to `matplotlib.pyplot.plot.subplots` only if
             no axis is given (through the `ax` argument).
-        metric_kws : dict, default None
+        metric_kwargs : dict, default None
             Keyword arguments to be passed to the method that computes the metric
             (specified in the `metric` argument) for each landscape.
 
         Returns
         -------
         ax : matplotlib.axes.Axes
             Returns the `Axes` object with the plot drawn onto it.
         """
-        # TODO: metric_legend parameter acepting a set of str values indicating, e.g.,
+        # TODO: metric_legend parameter accepting a set of str values indicating, e.g.,
         # whether the metric label should appear as legend or as yaxis label
         # TODO: if we use seaborn in the future, we can use the pd.Series directly,
         # since its index corresponds to this SpatioTemporalAnalysis dates
-        if metric_kws is None:
-            metric_kws = {}
+        if metric_kwargs is None:
+            metric_kwargs = {}
         # since we are using the compute data frame methods even though we are just
         # computing a single metric (so that error management regarding the computation
-        # of metrics is defined in a single place), we need to provide the `metrics_kws`
-        # (mapping a metric to its keyword-arguments `metric_kws`).
-        metrics_kws = {metric: metric_kws}
+        # of metrics is defined in a single place), we need to provide the
+        # `metrics_kwargs` (mapping a metric to its keyword-arguments `metric_kwargs`).
+        metrics_kwargs = {metric: metric_kwargs}
         metrics = [metric]
         if class_val is None:
             metric_values = self.compute_landscape_metrics_df(
-                metrics=metrics, metrics_kws=metrics_kws
+                metrics=metrics, metrics_kwargs=metrics_kwargs
             ).values
         else:
             metric_values = self.compute_class_metrics_df(
-                metrics=metrics, classes=[class_val], metrics_kws=metrics_kws
+                metrics=metrics, classes=[class_val], metrics_kwargs=metrics_kwargs
             ).values
 
         if ax is None:
-            if subplots_kws is None:
-                subplots_kws = {}
-            fig, ax = plt.subplots(**subplots_kws)
-
-        # for `SpatioTemporalAnalysis`, `attribute_values` will be `dates`; for
-        # `BufferAnalysis`, `attribute_values` will be `buffer_dists`
-        attribute_values = getattr(self, self.attribute_name)
+            if subplots_kwargs is None:
+                subplots_kwargs = {}
+            fig, ax = plt.subplots(**subplots_kwargs)
 
-        if plot_kws is None:
-            plot_kws = {}
+        if plot_kwargs is None:
+            plot_kwargs = {}
 
-        ax.plot(attribute_values, metric_values, fmt, **plot_kws)
+        ax.plot(self.landscape_ser.index, metric_values, fmt, **plot_kwargs)
 
         if metric_legend:
             if metric_label is None:
                 # get the metric label from the settings, otherwise use the metric
                 # method name, i.e., metric name in camel-case
                 metric_label = settings.metric_label_dict.get(metric, metric)
 
@@ -336,63 +344,61 @@
         return ax
 
     def plot_landscapes(
         self,
         *,
         cmap=None,
         legend=True,
-        subplots_kws=None,
-        show_kws=None,
-        subplots_adjust_kws=None,
+        subplots_kwargs=None,
+        show_kwargs=None,
+        subplots_adjust_kwargs=None,
     ):
         """Plot each landscape snapshot in a dedicated matplotlib axis.
 
         Uses the `Landscape.plot_landscape` method of each instance.
 
         Parameters
         ----------
         cmap : str or `~matplotlib.colors.Colormap`, optional
             A Colormap instance.
         legend : bool, optional
             If ``True``, display the legend of the land use/cover color codes.
-        subplots_kws : dict, default None
+        subplots_kwargs : dict, default None
             Keyword arguments to be passed to `matplotlib.pyplot.subplots`.
-        show_kws : dict, default None
+        show_kwargs : dict, default None
             Keyword arguments to be passed to `rasterio.plot.show`.
-        subplots_adjust_kws : dict, default None
+        subplots_adjust_kwargs : dict, default None
             Keyword arguments to be passed to `matplotlib.pyplot.subplots_adjust`.
 
         Returns
         -------
         fig : matplotlib.figure.Figure
             The figure with its corresponding plots drawn into its axes.
         """
-        attribute_values = getattr(self, self.attribute_name)
+        num_landscapes = len(self.landscape_ser)
 
-        # avoid alias/refrence issues
-        if subplots_kws is None:
-            _subplots_kws = {}
+        # avoid alias/reference issues
+        if subplots_kwargs is None:
+            _subplots_kwargs = {}
         else:
-            _subplots_kws = subplots_kws.copy()
-        figsize = _subplots_kws.pop("figsize", None)
+            _subplots_kwargs = subplots_kwargs.copy()
+        figsize = _subplots_kwargs.pop("figsize", None)
         if figsize is None:
             figwidth, figheight = plt.rcParams["figure.figsize"]
-            figsize = (figwidth * len(attribute_values), figheight)
+            figsize = (figwidth * num_landscapes, figheight)
 
-        fig, axes = plt.subplots(
-            1, len(attribute_values), figsize=figsize, **_subplots_kws
-        )
+        fig, axes = plt.subplots(1, num_landscapes, figsize=figsize, **_subplots_kwargs)
         if len(axes) == 1:  # len(attribute_values) == 1
             axes = [axes]
-        if show_kws is None:
-            show_kws = {}
-        for attribute_value, landscape, ax in zip(
-            attribute_values, self.landscapes, axes
-        ):
-            ax = landscape.plot_landscape(cmap=cmap, ax=ax, legend=legend, **show_kws)
+        if show_kwargs is None:
+            show_kwargs = {}
+        for (attribute_value, landscape), ax in zip(self.landscape_ser.items(), axes):
+            ax = landscape.plot_landscape(
+                cmap=cmap, ax=ax, legend=legend, **show_kwargs
+            )
             ax.set_title(attribute_value)
 
         # adjust spacing between axes
-        if subplots_adjust_kws is not None:
-            fig.subplots_adjust(**subplots_adjust_kws)
+        if subplots_adjust_kwargs is not None:
+            fig.subplots_adjust(**subplots_adjust_kwargs)
 
         return fig
```

### Comparing `pylandstats-3.0.0rc1/pylandstats/settings.py` & `pylandstats-3.0.0rc2/pylandstats/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pylandstats settings."""
+
 from os import environ
 
 try:
     import dotenv
 
     # load environment variables from a '.env' file of a parent directory
     dotenv.load_dotenv(dotenv.find_dotenv())
@@ -21,15 +22,15 @@
     "number_of_core_areas": "NCORE",
     "core_area_index": "CAI",
     "euclidean_nearest_neighbor": "ENN",
     # class-level metrics (can also be landscape-level except for PLAND)
     # ACHTUNG: the 'total_area' metric might be 'CA' or 'TA' in FRAGSTATS (depending on
     # whether the metric is computed at the class or landscape level respectively).
     # Nevertheless, considering the implementation/functioning of PyLandStats, making
-    # this disctinction in the abbreviations of 'total_area' might be arduous. To
+    # this distinction in the abbreviations of 'total_area' might be arduous. To
     # simplify, we will use 'TA' in all cases.
     "total_area": "TA",
     "proportion_of_landscape": "PLAND",
     "number_of_patches": "NP",
     "patch_density": "PD",
     "largest_patch_index": "LPI",
     "total_edge": "TE",
@@ -38,33 +39,38 @@
     "effective_mesh_size": "MESH",
     # landscape-level metrics
     "contagion": "CONTAG",
     "shannon_diversity_index": "SHDI",
 }
 # add the class/landscape distribution statistics metrics to the fragstats abbreviation
 # dictionary
+
 for metric in [
     "area",
     "perimeter",
     "perimeter_area_ratio",
     "shape_index",
     "fractal_dimension",
+    "core_area",
+    "core_area_index",
     "euclidean_nearest_neighbor",
 ]:
     for suffix in ["mn", "am", "md", "ra", "sd", "cv"]:
-        fragstats_abbrev_dict["{}_{}".format(metric, suffix)] = "{}_{}".format(
-            fragstats_abbrev_dict[metric], suffix.upper()
+        fragstats_abbrev_dict[f"{metric}_{suffix}"] = (
+            f"{fragstats_abbrev_dict[metric]}_{suffix.upper()}"
         )
+for suffix in ["mn", "am", "md", "ra", "sd", "cv"]:
+    fragstats_abbrev_dict[f"disjunct_core_area_{suffix}"] = f"DCORE_{suffix}"
 
 # SETTINGS
-# TODO: is it worth integrating `metrics` and `metrics_kws` into the settings scheme?
+# TODO: is it worth integrating `metrics` and `metrics_kwargs` into the settings scheme?
 # The main difficulty is that depending on the method, the `metrics` argument might
 # concern only patch-level metrics, class-level metrics (or landscape-level metrics,
 # e.g., see the methods of the form `landscape.Landscape.compute_{level}_metrics_df`,
 # where 'level' can be `patch`, `class` or `landscape`. On the other hand, integrating
-# `metrics_kws` should be more straight-forward.
+# `metrics_kwargs` should be more straight-forward.
 metric_label_dict = environ.get("METRIC_LABEL_DICT", fragstats_abbrev_dict)
 
 # OTHER
 DEFAULT_LANDSCAPE_NODATA = 0
 DEFAULT_NEIGHBORHOOD_RULE = "8"
 CLASS_METRICS_DF_FILLNA = True
```

### Comparing `pylandstats-3.0.0rc1/pylandstats/spatiotemporal.py` & `pylandstats-3.0.0rc2/pylandstats/spatiotemporal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Spatio-temporal analysis."""
+
 import functools
 
-import geopandas as gpd
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import rasterio as rio
 from rasterio import mask
 
-from . import multilandscape, zonal
+from . import multilandscape, settings, zonal
 from .landscape import Landscape
 
 __all__ = [
     "SpatioTemporalAnalysis",
     "SpatioTemporalZonalAnalysis",
     "SpatioTemporalBufferAnalysis",
     "SpatioTemporalZonalGridAnalysis",
 ]
 
-_plot_metric_doc = """Plot the time series of the metric accross {zone_descr}s.
+_plot_metric_doc = """Plot the time series of the metric across {zone_descr}s.
 
 Parameters
 ----------
 metric : str
     A string indicating the name of the metric to plot.
 class_val : int, optional
     If provided, the metric will be plotted at the level of the corresponding class,
@@ -36,35 +36,35 @@
     Label of the y-axis to be displayed if `metric_legend` is `True`. If the provided
     value is `None`, the label will be taken from the `settings` module.
 {zone_var_name}_legend : bool, default True
     Whether a legend linking each plotted line to a {zone_descr} should be displayed
     within the plot.
 fmt : str, default '--o'
     A format string for `matplotlib.pyplot.plot`.
-plot_kws : dict, default None
+plot_kwargs : dict, default None
     Keyword arguments to be passed to `matplotlib.pyplot.plot`.
-subplots_kws : dict, default None
+subplots_kwargs : dict, default None
     Keyword arguments to be passed to `matplotlib.pyplot.subplots` only if no axis is
     given (through the `ax` argument).
-metric_kws : dict, default None
+metric_kwargs : dict, default None
     Keyword arguments to be passed to the method that computes the metric (specified in
     the `metric` argument) for each landscape.
 
 Returns
 -------
 ax : matplotlib.axes.Axes
     Returns the `Axes` object with the plot drawn onto it.
 """
 
 
 class SpatioTemporalAnalysis(multilandscape.MultiLandscape):
     """Spatio-temporal analysis."""
 
     def __init__(
-        self, landscapes, *, dates=None, neighborhood_rule=None, **landscape_kws
+        self, landscapes, *, dates=None, neighborhood_rule=None, **landscape_kwargs
     ):
         """Initialize the spatio-temporal analysis.
 
         Parameters
         ----------
         landscapes : list-like
             A list-like of `Landscape` instances or of strings/file-like/pathlib.Path
@@ -75,72 +75,72 @@
             `landscapes` (for DataFrame indices and plot labels).
         neighborhood_rule : {'8', '4'}, optional
             Neighborhood rule to determine patch adjacencies, i.e: '8' (queen's
             case/Moore neighborhood) or '4' (rook's case/Von Neumann neighborhood).
             Ignored if the passed-in landscapes are `Landscape` instances. If no value
             is provided and the passed-in landscapes are file-like objects or paths, the
             default value set in `settings.DEFAULT_NEIGHBORHOOD_RULE` will be taken.
-        landscape_kws : dict, optional
+        landscape_kwargs : dict, optional
             Other keyword arguments to be passed to the instantiation of
            `pylandstats.Landscape` for each element of `landscapes`. Ignored if the
             elements of `landscapes` are already instances of `pylandstats.Landcape`.
         """
         if dates is None:
             dates = ["t{}".format(i) for i in range(len(landscapes))]
 
-        # pop the `neighborhood_rule` from `landscape_kws` (this is merely done so that
-        # the `neighborhood_rule` argument is explicitly documented in this method
-        _ = landscape_kws.pop("neighborhood_rule", None)
+        # pop the `neighborhood_rule` from `landscape_kwargs` (this is merely done so
+        # that the `neighborhood_rule` argument is explicitly documented in this method
+        _ = landscape_kwargs.pop("neighborhood_rule", None)
         # call the parent's init
         super().__init__(
             landscapes,
             "dates",
             dates,
             neighborhood_rule=neighborhood_rule,
-            **landscape_kws,
+            **landscape_kwargs,
         )
 
     # override docs
     def compute_class_metrics_df(  # noqa: D102
-        self, *, metrics=None, classes=None, metrics_kws=None, fillna=None
+        self, *, metrics=None, classes=None, metrics_kwargs=None, fillna=None
     ):
         return super().compute_class_metrics_df(
             metrics=metrics,
             classes=classes,
-            metrics_kws=metrics_kws,
+            metrics_kwargs=metrics_kwargs,
             fillna=fillna,
         )
 
     compute_class_metrics_df.__doc__ = (
         multilandscape._compute_class_metrics_df_doc.format(
             index_descr="multi-indexed by the class and date",
             index_return="class, date (multi-index)",
         )
     )
 
     def compute_landscape_metrics_df(  # noqa: D102
-        self, *, metrics=None, metrics_kws=None
+        self, *, metrics=None, metrics_kwargs=None
     ):
         return super().compute_landscape_metrics_df(
-            metrics=metrics, metrics_kws=metrics_kws
+            metrics=metrics, metrics_kwargs=metrics_kwargs
         )
 
     compute_landscape_metrics_df.__doc__ = (
         multilandscape._compute_landscape_metrics_df_doc.format(
             index_descr="indexed by the date", index_return="date (index)"
         )
     )
 
     # def plot_patch_metric(metric):
     #     # TODO: sns distplot?
     #     fig, ax = plt.subplots()
     #     ax.hist()
 
 
-class SpatioTemporalZonalAnalysis(SpatioTemporalAnalysis):
+class SpatioTemporalZonalAnalysis(SpatioTemporalAnalysis, zonal.ZonalAnalysis):
     """Spatio-temporal zonal analysis."""
 
     def __init__(
         self,
         landscape_filepaths,
         zones,
         *,
@@ -183,261 +183,166 @@
             `landscapes` (for DataFrame indices and plot labels).
         neighborhood_rule : {'8', '4'}, optional
             Neighborhood rule to determine patch adjacencies, i.e: '8' (queen's
             case/Moore neighborhood) or '4' (rook's case/Von Neumann neighborhood).
             Ignored if `landscape` is a `Landscape` instance. If no value is provided,
             the default value set in `settings.DEFAULT_NEIGHBORHOOD_RULE` will be taken.
         """
+        # we first instantiate only a zonal analysis to use its (after initialization)
+        # attributes
         za = zonal.ZonalAnalysis(
             landscape_filepaths[0],
             zones,
             zone_index=zone_index,
             zone_nodata=zone_nodata,
             neighborhood_rule=neighborhood_rule,
         )
 
         # while `ZonalAnalysis.__init__` will set the `zone_gser` attribute to the
         # instantiated object (stored in the variable `ba`), it will not set it to the
         # current `SpatioTemporalZonalAnalysis`, so we need to do it here
         self.zone_gser = za.zone_gser
-        self.attribute_name = za.attribute_name
 
-        # init the `SpatioTemporalAnalysis` instances
-        self.stas = []
+        # init the landscape instances
+        landscapes = []
         for _, zone_geom in za.zone_gser.items():
-            zone_landscapes = []
             for landscape in landscape_filepaths:
                 with rio.open(landscape) as src:
                     zone_arr, zone_transform = mask.mask(src, [zone_geom], crop=True)
-                    zone_landscapes.append(
+                    landscapes.append(
                         Landscape(
                             zone_arr[0],
                             res=src.res,
                             transform=zone_transform,
                             neighborhood_rule=neighborhood_rule,
                         )
                     )
-            self.stas.append(SpatioTemporalAnalysis(zone_landscapes, dates=dates))
-
-        # We need to get the union of the classes found at the spatio-temporal analysis
-        # instance of each zone
-        self.present_classes = functools.reduce(
-            np.union1d, tuple(sta.present_classes for sta in self.stas)
-        )
-
-        # the dates will be the same for all the `SpatioTemporalAnalysis` instances
-        # stored in `self.stas`. We will just take them from the first instance and
-        # store them as attribute of this `SpatioTemporalZonalAnalysis` so that it can
-        # be used more conveniently below.
-        # ACHTUNG: we do it AFTER instantiating the `SpatioTemporalAnalysis` instances
-        # of `self.stats` so that we let the `__init__` method of
-        # `SpatioTemporalAnalysis.__init__` deal with the logic of what to do with the
-        # `dates` argument
-        self.dates = self.stas[0].dates
 
-    def compute_class_metrics_df(  # noqa: D102
-        self, *, metrics=None, classes=None, metrics_kws=None, fillna=None
-    ):
-        if classes is None:
-            classes = self.present_classes
-
-        # get the columns to init the data frame
-        if metrics is None:
-            columns = Landscape.CLASS_METRICS
-        else:
-            columns = metrics
+        # TODO: DRY this from `SpatioTemporalAnalysis.__init__`
+        if dates is None:
+            dates = ["t{}".format(i) for i in range(len(landscape_filepaths))]
 
-        # IMPORTANT: since some classes might not be present for each date and/or zone,
-        # we will init the MultiIndex manually to ensure that every class is present in
-        # the resulting data frame. If some class does not appear for some date/zone,
-        # the corresponding row will be nan. This probably preferable than having a
-        # MultiIndex that can have different levels (i.e., the second level `class_val`)
-        # for each zone. Note that this approach is likely slower since for each zone,
-        # we have to iterate as in (see below):
-        # `for class_val, date in class_metrics_df.loc[zone].index`
-        class_metrics_df = pd.DataFrame(
+        # instantiate the series of landscapes but using a multi-index
+        self.landscape_ser = pd.Series(
+            landscapes,
             index=pd.MultiIndex.from_product(
-                [self.zone_gser.index, classes, self.dates]
+                [self.zone_gser.index, dates],
+                names=[self.zone_gser.index.name, "date"],
             ),
-            columns=columns,
         )
-        class_metrics_df.index.names = self.attribute_name, "class_val", "dates"
-        class_metrics_df.columns.name = "metric"
 
-        for zone, sta in zip(self.zone_gser.index, self.stas):
-            # get the class metrics data frame for the `SpatioTemporalAnalysis` instance
-            # that corresponds to this zone
-            df = sta.compute_class_metrics_df(
-                metrics=metrics,
-                classes=classes,
-                metrics_kws=metrics_kws,
-                fillna=fillna,
-            )
-            # put the metrics data frame of the `SpatioTemporalAnalysis` of this zone
-            # into the global metrics data frame of the `SpatioTemporalZoneAnalysis`
-            for class_val, date in class_metrics_df.loc[zone].index:
-                # use `class_metrics_df.loc` for the first level (i.e., zone) again (we
-                # have already used it in the iterator above) to avoid
-                # `SettingWithCopyWarning`
-                try:
-                    class_metrics_df.loc[zone, class_val, date] = df.loc[
-                        class_val, date
-                    ]
-                except KeyError:
-                    # this means that `class_val` is not in `df`, therefore we do
-                    # nothing and the corresponding row of `class_metrics_df` will stay
-                    # as nan
-                    pass
+        # get the all classes present in the provided landscapes
+        # TODO: DRY this from `MultiLandscape.__init__`
+        self.present_classes = functools.reduce(
+            np.union1d,
+            tuple(landscape.classes for landscape in self.landscape_ser),
+        )
 
-        return class_metrics_df.apply(pd.to_numeric)
+    def compute_class_metrics_df(  # noqa: D102
+        self, *, metrics=None, classes=None, metrics_kwargs=None, fillna=None
+    ):
+        return super().compute_class_metrics_df(
+            metrics=metrics,
+            classes=classes,
+            metrics_kwargs=metrics_kwargs,
+            fillna=fillna,
+        )
 
     compute_class_metrics_df.__doc__ = (
         multilandscape._compute_class_metrics_df_doc.format(
             index_descr="multi-indexed by the zone, class and date",
             index_return="zone, class, distance (multi-index)",
         )
     )
 
     def compute_landscape_metrics_df(  # noqa: D102
-        self, *, metrics=None, metrics_kws=None
+        self, *, metrics=None, metrics_kwargs=None
     ):
-        # we will create a dict where each key is a zone id, and its value is the
-        # corresponding metrics data frame of the `SpatioTemporalAnalysis` instance
-        df_dict = {
-            zone: sta.compute_landscape_metrics_df(
-                metrics=metrics, metrics_kws=metrics_kws
-            )
-            for zone, sta in zip(self.zone_gser.index, self.stas)
-        }
-
-        # we concatenate each value of the dict dataframe using its respective
-        # `buffer_dist` key to create an extra index level (i.e., using the `keys`
-        # argument of `pd.concat`)
-        landscape_metrics_df = pd.concat(df_dict.values(), keys=df_dict.keys())
-        # now we set the name of each index and column level
-        landscape_metrics_df.index.names = self.attribute_name, "dates"
-        landscape_metrics_df.columns.name = "metric"
-
-        return landscape_metrics_df
+        return super().compute_landscape_metrics_df(
+            metrics=metrics, metrics_kwargs=metrics_kwargs
+        )
 
     compute_landscape_metrics_df.__doc__ = (
         multilandscape._compute_landscape_metrics_df_doc.format(
             index_descr="multi-indexed by the buffer distance and date",
             index_return="buffer distance, date (multi-index)",
         )
     )
 
-    def compute_zonal_statistics_gdf(
-        self, metrics, *, class_val=None, metrics_kws=None
+    def compute_zonal_statistics_gdf(  # noqa: D102
+        self, *, metrics=None, class_val=None, metrics_kwargs=None
     ):
-        """Compute the zonal statistics geo-data frame over the landscape raster.
-
-        Parameters
-        ----------
-        metrics : list-like, optional
-            A list-like of strings with the names of the metrics that should be
-            computed. If `None`, all the implemented class-level metrics will be
-            computed.
-        class_val : int, optional
-            If provided, the zonal statistics will be computed at the level of the
-            corresponding class, otherwise they will be computed at the landscape level.
-        metrics_kws : dict, optional
-            Dictionary mapping the keyword arguments (values) that should be passed to
-            each metric method (key), e.g., to exclude the boundary from the computation
-            of `total_edge`, metric_kws should map the string 'total_edge' (method name)
-            to {'count_boundary': False}. If `None`, each metric will be computed
-            according to FRAGSTATS defaults.
-
-        Returns
-        -------
-        zonal_statistics_gdf : geopandas.GeoDataFrame
-            Geo-data frame with the computed zonal statistics.
-        """
+        return super().compute_zonal_statistics_gdf(
+            metrics=metrics, class_val=class_val, metrics_kwargs=metrics_kwargs
+        )
 
-        # TODO: DRY with `ZonalAnalysis.compute_zonal_statistics_gdf`?
-        def _compute_zonal_metrics_df(sta):
-            if class_val is None:
-                zonal_metrics_df = sta.compute_landscape_metrics_df(
-                    metrics=metrics, metrics_kws=metrics_kws
-                )
-            else:
-                zonal_metrics_df = sta.compute_class_metrics_df(
-                    metrics=metrics, classes=[class_val], metrics_kws=metrics_kws
-                )
-            return zonal_metrics_df
-
-        zonal_metrics_df = pd.concat(
-            [
-                _compute_zonal_metrics_df(sta).assign(**{self.attribute_name: zone})
-                for zone, sta in zip(self.zone_gser.index, self.stas)
-            ]
-        )
-
-        return gpd.GeoDataFrame(
-            # first set zone as outermost index
-            zonal_metrics_df.reset_index().set_index(
-                [self.attribute_name] + zonal_metrics_df.index.names
-            ),
-            geometry=zonal_metrics_df.reset_index()[self.attribute_name]
-            .map(self.zone_gser)
-            .values,
-            crs=self.zone_gser.crs,
+    compute_zonal_statistics_gdf.__doc__ = (
+        zonal._compute_zonal_statistics_gdf_doc.format(
+            col_return="metrics and dates (multi-index)"
         )
+    )
 
     def plot_metric(  # noqa: D102
         self,
         metric,
         *,
         class_val=None,
         ax=None,
         metric_legend=True,
         metric_label=None,
         zone_legend=True,
         fmt="--o",
-        plot_kws=None,
-        subplots_kws=None,
-        metric_kws=None,
+        plot_kwargs=None,
+        subplots_kwargs=None,
+        metric_kwargs=None,
     ):
         # TODO: refactor this method so that it uses `class_metrics_df` and
         # `landscape_metrics_df` properties?
         if ax is None:
-            if subplots_kws is None:
-                subplots_kws = {}
-            fig, ax = plt.subplots(**subplots_kws)
-
-        if plot_kws is None:
-            plot_kws = {}
-
-        if "label" not in plot_kws:
-            # avoid alias/refrence issues
-            _plot_kws = plot_kws.copy()
-            for zone, sta in zip(self.zone_gser.index, self.stas):
-                _plot_kws["label"] = zone
-                ax = sta.plot_metric(
-                    metric,
-                    class_val=class_val,
-                    ax=ax,
-                    metric_legend=metric_legend,
-                    metric_label=metric_label,
-                    fmt=fmt,
-                    plot_kws=_plot_kws,
-                    metric_kws=metric_kws,
-                )
+            if subplots_kwargs is None:
+                subplots_kwargs = {}
+            fig, ax = plt.subplots(**subplots_kwargs)
+
+        if plot_kwargs is None:
+            plot_kwargs = {}
+
+        # start: compute metrics - TODO: DRY from multilandscape.plot_metric?
+        if metric_kwargs is None:
+            metric_kwargs = {}
+        metrics_kwargs = {metric: metric_kwargs}
+        metrics = [metric]
+        if class_val is None:
+            metric_df = self.compute_landscape_metrics_df(
+                metrics=metrics, metrics_kwargs=metrics_kwargs
+            )
+        else:
+            metric_df = self.compute_class_metrics_df(
+                metrics=metrics, classes=[class_val], metrics_kwargs=metrics_kwargs
+            ).loc[class_val]
+        # end: compute metrics
+
+        if "label" not in plot_kwargs:
+            # avoid alias/reference issues
+            _plot_kwargs = plot_kwargs.copy()
+            for zone, zone_df in metric_df.groupby(level=0):
+                _plot_kwargs["label"] = zone
+                ax.plot(zone_df.loc[zone].index, zone_df.values, fmt, **_plot_kwargs)
         else:
-            for sta in self.stas:
-                ax = sta.plot_metric(
-                    metric,
-                    class_val=class_val,
-                    ax=ax,
-                    metric_legend=metric_legend,
-                    metric_label=metric_label,
-                    fmt=fmt,
-                    plot_kws=plot_kws,
-                    metric_kws=metric_kws,
-                )
+            for zone, zone_df in metric_df.groupby(level=0):
+                ax.plot(zone_df.loc[zone].index, zone_df.values, fmt, **plot_kwargs)
+
+        # start: metric legend - TODO: DRY from multilandscape
+        if metric_legend:
+            if metric_label is None:
+                # get the metric label from the settings, otherwise use the metric
+                # method name, i.e., metric name in camel-case
+                metric_label = settings.metric_label_dict.get(metric, metric)
+
+            ax.set_ylabel(metric_label)
+        # end metric legend
 
         if zone_legend:
             ax.legend()
 
         return ax
 
     plot_metric.__doc__ = _plot_metric_doc.format(
@@ -446,78 +351,74 @@
     )
 
     def plot_landscapes(
         self,
         *,
         cmap=None,
         legend=True,
-        subplots_kws=None,
-        show_kws=None,
-        subplots_adjust_kws=None,
+        subplots_kwargs=None,
+        show_kwargs=None,
+        subplots_adjust_kwargs=None,
     ):
         """Plot each landscape snapshot in a dedicated matplotlib axis.
 
         Parameters
         ----------
         cmap : str or `~matplotlib.colors.Colormap`, optional
             A Colormap instance.
         legend : bool, optional
             If ``True``, display the legend of the land use/cover color codes.
-        subplots_kws : dict, default None
+        subplots_kwargs : dict, default None
             Keyword arguments to be passed to `matplotlib.pyplot.subplots`.
-        show_kws : dict, default None
+        show_kwargs : dict, default None
             Keyword arguments to be passed to `rasterio.plot.show`.
-        subplots_adjust_kws : dict, default None
+        subplots_adjust_kwargs : dict, default None
             Keyword arguments to be passed to `matplotlib.pyplot.subplots_adjust`.
 
         Returns
         -------
         fig : matplotlib.figure.Figure
             The figure with its corresponding plots drawn into its axes.
         """
-        # the number of rows is the number of dates, which will be the same for all the
-        # `SpatioTemporalAnalysis` instances of `self.stas`
-        dates = self.stas[0].dates
-
-        # avoid alias/refrence issues
-        if subplots_kws is None:
-            _subplots_kws = {}
+        # avoid alias/reference issues
+        if subplots_kwargs is None:
+            _subplots_kwargs = {}
         else:
-            _subplots_kws = subplots_kws.copy()
-        figsize = _subplots_kws.pop("figsize", None)
+            _subplots_kwargs = subplots_kwargs.copy()
+        figsize = _subplots_kwargs.pop("figsize", None)
+        dates = self.landscape_ser.index.get_level_values("date").unique()
         if figsize is None:
             figwidth, figheight = plt.rcParams["figure.figsize"]
             figsize = (
                 figwidth * len(self.zone_gser),
                 figheight * len(dates),
             )
 
         fig, axes = plt.subplots(
-            len(self.zone_gser), len(dates), figsize=figsize, **_subplots_kws
+            len(self.zone_gser), len(dates), figsize=figsize, **_subplots_kwargs
         )
 
-        if show_kws is None:
-            show_kws = {}
+        if show_kwargs is None:
+            show_kwargs = {}
         flat_axes = axes.flat
-        for _, sta in zip(self.zone_gser.index, self.stas):
-            for date, landscape in zip(sta.dates, sta.landscapes):
-                ax = landscape.plot_landscape(
-                    cmap=cmap, ax=next(flat_axes), legend=legend, **show_kws
-                )
+        for landscape in self.landscape_ser:
+            ax = landscape.plot_landscape(
+                cmap=cmap, ax=next(flat_axes), legend=legend, **show_kwargs
+            )
 
         # labels in first row and column only
         for date, ax in zip(dates, axes[0]):
             ax.set_title(date)
 
         for zone, ax in zip(self.zone_gser.index, axes[:, 0]):
             ax.set_ylabel(zone)
 
         # adjust spacing between axes
-        if subplots_adjust_kws is not None:
-            fig.subplots_adjust(**subplots_adjust_kws)
+        if subplots_adjust_kwargs is not None:
+            fig.subplots_adjust(**subplots_adjust_kwargs)
 
         return fig
 
 
 class SpatioTemporalBufferAnalysis(SpatioTemporalZonalAnalysis):
     """Spatio-temporal buffer analysis around a feature of interest."""
 
@@ -574,35 +475,35 @@
             landscape_filepaths,
             zones=ba.zone_gser,
             dates=dates,
             neighborhood_rule=neighborhood_rule,
         )
 
     def compute_class_metrics_df(  # noqa: D102
-        self, *, metrics=None, classes=None, metrics_kws=None, fillna=None
+        self, *, metrics=None, classes=None, metrics_kwargs=None, fillna=None
     ):
         return super().compute_class_metrics_df(
             metrics=metrics,
             classes=classes,
-            metrics_kws=metrics_kws,
+            metrics_kwargs=metrics_kwargs,
             fillna=fillna,
         )
 
     compute_class_metrics_df.__doc__ = (
         multilandscape._compute_class_metrics_df_doc.format(
             index_descr="multi-indexed by the buffer distance, class and date",
             index_return="buffer distance, class, distance (multi-index)",
         )
     )
 
     def compute_landscape_metrics_df(  # noqa: D102
-        self, *, metrics=None, metrics_kws=None
+        self, *, metrics=None, metrics_kwargs=None
     ):
         return super().compute_landscape_metrics_df(
-            metrics=metrics, metrics_kws=metrics_kws
+            metrics=metrics, metrics_kwargs=metrics_kwargs
         )
 
     compute_landscape_metrics_df.__doc__ = (
         multilandscape._compute_landscape_metrics_df_doc.format(
             index_descr="multi-indexed by the buffer distance and date",
             index_return="buffer distance, date (multi-index)",
         )
@@ -614,29 +515,29 @@
         *,
         class_val=None,
         ax=None,
         metric_legend=True,
         metric_label=None,
         buffer_dist_legend=True,
         fmt="--o",
-        plot_kws=None,
-        subplots_kws=None,
-        metric_kws=None,
+        plot_kwargs=None,
+        subplots_kwargs=None,
+        metric_kwargs=None,
     ):
         return super().plot_metric(
             metric,
             class_val=class_val,
             ax=ax,
             metric_legend=metric_legend,
             metric_label=metric_label,
             zone_legend=buffer_dist_legend,
             fmt=fmt,
-            plot_kws=plot_kws,
-            subplots_kws=subplots_kws,
-            metric_kws=metric_kws,
+            plot_kwargs=plot_kwargs,
+            subplots_kwargs=subplots_kwargs,
+            metric_kwargs=metric_kwargs,
         )
 
     plot_metric.__doc__ = _plot_metric_doc.format(
         zone_descr="buffer zone", zone_var_name="buffer_dist"
     )
 
 
@@ -701,35 +602,35 @@
             landscape_filepaths,
             zones=zga.zone_gser,
             dates=dates,
             neighborhood_rule=neighborhood_rule,
         )
 
     def compute_class_metrics_df(  # noqa: D102
-        self, *, metrics=None, classes=None, metrics_kws=None, fillna=None
+        self, *, metrics=None, classes=None, metrics_kwargs=None, fillna=None
     ):
         return super().compute_class_metrics_df(
             metrics=metrics,
             classes=classes,
-            metrics_kws=metrics_kws,
+            metrics_kwargs=metrics_kwargs,
             fillna=fillna,
         )
 
     compute_class_metrics_df.__doc__ = (
         multilandscape._compute_class_metrics_df_doc.format(
             index_descr="multi-indexed by the grid cell, class and date",
             index_return="grid cell, class, distance (multi-index)",
         )
     )
 
     def compute_landscape_metrics_df(  # noqa: D102
-        self, *, metrics=None, metrics_kws=None
+        self, *, metrics=None, metrics_kwargs=None
     ):
         return super().compute_landscape_metrics_df(
-            metrics=metrics, metrics_kws=metrics_kws
+            metrics=metrics, metrics_kwargs=metrics_kwargs
         )
 
     compute_landscape_metrics_df.__doc__ = (
         multilandscape._compute_landscape_metrics_df_doc.format(
             index_descr="multi-indexed by the grid cell and date",
             index_return="grid cell, date (multi-index)",
         )
@@ -741,27 +642,27 @@
         *,
         class_val=None,
         ax=None,
         metric_legend=True,
         metric_label=None,
         grid_cell_legend=True,
         fmt="--o",
-        plot_kws=None,
-        subplots_kws=None,
-        metric_kws=None,
+        plot_kwargs=None,
+        subplots_kwargs=None,
+        metric_kwargs=None,
     ):
         return super().plot_metric(
             metric,
             class_val=class_val,
             ax=ax,
             metric_legend=metric_legend,
             metric_label=metric_label,
             zone_legend=grid_cell_legend,
             fmt=fmt,
-            plot_kws=plot_kws,
-            subplots_kws=subplots_kws,
-            metric_kws=metric_kws,
+            plot_kwargs=plot_kwargs,
+            subplots_kwargs=subplots_kwargs,
+            metric_kwargs=metric_kwargs,
         )
 
     plot_metric.__doc__ = _plot_metric_doc.format(
         zone_descr="zone grid", zone_var_name="grid_cell"
     )
```

### Comparing `pylandstats-3.0.0rc1/pylandstats/zonal.py` & `pylandstats-3.0.0rc2/pylandstats/zonal.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,58 @@
 import numpy as np
 import pandas as pd
 import rasterio as rio
 from rasterio import features, mask
 from shapely import geometry
 from shapely.geometry import base as geometry_base
 
+try:
+    from fiona import errors as fiona_errors
+except ImportError:
+    fiona_errors = None
+
 from . import multilandscape
 from .landscape import Landscape
 
 __all__ = ["ZonalAnalysis", "BufferAnalysis", "ZonalGridAnalysis"]
 
+ZONES_READ_ERRORS = [AttributeError, TypeError]
+if fiona_errors is not None:
+    ZONES_READ_ERRORS.append(fiona_errors.DriverError)
+ZONES_READ_ERRORS = tuple(ZONES_READ_ERRORS)
+
+_compute_zonal_statistics_gdf_doc = """
+Compute the zonal statistics geo-data frame over the landscape raster.
+
+Parameters
+----------
+metrics : list-like, optional
+    A list-like of strings with the names of the metrics that should be computed. If
+    `None`, all the implemented metrics at the specified level will be computed.
+level : {{'class', 'landscape'}}, optional
+    Whether the metrics should be computed at the class or landscape level. If `None`,
+    the metrics will be computed (a) at the class level when a non-None `classes` is
+    provided, otherwise (b) at the landscape level.
+class_val : int, optional
+    If provided, the metric will be computed at the level of the corresponding class,
+    otherwise it will be computed at the landscape level.
+metrics_kwargs : dict, optional
+    Dictionary mapping the keyword arguments (values) that should be passed to
+    each metric method (key), e.g., to exclude the boundary from the computation
+    of `total_edge`, metric_kwargs should map the string 'total_edge' (method name)
+    to {{'count_boundary': False}}. If `None`, each metric will be computed
+    according to FRAGSTATS defaults.
+
+Returns
+-------
+zonal_statistics_gdf : geopandas.GeoDataFrame
+    Geo-data frame with the computed zonal statistics, with the zones as rows and
+    {col_return} as columns.
+"""
+
 
 class ZonalAnalysis(multilandscape.MultiLandscape):
     """Zonal analysis."""
 
     def __init__(
         self,
         landscape_filepath,
@@ -65,20 +104,18 @@
         # provided as a geo-series or a list-like of shapely geometries, we first
         # convert it to a geo-data frame, process it (mainly try to get the proper
         # index) and then convert it to a geo-series to store it as instance attribute
 
         # first, try to read the `zones` argument as a geo-data frame-like file
         try:
             zones = gpd.read_file(zones)
-        except (AttributeError, TypeError):
-            # for GeoDataFrame, GeoSeries, list-like or ndarrays, we will get
-            # "AttributeError: object has no attribute 'startswith'" in windows, fiona
-            # will try to read `masks` as a regular expression and raise a TypeError
-            # (see https://github.com/Toblerity/Fiona/blob/master/fiona/path.py). we let
-            # this continue and try to read the `zones` argument differently below
+        except ZONES_READ_ERRORS:
+            # Depending on the system and installed libraries, geopandas may raise an
+            # `AttributeError`, `TypeError` or `fiona.errors.DriverError`. we let this
+            # continue and try to read the `zones` argument differently below
             pass
 
         with rio.open(landscape_filepath) as src:
             if isinstance(zones, np.ndarray):
                 # zones is an ndarray labelling each zone by a unique integer value
                 # we first instantiate a geo-data frame because we will use the labels
                 # as zone ids
@@ -116,16 +153,16 @@
                         zone_index = pd.Series(zone_index, name="zone")
                     zone_index = zones.set_index(zone_index).index
                     # we now take just the "geometry" column and treat `zones` as
                     # GeoSeries.
                     zones = zones.geometry
                 else:
                     # take just the "geometry" column, treat `zones` as GeoSeries but
-                    # rename it to "zone"
-                    zones = zones.geometry.rename("zone")
+                    # rename the index to "zone"
+                    zones = zones.geometry.rename_axis("zone")
 
             # at this point, `zones` must be a geo-series or a list-like of shapely
             # geometries
             if not isinstance(zones, gpd.GeoSeries):
                 # convert to a geo-series with the CRS of the landscape raster
                 zones = gpd.GeoSeries(zones, crs=src.crs)
             else:
@@ -185,59 +222,47 @@
         # * `attribute_values`: the index of the zones geo-series
         super().__init__(
             landscapes,
             self.zone_gser.index.name or self.zone_gser.name or "zone",
             self.zone_gser.index.values,
         )
 
-    def compute_zonal_statistics_gdf(
-        self, metrics, *, class_val=None, metrics_kws=None
+    def compute_zonal_statistics_gdf(  # noqa: D102
+        self,
+        *,
+        metrics=None,
+        class_val=None,
+        metrics_kwargs=None,
     ):
-        """Compute the zonal statistics geo-data frame over the landscape raster.
-
-        Parameters
-        ----------
-        metrics : list-like, optional
-            A list-like of strings with the names of the metrics that should be
-            computed. If `None`, all the implemented class-level metrics will be
-            computed.
-        class_val : int, optional
-            If provided, the zonal statistics will be computed at the level of the
-            corresponding class, otherwise they will be computed at the landscape level.
-        metrics_kws : dict, optional
-            Dictionary mapping the keyword arguments (values) that should be passed to
-            each metric method (key), e.g., to exclude the boundary from the computation
-            of `total_edge`, metric_kws should map the string 'total_edge' (method name)
-            to {'count_boundary': False}. If `None`, each metric will be computed
-            according to FRAGSTATS defaults.
-
-        Returns
-        -------
-        zonal_statistics_gdf : geopandas.GeoDataFrame
-            Geo-data frame with the computed zonal statistics.
-        """
-        if class_val is None:
-            zonal_metrics_df = self.compute_landscape_metrics_df(
-                metrics=metrics, metrics_kws=metrics_kws
-            )
-        else:
+        if class_val is not None:
             zonal_metrics_df = self.compute_class_metrics_df(
-                metrics=metrics, classes=[class_val], metrics_kws=metrics_kws
+                metrics=metrics, classes=[class_val], metrics_kwargs=metrics_kwargs
+            ).loc[class_val]
+        else:
+            zonal_metrics_df = self.compute_landscape_metrics_df(
+                metrics=metrics, metrics_kwargs=metrics_kwargs
             )
+
         # ensure that we have numeric types (not strings)
         # metric_ser = pd.to_numeric(metric_ser)
 
+        # return a geo-data frame
+        zone_name = self.zone_gser.index.name
         return gpd.GeoDataFrame(
-            zonal_metrics_df,
-            geometry=zonal_metrics_df.reset_index()[self.attribute_name]
-            .map(self.zone_gser)
-            .values,
-            crs=self.zone_gser.crs,
+            zonal_metrics_df.pivot_table(
+                index=zone_name,
+                columns=zonal_metrics_df.index.names.difference([zone_name]),
+            ),
+            geometry=self.zone_gser,
         )
 
+    compute_zonal_statistics_gdf.__doc__ = _compute_zonal_statistics_gdf_doc.format(
+        col_return="metrics"
+    )
+
 
 class BufferAnalysis(ZonalAnalysis):
     """Buffer analysis around a feature of interest."""
 
     def __init__(
         self,
         landscape_filepath,
@@ -349,35 +374,35 @@
             landscape_filepath,
             zones=zone_gser.rename_axis("buffer_dist"),  # set the index name
             neighborhood_rule=neighborhood_rule,
         )
 
     # override docs
     def compute_class_metrics_df(  # noqa: D102
-        self, *, metrics=None, classes=None, metrics_kws=None, fillna=None
+        self, *, metrics=None, classes=None, metrics_kwargs=None, fillna=None
     ):
         return super().compute_class_metrics_df(
             metrics=metrics,
             classes=classes,
-            metrics_kws=metrics_kws,
+            metrics_kwargs=metrics_kwargs,
             fillna=fillna,
         )
 
     compute_class_metrics_df.__doc__ = (
         multilandscape._compute_class_metrics_df_doc.format(
             index_descr="multi-indexed by the class and buffer distance",
             index_return="class, buffer distance (multi-index)",
         )
     )
 
     def compute_landscape_metrics_df(  # noqa: D102
-        self, *, metrics=None, metrics_kws=None
+        self, *, metrics=None, metrics_kwargs=None
     ):
         return super().compute_landscape_metrics_df(
-            metrics=metrics, metrics_kws=metrics_kws
+            metrics=metrics, metrics_kwargs=metrics_kwargs
         )
 
     compute_landscape_metrics_df.__doc__ = (
         multilandscape._compute_landscape_metrics_df_doc.format(
             index_descr="indexed by the buffer distance",
             index_return="buffer distance (index)",
         )
@@ -519,26 +544,26 @@
         # geoseries
         super().__init__(
             landscape_filepath,
             zones=zone_gser.rename_axis("grid_cell"),  # set the index name
             neighborhood_rule=neighborhood_rule,
         )
 
-    def plot_landscapes(self, *, cmap=None, ax=None, figsize=None, **plot_kws):
+    def plot_landscapes(self, *, cmap=None, ax=None, figsize=None, **plot_kwargs):
         """Plot the spatial distribution of the landscape zones.
 
         Parameters
         ----------
         cmap : str or `~matplotlib.colors.Colormap`, optional
             A Colormap instance.
         ax : axis object, optional
             Plot in given axis; if None creates a new figure.
         figsize : tuple of two numeric types, optional
             Size of the figure to create. Ignored if axis `ax` is provided.
-        **plot_kws : optional
+        **plot_kwargs : optional
             Keyword arguments to be passed to `geopandas.GeoSeries.plot`.
 
         Returns
         -------
         ax : matplotlib.axes.Axes
             Returns the `Axes` object with the plot drawn onto it.
         """
@@ -548,15 +573,15 @@
         if isinstance(cmap, str):
             cmap = plt.get_cmap(cmap)
 
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
             ax.set_aspect("equal")
 
-        if plot_kws is None:
-            plot_kws = {}
+        if plot_kwargs is None:
+            plot_kwargs = {}
 
         gpd.GeoDataFrame(
             {"color": np.arange(len(self.zone_gser))}, geometry=self.zone_gser
-        ).plot("color", ax=ax, cmap=cmap, **plot_kws)
+        ).plot("color", ax=ax, cmap=cmap, **plot_kwargs)
 
         return ax
```

### Comparing `pylandstats-3.0.0rc1/pylandstats.egg-info/PKG-INFO` & `pylandstats-3.0.0rc2/pylandstats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pylandstats
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: Computing landscape metrics in the Python ecosystem.
 Author-email: Martí Bosch <marti.bosch@epfl.ch>
 License: GPL-3.0
 Project-URL: Repository, https://github.com/martibosch/pylandstats
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: black
+Requires-Dist: dask
 Requires-Dist: geopandas
 Requires-Dist: matplotlib>=2.2
 Requires-Dist: numba; platform_system == "Windows"
 Requires-Dist: numpy>=1.15
 Requires-Dist: pandas>=0.23
 Requires-Dist: rasterio>=1.0.0
 Requires-Dist: scipy>=1.0.0
```

### Comparing `pylandstats-3.0.0rc1/pyproject.toml` & `pylandstats-3.0.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [build-system]
-requires = ["setuptools>=61.0", "wheel", "numpy", "pythran", "transonic>=0.4.0"]
+requires = ["setuptools>=61.0", "wheel", "numpy", "pythran>=0.16.0", "transonic>=0.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pylandstats"
-version = "3.0.0rc1"
+version = "3.0.0rc2"
 description = "Computing landscape metrics in the Python ecosystem."
 readme = "README.md"
 authors = [
     { name = "Martí Bosch", email = "marti.bosch@epfl.ch" },
 ]
 license = { text = "GPL-3.0" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "black",
+    "dask",
     "geopandas",
     "matplotlib >= 2.2",
     "numba ; platform_system == 'Windows'",
     "numpy >= 1.15",
     "pandas >= 0.23",
     "rasterio >= 1.0.0",
     "scipy >= 1.0.0",
@@ -40,22 +42,22 @@
 test = ["black", "coverage[toml]", "pytest", "pytest-cov", "python-dotenv", "ruff"]
 dev = ["build", "commitizen", "pre-commit", "pip", "toml", "tox", "twine"]
 doc = ["m2r2", "pydata-sphinx-theme", "sphinx"]
 
 [tool.setuptools.packages.find]
 include = ["pylandstats", "pylandstats.*"]
 
-[tool.black]
-line-length = 88
-
 [tool.ruff]
-line-length = 88
 select = ["D", "E", "F", "I"]
+line-length = 88
+
+[tool.ruff.format]
+docstring-code-format = true
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.ruff.isort]
 known-first-party = ["pylandstats"]
 
 [tool.ruff.per-file-ignores]
 "**/__init__.py" = ["F403"]
@@ -82,9 +84,13 @@
 version_provider = "pep621"
 version_files = [
     "pylandstats/__init__.py",
     "pyproject.toml:version"
 ]
 
 [tool.cibuildwheel]
-build = ["cp38-*", "cp39-*", "cp310-*", "cp311-*"]
+build = ["cp38-*", "cp39-*", "cp310-*", "cp311-*", "cp312-*"]
 skip = "*-musllinux_i686"
+
+[tool.codespell]
+ignore-words-list = "te"
+skip = "CHANGELOG.md"
```

### Comparing `pylandstats-3.0.0rc1/setup.py` & `pylandstats-3.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `pylandstats-3.0.0rc1/tests/test_pylandstats.py` & `pylandstats-3.0.0rc2/tests/test_pylandstats.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         # patch-level metrics
         self.assertTrue((ls.area()["area"] > 0).all())
         self.assertTrue((ls.perimeter()["perimeter"] > 0).all())
         self.assertTrue((ls.perimeter_area_ratio()["perimeter_area_ratio"] > 0).all())
         self.assertTrue((ls.shape_index()["shape_index"] >= 1).all())
         _fractal_dimension_ser = ls.fractal_dimension()["fractal_dimension"]
         self.assertTrue((_fractal_dimension_ser <= 2).all())
-        # ACHTUNG: ugly hardcoded tolerance to correct for misterious errors in GitHub
+        # ACHTUNG: ugly hardcoded tolerance to correct for mysterious errors in GitHub
         # Actions with some Python versions
         self.assertTrue((_fractal_dimension_ser >= 1 - 1e-3).all())
         self.assertTrue((ls.core_area()["core_area"] >= 0).all())
         self.assertTrue((ls.number_of_core_areas()["number_of_core_areas"] >= 0).all())
         _core_area_index_ser = ls.core_area_index()["core_area_index"]
         self.assertTrue((_core_area_index_ser >= 0).all())
         self.assertTrue((_core_area_index_ser < 100).all())
@@ -389,15 +389,15 @@
         self.assertAlmostEqual(ax.get_xlim()[0], ls.transform.xoff)
         self.assertAlmostEqual(ax.get_ylim()[1], ls.transform.yoff)
 
         # test legend arguments
         self.assertIsNone(ls.plot_landscape(legend=False).get_legend())
         self.assertIsNotNone(ls.plot_landscape(legend=True))
         self.assertIsNotNone(
-            ls.plot_landscape(legend=True, legend_kws=dict(loc="center right"))
+            ls.plot_landscape(legend=True, legend_kwargs=dict(loc="center right"))
         )
 
 
 class TestMultiLandscape(unittest.TestCase):
     def setUp(self):
         from pylandstats import multilandscape
 
@@ -429,41 +429,44 @@
     def test_multilandscape_init(self):
         from pylandstats import multilandscape
 
         # test that we cannot instantiate an abstract class
         self.assertRaises(TypeError, multilandscape.MultiLandscape)
 
         # test that if we init a MultiLandscape from filepaths, Landscape instances are
-        # automaticaly built
+        # automatically built
         ml = self.InstantiableMultiLandscape(
             self.landscape_fps, self.attribute_name, self.attribute_values
         )
-        for landscape in ml.landscapes:
+        for landscape in ml.landscape_ser:
             self.assertIsInstance(landscape, pls.Landscape)
         # test that we can pass keyword arguments to the `Landscape` instantiation when
         # providing filepaths
-        landscape_kws = {"neighborhood_rule": "4"}
+        landscape_kwargs = {"neighborhood_rule": "4"}
         ml = self.InstantiableMultiLandscape(
             self.landscape_fps,
             self.attribute_name,
             self.attribute_values,
-            **landscape_kws,
+            **landscape_kwargs,
         )
-        for landscape in ml.landscapes:
+        for landscape in ml.landscape_ser:
             self.assertEqual(
-                landscape.neighborhood_rule, landscape_kws["neighborhood_rule"]
+                landscape.neighborhood_rule, landscape_kwargs["neighborhood_rule"]
             )
         # test that if we instantiate providing `Landscape` instances, the provided
         # keyword arguments are ignored
         ml = self.InstantiableMultiLandscape(
-            self.landscapes, self.attribute_name, self.attribute_values, **landscape_kws
+            self.landscapes,
+            self.attribute_name,
+            self.attribute_values,
+            **landscape_kwargs,
         )
-        for landscape in ml.landscapes:
+        for landscape in ml.landscape_ser:
             self.assertNotEqual(
-                landscape.neighborhood_rule, landscape_kws["neighborhood_rule"]
+                landscape.neighborhood_rule, landscape_kwargs["neighborhood_rule"]
             )
 
         # from this point on, always instantiate from filepaths
 
         # test that constructing a MultiLandscape where the list of values of the
         # identifying attributes `attribute_values` (in this example, the list of
         # resolutions `[100, 250]`) mismatches the length of the list of landscapes
@@ -479,15 +482,15 @@
     def test_multilandscape_dataframes(self):
         ml = self.InstantiableMultiLandscape(
             self.landscape_fps, self.attribute_name, self.attribute_values
         )
         # test that the data frames that result from `compute_class_metrics_df` and
         # `compute_landscape_metrics_df` are well constructed
         class_metrics_df = ml.compute_class_metrics_df()
-        attribute_values = getattr(ml, ml.attribute_name)
+        attribute_values = ml.landscape_ser.index
         self.assertTrue(np.all(class_metrics_df.columns == pls.Landscape.CLASS_METRICS))
         self.assertTrue(
             np.all(
                 class_metrics_df.index
                 == pd.MultiIndex.from_product([ml.present_classes, attribute_values])
             )
         )
@@ -496,18 +499,18 @@
             np.all(landscape_metrics_df.columns == pls.Landscape.LANDSCAPE_METRICS)
         )
         self.assertTrue(np.all(landscape_metrics_df.index == attribute_values))
 
         # now test the same but with an analysis that only considers a subset of metrics
         # and a subset of classes
         metrics = ["total_area", "edge_density", "proportion_of_landscape"]
-        classes = self.landscapes[0].classes[:2]
+        classes = ml.landscape_ser.iloc[0].classes[:2]
 
         class_metrics_df = ml.compute_class_metrics_df(metrics=metrics, classes=classes)
-        attribute_values = getattr(ml, ml.attribute_name)
+        attribute_values = ml.landscape_ser.index
         self.assertTrue(np.all(class_metrics_df.columns == metrics))
         self.assertTrue(
             np.all(
                 class_metrics_df.index
                 == pd.MultiIndex.from_product([classes, attribute_values])
             )
         )
@@ -535,88 +538,92 @@
                     np.count_nonzero(fillna_df[metric][nofillna_df[metric].isna()]),
                     0,
                 )
             else:
                 # the columns for this metric should be identical in both data frames
                 self.assertTrue(fillna_df[metric].equals(nofillna_df[metric]))
 
-    def test_multilandscape_metrics_kws(self):
+    def test_multilandscape_metrics_kwargs(self):
         # Instantiate two multilandscape analyses, one with FRAGSTATS' defaults and the
         # other with keyword arguments specifying the total area in meters and including
         # the boundary in the computation of the total edge.
         ml = self.InstantiableMultiLandscape(
             self.landscape_fps, self.attribute_name, self.attribute_values
         )
         # entropy metrics that accept a `base` keyword argument (all entropy metrics
         # except for Shannon's diversity index and contagion)
         entropy_metrics = [
             "entropy",
             "joint_entropy",
             "conditional_entropy",
             "mutual_information",
         ]
-        metrics_kws = {
+        metrics_kwargs = {
             "total_area": {"hectares": False},
             "perimeter_area_ratio_mn": {"hectares": True},
             "total_edge": {"count_boundary": True},
             **{entropy_metric: {"base": 10} for entropy_metric in entropy_metrics},
         }
 
         class_metrics_df = ml.compute_class_metrics_df()
-        class_metrics_kws_df = ml.compute_class_metrics_df(metrics_kws=metrics_kws)
+        class_metrics_kwargs_df = ml.compute_class_metrics_df(
+            metrics_kwargs=metrics_kwargs
+        )
         landscape_metrics_df = ml.compute_landscape_metrics_df()
-        landscape_metrics_kws_df = ml.compute_landscape_metrics_df(
-            metrics_kws=metrics_kws
+        landscape_metrics_kwargs_df = ml.compute_landscape_metrics_df(
+            metrics_kwargs=metrics_kwargs
         )
-        for attribute_value in getattr(ml, ml.attribute_name):
+        for attribute_value in ml.landscape_ser.index:
             # For all attribute values and all classes, metric values in hectares should
             # be less than in meters, and excluding boundaries should be less or equal
             # than including them
             landscape_metrics = landscape_metrics_df.loc[attribute_value]
-            landscape_metrics_kws = landscape_metrics_kws_df.loc[attribute_value]
+            landscape_metrics_kwargs = landscape_metrics_kwargs_df.loc[attribute_value]
             self.assertLess(
                 landscape_metrics["total_area"],
-                landscape_metrics_kws["total_area"],
+                landscape_metrics_kwargs["total_area"],
             )
             self.assertLessEqual(
                 landscape_metrics["total_edge"],
-                landscape_metrics_kws["total_edge"],
+                landscape_metrics_kwargs["total_edge"],
             )
 
             for class_val in ml.present_classes:
                 class_metrics = class_metrics_df.loc[class_val, attribute_value]
-                class_metrics_kws = class_metrics_kws_df.loc[class_val, attribute_value]
+                class_metrics_kwargs = class_metrics_kwargs_df.loc[
+                    class_val, attribute_value
+                ]
 
                 # It could be that for some attribute values, some classes are not
                 # present within the respective Landscape. If so, some metrics (e.g.,
                 # 'perimeter_area_ratio_mn') will be `nan`, both for the analysis with
                 # and without keyword arguments.
-                # For area and edge metrics, PyLandStats inteprets such `nan` values as
+                # For area and edge metrics, PyLandStats interprets such `nan` values as
                 # 0, which is why we need to include the equality in the comparison
                 if class_metrics.isnull().all():
-                    self.assertTrue(class_metrics_kws.isnull().all())
+                    self.assertTrue(class_metrics_kwargs.isnull().all())
                 else:
                     self.assertLessEqual(
                         class_metrics["total_area"],
-                        class_metrics_kws["total_area"],
+                        class_metrics_kwargs["total_area"],
                     )
                     # we need quite some tolerance because pixel resolutions in raster
-                    # files might be wierd float values, e.g., 99.13213 instead of 100
+                    # files might be weird float values, e.g., 99.13213 instead of 100
                     # (meters)
                     self.assertLessEqual(
                         class_metrics["total_edge"],
-                        1.01 * class_metrics_kws["total_edge"],
+                        1.01 * class_metrics_kwargs["total_edge"],
                     )
 
             # For all attribute values, entropy metric values computed with the default
             # base=2 should be greater than those computed with a custom base=10
             for entropy_metric in entropy_metrics:
                 self.assertGreater(
                     landscape_metrics[entropy_metric],
-                    landscape_metrics_kws[entropy_metric],
+                    landscape_metrics_kwargs[entropy_metric],
                 )
 
     def test_multilandscape_plot_metrics(self):
         ml = self.InstantiableMultiLandscape(
             self.landscape_fps, self.attribute_name, self.attribute_values
         )
 
@@ -629,15 +636,15 @@
         self.assertEqual(len(ax.lines), 1)
         # test that there are two lines if we add the plot of a single metric (e.g., at
         # the level of an existent class) to the previous axis
         ax = ml.plot_metric("patch_density", class_val=existent_class_val, ax=ax)
         self.assertEqual(len(ax.lines), 2)
         # test that the x data of any line corresponds to the attribute values
         for line in ax.lines:
-            self.assertTrue(np.all(line.get_xdata() == getattr(ml, ml.attribute_name)))
+            self.assertTrue(np.all(line.get_xdata() == ml.landscape_ser.index))
 
         # test metric label arguments/settings
         # when passing default arguments, the axis ylabel must be the one set within the
         # settings module
         self.assertEqual(
             ml.plot_metric("edge_density").get_ylabel(),
             pls.settings.metric_label_dict["edge_density"],
@@ -687,15 +694,15 @@
         # we have `len(ml)` axis, therefore the actual `figwidth` must be
         # `len(ml) * rc_figwidth`
         self.assertAlmostEqual(figwidth, len(ml) * rc_figwidth)
         self.assertAlmostEqual(figheight, rc_figheight)
         # if instead, we customize the figure size, the dimensions of the resulting
         # figure must be the customized ones
         custom_figsize = (10, 10)
-        fig = ml.plot_landscapes(subplots_kws={"figsize": custom_figsize})
+        fig = ml.plot_landscapes(subplots_kwargs={"figsize": custom_figsize})
         figwidth, figheight = fig.get_size_inches()
         self.assertAlmostEqual(custom_figsize[0], figwidth)
         self.assertAlmostEqual(custom_figsize[1], figheight)
 
 
 class TestSpatioTemporalAnalysis(unittest.TestCase):
     def setUp(self):
@@ -706,89 +713,91 @@
             path.join(tests_data_dir, "ls250_06.tif"),
             path.join(tests_data_dir, "ls250_12.tif"),
         ]
         self.dates = [2006, 2012]
         self.inexistent_class_val = 999
 
     def test_spatiotemporalanalysis_init(self):
-        # test that the `attribute_name` is dates, and that if the `dates` argument is
-        # not provided when instantiating a `SpatioTemporalAnalysis`, the dates
+        # test that the landscape index name is dates, and that if the `dates` argument
+        # is not provided when instantiating a `SpatioTemporalAnalysis`, the dates
         # attribute is properly and automatically generated
         sta = pls.SpatioTemporalAnalysis(self.landscape_fps)
-        self.assertEqual(sta.attribute_name, "dates")
-        self.assertEqual(len(sta), len(sta.dates))
+        self.assertEqual(sta.landscape_ser.index.name, "dates")
+        self.assertEqual(len(sta), len(sta.landscape_ser))
 
         # test the `neighborhood_rule` argument
         neighborhood_rule = "4"
         other_neighborhood_rule = "8"
         # test that if provided and the elements of `landscapes` are filepaths, the
         # value is passed to each landscape
         for ls in pls.SpatioTemporalAnalysis(
             self.landscape_fps,
             dates=self.dates,
             neighborhood_rule=neighborhood_rule,
-        ).landscapes:
+        ).landscape_ser:
             self.assertEqual(ls.neighborhood_rule, neighborhood_rule)
         # test that if provided and the elements of `landscapes` are `Landscape`
         # instances, the value is ignored
         for ls in pls.SpatioTemporalAnalysis(
             [
                 pls.Landscape(landscape_fp, neighborhood_rule=other_neighborhood_rule)
                 for landscape_fp in self.landscape_fps
             ],
             dates=self.dates,
             neighborhood_rule=neighborhood_rule,
-        ).landscapes:
+        ).landscape_ser:
             self.assertEqual(ls.neighborhood_rule, other_neighborhood_rule)
         # test that if not provided and the elements of `landscapes` are filepaths, the
         # default value is taken
         for ls in pls.SpatioTemporalAnalysis(
             self.landscape_fps, dates=self.dates
-        ).landscapes:
+        ).landscape_ser:
             self.assertEqual(
                 ls.neighborhood_rule, pls.settings.DEFAULT_NEIGHBORHOOD_RULE
             )
 
     def test_spatiotemporalanalysis_dataframes(self):
         # test with the default constructor
         sta = pls.SpatioTemporalAnalysis(self.landscape_fps)
 
         # test that the data frames that result from `compute_class_metrics_df` and
         # `compute_landscape_metrics_df` are well constructed
         class_metrics_df = sta.compute_class_metrics_df()
         self.assertTrue(
             np.all(
                 class_metrics_df.index
-                == pd.MultiIndex.from_product([sta.present_classes, sta.dates])
+                == pd.MultiIndex.from_product(
+                    [sta.present_classes, sta.landscape_ser.index]
+                )
             )
         )
         landscape_metrics_df = sta.compute_landscape_metrics_df()
-        self.assertTrue(np.all(landscape_metrics_df.index == sta.dates))
+        self.assertTrue(np.all(landscape_metrics_df.index == sta.landscape_ser.index))
 
         # now test the same but with an analysis that only considers a subset of metrics
         # and a subset of classes
         metrics = ["total_area", "edge_density", "proportion_of_landscape"]
         classes = sta.present_classes[:2]
 
         class_metrics_df = sta.compute_class_metrics_df(
             metrics=metrics, classes=classes
         )
         self.assertTrue(
             np.all(
                 class_metrics_df.index
-                == pd.MultiIndex.from_product([classes, sta.dates])
+                == pd.MultiIndex.from_product([classes, sta.landscape_ser.index])
             )
         )
         # 'proportion_of_landscape' cannot be computed at the landscape level (TODO:
         # test for that elsewhere)
         landscape_metrics = metrics[:2]
         landscape_metrics_df = sta.compute_landscape_metrics_df(
             metrics=landscape_metrics
         )
-        self.assertTrue(np.all(landscape_metrics_df.index == sta.dates))
+        self.assertTrue(np.all(landscape_metrics_df.index == sta.landscape_ser.index))
 
     def test_spatiotemporalanalysis_plot_metrics(self):
         sta = pls.SpatioTemporalAnalysis(self.landscape_fps, dates=self.dates)
 
         # test for `None` (landscape-level) and an existing class (class-level)
         for class_val in [None, sta.present_classes[0]]:
             # test that the x data of the line corresponds to the dates
@@ -828,82 +837,82 @@
         # files as `zones`
         # first test the GeoSeries and list-like of shapely geometries, which work like
         # the others except that we cannot set a column as the zone index
         zone_gser = self.zone_gdf["geometry"].copy()
         za = pls.ZonalAnalysis(self.landscape_fp, zone_gser)
         self.assertLessEqual(len(za), len(self.zone_gdf))
         self.assertTrue(np.all(za.zone_gser.index == zone_gser.index))
-        # also test that attribute name is properly set when using geoseries as `zones`
-        # first test for a geoseries with name and unnamed index
+        # also test that landscape index name is properly set when using geoseries as
+        # `zones` first test for a geoseries with name and unnamed index
         zone_gser.name = "bar"
         za = pls.ZonalAnalysis(self.landscape_fp, zone_gser)
-        self.assertEqual(za.attribute_name, zone_gser.name)
+        self.assertEqual(za.landscape_ser.index.name, zone_gser.name)
         # now test that for a named geoseries with a named index, the geoseries index
         # name takes precedence
         zone_gser.index.name = "name"
         za = pls.ZonalAnalysis(self.landscape_fp, zone_gser)
-        self.assertEqual(za.attribute_name, zone_gser.index.name)
+        self.assertEqual(za.landscape_ser.index.name, zone_gser.index.name)
         # test that for an named geoseries with an unnamed index, the geoseries name is
         # taken
         zone_gser.index.name = None
         za = pls.ZonalAnalysis(self.landscape_fp, zone_gser)
-        self.assertEqual(za.attribute_name, zone_gser.name)
+        self.assertEqual(za.landscape_ser.index.name, zone_gser.name)
         # test overriding the zone index
         zone_index = zone_gser.index + 1
         za = pls.ZonalAnalysis(self.landscape_fp, zone_gser, zone_index=zone_index)
         self.assertTrue(np.all(za.zone_gser.index == zone_index))
         # test overriding the zone index with a named index
         zone_index = zone_index.rename("foo")
         za = pls.ZonalAnalysis(self.landscape_fp, zone_gser, zone_index=zone_index)
-        self.assertEqual(za.attribute_name, zone_index.name)
+        self.assertEqual(za.landscape_ser.index.name, zone_index.name)
         # test that for a list-like of shapely geometries, the CRS of the landscape is
         # taken
         zones = list(zone_gser)
         za = pls.ZonalAnalysis(self.landscape_fp, zones)
         self.assertEqual(za.zone_gser.crs, self.landscape_crs)
 
         # now test the GeoDataFrame and geopandas file
         zone_index_col = "GMDNAME"
         for zones in self.zones_fp, self.zone_gdf:
             # test init
             za = pls.ZonalAnalysis(self.landscape_fp, zones)
             self.assertLessEqual(len(za), len(self.zone_gdf))
             self.assertTrue(
-                np.all(np.isin(getattr(za, za.attribute_name), self.zone_gdf.index))
+                np.all(np.isin(za.landscape_ser.index, self.zone_gdf.index))
             )
             # test that we can set a column as the zone index
             za = pls.ZonalAnalysis(self.landscape_fp, zones, zone_index=zone_index_col)
             self.assertTrue(
                 np.all(
                     np.isin(
-                        getattr(za, zone_index_col),
+                        za.zone_gser.index,
                         self.zone_gdf[zone_index_col],
                     )
                 )
             )
 
         # test that we can still pass a raster labelled array
-        # test that the attribute names and values are consistent with the provided
+        # test that the landscape index name and values are consistent with the provided
         # `label_arr`
         za = pls.ZonalAnalysis(self.landscape_fp, self.label_arr)
-        self.assertEqual(za.attribute_name, "zone")
+        self.assertEqual(za.landscape_ser.index.name, "zone")
         # the number of zones must be equal to the number of unique labels (excluding
         # the nodata value)
         zone_nodata = 0
         zones = list(set(np.unique(self.label_arr)).difference({zone_nodata}))
         self.assertEqual(len(za), len(zones))
-        # test that Landscape instances are automaticaly built
-        for landscape in za.landscapes:
+        # test that Landscape instances are automatically built
+        for landscape in za.landscape_ser:
             self.assertIsInstance(landscape, pls.Landscape)
         # test that the zone index corresponds to the zone labels
         self.assertTrue(np.all(np.isin(zones, za.zone_gser.index)))
         # test that we can override the zone index
         zone_index = pd.Series(range(1, len(zones) + 1), name="foo")
         za = pls.ZonalAnalysis(self.landscape_fp, self.label_arr, zone_index=zone_index)
-        self.assertEqual(za.attribute_name, "foo")
+        self.assertEqual(za.landscape_ser.index.name, "foo")
         self.assertTrue(np.all(za.zone_gser.index == zone_index))
 
         # test that we can override the nodata value
         zone_nodata = 255
         label_arr = np.where(self.label_arr != 0, self.label_arr, zone_nodata)
         # in this case, if we do not specify the nodata value, we will have another zone
         # (since by default, 0 are considered nodata)
@@ -920,18 +929,18 @@
         # test the `neighborhood_rule` argument
         neighborhood_rule = "4"
         # test that if provided, the value is passed to each landscape
         for ls in pls.ZonalAnalysis(
             self.landscape_fp,
             zone_gser,
             neighborhood_rule=neighborhood_rule,
-        ).landscapes:
+        ).landscape_ser:
             self.assertEqual(ls.neighborhood_rule, neighborhood_rule)
         # test that if not provided, the default value is taken
-        for ls in pls.ZonalAnalysis(self.landscape_fp, self.label_arr).landscapes:
+        for ls in pls.ZonalAnalysis(self.landscape_fp, self.label_arr).landscape_ser:
             self.assertEqual(
                 ls.neighborhood_rule, pls.settings.DEFAULT_NEIGHBORHOOD_RULE
             )
 
     def test_zonal_plot_metrics(self):
         za = pls.ZonalAnalysis(self.landscape_fp, self.zone_gdf)
 
@@ -951,31 +960,35 @@
     def test_compute_zonal_statistics_gdf(self):
         za = pls.ZonalAnalysis(self.landscape_fp, self.zone_gdf)
 
         # test that the gdf has the proper shape (number of zones, number of metrics +
         # geometry column)
         for class_val in [None, za.present_classes[0]]:
             metrics = ["patch_density"]
-            zs_gdf = za.compute_zonal_statistics_gdf(metrics, class_val=class_val)
+            zs_gdf = za.compute_zonal_statistics_gdf(
+                metrics=metrics, class_val=class_val
+            )
             self.assertEqual(zs_gdf.shape, (len(self.zone_gdf), len(metrics) + 1))
             # test that the crs is set correctly
             self.assertEqual(zs_gdf.crs, self.zone_gdf.crs)
             # test that the geometry column is not None
             self.assertFalse(zs_gdf.geometry.isna().any())
 
             # test that the zonal statistics when excluding boundaries should be less or
             # equal than including them
             metric = "total_edge"
-            metric_kws = {"count_boundary": True}
+            metric_kwargs = {"count_boundary": True}
             self.assertLessEqual(
-                za.compute_zonal_statistics_gdf([metric], class_val=class_val)[
+                za.compute_zonal_statistics_gdf(metrics=[metric], class_val=class_val)[
                     metric
                 ].sum(),
                 za.compute_zonal_statistics_gdf(
-                    [metric], class_val=class_val, metrics_kws={metric: metric_kws}
+                    metrics=[metric],
+                    class_val=class_val,
+                    metrics_kwargs={metric: metric_kwargs},
                 )[metric].sum(),
             )
 
     def test_buffer_init(self):
         naive_gser = gpd.GeoSeries([self.geom])
         gser = gpd.GeoSeries([self.geom], crs=geom_crs)
         naive_gdf = gpd.GeoDataFrame(geometry=naive_gser)
@@ -1027,15 +1040,15 @@
             pls.BufferAnalysis(
                 self.landscape_fp,
                 gdf,
                 self.buffer_dists,
                 base_geom_crs=geom_crs,
             ),
         ]:
-            self.assertEqual(ba.attribute_name, "buffer_dist")
+            self.assertEqual(ba.landscape_ser.index.name, "buffer_dist")
             self.assertEqual(len(ba), len(ba.zone_gser))
 
         # test that we cannot instantiate a `BufferAnalysis` with `buffer_rings=True` if
         # `base_mask` is a polygon or a GeoSeries containing a polygon
         polygon = self.geom.buffer(1000)  # this will return a polygon instance
         self.assertRaises(
             ValueError,
@@ -1118,22 +1131,22 @@
         neighborhood_rule = "4"
         # test that the value is passed to each landscape
         for ls in pls.ZonalGridAnalysis(
             self.landscape_fp,
             zone_width=zone_width,
             zone_height=zone_height,
             neighborhood_rule=neighborhood_rule,
-        ).landscapes:
+        ).landscape_ser:
             self.assertEqual(ls.neighborhood_rule, neighborhood_rule)
         # test that if not provided, the default value is taken
         for ls in pls.ZonalGridAnalysis(
             self.landscape_fp,
             zone_width=zone_width,
             zone_height=zone_height,
-        ).landscapes:
+        ).landscape_ser:
             self.assertEqual(
                 ls.neighborhood_rule, pls.settings.DEFAULT_NEIGHBORHOOD_RULE
             )
 
 
 class TestSpatioTemporalZonalAnalysis(unittest.TestCase):
     def setUp(self):
@@ -1172,166 +1185,213 @@
             ],
             ["zone", "buffer_dist", "grid_cell"],
         )
 
     def test_init(self):
         # we will just test the base init, the rest of functionalities have already been
         # tested above (in `TestSpatioTemporalAnalysis` and `TestZonalAnalysis`)
-        for _class, init_args, init_kws, attr_name in self.init_combinations:
+        for _class, init_args, init_kwargs, attr_name in self.init_combinations:
             # test zones and dates
-            stza = _class(self.landscape_fps, *init_args, dates=self.dates, **init_kws)
-            self.assertEqual(len(stza.zone_gser), len(stza.stas))
-            self.assertEqual(stza.attribute_name, attr_name)
-
-            for sta in stza.stas:
-                self.assertEqual(sta.dates, self.dates)
+            stza = _class(
+                self.landscape_fps, *init_args, dates=self.dates, **init_kwargs
+            )
+            # test that we have the same zone labels in `zone_gser` and `landscape_ser`
+            self.assertTrue(
+                (
+                    stza.zone_gser.index
+                    == stza.landscape_ser.index.get_level_values(
+                        stza.zone_gser.index.name
+                    ).unique()
+                ).all()
+            )
+            # test the `zone_gser` index name
+            self.assertEqual(stza.zone_gser.index.name, attr_name)
+            # test that we have the same date labels in `dates` and `landscape_ser`
+            self.assertTrue(
+                (
+                    self.dates
+                    == stza.landscape_ser.index.get_level_values("date").unique()
+                ).all()
+            )
 
             # test the `neighborhood_rule` argument
             # test that if not provided, the default value is taken
-            for sta in stza.stas:
-                for ls in sta.landscapes:
-                    self.assertEqual(
-                        ls.neighborhood_rule,
-                        pls.settings.DEFAULT_NEIGHBORHOOD_RULE,
-                    )
+            for ls in stza.landscape_ser:
+                self.assertEqual(
+                    ls.neighborhood_rule,
+                    pls.settings.DEFAULT_NEIGHBORHOOD_RULE,
+                )
             neighborhood_rule = "4"
             # test that if provided, the value is passed to each landscape
             stza = _class(
                 self.landscape_fps,
                 *init_args,
                 neighborhood_rule=neighborhood_rule,
-                **init_kws,
+                **init_kwargs,
             )
-            for sta in stza.stas:
-                for ls in sta.landscapes:
-                    self.assertEqual(ls.neighborhood_rule, neighborhood_rule)
+            for ls in stza.landscape_ser:
+                self.assertEqual(ls.neighborhood_rule, neighborhood_rule)
 
     def test_dataframes(self):
-        for _class, init_args, init_kws, _ in self.init_combinations:
-            stza = _class(self.landscape_fps, *init_args, dates=self.dates, **init_kws)
+        for _class, init_args, init_kwargs, _ in self.init_combinations:
+            stza = _class(
+                self.landscape_fps, *init_args, dates=self.dates, **init_kwargs
+            )
             zone_index = stza.zone_gser.index
+            dates = stza.landscape_ser.index.get_level_values("date").unique()
 
             # test that the data frames that result from `compute_class_metrics_df` and
-            # `compute_landscape_metrics_df` are well constructed
+            # `compute_landscape_metrics_df` are well constructed, i.e., they are a
+            # subset of all class/zone/date combinations
             class_metrics_df = stza.compute_class_metrics_df()
             self.assertTrue(
-                np.all(
-                    class_metrics_df.index
-                    == pd.MultiIndex.from_product(
-                        [zone_index, stza.present_classes, stza.dates]
+                class_metrics_df.index.isin(
+                    pd.MultiIndex.from_product(
+                        [stza.present_classes, zone_index, dates]
                     )
-                )
+                ).all()
             )
             landscape_metrics_df = stza.compute_landscape_metrics_df()
             self.assertTrue(
-                np.all(
-                    landscape_metrics_df.index
-                    == pd.MultiIndex.from_product([zone_index, stza.dates])
-                )
+                landscape_metrics_df.index.isin(
+                    pd.MultiIndex.from_product([zone_index, dates])
+                ).all()
             )
 
             # now test the same but with an analysis that only considers a subset of
             # metrics and a subset of classes
             metrics = ["total_area", "edge_density", "proportion_of_landscape"]
             classes = stza.present_classes[:2]
 
             class_metrics_df = stza.compute_class_metrics_df(
                 metrics=metrics, classes=classes
             )
             self.assertTrue(
-                np.all(
-                    class_metrics_df.index
-                    == pd.MultiIndex.from_product([zone_index, classes, stza.dates])
-                )
+                class_metrics_df.index.isin(
+                    pd.MultiIndex.from_product([classes, zone_index, dates])
+                ).all()
             )
             # 'proportion_of_landscape' cannot be computed at the landscape level (TODO:
             # test for that elsewhere)
             landscape_metrics = metrics[:2]
             landscape_metrics_df = stza.compute_landscape_metrics_df(
                 metrics=landscape_metrics
             )
             self.assertTrue(
-                np.all(
-                    landscape_metrics_df.index
-                    == pd.MultiIndex.from_product([zone_index, stza.dates])
-                )
+                landscape_metrics_df.index.isin(
+                    pd.MultiIndex.from_product([zone_index, dates])
+                ).all()
             )
 
     def test_compute_zonal_statistics_gdf(self):
-        for _class, init_args, init_kws, _ in self.init_combinations:
-            stza = _class(self.landscape_fps, *init_args, dates=self.dates, **init_kws)
+        for _class, init_args, init_kwargs, _ in self.init_combinations:
+            stza = _class(
+                self.landscape_fps, *init_args, dates=self.dates, **init_kwargs
+            )
             # test that the gdf has the proper shape (number of zones, number of metrics
             # + geometry column)
             for class_val in [None, stza.present_classes[0]]:
                 metrics = ["patch_density"]
-                zs_gdf = stza.compute_zonal_statistics_gdf(metrics, class_val=class_val)
-                self.assertEqual(
-                    zs_gdf.shape,
-                    (len(stza.zone_gser) * len(self.dates), len(metrics) + 1),
+                zs_gdf = stza.compute_zonal_statistics_gdf(
+                    metrics=metrics, class_val=class_val
                 )
+                self.assertLessEqual(
+                    zs_gdf.shape[0],
+                    len(stza.zone_gser),
+                )
+                self.assertEqual(zs_gdf.shape[1], len(metrics) * len(self.dates) + 1)
                 # test that the crs is set correctly
                 self.assertEqual(zs_gdf.crs, self.zone_gser.crs)
                 # test that the geometry column is not None
                 self.assertFalse(zs_gdf.geometry.isna().any())
 
                 # test that the zonal statistics when excluding boundaries should be
                 # less or equal than including them
                 metric = "total_edge"
-                metric_kws = {"count_boundary": True}
+                metric_kwargs = {"count_boundary": True}
                 self.assertLessEqual(
-                    stza.compute_zonal_statistics_gdf([metric], class_val=class_val)[
-                        metric
-                    ].sum(),
                     stza.compute_zonal_statistics_gdf(
-                        [metric], class_val=class_val, metrics_kws={metric: metric_kws}
-                    )[metric].sum(),
+                        metrics=[metric], class_val=class_val
+                    )[metric]
+                    .sum()
+                    .sum(),
+                    stza.compute_zonal_statistics_gdf(
+                        metrics=[metric],
+                        class_val=class_val,
+                        metrics_kwargs={metric: metric_kwargs},
+                    )[metric]
+                    .sum()
+                    .sum(),
                 )
 
     def test_plot_metric(self):
-        for _class, init_args, init_kws, _ in self.init_combinations:
-            stza = _class(self.landscape_fps, *init_args, dates=self.dates, **init_kws)
+        for _class, init_args, init_kwargs, _ in self.init_combinations:
+            stza = _class(
+                self.landscape_fps, *init_args, dates=self.dates, **init_kwargs
+            )
             # test for `None` (landscape-level) and an existing class (class-level)
-            for class_val in [None, stza.stas[0].present_classes[0]]:
-                ax = stza.plot_metric("patch_density", class_val=class_val)
-                # test that there is a line for each zone
-                self.assertEqual(len(ax.lines), len(stza.zone_gser))
+            metric = "patch_density"
+            for class_val in [None, stza.present_classes[0]]:
+                ax = stza.plot_metric(metric, class_val=class_val)
+                # test that there is a line for each zone with that metric
+                if class_val is None:
+                    metric_ser = stza.compute_landscape_metrics_df(metrics=[metric])[
+                        metric
+                    ]
+                else:
+                    metric_ser = stza.compute_class_metrics_df(
+                        metrics=[metric], classes=[class_val]
+                    )[metric]
+                num_lines = len(
+                    metric_ser.index.get_level_values(
+                        stza.zone_gser.index.name
+                    ).unique()
+                )
+                self.assertEqual(
+                    len(ax.lines),
+                    num_lines,
+                )
                 # test that there is a legend label for each zone
-                handles, labels = ax.get_legend_handles_labels()
-                self.assertEqual(len(labels), len(stza.zone_gser))
+                _, labels = ax.get_legend_handles_labels()
+                self.assertEqual(len(labels), num_lines)
 
     def test_plot_landscapes(self):
-        for _class, init_args, init_kws, _ in self.init_combinations:
-            stza = _class(self.landscape_fps, *init_args, dates=self.dates, **init_kws)
+        for _class, init_args, init_kwargs, _ in self.init_combinations:
+            stza = _class(
+                self.landscape_fps, *init_args, dates=self.dates, **init_kwargs
+            )
+            dates = stza.landscape_ser.index.get_level_values("date").unique()
+
             fig = stza.plot_landscapes()
 
             # there must be one column for each buffer distance and one row for each
             # date
-            self.assertEqual(len(fig.axes), len(stza.zone_gser) * len(stza.dates))
+            self.assertEqual(len(fig.axes), len(stza.zone_gser) * len(dates))
 
             # returned axes must be instances of matplotlib axes
             for ax in fig.axes:
                 self.assertIsInstance(ax, plt.Axes)
 
             # test that by default, the dimensions of the resulting will come from
             # matplotlib's settings
             rc_figwidth, rc_figheight = plt.rcParams["figure.figsize"]
             figwidth, figheight = fig.get_size_inches()
             # the actual `figwidth` must be `len(stba.buffer_dists) * rc_figwidth` and
             # `figheight` must be `len(stba.dates) * rc_figheight`
             self.assertAlmostEqual(figwidth, len(stza.zone_gser) * rc_figwidth)
-            self.assertAlmostEqual(figheight, len(stza.dates) * rc_figheight)
+            self.assertAlmostEqual(figheight, len(dates) * rc_figheight)
             # if instead, we customize the figure size, the dimensions of the resulting
             # figure must be the customized ones
             custom_figsize = (10, 10)
-            fig = stza.plot_landscapes(subplots_kws={"figsize": custom_figsize})
+            fig = stza.plot_landscapes(subplots_kwargs={"figsize": custom_figsize})
             figwidth, figheight = fig.get_size_inches()
             self.assertAlmostEqual(custom_figsize[0], figwidth)
             self.assertAlmostEqual(custom_figsize[1], figheight)
 
             # first row has the date as title
-            for date, ax in zip(stza.dates, fig.axes):
+            for date, ax in zip(dates, fig.axes):
                 self.assertEqual(str(date), ax.get_title())
             # first column has the buffer distance as `ylabel`
             for zone, i in zip(
-                stza.zone_gser.index, range(0, len(fig.axes), len(stza.dates))
+                stza.zone_gser.index, range(0, len(fig.axes), len(dates))
             ):
                 self.assertEqual(str(zone), fig.axes[i].get_ylabel())
```

