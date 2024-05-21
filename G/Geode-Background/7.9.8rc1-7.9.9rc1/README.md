# Comparing `tmp/Geode_Background-7.9.8rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Background-7.9.9rc1-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 4725539 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      216 b- defN 24-Apr-24 09:02 geode_background/__init__.py
--rw-rw-rw-  2.0 fat      199 b- defN 24-Apr-24 09:02 geode_background/brep.py
--rw-rw-rw-  2.0 fat      199 b- defN 24-Apr-24 09:02 geode_background/solid.py
--rw-rw-rw-  2.0 fat      203 b- defN 24-Apr-24 09:02 geode_background/surface.py
--rw-rw-rw-  2.0 fat  3766784 b- defN 24-Apr-24 09:03 geode_background/bin/Geode-Background_brep.dll
--rw-rw-rw-  2.0 fat    53248 b- defN 24-Apr-24 09:03 geode_background/bin/Geode-Background_common.dll
--rw-rw-rw-  2.0 fat  3963392 b- defN 24-Apr-24 09:03 geode_background/bin/Geode-Background_solid.dll
--rw-rw-rw-  2.0 fat  3811328 b- defN 24-Apr-24 09:03 geode_background/bin/Geode-Background_surface.dll
--rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-24 09:03 geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-24 09:03 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-24 09:03 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-24 09:03 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1104 b- defN 24-Apr-24 09:03 Geode_Background-7.9.8rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-24 09:03 Geode_Background-7.9.8rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-24 09:03 Geode_Background-7.9.8rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1601 b- defN 24-Apr-24 09:03 Geode_Background-7.9.8rc1.dist-info/RECORD
-16 files, 12100151 bytes uncompressed, 4722837 bytes compressed:  61.0%
+Zip file size: 3221368 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      110 b- defN 24-May-21 07:25 geode_background/__init__.py
+-rw-r--r--  2.0 unx      191 b- defN 24-May-21 07:25 geode_background/brep.py
+-rw-r--r--  2.0 unx      192 b- defN 24-May-21 07:25 geode_background/solid.py
+-rw-r--r--  2.0 unx      196 b- defN 24-May-21 07:25 geode_background/surface.py
+-rwxr-xr-x  2.0 unx   122264 b- defN 24-May-21 07:26 geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122264 b- defN 24-May-21 07:26 geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122264 b- defN 24-May-21 07:26 geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122264 b- defN 24-May-21 07:26 geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   155192 b- defN 24-May-21 07:26 geode_background/lib64/libGeode-Background_brep.so
+-rwxr-xr-x  2.0 unx   109008 b- defN 24-May-21 07:26 geode_background/lib64/libGeode-Background_common.so
+-rwxr-xr-x  2.0 unx  3420816 b- defN 24-May-21 07:26 geode_background/lib64/libGeode-Background_solid.so
+-rwxr-xr-x  2.0 unx  3235312 b- defN 24-May-21 07:26 geode_background/lib64/libGeode-Background_surface.so
+-rw-r--r--  2.0 unx     1060 b- defN 24-May-21 07:26 Geode_Background-7.9.9rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 24-May-21 07:26 Geode_Background-7.9.9rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-May-21 07:26 Geode_Background-7.9.9rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1673 b- defN 24-May-21 07:26 Geode_Background-7.9.9rc1.dist-info/RECORD
+16 files, 7412926 bytes uncompressed, 3218522 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -6,44 +6,44 @@
 
 Filename: geode_background/solid.py
 Comment: 
 
 Filename: geode_background/surface.py
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_brep.dll
+Filename: geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_common.dll
+Filename: geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_solid.dll
+Filename: geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_surface.dll
+Filename: geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_brep.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_common.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_solid.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_surface.so
 Comment: 
 
-Filename: Geode_Background-7.9.8rc1.dist-info/METADATA
+Filename: Geode_Background-7.9.9rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Background-7.9.8rc1.dist-info/WHEEL
+Filename: Geode_Background-7.9.9rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Background-7.9.8rc1.dist-info/top_level.txt
+Filename: Geode_Background-7.9.9rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Background-7.9.8rc1.dist-info/RECORD
+Filename: Geode_Background-7.9.9rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_background/__init__.py

```diff
@@ -1,8 +1,5 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .surface import *
-from .solid import *
-from .brep import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+from .surface import *
+from .solid import *
+from .brep import *
```

## geode_background/brep.py

```diff
@@ -1,10 +1,10 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_brep import *
-
-BackgroundBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_brep import *
+
+BackgroundBRepLibrary.initialize()
```

## geode_background/solid.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_solid import *
-BackgroundSolidLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_solid import *
+BackgroundSolidLibrary.initialize()
```

## geode_background/surface.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_surface import *
-BackgroundSurfaceLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_surface import *
+BackgroundSurfaceLibrary.initialize()
```

## Comparing `Geode_Background-7.9.8rc1.dist-info/METADATA` & `Geode_Background-7.9.9rc1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1
-Name: Geode-Background
-Version: 7.9.8rc1
-Summary: Geode-solutions OpenGeode module for building background meshes
-Home-page: https://github.com/Geode-solutions/Geode-Background
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-common ==31.*,>=31.0.8
-Requires-Dist: opengeode-core ==14.*,>=14.19.2
-
-<h1 align="center">Background<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Module to generate background meshes and background models for OpenGeode</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Background_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Background_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Background_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Background_private.svg" alt="Version">
-</p>
-
-
+Metadata-Version: 2.1
+Name: Geode-Background
+Version: 7.9.9rc1
+Summary: Geode-solutions OpenGeode module for building background meshes
+Home-page: https://github.com/Geode-solutions/Geode-Background
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-common ==31.*,>=31.1.0
+Requires-Dist: opengeode-core ==14.*,>=14.20.0
+
+<h1 align="center">Background<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Module to generate background meshes and background models for OpenGeode</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Background_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Background_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Background_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Background_private.svg" alt="Version">
+</p>
```

## Comparing `Geode_Background-7.9.8rc1.dist-info/RECORD` & `Geode_Background-7.9.9rc1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-geode_background/__init__.py,sha256=nrly-bKXLsgtI1cSxS2toM6MvcxIM8FMKiC07JhlV9U,216
-geode_background/brep.py,sha256=tYHPoFSpQe7DcP4UdByklZuv6cIhtVzy4AtC6FDmb5g,199
-geode_background/solid.py,sha256=XU7nXDgAjD_8fRTQOQteGvL812oy5pCNNxAPDjXg21c,199
-geode_background/surface.py,sha256=gYOsu70XBpFHsMsTG56V05oAa8xWQLPsZpDhdkPP7PY,203
-geode_background/bin/Geode-Background_brep.dll,sha256=7TkCd04vlQp5GoTEUFU9uc4GloS-dM2auldgZ8BYFxs,3766784
-geode_background/bin/Geode-Background_common.dll,sha256=Myj3Wu5hTYzHQNFWlFS0RDHuJmB1SNoxTTZcB9_q4JM,53248
-geode_background/bin/Geode-Background_solid.dll,sha256=m7AcRyngAfdFWJ4C0UFLVyPUnD2NhLPERGWaoAMt-88,3963392
-geode_background/bin/Geode-Background_surface.dll,sha256=F0Y6SiuSz820zx7GOk17DNjvo5TF_kYEF9_JU3u4k-Y,3811328
-geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd,sha256=vo7z43AtR-Ij5LIYn4nRMEoASBQT8yV3UfesqXfFXnE,125440
-geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd,sha256=cdRYWjO5xET57mVFrqYDpyl6B1NTReOeBW49W87g50A,125440
-geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd,sha256=3b0fpEegtR31XCCe5Lubasblw1HKqjNWxjPgpDIAmIM,125440
-geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd,sha256=LC0Cabrv0pZgvv2U50zk4XNDO0ZQqBINpGIE7Xk4Xfk,125440
-Geode_Background-7.9.8rc1.dist-info/METADATA,sha256=2fLYSgJNd8NO_cXLHC_W16A7L57Viu2ZvqP55z2oV4E,1104
-Geode_Background-7.9.8rc1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-Geode_Background-7.9.8rc1.dist-info/top_level.txt,sha256=Zrf1AIA63yPEiQFwdZwLsHzGAE3soNFO7AVs5NdN_r4,17
-Geode_Background-7.9.8rc1.dist-info/RECORD,,
+geode_background/__init__.py,sha256=blPQYNF5G29FTzV7qPxTRuHFNAO7q4zkFMBd-AbHTnY,110
+geode_background/brep.py,sha256=CvXUH_pK1hYWw4q37x5Zc0jKhFSrRG0yQd7o7mPz5vM,191
+geode_background/solid.py,sha256=N0pBLglv9f58p0rmzx7H2kXI7UTDCxwLvojSDoA6oUg,192
+geode_background/surface.py,sha256=y1CRwP6BtWw-IJIJVbB8Ihg0qeL8cG7cB4WEj5ls1Aw,196
+geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so,sha256=lfggwPDufRQeW5joF6Fv5Gq3PTmdta8cIa-sDA43RmY,122264
+geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so,sha256=QtPGfkeeJB-r-yv5qcufV9VdwQj53qHsgormdxZT7TI,122264
+geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so,sha256=67ZScfbbii3sTHyWSDXpc2C91GQ7XlIMMlsdOrmYe2c,122264
+geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so,sha256=Yv7Mfj6cPs0oSkDBXAyJGzq_9ZE-Buh6p5P6UEutIY0,122264
+geode_background/lib64/libGeode-Background_brep.so,sha256=HvZvlmuo_DcVsXWFM7lQII6j1kZvgdCQQ7l92YoigTA,155192
+geode_background/lib64/libGeode-Background_common.so,sha256=DcUzWfEtYrren8GYivc9TtBwjFkXwcGCBu_cxAIMDqk,109008
+geode_background/lib64/libGeode-Background_solid.so,sha256=MTVqVOKJt3tXdLEMyJFrgeolaJAq5eH45Cm4tp0R2Rs,3420816
+geode_background/lib64/libGeode-Background_surface.so,sha256=aY2ZRdpKalKcjcUxjcUBL9u0nfM7zHepOqxJaKWcDys,3235312
+Geode_Background-7.9.9rc1.dist-info/METADATA,sha256=j9ELhPBkHhhIw-bH75kAQ0FOVn6kUhzwFP04ncJoSg4,1060
+Geode_Background-7.9.9rc1.dist-info/WHEEL,sha256=cPiEulY4lHJMdGCxx29HxfDkwhV9C6172sJgZUA9dSs,103
+Geode_Background-7.9.9rc1.dist-info/top_level.txt,sha256=Zrf1AIA63yPEiQFwdZwLsHzGAE3soNFO7AVs5NdN_r4,17
+Geode_Background-7.9.9rc1.dist-info/RECORD,,
```

