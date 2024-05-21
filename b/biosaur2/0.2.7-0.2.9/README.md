# Comparing `tmp/biosaur2-0.2.7.tar.gz` & `tmp/biosaur2-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosaur2-0.2.7.tar", last modified: Mon Oct 24 13:51:47 2022, max compression
+gzip compressed data, was "biosaur2-0.2.9.tar", last modified: Wed Dec  7 15:20:19 2022, max compression
```

## Comparing `biosaur2-0.2.7.tar` & `biosaur2-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 13:51:47.685840 biosaur2-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-24 13:51:19.000000 biosaur2-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-10-24 13:51:19.000000 biosaur2-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-10-24 13:51:47.681840 biosaur2-0.2.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     1541 2022-10-24 13:51:19.000000 biosaur2-0.2.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)        6 2022-10-24 13:51:19.000000 biosaur2-0.2.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 13:51:47.681840 biosaur2-0.2.7/biosaur2/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 13:51:19.000000 biosaur2-0.2.7/biosaur2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  1101144 2022-10-24 13:51:47.000000 biosaur2-0.2.7/biosaur2/cutils.c
--rw-r--r--   0 runner    (1001) docker     (121)    30237 2022-10-24 13:51:19.000000 biosaur2-0.2.7/biosaur2/cutils.pyx
--rwxr-xr-x   0 runner    (1001) docker     (121)    19209 2022-10-24 13:51:19.000000 biosaur2-0.2.7/biosaur2/main.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7793 2022-10-24 13:51:19.000000 biosaur2-0.2.7/biosaur2/main_dia.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5359 2022-10-24 13:51:19.000000 biosaur2-0.2.7/biosaur2/search.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19774 2022-10-24 13:51:19.000000 biosaur2-0.2.7/biosaur2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 13:51:47.681840 biosaur2-0.2.7/biosaur2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-10-24 13:51:47.000000 biosaur2-0.2.7/biosaur2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-24 13:51:47.000000 biosaur2-0.2.7/biosaur2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 13:51:47.000000 biosaur2-0.2.7/biosaur2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-24 13:51:47.000000 biosaur2-0.2.7/biosaur2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-24 13:51:47.000000 biosaur2-0.2.7/biosaur2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-24 13:51:47.000000 biosaur2-0.2.7/biosaur2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-24 13:51:19.000000 biosaur2-0.2.7/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)       57 2022-10-24 13:51:19.000000 biosaur2-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 13:51:47.685840 biosaur2-0.2.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2315 2022-10-24 13:51:19.000000 biosaur2-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 15:20:19.188417 biosaur2-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-12-07 15:19:58.000000 biosaur2-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2022-12-07 15:19:58.000000 biosaur2-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2022-12-07 15:20:19.188417 biosaur2-0.2.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1541 2022-12-07 15:19:58.000000 biosaur2-0.2.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)        6 2022-12-07 15:19:58.000000 biosaur2-0.2.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 15:20:19.188417 biosaur2-0.2.9/biosaur2/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 15:19:58.000000 biosaur2-0.2.9/biosaur2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1101144 2022-12-07 15:20:19.000000 biosaur2-0.2.9/biosaur2/cutils.c
+-rw-r--r--   0 runner    (1001) docker     (122)    30237 2022-12-07 15:19:58.000000 biosaur2-0.2.9/biosaur2/cutils.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (122)    19209 2022-12-07 15:19:58.000000 biosaur2-0.2.9/biosaur2/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7793 2022-12-07 15:19:58.000000 biosaur2-0.2.9/biosaur2/main_dia.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5359 2022-12-07 15:19:58.000000 biosaur2-0.2.9/biosaur2/search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    19941 2022-12-07 15:19:58.000000 biosaur2-0.2.9/biosaur2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 15:20:19.188417 biosaur2-0.2.9/biosaur2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2022-12-07 15:20:19.000000 biosaur2-0.2.9/biosaur2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2022-12-07 15:20:19.000000 biosaur2-0.2.9/biosaur2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-07 15:20:19.000000 biosaur2-0.2.9/biosaur2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-07 15:20:19.000000 biosaur2-0.2.9/biosaur2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2022-12-07 15:20:19.000000 biosaur2-0.2.9/biosaur2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2022-12-07 15:20:19.000000 biosaur2-0.2.9/biosaur2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2022-12-07 15:19:58.000000 biosaur2-0.2.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)       57 2022-12-07 15:19:58.000000 biosaur2-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-07 15:20:19.188417 biosaur2-0.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2315 2022-12-07 15:19:58.000000 biosaur2-0.2.9/setup.py
```

### Comparing `biosaur2-0.2.7/LICENSE` & `biosaur2-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biosaur2-0.2.7/PKG-INFO` & `biosaur2-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosaur2
-Version: 0.2.7
+Version: 0.2.9
 Summary: A feature detection LC-MS1 spectra.
 Author: Mark Ivanov
 Author-email: markmipt@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education
```

### Comparing `biosaur2-0.2.7/README.md` & `biosaur2-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `biosaur2-0.2.7/biosaur2/cutils.c` & `biosaur2-0.2.9/biosaur2/cutils.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 0.29.32 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/core/include"
+            "/opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "biosaur2.cutils",
         "sources": [
             "biosaur2/cutils.pyx"
         ]
     },
     "module_name": "biosaur2.cutils"
@@ -1006,195 +1006,195 @@
 
 static const char *__pyx_f[] = {
   "biosaur2/cutils.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1223,42 +1223,42 @@
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8biosaur2_6cutils___pyx_scope_struct__get_and_calc_values_for_cos_corr;
 struct __pyx_obj_8biosaur2_6cutils___pyx_scope_struct_1_genexpr;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -16257,15 +16257,15 @@
   __Pyx_XDECREF(__pyx_v_orig_idx_val);
   __Pyx_XDECREF(__pyx_v_scan_val);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -16274,29 +16274,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -16307,15 +16307,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -16324,29 +16324,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -16357,15 +16357,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -16374,29 +16374,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -16407,15 +16407,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -16424,29 +16424,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -16457,15 +16457,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -16474,29 +16474,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -16507,212 +16507,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -16728,15 +16728,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -16744,53 +16744,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -16798,30 +16798,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -16836,15 +16836,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -16860,15 +16860,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -16876,53 +16876,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -16930,30 +16930,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -16968,15 +16968,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -16992,15 +16992,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -17008,53 +17008,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -17062,30 +17062,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -17100,176 +17100,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -17864,26 +17864,26 @@
  *     else:
  * 
  */
   __pyx_tuple__2 = PyTuple_Pack(2, __pyx_int_0, __pyx_int_0); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -18776,15 +18776,15 @@
  * cimport openmp
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.10.8/x64/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.0/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `biosaur2-0.2.7/biosaur2/cutils.pyx` & `biosaur2-0.2.9/biosaur2/cutils.pyx`

 * *Files identical despite different names*

### Comparing `biosaur2-0.2.7/biosaur2/main.py` & `biosaur2-0.2.9/biosaur2/main.py`

 * *Files identical despite different names*

### Comparing `biosaur2-0.2.7/biosaur2/main_dia.py` & `biosaur2-0.2.9/biosaur2/main_dia.py`

 * *Files identical despite different names*

### Comparing `biosaur2-0.2.7/biosaur2/search.py` & `biosaur2-0.2.9/biosaur2/search.py`

 * *Files identical despite different names*

### Comparing `biosaur2-0.2.7/biosaur2/utils.py` & `biosaur2-0.2.9/biosaur2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         pep_feature['massCalib'] = pep_feature['mz'] * pep_feature['charge'] - 1.0072765 * pep_feature['charge'] * (-1 if negative_mode else 1)
 
         hills_dict, _, _ = get_and_calc_apex_intensity_and_scan(hills_dict, pep_feature['monoisotope idx'])
 
         pep_feature['scanApex'] = hills_dict['hills_scan_apex'][pep_feature['monoisotope idx']]
         pep_feature['rtApex'] = RT_dict[hills_dict['hills_scan_apex'][pep_feature['monoisotope idx']]+data_start_id]
         pep_feature['intensityApex'] = hills_dict['hills_intensity_apex'][pep_feature['monoisotope idx']]
+        pep_feature['intensitySum'] = sum(hills_dict['hills_intensity_array'][pep_feature['monoisotope idx']])
         pep_feature['rtStart'] = RT_dict[hills_dict['hills_scan_lists'][pep_feature['monoisotope idx']][0]+data_start_id]
         pep_feature['rtEnd'] = RT_dict[hills_dict['hills_scan_lists'][pep_feature['monoisotope idx']][-1]+data_start_id]
         pep_feature['mono_hills_scan_lists'] = hills_dict['hills_scan_lists'][pep_feature['monoisotope idx']]
         pep_feature['mono_hills_intensity_list'] =  hills_dict['hills_intensity_array'][pep_feature['monoisotope idx']]
 
     return peptide_features
 
@@ -85,26 +86,28 @@
             + path.extsep + ('features.tsv' if not hills else 'hills.tsv')
 
     if hills:
 
         columns_for_output = [
             'rtApex',
             'intensityApex',
+            'intensitySum',
             'nScans',
             'mz',
             'rtStart',
             'rtEnd',
             'FAIMS',
             'im',
         ]
     else:
         columns_for_output = [
             'massCalib',
             'rtApex',
             'intensityApex',
+            'intensitySum',
             'charge',
             'nIsotopes',
             'nScans',
             'mz',
             'rtStart',
             'rtEnd',
             'FAIMS',
```

### Comparing `biosaur2-0.2.7/biosaur2.egg-info/PKG-INFO` & `biosaur2-0.2.9/biosaur2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosaur2
-Version: 0.2.7
+Version: 0.2.9
 Summary: A feature detection LC-MS1 spectra.
 Author: Mark Ivanov
 Author-email: markmipt@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education
```

### Comparing `biosaur2-0.2.7/setup.py` & `biosaur2-0.2.9/setup.py`

 * *Files identical despite different names*

