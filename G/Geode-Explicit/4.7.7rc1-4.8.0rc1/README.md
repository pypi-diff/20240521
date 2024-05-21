# Comparing `tmp/Geode_Explicit-4.7.7rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.8.0rc1-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 3139169 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 24-May-21 07:35 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 24-May-21 07:35 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 24-May-21 07:35 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  4021248 b- defN 24-May-21 07:35 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    33792 b- defN 24-May-21 07:35 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  3715072 b- defN 24-May-21 07:35 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   147456 b- defN 24-May-21 07:35 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   135680 b- defN 24-May-21 07:35 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2211 b- defN 24-May-21 07:35 Geode_Explicit-4.7.7rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-21 07:35 Geode_Explicit-4.7.7rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-May-21 07:35 Geode_Explicit-4.7.7rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1130 b- defN 24-May-21 07:35 Geode_Explicit-4.7.7rc1.dist-info/RECORD
-12 files, 8057418 bytes uncompressed, 3137245 bytes compressed:  61.1%
+Zip file size: 361352 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       89 b- defN 24-May-21 18:40 geode_explicit/__init__.py
+-rw-r--r--  2.0 unx      261 b- defN 24-May-21 18:40 geode_explicit/brep.py
+-rw-r--r--  2.0 unx      240 b- defN 24-May-21 18:40 geode_explicit/section.py
+-rwxr-xr-x  2.0 unx   159296 b- defN 24-May-21 18:41 geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   138752 b- defN 24-May-21 18:41 geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   467952 b- defN 24-May-21 18:41 geode_explicit/lib64/libGeode-Explicit_brep.so
+-rwxr-xr-x  2.0 unx    35352 b- defN 24-May-21 18:41 geode_explicit/lib64/libGeode-Explicit_common.so
+-rwxr-xr-x  2.0 unx    77016 b- defN 24-May-21 18:41 geode_explicit/lib64/libGeode-Explicit_section.so
+-rw-r--r--  2.0 unx     2149 b- defN 24-May-21 18:41 Geode_Explicit-4.8.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 24-May-21 18:41 Geode_Explicit-4.8.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-21 18:41 Geode_Explicit-4.8.0rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1166 b- defN 24-May-21 18:41 Geode_Explicit-4.8.0rc1.dist-info/RECORD
+12 files, 882391 bytes uncompressed, 359348 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -3,35 +3,35 @@
 
 Filename: geode_explicit/brep.py
 Comment: 
 
 Filename: geode_explicit/section.py
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_brep.dll
+Filename: geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_common.dll
+Filename: geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_section.dll
+Filename: geode_explicit/lib64/libGeode-Explicit_brep.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_common.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_section.so
 Comment: 
 
-Filename: Geode_Explicit-4.7.7rc1.dist-info/METADATA
+Filename: Geode_Explicit-4.8.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.7.7rc1.dist-info/WHEEL
+Filename: Geode_Explicit-4.8.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.7.7rc1.dist-info/top_level.txt
+Filename: Geode_Explicit-4.8.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.7.7rc1.dist-info/RECORD
+Filename: Geode_Explicit-4.8.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/__init__.py

```diff
@@ -1,7 +1,4 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .section import *
-from .brep import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+from .section import *
+from .brep import *
```

## geode_explicit/brep.py

```diff
@@ -1,12 +1,12 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import opengeode_inspector
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_brep import *
-ExplicitBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import opengeode_inspector
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_brep import *
+ExplicitBRepLibrary.initialize()
```

## geode_explicit/section.py

```diff
@@ -1,11 +1,11 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_section import *
-ExplicitSectionLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_section import *
+ExplicitSectionLibrary.initialize()
```

