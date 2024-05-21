# Comparing `tmp/mapmaker-1.6.0.tar.gz` & `tmp/mapmaker-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapmaker-1.6.0.tar", last modified: Sun Nov  5 11:35:12 2023, max compression
+gzip compressed data, was "mapmaker-1.6.1.tar", last modified: Tue May 21 08:02:21 2024, max compression
```

## Comparing `mapmaker-1.6.0.tar` & `mapmaker-1.6.1.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2023-11-05 11:35:12.507580 mapmaker-1.6.0/
--rw-r--r--   0 akeil     (1000) akeil     (1000)      416 2022-08-07 12:16:15.000000 mapmaker-1.6.0/.gitignore
--rw-r--r--   0 akeil     (1000) akeil     (1000)     1075 2021-12-05 11:47:08.000000 mapmaker-1.6.0/LICENSE.txt
--rw-r--r--   0 akeil     (1000) akeil     (1000)      113 2021-12-05 11:47:08.000000 mapmaker-1.6.0/MANIFEST.in
--rw-r--r--   0 akeil     (1000) akeil     (1000)     1042 2023-11-05 11:31:22.000000 mapmaker-1.6.0/Makefile
--rw-r--r--   0 akeil     (1000) akeil     (1000)    11034 2023-11-05 11:35:12.507580 mapmaker-1.6.0/PKG-INFO
--rw-r--r--   0 akeil     (1000) akeil     (1000)      172 2023-11-05 11:31:22.000000 mapmaker-1.6.0/README.pws
--rw-r--r--   0 akeil     (1000) akeil     (1000)    10043 2023-11-05 11:31:22.000000 mapmaker-1.6.0/README.rst
--rw-r--r--   0 akeil     (1000) akeil     (1000)     1974 2022-08-07 12:16:15.000000 mapmaker-1.6.0/default.ini
-drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2023-11-05 11:35:12.504246 mapmaker-1.6.0/examples/
--rw-r--r--   0 akeil     (1000) akeil     (1000)      992 2022-08-07 12:16:15.000000 mapmaker-1.6.0/examples/Makefile
--rw-r--r--   0 akeil     (1000) akeil     (1000)    12460 2022-08-07 12:16:15.000000 mapmaker-1.6.0/examples/feature-collection.json
--rw-r--r--   0 akeil     (1000) akeil     (1000)      407 2022-08-07 12:16:15.000000 mapmaker-1.6.0/examples/feature.json
--rw-r--r--   0 akeil     (1000) akeil     (1000)    17420 2022-08-07 12:16:15.000000 mapmaker-1.6.0/examples/geometry-collection.json
-drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2023-11-05 11:35:12.504246 mapmaker-1.6.0/mapmaker/
--rw-r--r--   0 akeil     (1000) akeil     (1000)      240 2023-11-05 11:33:33.000000 mapmaker-1.6.0/mapmaker/__init__.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)     9594 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/core.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)    21377 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/decorations.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)    10000 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/default.ini
--rw-r--r--   0 akeil     (1000) akeil     (1000)    21594 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/draw.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)     6997 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/geo.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)    10455 2022-09-11 05:31:37.000000 mapmaker-1.6.0/mapmaker/geojson.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)     6386 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/icons.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)    11443 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/main.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)    16752 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/parse.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)    15809 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/render.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)    20259 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/service.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)     7036 2023-11-05 11:31:22.000000 mapmaker-1.6.0/mapmaker/tilemap.py
-drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2023-11-05 11:35:12.504246 mapmaker-1.6.0/mapmaker.egg-info/
--rw-r--r--   0 akeil     (1000) akeil     (1000)    11034 2023-11-05 11:35:12.000000 mapmaker-1.6.0/mapmaker.egg-info/PKG-INFO
--rw-r--r--   0 akeil     (1000) akeil     (1000)      777 2023-11-05 11:35:12.000000 mapmaker-1.6.0/mapmaker.egg-info/SOURCES.txt
--rw-r--r--   0 akeil     (1000) akeil     (1000)        1 2023-11-05 11:35:12.000000 mapmaker-1.6.0/mapmaker.egg-info/dependency_links.txt
--rw-r--r--   0 akeil     (1000) akeil     (1000)       48 2023-11-05 11:35:12.000000 mapmaker-1.6.0/mapmaker.egg-info/entry_points.txt
--rw-r--r--   0 akeil     (1000) akeil     (1000)       41 2023-11-05 11:35:12.000000 mapmaker-1.6.0/mapmaker.egg-info/requires.txt
--rw-r--r--   0 akeil     (1000) akeil     (1000)        9 2023-11-05 11:35:12.000000 mapmaker-1.6.0/mapmaker.egg-info/top_level.txt
--rw-r--r--   0 akeil     (1000) akeil     (1000)       49 2023-11-05 11:31:22.000000 mapmaker-1.6.0/requirements.txt
--rw-r--r--   0 akeil     (1000) akeil     (1000)       38 2023-11-05 11:35:12.507580 mapmaker-1.6.0/setup.cfg
--rwxr-xr-x   0 akeil     (1000) akeil     (1000)     1598 2022-02-19 08:35:58.000000 mapmaker-1.6.0/setup.py
-drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2023-11-05 11:35:12.504246 mapmaker-1.6.0/test/
--rw-r--r--   0 akeil     (1000) akeil     (1000)        0 2021-12-12 17:37:03.000000 mapmaker-1.6.0/test/__init__.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)       59 2022-03-06 14:27:33.000000 mapmaker-1.6.0/test/geojson_point.json
--rw-r--r--   0 akeil     (1000) akeil     (1000)     1137 2022-02-19 08:35:58.000000 mapmaker-1.6.0/test/test_geo.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)     5614 2022-08-07 12:16:15.000000 mapmaker-1.6.0/test/test_geojson.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)     7415 2022-02-19 08:35:58.000000 mapmaker-1.6.0/test/test_parse.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)     2379 2022-02-19 08:35:58.000000 mapmaker-1.6.0/test/test_tiles.py
--rw-r--r--   0 akeil     (1000) akeil     (1000)       75 2022-02-19 08:35:58.000000 mapmaker-1.6.0/tox.ini
+drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2024-05-21 08:02:21.860136 mapmaker-1.6.1/
+-rw-r--r--   0 akeil     (1000) akeil     (1000)      416 2022-08-07 12:16:15.000000 mapmaker-1.6.1/.gitignore
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     1075 2021-12-05 11:47:08.000000 mapmaker-1.6.1/LICENSE.txt
+-rw-r--r--   0 akeil     (1000) akeil     (1000)      113 2021-12-05 11:47:08.000000 mapmaker-1.6.1/MANIFEST.in
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     1042 2024-05-21 07:51:39.000000 mapmaker-1.6.1/Makefile
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    11071 2024-05-21 08:02:21.860136 mapmaker-1.6.1/PKG-INFO
+-rw-r--r--   0 akeil     (1000) akeil     (1000)      172 2023-11-05 11:31:22.000000 mapmaker-1.6.1/README.pws
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    10054 2024-05-21 08:00:29.000000 mapmaker-1.6.1/README.rst
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     1974 2022-08-07 12:16:15.000000 mapmaker-1.6.1/default.ini
+drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2024-05-21 08:02:21.856803 mapmaker-1.6.1/examples/
+-rw-r--r--   0 akeil     (1000) akeil     (1000)      992 2022-08-07 12:16:15.000000 mapmaker-1.6.1/examples/Makefile
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    12460 2022-08-07 12:16:15.000000 mapmaker-1.6.1/examples/feature-collection.json
+-rw-r--r--   0 akeil     (1000) akeil     (1000)      407 2022-08-07 12:16:15.000000 mapmaker-1.6.1/examples/feature.json
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    17420 2022-08-07 12:16:15.000000 mapmaker-1.6.1/examples/geometry-collection.json
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     1125 2024-05-21 08:00:29.000000 mapmaker-1.6.1/examples/mapdef.ini
+drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2024-05-21 08:02:21.856803 mapmaker-1.6.1/mapmaker/
+-rw-r--r--   0 akeil     (1000) akeil     (1000)      240 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/__init__.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     9814 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/core.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    22835 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/decorations.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    10000 2023-11-05 11:31:22.000000 mapmaker-1.6.1/mapmaker/default.ini
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    21536 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/draw.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     7582 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/geo.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    10454 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/geojson.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     6332 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/icons.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     9972 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/main.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    13935 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/mapdef.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    16592 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/parse.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    15804 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/render.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    21354 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/service.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     7771 2024-05-21 08:00:29.000000 mapmaker-1.6.1/mapmaker/tilemap.py
+drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2024-05-21 08:02:21.860136 mapmaker-1.6.1/mapmaker.egg-info/
+-rw-r--r--   0 akeil     (1000) akeil     (1000)    11071 2024-05-21 08:02:21.000000 mapmaker-1.6.1/mapmaker.egg-info/PKG-INFO
+-rw-r--r--   0 akeil     (1000) akeil     (1000)      893 2024-05-21 08:02:21.000000 mapmaker-1.6.1/mapmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 akeil     (1000) akeil     (1000)        1 2024-05-21 08:02:21.000000 mapmaker-1.6.1/mapmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 akeil     (1000) akeil     (1000)       48 2024-05-21 08:02:21.000000 mapmaker-1.6.1/mapmaker.egg-info/entry_points.txt
+-rw-r--r--   0 akeil     (1000) akeil     (1000)       52 2024-05-21 08:02:21.000000 mapmaker-1.6.1/mapmaker.egg-info/requires.txt
+-rw-r--r--   0 akeil     (1000) akeil     (1000)        9 2024-05-21 08:02:21.000000 mapmaker-1.6.1/mapmaker.egg-info/top_level.txt
+-rw-r--r--   0 akeil     (1000) akeil     (1000)       76 2024-05-21 08:00:29.000000 mapmaker-1.6.1/requirements.txt
+-rw-r--r--   0 akeil     (1000) akeil     (1000)       38 2024-05-21 08:02:21.860136 mapmaker-1.6.1/setup.cfg
+-rwxr-xr-x   0 akeil     (1000) akeil     (1000)     1598 2022-02-19 08:35:58.000000 mapmaker-1.6.1/setup.py
+drwxr-xr-x   0 akeil     (1000) akeil     (1000)        0 2024-05-21 08:02:21.860136 mapmaker-1.6.1/test/
+-rw-r--r--   0 akeil     (1000) akeil     (1000)        0 2021-12-12 17:37:03.000000 mapmaker-1.6.1/test/__init__.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)       59 2022-03-06 14:27:33.000000 mapmaker-1.6.1/test/geojson_point.json
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     1608 2024-05-21 08:00:29.000000 mapmaker-1.6.1/test/test_core.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     9062 2024-05-21 08:00:29.000000 mapmaker-1.6.1/test/test_geo.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     5614 2022-08-07 12:16:15.000000 mapmaker-1.6.1/test/test_geojson.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     5915 2024-05-21 08:00:29.000000 mapmaker-1.6.1/test/test_main.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     5854 2024-05-21 08:00:29.000000 mapmaker-1.6.1/test/test_mapdef.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     4425 2024-05-21 08:00:29.000000 mapmaker-1.6.1/test/test_parse.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     6096 2024-05-21 08:00:29.000000 mapmaker-1.6.1/test/test_service.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)     8049 2024-05-21 08:00:29.000000 mapmaker-1.6.1/test/test_tiles.py
+-rw-r--r--   0 akeil     (1000) akeil     (1000)       75 2022-02-19 08:35:58.000000 mapmaker-1.6.1/tox.ini
```

### Comparing `mapmaker-1.6.0/LICENSE.txt` & `mapmaker-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapmaker-1.6.0/Makefile` & `mapmaker-1.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `mapmaker-1.6.0/PKG-INFO` & `mapmaker-1.6.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: mapmaker
-Version: 1.6.0
-Summary: Create map images from slippy map tiles.
-Home-page: http://github.com/akeil/mapmaker
-Author: Alexander Keil
-Author-email: alex@akeil.net
-Maintainer: Alexander Keil
-License: MIT
-Project-URL: Source, http://github.com/akeil/mapmaker
-Project-URL: Bug Reports, http://github.com/akeil/mapmaker/issues
-Keywords: osm,openstreetmap,tiles,map,image,cli
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-Requires-Dist: appdirs
-Requires-Dist: Pillow
-Requires-Dist: requests
-Requires-Dist: geojson
-Requires-Dist: cairosvg
-
 Map Maker
 #########
 ``mapmaker`` is a simple script to generate map images for "Slippy Tile" maps.
 Map tiles are downloaded from services such as OpenStreetMap and are combined
 into a single image.
 
 
@@ -97,36 +68,27 @@
 Additional Options
 ------------------
 Specify the **zoom level** with the ``--zoom`` flag. The default is 8.
 Higher values mean more detail and result in larger map images.
 
 .. code:: shell-session
 
-    $ mapmaker --zoom 12 63.0695,-151.0074 100km
+    $ mapmaker 63.0695,-151.0074 100km --zoom 12
 
 Use ``--style`` to control the **look** of the map:
 
 .. code:: shell-session
 
-    $ mapmaker --style human 63.0695,-151.0074 100km
-
-Use the ``--shading`` flag to overlay a hillshading layer over the map image.
-Note that hillshading is not available for all regions.
-
-.. code:: shell-session
-
-    $ mapmaker --shading 45.83,6.88 100km
-
-Note that some map styles already come with hillshading.
+    $ mapmaker 63.0695,-151.0074 100km --style human
 
 To control the resulting image format, use ``--aspect``:
 
 .. code:: shell-session
 
-    $ mapmaker --aspect 16:9 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --aspect 16:9
 
 The aspect ratio is given in the format ``W:H`` (e.g. 4:3 or 19:9).
 The resulting map image will contain the given bounding box (or point w/ radius)
 and max be extended to North/South or East/West to match the aspect ratio.
 Note that the *resolution* of the image depends on the ``--zoom`` factor.
 
 
@@ -138,51 +100,53 @@
 large enough to accommodate the title.
 
 :PLACEMENT:   one of the cardinal directions e.g. ``NW, NNW, N, NNE, NE, ...``.
 :BORDER:      a single integer value for the border width in in pixels.
 :COLOR:       RGB(A) tuple as a comma separated string, e.g. "255,0,0".
 :BACKGROUND:  RGB(A) tuple as a comma separated string, e.g. "255,0,0".
 
-.. code:: shell-session
+Colors can also be specified as hex values, e.g. ``#ff0000``
+or ``#ff000080`` (with opacity).
 
-    $ mapmaker --title My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW 5 My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW 5 255,0,0 My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW 5 255,0,0 0,0,255 My Map -- 45.83,6.88 100km
+.. code:: shell-session
 
-*Note the ``--`` to indicate the end of non-positional arguments.*
+    $ mapmaker 45.83,6.88 100km --title My Map
+    $ mapmaker 45.83,6.88 100km --title NNW My Map
+    $ mapmaker 45.83,6.88 100km --title NNW 5 My Map
+    $ mapmaker 45.83,6.88 100km --title NNW 5 255,0,0 My Map
+    $ mapmaker 45.83,6.88 100km --title NNW 5 255,0,0 0,0,255 My Map
 
 Use ``--comment`` to add a comment in small print. Arguments are the same
 as for ``--title``:
 
 .. code:: shell-session
 
-    $ mapmaker --comment My Comment 45.83,6.88 100km
-    $ mapmaker --comment SE 200,200,200 My Comment 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --comment My Comment
+    $ mapmaker 45.83,6.88 100km --comment SE 200,200,200 My Comment
 
 Use ``--margin`` and ``--background`` to apply a border around the map.
 Note that some decoration arguments will automatically add a margin area.
 
 ``margin`` is given in pixels as a single value (all sides),
 a pair of two values (top/bottom and left/right)
 or as four separate values for top, right, bottom, left (clockwise).
 
 .. code:: shell-session
 
-    $ mapmaker --margin 50 45.83,6.88 100km
-    $ mapmaker --margin 20 40 45.83,6.88 100km
-    $ mapmaker --margin 10 15 20 15 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --margin 50
+    $ mapmaker 45.83,6.88 100km --margin 20 40
+    $ mapmaker 45.83,6.88 100km --margin 10 15 20 15
 
+The color of the margin area can be controlled with ``--background``.
 ``background`` is given as a comma separated RGB(A) value:
 
 .. code:: shell-session
 
-    $ mapmaker --background 200,200,200 45.83,6.88 100km
-    $ mapmaker --background 200,200,200,128 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --margin 10 --background 200,200,200
+    $ mapmaker 45.83,6.88 100km --margin 10 --background 200,200,200,128
 
 The ``--frame`` argument adds a border around the map content, that is between
 the map and the (optional) margin area.
 ``frame`` has up to four optional parameters:
 
 :``WIDTH``:     The width in pixels, e.g. "8".
 :``COLOR``:     The main color as an RGB(A) value, e.g. "0,0,0" (black).
@@ -196,41 +160,44 @@
 All arguments are optional and if ``--frame`` is specified without arguments,
 a default frame will be drawn.
 
 Examples:
 
 .. code:: shell-session
 
-    $ mapmaker --frame 45.83,6.88 100km
-    $ mapmaker --frame 12 45.83,6.88 100km
-    $ mapmaker --frame 12 255,0,0 45.83,6.88 100km
-    $ mapmaker --frame 12 255,0,0 0,0,255 coordinates 45.83,6.88 100km
-    $ mapmaker --frame coordinates 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --frame
+    $ mapmaker 45.83,6.88 100km --frame 12
+    $ mapmaker 45.83,6.88 100km --frame 12 255,0,0
+    $ mapmaker 45.83,6.88 100km --frame 12 255,0,0 0,0,255 coordinates
+    $ mapmaker 45.83,6.88 100km --frame coordinates
 
 Use ``--scale`` to show a scale bar on the map.
 Optional arguments for scale are:
 
 :``PLACEMENT``: Where to place the scale, must be one of the map areas
                 (e.g "SW").
 :``WIDTH``:     The width of the scale bar in pixels (e.g. "2").
 :``COLOR``:     The color to use for the scale bar an label, e.g. "0,0,0".
 :``LABEL``:     The label style, either ``default`` or ``nolabel``.
+:``UNDERLAY``:  Draw a partly transparent box below the scale bar to improve
+                its readability against the map content.
 
 The label shows the size of the scale in meters or kilometers.
 
 Examples:
 
 .. code:: shell-session
 
-    $ mapmaker --scale -- 45.83,6.88 100km
-    $ mapmaker --scale SE -- 45.83,6.88 100km
-    $ mapmaker --scale 1 -- 45.83,6.88 100km
-    $ mapmaker --scale 120,120,120 -- 45.83,6.88 100km
-    $ mapmaker --scale nolabel -- 45.83,6.88 100km
-    $ mapmaker --scale SE 1 120,120,120 nolabel -- 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --scale
+    $ mapmaker 45.83,6.88 100km --scale SE
+    $ mapmaker 45.83,6.88 100km --scale 1
+    $ mapmaker 45.83,6.88 100km --scale 120,120,120
+    $ mapmaker 45.83,6.88 100km --scale nolabel
+    $ mapmaker 45.83,6.88 100km --scale full
+    $ mapmaker 45.83,6.88 100km --scale SE 1 120,120,120 nolabel full
 
 
 GeoJSON
 -------
 The ``--geojson`` option can be used to draw `GeoJSON <https://geojson.org/>`_
 objects onto the map.
```

### Comparing `mapmaker-1.6.0/README.rst` & `mapmaker-1.6.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: mapmaker
+Version: 1.6.1
+Summary: Create map images from slippy map tiles.
+Home-page: http://github.com/akeil/mapmaker
+Author: Alexander Keil
+Author-email: alex@akeil.net
+Maintainer: Alexander Keil
+License: MIT
+Project-URL: Source, http://github.com/akeil/mapmaker
+Project-URL: Bug Reports, http://github.com/akeil/mapmaker/issues
+Keywords: osm,openstreetmap,tiles,map,image,cli
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: GIS
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: appdirs
+Requires-Dist: Pillow
+Requires-Dist: requests
+Requires-Dist: geojson
+Requires-Dist: cairosvg
+Requires-Dist: setuptools
+
 Map Maker
 #########
 ``mapmaker`` is a simple script to generate map images for "Slippy Tile" maps.
 Map tiles are downloaded from services such as OpenStreetMap and are combined
 into a single image.
 
 
@@ -68,36 +98,27 @@
 Additional Options
 ------------------
 Specify the **zoom level** with the ``--zoom`` flag. The default is 8.
 Higher values mean more detail and result in larger map images.
 
 .. code:: shell-session
 
-    $ mapmaker --zoom 12 63.0695,-151.0074 100km
+    $ mapmaker 63.0695,-151.0074 100km --zoom 12
 
 Use ``--style`` to control the **look** of the map:
 
 .. code:: shell-session
 
-    $ mapmaker --style human 63.0695,-151.0074 100km
-
-Use the ``--shading`` flag to overlay a hillshading layer over the map image.
-Note that hillshading is not available for all regions.
-
-.. code:: shell-session
-
-    $ mapmaker --shading 45.83,6.88 100km
-
-Note that some map styles already come with hillshading.
+    $ mapmaker 63.0695,-151.0074 100km --style human
 
 To control the resulting image format, use ``--aspect``:
 
 .. code:: shell-session
 
-    $ mapmaker --aspect 16:9 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --aspect 16:9
 
 The aspect ratio is given in the format ``W:H`` (e.g. 4:3 or 19:9).
 The resulting map image will contain the given bounding box (or point w/ radius)
 and max be extended to North/South or East/West to match the aspect ratio.
 Note that the *resolution* of the image depends on the ``--zoom`` factor.
 
 
@@ -109,51 +130,53 @@
 large enough to accommodate the title.
 
 :PLACEMENT:   one of the cardinal directions e.g. ``NW, NNW, N, NNE, NE, ...``.
 :BORDER:      a single integer value for the border width in in pixels.
 :COLOR:       RGB(A) tuple as a comma separated string, e.g. "255,0,0".
 :BACKGROUND:  RGB(A) tuple as a comma separated string, e.g. "255,0,0".
 
-.. code:: shell-session
+Colors can also be specified as hex values, e.g. ``#ff0000``
+or ``#ff000080`` (with opacity).
 
-    $ mapmaker --title My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW 5 My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW 5 255,0,0 My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW 5 255,0,0 0,0,255 My Map -- 45.83,6.88 100km
+.. code:: shell-session
 
-*Note the ``--`` to indicate the end of non-positional arguments.*
+    $ mapmaker 45.83,6.88 100km --title My Map
+    $ mapmaker 45.83,6.88 100km --title NNW My Map
+    $ mapmaker 45.83,6.88 100km --title NNW 5 My Map
+    $ mapmaker 45.83,6.88 100km --title NNW 5 255,0,0 My Map
+    $ mapmaker 45.83,6.88 100km --title NNW 5 255,0,0 0,0,255 My Map
 
 Use ``--comment`` to add a comment in small print. Arguments are the same
 as for ``--title``:
 
 .. code:: shell-session
 
-    $ mapmaker --comment My Comment 45.83,6.88 100km
-    $ mapmaker --comment SE 200,200,200 My Comment 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --comment My Comment
+    $ mapmaker 45.83,6.88 100km --comment SE 200,200,200 My Comment
 
 Use ``--margin`` and ``--background`` to apply a border around the map.
 Note that some decoration arguments will automatically add a margin area.
 
 ``margin`` is given in pixels as a single value (all sides),
 a pair of two values (top/bottom and left/right)
 or as four separate values for top, right, bottom, left (clockwise).
 
 .. code:: shell-session
 
-    $ mapmaker --margin 50 45.83,6.88 100km
-    $ mapmaker --margin 20 40 45.83,6.88 100km
-    $ mapmaker --margin 10 15 20 15 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --margin 50
+    $ mapmaker 45.83,6.88 100km --margin 20 40
+    $ mapmaker 45.83,6.88 100km --margin 10 15 20 15
 
+The color of the margin area can be controlled with ``--background``.
 ``background`` is given as a comma separated RGB(A) value:
 
 .. code:: shell-session
 
-    $ mapmaker --background 200,200,200 45.83,6.88 100km
-    $ mapmaker --background 200,200,200,128 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --margin 10 --background 200,200,200
+    $ mapmaker 45.83,6.88 100km --margin 10 --background 200,200,200,128
 
 The ``--frame`` argument adds a border around the map content, that is between
 the map and the (optional) margin area.
 ``frame`` has up to four optional parameters:
 
 :``WIDTH``:     The width in pixels, e.g. "8".
 :``COLOR``:     The main color as an RGB(A) value, e.g. "0,0,0" (black).
@@ -167,41 +190,44 @@
 All arguments are optional and if ``--frame`` is specified without arguments,
 a default frame will be drawn.
 
 Examples:
 
 .. code:: shell-session
 
-    $ mapmaker --frame 45.83,6.88 100km
-    $ mapmaker --frame 12 45.83,6.88 100km
-    $ mapmaker --frame 12 255,0,0 45.83,6.88 100km
-    $ mapmaker --frame 12 255,0,0 0,0,255 coordinates 45.83,6.88 100km
-    $ mapmaker --frame coordinates 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --frame
+    $ mapmaker 45.83,6.88 100km --frame 12
+    $ mapmaker 45.83,6.88 100km --frame 12 255,0,0
+    $ mapmaker 45.83,6.88 100km --frame 12 255,0,0 0,0,255 coordinates
+    $ mapmaker 45.83,6.88 100km --frame coordinates
 
 Use ``--scale`` to show a scale bar on the map.
 Optional arguments for scale are:
 
 :``PLACEMENT``: Where to place the scale, must be one of the map areas
                 (e.g "SW").
 :``WIDTH``:     The width of the scale bar in pixels (e.g. "2").
 :``COLOR``:     The color to use for the scale bar an label, e.g. "0,0,0".
 :``LABEL``:     The label style, either ``default`` or ``nolabel``.
+:``UNDERLAY``:  Draw a partly transparent box below the scale bar to improve
+                its readability against the map content.
 
 The label shows the size of the scale in meters or kilometers.
 
 Examples:
 
 .. code:: shell-session
 
-    $ mapmaker --scale -- 45.83,6.88 100km
-    $ mapmaker --scale SE -- 45.83,6.88 100km
-    $ mapmaker --scale 1 -- 45.83,6.88 100km
-    $ mapmaker --scale 120,120,120 -- 45.83,6.88 100km
-    $ mapmaker --scale nolabel -- 45.83,6.88 100km
-    $ mapmaker --scale SE 1 120,120,120 nolabel -- 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --scale
+    $ mapmaker 45.83,6.88 100km --scale SE
+    $ mapmaker 45.83,6.88 100km --scale 1
+    $ mapmaker 45.83,6.88 100km --scale 120,120,120
+    $ mapmaker 45.83,6.88 100km --scale nolabel
+    $ mapmaker 45.83,6.88 100km --scale full
+    $ mapmaker 45.83,6.88 100km --scale SE 1 120,120,120 nolabel full
 
 
 GeoJSON
 -------
 The ``--geojson`` option can be used to draw `GeoJSON <https://geojson.org/>`_
 objects onto the map.
```

### Comparing `mapmaker-1.6.0/default.ini` & `mapmaker-1.6.1/default.ini`

 * *Files identical despite different names*

### Comparing `mapmaker-1.6.0/examples/Makefile` & `mapmaker-1.6.1/examples/Makefile`

 * *Files identical despite different names*

### Comparing `mapmaker-1.6.0/examples/feature-collection.json` & `mapmaker-1.6.1/examples/feature-collection.json`

 * *Files identical despite different names*

### Comparing `mapmaker-1.6.0/examples/geometry-collection.json` & `mapmaker-1.6.1/examples/geometry-collection.json`

 * *Files identical despite different names*

### Comparing `mapmaker-1.6.0/mapmaker/core.py` & `mapmaker-1.6.1/mapmaker/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,18 @@
     @property
     def _has_decorations(self):
         if self._margin and sum(self._margin):
             return True
 
         return self._decorations or self._frame
 
-    def render(self, service, zoom, icons=None, parallel_downloads=None, reporter=None):
+    def render(self, service, zoom,
+               icons=None,
+               parallel_downloads=None,
+               reporter=None):
         '''Render this map into a PIL image.
 
         Uses the given *TileService* and zoom level to obtain map tiles.
         '''
         tiles = TileMap.from_bbox(self.bbox, zoom)
 
         builder = MapBuilder(service, tiles,
@@ -90,32 +93,33 @@
         return builder.build()
 
     def add_element(self, element):
         '''Add a drawable element to the map.
 
         Drawable elements are considered part of the map contents. Their
         position is defined by lat/lon coordinates and they are drawn over the
-        map image but blow decorations.
+        map image but below decorations.
         '''
         self.elements.append(element)
 
     def add_decoration(self, area, decoration):
         '''Add a decoration to the given map area.
 
         ``area is one of ``MAP`` or ``MARGIN``,
         ``decoration`` must be a subclass of ``Decoration``.
 
         The decoration must specify its *placement* slot and the slot must be
         valid for the selected *area*.
         '''
         try:
             if decoration.placement not in Map._SLOTS[area]:
-                raise ValueError('invalid area/placement %r' % area)
+                raise ValueError(('invalid placement %r for'
+                                  ' area %r') % (decoration.placement, area))
         except (KeyError, AttributeError):
-            raise ValueError('invalid area/placement %r' % area)
+            raise ValueError('area/placement not defined %r' % area)
 
         self._decorations[area].append(decoration)
 
     def add_title(self, text,
                   area='MARGIN',
                   placement='N',
                   color=(0, 0, 0, 255),
@@ -161,23 +165,25 @@
                             font_name=font_name))
 
     def add_scale(self,
                   area='MAP',
                   placement='SW',
                   color=(0, 0, 0, 255),
                   border_width=2,
+                  underlay='compact',
                   label_style='default',
                   font_size=10,
                   font_name=None):
         '''Add a scale bar to the map.
 
         See ``Scale``.'''
         self.add_decoration(area, Scale(placement=placement,
                                         color=color,
                                         border_width=border_width,
+                                        underlay=underlay,
                                         label_style=label_style,
                                         font_size=font_size,
                                         font_name=font_name))
 
     def add_compass_rose(self,
                          area='MAP',
                          placement='SE',
@@ -237,19 +243,19 @@
 
         self._margin = m
 
     def set_background(self, *args):
         '''Set the background color for the map (margin area).
         The color is an RGBA tuple.'''
         if len(args) == 1:
-            self.background = args[0]
+            self._background = args[0]
         elif len(args) == 3:
-            self.background = (args[0], args[1], args[2], 255)
+            self._background = (args[0], args[1], args[2], 255)
         elif len(args) == 4:
-            self.background = args
+            self._background = args
         else:
             raise ValueError(('invalid number of arguments,'
                               ' expected 1, 3 or 4 args'))
 
     def set_frame(self,
                   width=5,
                   color=(0, 0, 0, 255),
```

### Comparing `mapmaker-1.6.0/mapmaker/decorations.py` & `mapmaker-1.6.1/mapmaker/decorations.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 from math import ceil, floor
 
 from . import geo
 from .geo import decimal
 from .geo import dms
-from .render import load_font
+from .render import contrast_color, load_font
 
 
 # Placment locations on the MAP and MARGIN area.
 PLACEMENTS = (
     'NW', 'NNW', 'N', 'NNE', 'NE',
     'WNW', 'W', 'WSW',
     'ENE', 'E', 'ESE',
@@ -195,18 +195,20 @@
         # TODO: this belongs into calc_margin_pos
         mask = self._MARGIN_MASK[self.placement]
         masked_margins = [v * m for v, m in zip(self.margin, mask)]
         m_top, m_right, m_bottom, m_left = masked_margins
         p_top, p_right, p_bottom, p_left = self.padding
 
         # border/decoration
-        draw.rectangle([m_left, m_top, w - m_right - 1, h - m_bottom - 1],
-                       fill=self.background,
-                       outline=self.border_color or self.color,
-                       width=self.border_width)
+        if self.border_width:
+            draw.rectangle([m_left, m_top, w - m_right - 1, h - m_bottom - 1],
+                           fill=self.background,
+                           outline=self.border_color or self.color,
+                           width=self.border_width)
+
         # text
         x = {
             'l': 0 + p_left + m_left,
             'm': w // 2,
             's': w // 2,
             'r': w - p_right - m_right,
         }[self._anchor[0]]
@@ -227,57 +229,72 @@
     def _anchor(self):
         return self._TEXT_ANCHOR[self.placement]
 
     def __repr__(self):
         return '<Cartouche placement=%r, title=%r>' % (self.placement,
                                                        self.title)
 
+
 class Scale(Decoration):
     '''A scale bar that shows the size of the area on the map in meters or
     kilometers.
 
     :placement:     Where to place this decoration.
     :color:         The color for the scale and label as an RGBA tuple.
     :border_width:  Width in pixels for the lines of the scale bar.
+    :underlay:      Draws a transparent background below the scale to improve
+                    readability against the map content.
+                    One of ``compact``, ``full`` (width), ``none``.
     :draw_label:    Whether to draw a label (*boolean*).
     :font_name:     Name of the font in which the label should be drawn.
     :font_size:     Size of the label text.
     '''
 
     LABEL_STYLES = ('default', 'nolabel')
+    UNDERLAY_STYLES = ('compact', 'full', 'none')
 
     def __init__(self,
                  placement='SW',
                  color=(0, 0, 0, 255),
                  border_width=2,
+                 underlay='compact',
                  label_style='default',
                  font_name=None,
                  font_size=10):
         super().__init__(placement)
         self.color = color
         self.border_width = border_width
         self.font_name = font_name or 'DejaVuSans'
         self.font_size = font_size
 
+        if underlay not in Scale.UNDERLAY_STYLES:
+            raise ValueError('Invalid underlay style %r' % underlay)
+        self.underlay_style = underlay
+
         if label_style not in Scale.LABEL_STYLES:
             raise ValueError('Invalid label style %r' % label_style)
         self.label_style = label_style
 
         # TODO: might depend on placement?
         self._label_anchor = 'mt'  # centered, align-top
 
     def calc_size(self, rc, map_size):
         tick_size, tick_width, num_ticks = self._determine_tick(rc)
 
+        m_top, m_right, m_bottom, m_left = self.margin
+
         # Size of the scale bar w/ ticks
-        w = tick_width * num_ticks
-        h = tick_height = self._tick_height()
+        if self.underlay_style == 'full':
+            map_width, _ = map_size
+            w = map_width
+        else:
+            w = tick_width * num_ticks
+            w += m_left + m_right
 
-        m_top, m_right, m_bottom, m_left = self.margin
-        w += m_left + m_right
+        h = self._tick_height()
         h += m_top + m_bottom
 
         # Size of the label
         if self._show_label:
             font = load_font(self.font_name, self.font_size)
             label = self._label(tick_size, num_ticks)
             left, top, right, bottom = font.getbbox(label,
@@ -287,22 +304,46 @@
 
         return (w, h)
 
     def draw(self, draw, rc, map_size):
         tick_size, tick_width, num_ticks = self._determine_tick(rc)
         w = tick_width * num_ticks
 
+        if self.underlay_style != 'none':
+            self._draw_underlay(draw, rc, map_size)
+
         self._draw_bar(draw, w, tick_width, num_ticks)
 
         if self._show_label:
             self._draw_label(draw, w, tick_size, num_ticks)
 
+    def _draw_underlay(self, draw, rc, map_size):
+        '''Draw a flat background in a light color with some opacity
+        to improve the readability for the scale bar.'''
+        w, h = self.calc_size(rc, map_size)
+        p0 = (0, 0)
+        p1 = None
+        if self.underlay_style == 'compact':
+            p1 = (w, h)
+        elif self.underlay_style == 'full':
+            map_width, _ = map_size
+            p1 = (map_width, h)
+        else:
+            # should not happen
+            raise RuntimeError('Bad underlay style: %r' % self.underlay_style)
+
+        r, g, b, _ = contrast_color(self.color)
+        alpha = 255 // 3
+        draw.rectangle([p0, p1],
+                       fill=(r, g, b, alpha),
+                       width=0)
+
     def _draw_bar(self, draw, bar_width, tick_width, num_ticks):
         '''Draw the scale bar including ticks.'''
-        tick_height = tick_height = self._tick_height()
+        tick_height = self._tick_height()
         m_top, m_right, m_bottom, m_left = self.margin
 
         # base line + outer ticks
         y = tick_height + m_top
         start = (m_left, y)
         end = (bar_width + m_left, y)
 
@@ -353,15 +394,15 @@
         map_width = geo.distance(bbox.minlon,
                                  ref_lat,
                                  bbox.maxlon,
                                  ref_lat)
 
         tick_size = None    # in meters
         tick_count = None
-        tick_area = 10 # "n" to use ca. 1/n of the map
+        tick_area = 10  # "n" to use ca. 1/n of the map
         max_tick_count = 5 * tick_area
 
         # if a tick was "s" meters wide, how many would fit on the map?
         # "s" from 10,000 to 0.5
         for e in range(14, 0, -1):
             s = 10 ** e / 2
             c = floor(map_width / s)
```

### Comparing `mapmaker-1.6.0/mapmaker/default.ini` & `mapmaker-1.6.1/mapmaker/default.ini`

 * *Files identical despite different names*

### Comparing `mapmaker-1.6.0/mapmaker/draw.py` & `mapmaker-1.6.1/mapmaker/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 '''Draw elements on the map content.
 
 Map Elements are additional content such as *Placemarks* or *Tracks* that are
 painted over the map content.
 They are typically placed using lat/lon coordinates.
 '''
-from functools import partial
 from math import sqrt
 from math import floor
 from math import radians
 from math import sin
 
 from PIL import Image
 
@@ -69,15 +68,15 @@
 
     def __repr__(self):
         return '<Track waypoints=%d color=%s>' % (len(self.waypoints),
                                                   self.color)
 
 
 class Placemark(DrawLayer):
-    '''Draw a placemark with a ``symbol`` and a ``label`` at the given location.
+    '''Draw a placemark with ``symbol`` and ``label`` at the given location.
 
     :label:         Text the will be shown on the map.
     :symbol:        The icon that will be drawn on the map. Must be one of
                     *dot*, *square* or *triangle*.
                     Default is "dot", use *None* to omit the icon.
     :border:        If >0, draws a border around the icon.
     :color:         The main color for the icon.
@@ -143,15 +142,16 @@
                               color=self.color,
                               fill=self.fill,
                               border=self.border,
                               size=self.size)
             all.append(marker)
 
         if self.label:
-            offset=(0, (self.size + self.border) // 2 + 2)  # draw label slightly below marker
+            # draw label slightly below marker
+            offset = (0, (self.size + self.border) // 2 + 2)
             label = Label(self.lat, self.lon, self.label,
                           offset=offset,
                           color=self.label_color,
                           fill=self.label_bg,
                           border=self.border,
                           font_name=self.font_name,
                           font_size=self.font_size)
@@ -276,15 +276,14 @@
         self.border = border or 0
         self.size = 4 if size is None else size
 
     def draw(self, rc, draw):
         x, y = rc.to_pixels(self.lat, self.lon)
         # flat background "behind" the icon
         if self.fill:
-            #self._draw_background(draw, x, y)
             self._draw_glow(draw, x, y)
 
         # icon is a PILImage
         icon = rc.get_icon(self.name, width=self.size, height=self.size)
 
         # Place the icon centered over location
         offset = self.size // 2
@@ -295,16 +294,17 @@
     def _draw_glow(self, draw, x, y):
         '''draw a radial gradient behind the icon.
 
         The gradient is painted in the ``fill`` color with opacity from 1.0
         at the center to 0.0 on the edges.
         This creates a "glow" behind the icon.
         '''
-        # Image.radial_gradient creates a gradient from black to white at 256x256
-        # where only the outermost pixel (at the corners) are completely white
+        # Image.radial_gradient creates a gradient from black to white
+        # at 256x256 where only the outermost pixel (at the corners) are
+        # completely white.
         # https://pillow.readthedocs.io/en/stable/reference/Image.html
         #
         # So this WILL NOT work
         #
         # grad = Image.radial_gradient('L')
         # mask = ImageOps.invert(grad).resize(size)
 
@@ -418,15 +418,14 @@
             self._draw_background(draw, loc, text, font)
         else:
             stroke_width = Label._STROKE_WITH
             stroke_fill = contrast_color(self.color)
 
         self._draw_text(draw, loc, text, font, stroke_width, stroke_fill)
 
-
     def _draw_text(self, draw, loc, text, font, stroke_width, stroke_fill):
         '''Draw the label.'''
         draw.text(loc, text,
                   font=font,
                   anchor=self.anchor,
                   fill=self.color,
                   stroke_width=stroke_width,
```

### Comparing `mapmaker-1.6.0/mapmaker/geo.py` & `mapmaker-1.6.1/mapmaker/geo.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,26 +38,28 @@
         if self.minlat < -90.0:
             raise ValueError('minlat must not be < -90, got %s' % self.minlat)
         if self.maxlat > 90.0:
             raise ValueError('maxlat must not be >90, got %s' % self.maxlat)
         if self.minlon < -180.0:
             raise ValueError('minlon must not be < -180, got %s' % self.minlon)
         if self.maxlon > 180.0:
-            raise ValueError('maxlon must not be > 180.0, got %s' % self.maxlon)
+            raise ValueError('maxlon must not be > 180, got %s' % self.maxlon)
 
     def with_aspect(self, aspect):
         '''Extend the given bounding box so that it adheres to the given aspect
         ratio (given as a floating point number).
         Returns a new bounding box with the desired aspect ratio that contains
         the initial box in its center.'''
         # aspect = width : height
         #  4:3  =>  1.32  width > height, aspect is > 1.0
         #  2:3  =>  0.66  width < height, aspect is < 1.0
         if aspect == 1.0:
             return self
+        elif aspect <= 0.0:
+            raise ValueError('aspect must be >0.0, got %s' % aspect)
 
         lat = self.minlat
         lon = self.minlon
         height = distance(self.minlat, lon, self.maxlat, lon)
         width = distance(lat, self.minlon, lat, self.maxlon)
 
         current_aspect = width / height
@@ -88,15 +90,15 @@
     def padded(self, pad):
         '''Create a BBox that is extended towards all sides
         by the given amount in meters.'''
         if not pad:
             return self
 
         if pad < 0:
-            raise ValueError('Pad must be a positive value, got %s' % pad)
+            raise ValueError('pad must be a positive value, got %s' % pad)
 
         north = self.maxlat
         west = self.minlon
         south = self.minlat
         east = self.maxlon
 
         maxlat, minlon = destination_point(north, west, 315.0, pad)
@@ -137,15 +139,18 @@
 
     def __repr__(self):
         return '<BBox minlat=%s, minlon=%s, maxlat=%s, maxlon=%s>' % (
             self.minlat, self.minlon, self.maxlat, self.maxlon)
 
     @classmethod
     def from_radius(cls, lat, lon, radius):
-        '''Create a bounding box from a center point an a radius.'''
+        '''Create a bounding box from a center point and a radius.'''
+        if radius <= 0:
+            raise ValueError('radius must be >0, got %s' % radius)
+
         lat_n, lon_n = destination_point(lat, lon, BRG_NORTH, radius)
         lat_e, lon_e = destination_point(lat, lon, BRG_EAST, radius)
         lat_s, lon_s = destination_point(lat, lon, BRG_SOUTH, radius)
         lat_w, lon_w = destination_point(lat, lon, BRG_WEST, radius)
 
         return cls(minlat=min(lat_n, lat_e, lat_s, lat_w),
                    minlon=min(lon_n, lon_e, lon_s, lon_w),
@@ -159,14 +164,17 @@
 
 def distance(lat0, lon0, lat1, lon1):
     '''Calculate the distance as-the-crow-flies between two points in meters.
 
         P0 ------------> P1
 
     '''
+    if lat0 == lat1 and lon0 == lon1:
+        return 0
+
     lat0 = radians(lat0)
     lon0 = radians(lon0)
     lat1 = radians(lat1)
     lon1 = radians(lon1)
 
     d_lat = lat1 - lat0
     d_lon = lon1 - lon0
@@ -180,17 +188,28 @@
     return d * EARTH_RADIUS
 
 
 def destination_point(lat, lon, bearing, distance):
     '''Determine a destination point from a start location, a bearing
     and a distance.
 
-    Distance is given in METERS.
-    Bearing is given in DEGREES
+    Distance is given in METERS and must be non-negative.
+    Bearing is given in DEGREES and is in range 0...360
     '''
+    if distance == 0:
+        return lat, lon
+
+    if bearing == 360:
+        bearing = 0
+
+    if distance < 0:
+        raise ValueError('distance must be >0, got %s', distance)
+    if bearing < 0 or bearing > 360:
+        raise ValueError('bearing must be in range 0..360,got %s', bearing)
+
     # http://www.movable-type.co.uk/scripts/latlong.html
     # search for destinationPoint
     d = distance / EARTH_RADIUS  # angular distance
     brng = radians(bearing)
 
     lat = radians(lat)
     lon = radians(lon)
```

### Comparing `mapmaker-1.6.0/mapmaker/geojson.py` & `mapmaker-1.6.1/mapmaker/geojson.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,14 @@
             return []
 
     def _shape(self, points):
         return Shape(points,
                      color=self._color('color'),
                      fill=self._color('fill'))
 
-
     def drawables(self):
         points = self.coordinates
         return self._shape(points).drawables()
 
 
 class _MultiPolygon(_Polygon):
```

### Comparing `mapmaker-1.6.0/mapmaker/icons.py` & `mapmaker-1.6.1/mapmaker/icons.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,17 +116,16 @@
     def __init__(self, path):
         self._base = Path(path)
         self._prefix = None
         self._suffix = None
         self._ext = '.svg'
 
     def _icon_path(self, name):
-        #filename = self._pattern.format(name=name)
         filename = '{prefix}{name}{suffix}{ext}'.format(
-            prefix = self._prefix or '',
+            prefix=self._prefix or '',
             name=name,
             suffix=self._suffix or '',
             ext=self._ext or '')
         return self._base.joinpath(filename)
 
     def _icon_name(self, path):
         name = path.name
```

### Comparing `mapmaker-1.6.0/mapmaker/main.py` & `mapmaker-1.6.1/mapmaker/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 import io
 from pathlib import Path
 from pkg_resources import resource_stream
 import sys
 
 from . import __author__
 from . import __version__
-from .core import Map
 from .geo import distance
-from . import geojson
 from . import icons
 from . import parse
-from .parse import BBoxAction
+from .mapdef import MapParams
+from .parse import MapParamsAction
 from .parse import FrameAction
 from .parse import MarginAction
-from .parse import ScaleAction, ScaleParams
-from .parse import TextAction
+from .parse import ScaleAction
+from .parse import TitleAction, CommentAction
 from .service import ServiceRegistry
-from .service import TileService
+from .tilemap import MIN_ZOOM, MAX_ZOOM
 
 import appdirs
 
 
 APP_NAME = 'mapmaker'
 APP_DESC = 'Create map images from tile servers.'
 
@@ -40,14 +39,59 @@
 def main():
     '''Parse arguments and run the program.'''
     conf_dir = appdirs.user_config_dir(appname=APP_NAME)
     conf_file = Path(conf_dir).joinpath('config.ini')
     conf = read_config(conf_file)
     registry = ServiceRegistry.default()
 
+    args, params = parse_args(registry, sys.argv[1:])
+
+    reporter = _no_reporter if args.silent else _print_reporter
+
+
+    reporter('Using configuration from %r', str(conf_file))
+
+    try:
+        params.validate()
+
+        if args.gallery:
+            base = Path(args.dst)
+            base.mkdir(exist_ok=True)
+            for style in registry.list():
+                args.dst = base.joinpath(style + '.png')
+                try:
+                    _run(reporter, registry, conf, params,
+                         args, dry_run=args.dry_run)
+                except Exception as err:
+                    # on error, continue with next service
+                    reporter('ERROR for %r: %s', style, err)
+        else:
+            _run(reporter, registry, conf,
+                 params, args, dry_run=args.dry_run)
+    except Exception as err:
+        reporter('ERROR: %s', err)
+        raise
+        return 1
+
+    return 0
+
+
+def parse_args(registry, argv):
+    defaults = MapParams.default()
+    parser = _setup_parser(registry, defaults)
+    args = parser.parse_args(argv)
+
+    params = defaults
+    params.update(args.mapdef)
+    params.update(args)
+
+    return args, params
+
+
+def _setup_parser(registry, defaults):
     parser = argparse.ArgumentParser(
         prog=APP_NAME,
         description=APP_DESC,
         epilog='{p} version {v} -- {author}'.format(
             p=APP_NAME,
             v=__version__,
             author=__author__,
@@ -55,99 +99,96 @@
     )
 
     parser.add_argument('--version',
                         action='version',
                         version=__version__,
                         help='Print version number and exit')
 
-    parser.add_argument('bbox',
-                        metavar='AREA',
-                        action=BBoxAction,
-                        nargs=2,
-                        help=('Bounding box coordinates. Either two lat,lon'
+    parser.add_argument('mapdef',
+                        metavar='MAPDEF',
+                        action=MapParamsAction,
+                        nargs='+',
+                        help=('Map definition. Either two lat,lon'
                               ' pairs ("47.437,10.953 47.374,11.133")'
                               ' or a center point and a radius'
-                              ' ("47.437,10.953 4km").'))
+                              ' ("47.437,10.953 4km")'
+                              ' or the path to an ini-file.'))
 
     default_dst = 'map.png'
     parser.add_argument('dst',
-                        metavar='PATH',
+                        metavar='OUTPUT',
                         nargs='?',
                         default=default_dst,
                         help=('Where to save the generated image'
                               ' (default: %r).') % default_dst)
 
     def zoom(raw):
         v = int(raw)
-        if v < 0 or v > 19:
-            raise ValueError('Zoom value must be in interval 0..19')
+        if v < MIN_ZOOM or v > MAX_ZOOM:
+            raise ValueError(('Zoom value must be in interval'
+                              ' %s..%s') % (MIN_ZOOM, MAX_ZOOM))
         return v
 
-    default_zoom = 8
     parser.add_argument('-z', '--zoom',
-                        default=default_zoom,
                         type=zoom,
-                        help=('Zoom level (0..19), higher means more detailed'
-                              ' (default: %s).') % default_zoom)
+                        help=('Zoom level (%s..%s), higher means more detailed'
+                              ' (default: %s).') % (MIN_ZOOM, MAX_ZOOM,
+                                                    defaults.zoom))
 
-    default_style = 'osm'
     parser.add_argument('-s', '--style',
                         choices=registry.list(),
-                        default=default_style,
-                        help='Map style (default: %r)' % default_style)
+                        help='Map style (default: %r)' % defaults.style)
 
     parser.add_argument('-a', '--aspect',
                         type=parse.aspect,
-                        default=1.0,
                         help=(
                             'Aspect ratio (e.g. "16:9") for the generated map.'
                             ' Extends the bounding box to match the given'
                             ' aspect ratio.'))
 
     parser.add_argument('--copyright',
                         action='store_true',
                         help='Add copyright notice')
 
     parser.add_argument('--title',
-                        action=TextAction,
+                        action=TitleAction,
                         metavar='ARGS',
                         help=('Add a title to the map'
                               ' (optional args: PLACEMENT, COLOR, BORDER'
                               ' followed by title string)'))
 
     parser.add_argument('--comment',
-                        action=TextAction,
+                        action=CommentAction,
                         help='Add a comment to the map')
 
     parser.add_argument('--margin',
                         action=MarginAction,
-                        default=(0, 0, 0, 0),
                         help=('Add a margin (white space) around the map'
                               ' ("TOP RIGHT BOTTOM LEFT" or "ALL")'))
 
     parser.add_argument('--background',
                         type=parse.color,
                         metavar='RGBA',
-                        default=(255, 255, 255, 255),
                         help=('Background color for map margin'
                               ' (default: white)'))
 
     parser.add_argument('--frame',
                         action=FrameAction,
                         metavar='ARGS',
                         help=('Draw a frame around the map area'
-                              ' (any of: WIDTH, COLOR, ALT_COLOR and STYLE)'))
+                              ' (any of: WIDTH, COLOR, ALT_COLOR, STYLE and'
+                              ' UNDERLAY)'))
 
     parser.add_argument('--scale',
                         action=ScaleAction,
                         metavar='ARGS',
                         help=('Draw a scale bar into the map'
                               ' (any of: PLACEMENT, WIDTH, COLOR, LABEL)'))
 
-    # TODO: placement, color, marker "N"
+    # TODO: placement, color, outline, marker "N"
     parser.add_argument('--compass',
                         action='store_true',
                         help='Draw a compass rose on the map')
 
     parser.add_argument('--geojson',
                         nargs='+',
                         help=('Draw GeoJSON elements on the map.'
@@ -159,156 +200,89 @@
                             'Create a map image for each available style.'
                             ' WARNING: generates a lot of images.'))
 
     parser.add_argument('--dry-run',
                         action='store_true',
                         help='Show map info, do not download tiles')
 
+    parser.add_argument('--no-cache',
+                        action='store_true',
+                        help='Do not use cached map tiles')
+
     parser.add_argument('--silent',
                         action='store_true',
                         help='Do not output messages to the console')
 
-    args = parser.parse_args()
-
-    reporter = _no_reporter if args.silent else _print_reporter
-    bbox = args.bbox.with_aspect(args.aspect)
+    return parser
 
-    reporter('Using configuration from %r', str(conf_file))
 
-    try:
-        if args.gallery:
-            base = Path(args.dst)
-            base.mkdir(exist_ok=True)
-            for style in registry.list():
-                dst = base.joinpath(style + '.png')
-                try:
-                    _run(bbox, args.zoom, dst, style, reporter, registry, conf,
-                         args, dry_run=args.dry_run)
-                except Exception as err:
-                    # on error, continue with next service
-                    reporter('ERROR for %r: %s', style, err)
-        else:
-            _run(bbox, args.zoom, args.dst, args.style, reporter, registry,
-                 conf, args, dry_run=args.dry_run)
-    except Exception as err:
-        reporter('ERROR: %s', err)
-        raise
-        return 1
-
-    return 0
-
-
-def _run(bbox, zoom, dst, style, report, registry, conf, args, dry_run=False):
+def _run(report, registry, conf, params, args, dry_run=False):
     '''Build the tilemap, download tiles and create the image.'''
-    map = Map(bbox)
-    map.set_background(args.background)
-    map.set_margin(*args.margin)
-    if args.frame:
-        map.set_frame(width=args.frame.width or 5,
-                      color=args.frame.color or (0, 0, 0, 255),
-                      alt_color=args.frame.alt_color or (255, 255, 255, 255),
-                      style=args.frame.style or 'solid')
-    if args.title:
-        placement, border, color, bg_color, text = args.title
-        map.add_title(text,
-                      placement=placement or 'N',
-                      color=color or (0, 0, 0, 255),
-                      background=bg_color,
-                      border_color=color or (0, 0, 0, 255),
-                      border_width=border or 0,
-                      font_name='DejaVuSans',
-                      font_size=16)
-    if args.comment:
-        placement, border, color, bg_color, text = args.comment
-        map.add_comment(text,
-                        placement=placement or 'SSE',
-                        color=color or (0, 0, 0, 255),
-                        background=bg_color,
-                        border_color=color or (0, 0, 0, 255),
-                        border_width=border or 0,
-                        font_name='DejaVuSans',
-                        font_size=10)
-
-    if args.compass:
-        map.add_compass_rose()
-
-    if args.scale:
-        map.add_scale(area='MAP',
-                      placement=args.scale.place or 'SW',
-                      color=args.scale.color or (0, 0, 0, 255),
-                      border_width=args.scale.width or 2,
-                      label_style=args.scale.label or 'default',
-                      font_size=10,
-                      font_name='DejaVuSans')
-
-    if args.geojson:
-        for x in args.geojson:
-            elem = geojson.read(x)
-            map.add_element(elem)
-
-    service = registry.get(style)
-    service = service.cached(limit=conf.cache_limit)
-
-    if args.copyright:
-        copyright = conf.copyrights.get(service.top_level_domain)
-        map.add_comment(copyright, placement='ENE', font_size=8)
+    p = params
+    m = p.create_map()
 
     if dry_run:
+        _show_info(report, p)
         return
 
-    img = map.render(service,
-                     zoom,
-                     icons=icons.IconProvider(conf.icons_base),
-                     parallel_downloads=8,
-                     reporter=report)
-    with open(dst, 'wb') as f:
+    use_cache = not args.no_cache
+    img = _build_map(m, p.style, p.zoom, use_cache, conf, registry, report)
+
+    with open(args.dst, 'wb') as f:
         img.save(f, format='png')
 
-    report('Map saved to %s', dst)
+    report('Map saved to %s', args.dst)
+
+
+def _build_map(m, style, zoom, use_cache, conf, registry, report):
+    service = registry.get(style)
+    if use_cache:
+        service = service.cached(limit=conf.cache_limit)
+
+    return m.render(service,
+                    zoom,
+                    icons=icons.IconProvider(conf.icons_base),
+                    parallel_downloads=8,
+                    reporter=report)
 
 
 def _print_reporter(msg, *args):
     print(msg % args)
 
 
 def _no_reporter(msg, *args):
     pass
 
 
-def _show_info(report, service, map, rc):
-    bbox = map.bbox
+def _show_info(report, mapdef):
+    bbox = mapdef.bbox
     area_w = int(distance(bbox.minlat, bbox.minlon, bbox.maxlat, bbox.minlon))
     area_h = int(distance(bbox.minlat, bbox.minlon, bbox.minlat, bbox.maxlon))
     unit = 'm'
     if area_w > 1000 or area_h > 1000:
         area_w = int(area_w / 100) / 10
         area_h = int(area_h / 100) / 10
         unit = 'km'
 
-    x0, y0, x1, y1 = rc.crop_box
-    w = x1 - x0
-    h = y1 - y0
     report('-------------------------------')
     report('Area:        %s x %s %s', area_w, area_h, unit)
-    report('Zoom Level:  %s', map.zoom)
-    report('Dimensions:  %s x %s px', w, h)
-    report('Tiles:       %s', map.num_tiles)
-    report('Map Style:   %s', service.name)
-    report('URL Pattern: %s', service.url_pattern)
+    report('Dimensions:  %s x %s px', area_w, area_h)
+    report('Zoom Level:  %s', mapdef.zoom)
+    report('Style:       %s', mapdef.style)
     report('-------------------------------')
 
 
 def read_config(path):
     '''Read configuration from the given file in .ini format.
     Returns names and url patterns for services and API keys, combined from
     built-in configuration and the specified file.'''
     cfg = configparser.ConfigParser()
 
     # built-in defaults
-    cfg.readfp(io.TextIOWrapper(resource_stream('mapmaker', 'default.ini')))
+    cfg.read_file(io.TextIOWrapper(resource_stream('mapmaker', 'default.ini')))
 
     # user settings
     cfg.read([path, ])
 
     parallel = cfg.getint('mapmaker', 'parallel_downloads', fallback=1)
 
     icons_base = cfg.get('icons', 'base', fallback=None)
```

### Comparing `mapmaker-1.6.0/mapmaker/parse.py` & `mapmaker-1.6.1/mapmaker/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,89 +1,67 @@
 '''Helpers for parsing various information from strings.
 Intended to be used in conjunction with the Python ``argparse`` module.
 '''
-
-
 import argparse
 from argparse import ArgumentError
-from collections import namedtuple
 
-from .geo import BBox
-from .geo import decimal
-from .tilemap import MIN_LAT, MAX_LAT
-from .decorations import PLACEMENTS
 from .decorations import Frame
+from .decorations import PLACEMENTS
 from .decorations import Scale
+from .geo import decimal
+from .mapdef import MapParams
+from .mapdef import FrameParams
+from .mapdef import TitleParams
+from .mapdef import CommentParams
+from .mapdef import ScaleParams
 
 
-class BBoxAction(argparse.Action):
-    '''Parse a bounding box (see ``bbox()``).'''
+class MapParamsAction(argparse.Action):
+    '''Create a MapParams object either from an ini-file
+    or from a BBox definition'''
 
     def __call__(self, parser, namespace, values, option_string=None):
-        # expect one of;
-        #
-        # A: two lat/lon pairs
-        #    e.g. 47.437,10.953 47.374,11.133
-        #
-        # B: lat/lon and radius
-        #    e.g. 47.437,10.953 2km
-        try:
-            box = bbox(values)
-            setattr(namespace, self.dest, box)
-        except ValueError as err:
-            raise ArgumentError(self, ('failed to parse bounding box from'
-                                       ' %r: %s') % (' '.join(values), err))
-
-
-def bbox(values):
-    '''Parse a bounding box from a pair of coordinates or from a single
-    coordinate and a radius.
-
-    1. two lat lon pairs::
-
-        ["47.437,10.953", "47.374,11.133"]
-
-    2. single coordinate and radius::
-
-        ["47.437,10.953", "2km"]
-
-    If successful, returns a ``BBox`` object.
-
-    Raises *ValueError* on failure.
-    '''
-    lat0, lon0 = coordinates(values[0])
+        if len(values) > 2:
+            raise ArgumentError(self, 'Maximum number of arguments exceeded')
 
-    # simple case, BBox from lat,lon pairs
-    if ',' in values[1]:
-        lat1, lon1 = coordinates(values[1])
-        bbox = BBox(
-            minlat=min(lat0, lat1),
-            minlon=min(lon0, lon1),
-            maxlat=max(lat0, lat1),
-            maxlon=max(lon0, lon1),
-        )
-    # bbox from point and radius
-    else:
-        value = distance(values[1])
-        bbox = BBox.from_radius(lat0, lon0, value)
-
-    # constrain to min/max values of slippy tile map
-    bbox = bbox.constrained(minlat=MIN_LAT, maxlat=MAX_LAT)
-
-    # Validate
-    if bbox.minlat < MIN_LAT or bbox.minlat > MAX_LAT:
-        raise ValueError
-    if bbox.maxlat < MIN_LAT or bbox.maxlat > MAX_LAT:
-        raise ValueError
-    if bbox.minlon < -180.0 or bbox.minlon > 180.0:
-        raise ValueError
-    if bbox.maxlon < -180.0 or bbox.maxlon > 180.0:
-        raise ValueError
+        p = None
+        if len(values) == 1:
+            # assume path to ini
+            try:
+                with open(values[0]) as f:
+                    p = MapParams.from_file(f)
+            except Exception as err:
+                msg = ('could not read map definition from'
+                       ' %r: %s') % (values[0], err)
+                raise ArgumentError(self, msg)
+        else:
+            # assume bbox coordinates
+            try:
+                p = self._with_bbox(values)
+            except Exception as err:
+                msg = ('failed to parse bounding box from'
+                       ' %r: %s') % (' '.join(values), err)
+                raise ArgumentError(self, msg)
+
+        setattr(namespace, self.dest, p)
+
+    def _with_bbox(self, values):
+        pos0 = coordinates(values[0])
+        p = MapParams(pos0)
+
+        # simple case, BBox from lat,lon pairs
+        if ',' in values[1]:
+            pos1 = coordinates(values[1])
+            p.pos1 = pos1
+        # bbox from point and radius
+        else:
+            radius = distance(values[1])
+            p.radius = radius
 
-    return bbox
+        return p
 
 
 class MarginAction(argparse.Action):
     '''Parse the settings for the map margin.
     See ``margin()``.'''
 
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
@@ -140,35 +118,36 @@
     for v in margins:
         if v < 0:
             raise ValueError(('invalid margin %r, must not be negative') % v)
 
     return margins
 
 
-class TextAction(argparse.Action):
+class _TextAction(argparse.Action):
     '''Parse title or comment arguments.
     Expect three "formal" arguments:
 
     - placement (e.g. NW or S)
     - border (integer value)
     - color (RGBA tuple, comma separated)
 
     Followed by at least one "free form" argument which constitutes the actual
     title string.
     '''
 
+    _factory = None
+
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
         if nargs is not None:
-            raise ValueError("nargs must None")
+            raise ValueError("nargs must be None")
 
         super().__init__(option_strings, dest, nargs='+', **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
-
-        placement, border, foreground, background = None, None, None, None
+        placement, border, fg, bg = None, None, None, None
 
         consumed = 0
         for value in values:
             if placement is None:
                 try:
                     placement = _parse_placement(value)
                     consumed += 1
@@ -185,44 +164,55 @@
                         raise ArgumentError(self, msg)
 
                     consumed += 1
                     continue
                 except ValueError:
                     pass
 
-            if foreground is None:
+            if fg is None:
                 try:
-                    foreground = color(value)
+                    fg = color(value)
                     consumed += 1
                     continue
                 except ValueError:
                     pass
 
-            if background is None:
+            if bg is None:
                 try:
-                    background = color(value)
+                    bg = color(value)
                     consumed += 1
                     continue
                 except ValueError:
                     pass
 
             # stop parsing formal parameters
             # as soon as the first "free form" is encountered
             break
 
         text = ' '.join(values[consumed:])
         if not text:
             msg = 'missing title string in %r' % ' '.join(values)
             raise ArgumentError(self, msg)
 
-        params = (placement, border, foreground, background, text)
-        setattr(namespace, self.dest, params)
+        p = self._factory.default()
+        p.placement = placement if placement is not None else p.placement
+        p.border_width = border if border is not None else p.border_width
+        p.color = fg if fg is not None else p.color
+        p.border_color = fg if fg is not None else p.border_color
+        p.background = bg if bg is not None else p.background
+        p.text = text if text is not None else p.text
+        setattr(namespace, self.dest, p)
 
 
-FrameParams = namedtuple('FrameParams', 'width color alt_color style')
+class TitleAction(_TextAction):
+    _factory = TitleParams
+
+
+class CommentAction(_TextAction):
+    _factory = CommentParams
 
 
 class FrameAction(argparse.Action):
     '''Handle parameters for Frame:
 
     - border width as single integer
     - color as RGB(A) tuple from comma separated string
@@ -287,30 +277,20 @@
             # did not understand "value"
             unrecognized.append(value)
 
         if unrecognized:
             msg = 'unrecognized frame parameters: %r' % ', '.join(unrecognized)
             raise ArgumentError(self, msg)
 
-        # apply defaults
-        if self.default:
-            d_width, d_color, d_alt_color, d_style = self.default
-            width = d_width if width is None else width
-            primary = d_color if primary is None else primary
-            alternate = d_alt_color if alternate is None else alternate
-            style = d_style if style is None else style
-
-        setattr(namespace, self.dest, FrameParams(
-            width=width,
-            color=primary,
-            alt_color=alternate,
-            style=style))
-
-
-ScaleParams = namedtuple('ScaleParams', 'place width color label')
+        p = FrameParams.default()
+        p.width = width if width is not None else p.width
+        p.color = primary if primary is not None else p.color
+        p.alt_color = alternate if alternate is not None else p.alt_color
+        p.style = style if style is not None else p.style
+        setattr(namespace, self.dest, p)
 
 
 class ScaleAction(argparse.Action):
     '''Parse various parameters for the map's scale bar
 
     - placement (SW, SE, ...)
     - border width (single integer)
@@ -321,20 +301,21 @@
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
         if nargs is not None:
             raise ValueError("nargs must be None")
 
         super().__init__(option_strings, dest, nargs='*', **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
-        if len(values) > 4:
+        if len(values) > 5:
             msg = ('invalid number of arguments (%s) for frame, expected up to'
-                   ' four: PLACEMENT, BORDER, COLOR, LABEL') % len(values)
+                   ' five: PLACEMENT, BORDER, COLOR, LABEL,'
+                   ' UNDERLINE') % len(values)
             raise ArgumentError(self, msg)
 
-        place, width, fg_color, label = None, None, None, None
+        place, width, fg_color, label, underlay = None, None, None, None, None
 
         # accept values for BORDER, COLOR and STYLE in any order
         # accept each param only once
         # make sure all values are consumed
         unrecognized = []
         for value in values:
             if place is None:
@@ -365,34 +346,34 @@
                     pass
 
             if label is None:
                 if value.lower() in Scale.LABEL_STYLES:
                     label = value.lower()
                     continue
 
+            if underlay is None:
+                if value.lower() in Scale.UNDERLAY_STYLES:
+                    underlay = value.lower()
+                    continue
+
             # did not understand "value"
             unrecognized.append(value)
 
         if unrecognized:
             msg = 'unrecognized scale parameters: %r' % ', '.join(unrecognized)
             raise ArgumentError(self, msg)
 
-        # apply defaults
-        if self.default:
-            d_place, d_width, d_color, d_label = self.default
-            place = d_place if place is None else place
-            width = d_width if width is None else width
-            fg_color = d_color if fg_color is None else fg_color
-            label = d_label if label is None else label
-
-        setattr(namespace, self.dest, ScaleParams(
-            place=place,
-            width=width,
-            color=fg_color,
-            label=label))
+        p = ScaleParams.default()
+        p.placement = place if place is not None else p.placement
+        p.border_width = width if width is not None else p.border_width
+        p.color = fg_color if fg_color is not None else p.color
+        p.label_style = label if label is not None else p.label_style
+        p.underlay = underlay if underlay is not None else p.underlay
+
+        setattr(namespace, self.dest, p)
 
 
 def coordinates(raw):
     '''Parse a pair of lat/lon coordinates.
 
     Supports the following format:
```

### Comparing `mapmaker-1.6.0/mapmaker/render.py` & `mapmaker-1.6.1/mapmaker/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,15 @@
     pass
 
 
 def load_font(font_name, font_size):
     '''Load the given true type font, return fallback on failure.'''
     try:
         return ImageFont.truetype(font=font_name, size=font_size)
-    except OSError as e:
+    except OSError:
         return ImageFont.load_default()
 
 
 def is_dark(color):
     '''Tell if the given color is dark.'''
     # https://alienryderflex.com/hsp.html
     r, g, b = color[0], color[1], color[2]
```

### Comparing `mapmaker-1.6.0/mapmaker/service.py` & `mapmaker-1.6.1/mapmaker/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from urllib.parse import urlparse
 import threading
 
 import appdirs
 from PIL import Image
 import requests
 
-from mapmaker import __version__
-from mapmaker import __author__
+from mapmaker import __version__ as VERSION
+from mapmaker import __author__ as AUTHOR
 from mapmaker import __name__ as APP_NAME
 from mapmaker.tilemap import Tile
 
 
 _LOG = logging.getLogger(APP_NAME)
 
 
@@ -41,17 +41,17 @@
                            url_pattern,
                            subdomains=subdomains,
                            tile_size=tile_size,
                            api_key=api_key)
 
     def list(self):
         '''List the names of all registered styles.'''
-        l = [k for k in self._services]
-        l.sort()
-        return l
+        services = [s for s in self._services]
+        services.sort()
+        return services
 
     @classmethod
     def from_config(cls, cfg):
         '''Creates a new *ServiceRegistry* from a parsed configuration file.
         Does *not* include the built-in settings.'''
         d = {}
         sections = [s for s in cfg.sections() if s.startswith('service.')]
@@ -59,15 +59,16 @@
         for s in sections:
             styles = [o for o in cfg.options(s) if o not in reserved]
             api_key = cfg.get(s, 'api_key', fallback=None)
             tile_size = cfg.getint(s, 'tile_size', fallback=256)
             subdomains = cfg.get(s, 'subdomains', fallback='')
             for style in styles:
                 if style in d:
-                    _LOG.warning('Ignore duplicate service definition for %r in [%s]', style, s)
+                    _LOG.warning(('Ignore duplicate service definition for'
+                                  ' %r in [%s]'), style, s)
                     continue
 
                 url_pattern = cfg[s][style]
                 d[style] = (url_pattern, subdomains, tile_size, api_key)
 
         return cls(d)
 
@@ -75,15 +76,18 @@
     def from_file(cls, path):
         '''Creates a new *ServiceRegistry* from the configuration file at the
         given ``path``.
         Will also include the built-in configuration.
         '''
         cfg = configparser.ConfigParser()
         # built-in defaults
-        cfg.readfp(io.TextIOWrapper(resource_stream('mapmaker', 'default.ini')))
+        with resource_stream('mapmaker', 'default.ini') as res:
+            with io.TextIOWrapper(res) as f:
+                cfg.read_file(f)
+
         # user settings
         cfg.read([path, ])
         return cls.from_config(cfg)
 
     @classmethod
     def default(cls):
         '''Creates a new *ServiceRegistry* from the configuration file at the
@@ -130,15 +134,15 @@
         self.tile_size = tile_size or 256
         self.url_pattern = url_pattern
         self._subdomains = subdomains
         self._api_key = api_key
         self.max_retries = max_retries
 
         s = requests.Session()
-        ua = '%s/%s +https://github.com/akeil/mapmaker' % (APP_NAME, __version__)
+        ua = '%s/%s +https://github.com/akeil/mapmaker' % (APP_NAME, VERSION)
         s.headers['User-Agent'] = ua
         # TODO: should we use a custom HTTPAdapter with increased pool size?
         self._session = s
 
     def cached(self, basedir=None, limit=None, min_hours=24):
         '''Wrap this tile service in a file system cache with default
         parameters.
@@ -149,22 +153,33 @@
         If ``limit`` is set, the cache sized is limited to that size.
         '''
         return Cache(self, basedir=basedir, limit=limit, min_hours=min_hours)
 
     def memory_cache(self, size=100):
         '''Wrap this cache into a *MemoryCache*.
 
-        Note that if you also want a file system cahce (recommended), then
+        Note that if you also want a file system cache (recommended), then
         wrap the service in an FS-cache first, then with a memory cache.
+
+        .. code:: python
+
+            service = Service().cached().memory_cache()
         '''
         return MemoryCache(self, size=size)
 
     def with_fallback(self):
         '''Use lower resolution tiles as fallback if the requested zoom level
         is not available.
+
+        If you are also using a cache, set up the cache(s) first and then the
+        fallback wrapper:
+
+        .. code:: python
+
+            service = Service().cached().with_fallback()
         '''
         return Fallback(self)
 
     @property
     def top_level_domain(self):
         parts = self.domain.split('.')
         # TODO: not quite correct, will fail e.g. for 'foo.co.uk'
@@ -189,15 +204,15 @@
         The ``cached_only`` flag only makes sense if the service is wrapped
         into a cache. For a TileService without a cache, this will raise an
         error for every request.
 
         Returns the response ``etag`` and the raw image data.
         '''
         if cached_only:
-            raise LookupError('No cached tile for x=%s, y=%s, z=%s' % (x, y, z))
+            raise LookupError('No cached tile for x=%s,y=%s,z=%s' % (x, y, z))
 
         s = self._subdomain()
         url = self.url_pattern.format(
             x=x,
             y=y,
             z=z,
             s=s,
@@ -275,25 +290,31 @@
     The same basedir can be used for different services as long as they
     have unique names.
 
     ``min_hours`` controls how long we use the cached tile *without* checking
     the ETAG. Since it is unlikely that tiles change frequently *and* it is
     (assumed) likely that the same tiles are requested multiple times within
     a short timespan, this saves the additional request.
+
+    When the cache ``limit`` (in bytes) is set to a value above *0*, the cache
+    is trimmed to that size (more or less).
+    If multiple instances use the same cache directory with different limits,
+    the cache will eventually be trimmed to the lowest limit.
+    However, this will only happen when a new entry is written to the cache.
     '''
 
     def __init__(self, service, basedir=None, limit=None, min_hours=24):
         self._service = service
         self._limit = limit
         self._min_age = timedelta(hours=min_hours)
         self._lock = threading.Lock()
 
         if not basedir:
             basedir = appdirs.user_cache_dir(appname=APP_NAME,
-                                             appauthor=__author__)
+                                             appauthor=AUTHOR)
         self._base = Path(basedir)
 
     def memory_cache(self, size=100):
         '''Wrap this cache into a *MemoryCache*.'''
         return MemoryCache(self, size=size)
 
     def with_fallback(self):
@@ -323,29 +344,37 @@
         return self._service.domain
 
     def fetch(self, x, y, z, etag=None, cached_only=False):
         '''Attempt to serve the tile from the cache, if that fails, fetch it
         from the backing service.
         On a successful service call, put the result into the cache.
 
+        When ``etag`` is given, then a request against the service is always
+        made, using the etag.
+        If no etag is given, a request can still be made if we have a cached
+        entry beyond its max age.
+
         When ``cached_only`` is *True*, the cache entry is only returned
         if it can be done so without checking the ETAG against the server.
         That is, if the cache entry is younger than ``min_hours``.
         '''
         # etag is likely to be None
         if etag is None:
             etag, mtime = self._find(x, y, z)
+        else:
+            mtime = None
 
         # If the cached entry is not "too old", return it without checking
         # the ETAG.
         if mtime:
             modified = datetime.fromtimestamp(mtime, tz=timezone.utc)
             now = datetime.now(timezone.utc)
             age = now - modified
             if age < self._min_age:
+                # TODO: possible race-condition between _find() ... _get()
                 cached = self._get(x, y, z, etag)
                 return etag, cached
 
         recv_etag, data = self._service.fetch(x, y, z,
                                               etag=etag,
                                               cached_only=cached_only)
         if data is None:
@@ -386,15 +415,15 @@
 
         try:
             for entry in d.iterdir():
                 if entry.name.startswith(match):
                     if entry.is_file():
                         try:
                             safe_etag = entry.name.split('.')[1]
-                            etag_bytes = base64.b64decode(safe_etag)
+                            etag_bytes = base64.urlsafe_b64decode(safe_etag)
                             etag = etag_bytes.decode('ascii')
 
                             stat = entry.stat()
                             mtime = stat.st_mtime
 
                             return etag, mtime
                         except Exception:
@@ -428,15 +457,15 @@
         '''Remove outdated cache entries for a given tile.'''
         existing, _ = self._find(x, y, z)
         if existing and existing != current:
             p = self._path(x, y, z, existing)
             p.unlink(missing_ok=True)
 
     def _path(self, x, y, z, etag):
-        safe_etag = base64.b64encode(etag.encode()).decode('ascii')
+        safe_etag = base64.urlsafe_b64encode(etag.encode()).decode('ascii')
         filename = '%06d.%s.png' % (y, safe_etag)
 
         return self._base.joinpath(
             self._service.name,
             '%02d' % z,
             '%06d' % x,
             filename,
```

### Comparing `mapmaker-1.6.0/mapmaker/tilemap.py` & `mapmaker-1.6.1/mapmaker/tilemap.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from math import pow
 from math import radians
 from math import sin
 from math import sinh
 from math import tan
 
 from .geo import BBox
-from .geo import mercator_to_lat
 
 
 # supported lat/lon bounds for slippy map
 MAX_LAT = 85.0511
 MIN_LAT = -85.0511
 MIN_LON = -180.0
 MAX_LON = 180.0
@@ -30,19 +29,26 @@
 class TileMap:
     '''A slippy tile map with a given set of tiles and a fixed zoom level.
 
     The bounding box is fully contained within this map.
     '''
 
     def __init__(self, ax, ay, bx, by, zoom, bbox):
+        if ax < 0 or ay < 0 or bx < 0 or by < 0:
+            raise ValueError(('Tile numbers must be >0,'
+                              ' got %s,%s,%s,%s') % (ax, ay, bx, by))
+        if zoom < 0:
+            raise ValueError('Zoom level must be >0, got %s' % zoom)
+
         self.ax = min(ax, bx)
         self.ay = min(ay, by)
         self.bx = max(ax, bx)
         self.by = max(ay, by)
         self.zoom = zoom
+        # TODO: why is bbox a member attribute? This class doesn't need it.
         self.bbox = bbox
         self.tiles = None
         self._generate_tiles()
 
     @property
     def num_tiles(self):
         x = self.bx - self.ax + 1
@@ -84,14 +90,24 @@
         globe = pow(2, self.zoom)
         pixel_x = ((lon + 180.0) / 360.0) * globe
 
         sinlat = sin(lat * PI / 180.0)
         pixel_y = (0.5 - log((1 + sinlat) / (1 - sinlat)) / (4 * PI)) * globe
         return pixel_x, pixel_y
 
+    def __eq__(self, other):
+        if not isinstance(other, TileMap):
+            return False
+
+        return (self.ax == other.ax
+                and self.ay == other.ay
+                and self.bx == other.bx
+                and self.by == other.by
+                and self.zoom == other.zoom)
+
     def __repr__(self):
         return '<TileMap a=%s,%s b=%s,%s, zoom=%s>' % (self.ax,
                                                        self.ay,
                                                        self.bx,
                                                        self.by,
                                                        self.zoom)
 
@@ -187,17 +203,19 @@
     given point at the given zoom level.
 
     Returns a tuple (x, y).
 
     Raises *ValueError* if lat or lon are outside the allowed range.
     '''
     if lat < MIN_LAT or lat > MAX_LAT:
-        raise ValueError('latitude must be %s..%s, got %s' % (MIN_LAT, MAX_LAT, lat))
+        raise ValueError('latitude must be %s..%s, got %s' % (MIN_LAT,
+                                                              MAX_LAT, lat))
     if lon < MIN_LON or lon > MAX_LON:
-        raise ValueError('longitude must be %s..%s, got %s' % (MIN_LON, MAX_LON, lon))
+        raise ValueError('longitude must be %s..%s, got %s' % (MIN_LON,
+                                                               MAX_LON, lon))
 
     # taken from https://wiki.openstreetmap.org/wiki/Slippy_map_tilenames
     n = pow(2.0, zoom)
 
     x = (lon + 180.0) / 360.0 * n
 
     lat_rad = radians(lat)
```

### Comparing `mapmaker-1.6.0/mapmaker.egg-info/PKG-INFO` & `mapmaker-1.6.1/mapmaker.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapmaker
-Version: 1.6.0
+Version: 1.6.1
 Summary: Create map images from slippy map tiles.
 Home-page: http://github.com/akeil/mapmaker
 Author: Alexander Keil
 Author-email: alex@akeil.net
 Maintainer: Alexander Keil
 License: MIT
 Project-URL: Source, http://github.com/akeil/mapmaker
@@ -22,14 +22,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: appdirs
 Requires-Dist: Pillow
 Requires-Dist: requests
 Requires-Dist: geojson
 Requires-Dist: cairosvg
+Requires-Dist: setuptools
 
 Map Maker
 #########
 ``mapmaker`` is a simple script to generate map images for "Slippy Tile" maps.
 Map tiles are downloaded from services such as OpenStreetMap and are combined
 into a single image.
 
@@ -97,36 +98,27 @@
 Additional Options
 ------------------
 Specify the **zoom level** with the ``--zoom`` flag. The default is 8.
 Higher values mean more detail and result in larger map images.
 
 .. code:: shell-session
 
-    $ mapmaker --zoom 12 63.0695,-151.0074 100km
+    $ mapmaker 63.0695,-151.0074 100km --zoom 12
 
 Use ``--style`` to control the **look** of the map:
 
 .. code:: shell-session
 
-    $ mapmaker --style human 63.0695,-151.0074 100km
-
-Use the ``--shading`` flag to overlay a hillshading layer over the map image.
-Note that hillshading is not available for all regions.
-
-.. code:: shell-session
-
-    $ mapmaker --shading 45.83,6.88 100km
-
-Note that some map styles already come with hillshading.
+    $ mapmaker 63.0695,-151.0074 100km --style human
 
 To control the resulting image format, use ``--aspect``:
 
 .. code:: shell-session
 
-    $ mapmaker --aspect 16:9 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --aspect 16:9
 
 The aspect ratio is given in the format ``W:H`` (e.g. 4:3 or 19:9).
 The resulting map image will contain the given bounding box (or point w/ radius)
 and max be extended to North/South or East/West to match the aspect ratio.
 Note that the *resolution* of the image depends on the ``--zoom`` factor.
 
 
@@ -138,51 +130,53 @@
 large enough to accommodate the title.
 
 :PLACEMENT:   one of the cardinal directions e.g. ``NW, NNW, N, NNE, NE, ...``.
 :BORDER:      a single integer value for the border width in in pixels.
 :COLOR:       RGB(A) tuple as a comma separated string, e.g. "255,0,0".
 :BACKGROUND:  RGB(A) tuple as a comma separated string, e.g. "255,0,0".
 
-.. code:: shell-session
+Colors can also be specified as hex values, e.g. ``#ff0000``
+or ``#ff000080`` (with opacity).
 
-    $ mapmaker --title My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW 5 My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW 5 255,0,0 My Map -- 45.83,6.88 100km
-    $ mapmaker --title NNW 5 255,0,0 0,0,255 My Map -- 45.83,6.88 100km
+.. code:: shell-session
 
-*Note the ``--`` to indicate the end of non-positional arguments.*
+    $ mapmaker 45.83,6.88 100km --title My Map
+    $ mapmaker 45.83,6.88 100km --title NNW My Map
+    $ mapmaker 45.83,6.88 100km --title NNW 5 My Map
+    $ mapmaker 45.83,6.88 100km --title NNW 5 255,0,0 My Map
+    $ mapmaker 45.83,6.88 100km --title NNW 5 255,0,0 0,0,255 My Map
 
 Use ``--comment`` to add a comment in small print. Arguments are the same
 as for ``--title``:
 
 .. code:: shell-session
 
-    $ mapmaker --comment My Comment 45.83,6.88 100km
-    $ mapmaker --comment SE 200,200,200 My Comment 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --comment My Comment
+    $ mapmaker 45.83,6.88 100km --comment SE 200,200,200 My Comment
 
 Use ``--margin`` and ``--background`` to apply a border around the map.
 Note that some decoration arguments will automatically add a margin area.
 
 ``margin`` is given in pixels as a single value (all sides),
 a pair of two values (top/bottom and left/right)
 or as four separate values for top, right, bottom, left (clockwise).
 
 .. code:: shell-session
 
-    $ mapmaker --margin 50 45.83,6.88 100km
-    $ mapmaker --margin 20 40 45.83,6.88 100km
-    $ mapmaker --margin 10 15 20 15 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --margin 50
+    $ mapmaker 45.83,6.88 100km --margin 20 40
+    $ mapmaker 45.83,6.88 100km --margin 10 15 20 15
 
+The color of the margin area can be controlled with ``--background``.
 ``background`` is given as a comma separated RGB(A) value:
 
 .. code:: shell-session
 
-    $ mapmaker --background 200,200,200 45.83,6.88 100km
-    $ mapmaker --background 200,200,200,128 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --margin 10 --background 200,200,200
+    $ mapmaker 45.83,6.88 100km --margin 10 --background 200,200,200,128
 
 The ``--frame`` argument adds a border around the map content, that is between
 the map and the (optional) margin area.
 ``frame`` has up to four optional parameters:
 
 :``WIDTH``:     The width in pixels, e.g. "8".
 :``COLOR``:     The main color as an RGB(A) value, e.g. "0,0,0" (black).
@@ -196,41 +190,44 @@
 All arguments are optional and if ``--frame`` is specified without arguments,
 a default frame will be drawn.
 
 Examples:
 
 .. code:: shell-session
 
-    $ mapmaker --frame 45.83,6.88 100km
-    $ mapmaker --frame 12 45.83,6.88 100km
-    $ mapmaker --frame 12 255,0,0 45.83,6.88 100km
-    $ mapmaker --frame 12 255,0,0 0,0,255 coordinates 45.83,6.88 100km
-    $ mapmaker --frame coordinates 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --frame
+    $ mapmaker 45.83,6.88 100km --frame 12
+    $ mapmaker 45.83,6.88 100km --frame 12 255,0,0
+    $ mapmaker 45.83,6.88 100km --frame 12 255,0,0 0,0,255 coordinates
+    $ mapmaker 45.83,6.88 100km --frame coordinates
 
 Use ``--scale`` to show a scale bar on the map.
 Optional arguments for scale are:
 
 :``PLACEMENT``: Where to place the scale, must be one of the map areas
                 (e.g "SW").
 :``WIDTH``:     The width of the scale bar in pixels (e.g. "2").
 :``COLOR``:     The color to use for the scale bar an label, e.g. "0,0,0".
 :``LABEL``:     The label style, either ``default`` or ``nolabel``.
+:``UNDERLAY``:  Draw a partly transparent box below the scale bar to improve
+                its readability against the map content.
 
 The label shows the size of the scale in meters or kilometers.
 
 Examples:
 
 .. code:: shell-session
 
-    $ mapmaker --scale -- 45.83,6.88 100km
-    $ mapmaker --scale SE -- 45.83,6.88 100km
-    $ mapmaker --scale 1 -- 45.83,6.88 100km
-    $ mapmaker --scale 120,120,120 -- 45.83,6.88 100km
-    $ mapmaker --scale nolabel -- 45.83,6.88 100km
-    $ mapmaker --scale SE 1 120,120,120 nolabel -- 45.83,6.88 100km
+    $ mapmaker 45.83,6.88 100km --scale
+    $ mapmaker 45.83,6.88 100km --scale SE
+    $ mapmaker 45.83,6.88 100km --scale 1
+    $ mapmaker 45.83,6.88 100km --scale 120,120,120
+    $ mapmaker 45.83,6.88 100km --scale nolabel
+    $ mapmaker 45.83,6.88 100km --scale full
+    $ mapmaker 45.83,6.88 100km --scale SE 1 120,120,120 nolabel full
 
 
 GeoJSON
 -------
 The ``--geojson`` option can be used to draw `GeoJSON <https://geojson.org/>`_
 objects onto the map.
```

### Comparing `mapmaker-1.6.0/mapmaker.egg-info/SOURCES.txt` & `mapmaker-1.6.1/mapmaker.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,38 @@
 requirements.txt
 setup.py
 tox.ini
 examples/Makefile
 examples/feature-collection.json
 examples/feature.json
 examples/geometry-collection.json
+examples/mapdef.ini
 mapmaker/__init__.py
 mapmaker/core.py
 mapmaker/decorations.py
 mapmaker/default.ini
 mapmaker/draw.py
 mapmaker/geo.py
 mapmaker/geojson.py
 mapmaker/icons.py
 mapmaker/main.py
+mapmaker/mapdef.py
 mapmaker/parse.py
 mapmaker/render.py
 mapmaker/service.py
 mapmaker/tilemap.py
 mapmaker.egg-info/PKG-INFO
 mapmaker.egg-info/SOURCES.txt
 mapmaker.egg-info/dependency_links.txt
 mapmaker.egg-info/entry_points.txt
 mapmaker.egg-info/requires.txt
 mapmaker.egg-info/top_level.txt
 test/__init__.py
 test/geojson_point.json
+test/test_core.py
 test/test_geo.py
 test/test_geojson.py
+test/test_main.py
+test/test_mapdef.py
 test/test_parse.py
+test/test_service.py
 test/test_tiles.py
```

### Comparing `mapmaker-1.6.0/setup.py` & `mapmaker-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `mapmaker-1.6.0/test/test_geojson.py` & `mapmaker-1.6.1/test/test_geojson.py`

 * *Files identical despite different names*

