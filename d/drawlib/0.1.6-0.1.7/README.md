# Comparing `tmp/drawlib-0.1.6.tar.gz` & `tmp/drawlib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawlib-0.1.6.tar", max compression
+gzip compressed data, was "drawlib-0.1.7.tar", max compression
```

## Comparing `drawlib-0.1.6.tar` & `drawlib-0.1.7.tar`

### file list

```diff
@@ -1,64 +1,63 @@
--rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.6/README.md
--rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.6/drawlib/.pylintrc
--rw-r--r--   0        0        0     1039 2024-05-15 13:28:22.417672 drawlib-0.1.6/drawlib/__init__.py
--rw-r--r--   0        0        0      688 2024-04-06 11:43:47.512263 drawlib-0.1.6/drawlib/__main__.py
--rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.6/drawlib/apis.py
--rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.6/drawlib/assets/__init__.py
--rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.6/drawlib/assets/v0_1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.6/drawlib/assets/v0_1/fonticons/__init__.py
--rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.6/drawlib/assets/v0_1/fonts/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.6/drawlib/v0_1/__init__.py
--rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.6/drawlib/v0_1/__main__.py
--rw-r--r--   0        0        0     2475 2024-05-17 13:08:14.332089 drawlib-0.1.6/drawlib/v0_1/apis.py
--rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.6/drawlib/v0_1/private/__init__.py
--rw-r--r--   0        0        0     6207 2024-05-17 13:45:20.537581 drawlib-0.1.6/drawlib/v0_1/private/command.py
--rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.6/drawlib/v0_1/private/core/__init__.py
--rw-r--r--   0        0        0    12776 2024-04-23 00:24:17.718876 drawlib-0.1.6/drawlib/v0_1/private/core/colors.py
--rw-r--r--   0        0        0    13598 2024-05-17 11:32:14.717753 drawlib-0.1.6/drawlib/v0_1/private/core/dimage.py
--rw-r--r--   0        0        0    23775 2024-05-17 13:15:29.707391 drawlib-0.1.6/drawlib/v0_1/private/core/fonts.py
--rw-r--r--   0        0        0    33160 2024-05-17 07:10:44.348191 drawlib-0.1.6/drawlib/v0_1/private/core/model.py
--rw-r--r--   0        0        0    16716 2024-05-17 08:42:03.070585 drawlib-0.1.6/drawlib/v0_1/private/core/theme.py
--rw-r--r--   0        0        0    11892 2024-05-17 06:56:45.843326 drawlib-0.1.6/drawlib/v0_1/private/core/theme_officials.py
--rw-r--r--   0        0        0    51534 2024-05-17 08:42:26.352080 drawlib-0.1.6/drawlib/v0_1/private/core/theme_styles.py
--rw-r--r--   0        0        0    28300 2024-05-17 11:42:16.612394 drawlib-0.1.6/drawlib/v0_1/private/core/util.py
--rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.6/drawlib/v0_1/private/core_canvas/__init__.py
--rw-r--r--   0        0        0    15589 2024-05-17 11:33:32.642807 drawlib-0.1.6/drawlib/v0_1/private/core_canvas/base.py
--rw-r--r--   0        0        0     7992 2024-05-17 04:55:01.315534 drawlib-0.1.6/drawlib/v0_1/private/core_canvas/canvas.py
--rw-r--r--   0        0        0     4950 2024-05-17 04:01:16.413350 drawlib-0.1.6/drawlib/v0_1/private/core_canvas/image.py
--rw-r--r--   0        0        0     6593 2024-05-17 04:01:22.784734 drawlib-0.1.6/drawlib/v0_1/private/core_canvas/line.py
--rw-r--r--   0        0        0     4297 2024-05-17 04:01:28.386700 drawlib-0.1.6/drawlib/v0_1/private/core_canvas/original_arrow.py
--rw-r--r--   0        0        0    12132 2024-05-17 12:08:03.060649 drawlib-0.1.6/drawlib/v0_1/private/core_canvas/original_polygon.py
--rw-r--r--   0        0        0    16466 2024-05-17 04:01:43.093731 drawlib-0.1.6/drawlib/v0_1/private/core_canvas/patches.py
--rw-r--r--   0        0        0     3264 2024-05-17 04:02:22.095588 drawlib-0.1.6/drawlib/v0_1/private/core_canvas/text.py
--rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.6/drawlib/v0_1/private/download.py
--rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.6/drawlib/v0_1/private/dutil.py
--rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.6/drawlib/v0_1/private/icons/__init__.py
--rw-r--r--   0        0        0   902368 2024-05-17 00:56:51.813460 drawlib-0.1.6/drawlib/v0_1/private/icons/phosphor.py
--rw-r--r--   0        0        0     1998 2024-05-17 04:04:01.158522 drawlib-0.1.6/drawlib/v0_1/private/icons/util.py
--rw-r--r--   0        0        0     1206 2024-04-27 06:44:36.108567 drawlib-0.1.6/drawlib/v0_1/private/logging.py
--rw-r--r--   0        0        0     6687 2024-05-02 12:04:01.063777 drawlib-0.1.6/drawlib/v0_1/private/settings.py
--rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.6/drawlib/v0_1/private/smartarts/__init__.py
--rw-r--r--   0        0        0     3482 2024-05-17 07:07:04.377539 drawlib-0.1.6/drawlib/v0_1/private/smartarts/bubblespeech.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.6/drawlib/v0_1/private/smartarts/cycle.py
--rw-r--r--   0        0        0      686 2024-05-17 01:14:56.535422 drawlib-0.1.6/drawlib/v0_1/private/smartarts/dsart.py
--rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.6/drawlib/v0_1/private/smartarts/groups.py
--rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.6/drawlib/v0_1/private/smartarts/pyramid.py
--rw-r--r--   0        0        0     5905 2024-05-17 01:19:04.280798 drawlib-0.1.6/drawlib/v0_1/private/smartarts/sourcecode.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.6/drawlib/v0_1/private/smartarts/table.py
--rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.6/drawlib/v0_1/private/smartarts/tree.py
--rw-r--r--   0        0        0     5825 2024-05-17 13:46:11.831287 drawlib-0.1.6/drawlib/v0_1/private/tools.py
--rw-r--r--   0        0        0    10163 2024-05-17 08:48:29.142132 drawlib-0.1.6/drawlib/v0_1/private/util.py
--rw-r--r--   0        0        0      407 2024-05-17 07:28:29.821380 drawlib-0.1.6/drawlib/v0_1/private/validators/__init__.py
--rw-r--r--   0        0        0     7382 2024-05-17 07:25:34.994200 drawlib-0.1.6/drawlib/v0_1/private/validators/args.py
--rw-r--r--   0        0        0     1576 2024-05-17 07:25:58.475653 drawlib-0.1.6/drawlib/v0_1/private/validators/color.py
--rw-r--r--   0        0        0     3275 2024-05-17 08:44:34.098244 drawlib-0.1.6/drawlib/v0_1/private/validators/coordinate.py
--rw-r--r--   0        0        0      891 2024-05-17 08:44:42.485495 drawlib-0.1.6/drawlib/v0_1/private/validators/image.py
--rw-r--r--   0        0        0     1249 2024-05-17 08:44:59.932902 drawlib-0.1.6/drawlib/v0_1/private/validators/line.py
--rw-r--r--   0        0        0     1332 2024-05-17 08:45:07.566582 drawlib-0.1.6/drawlib/v0_1/private/validators/shape.py
--rw-r--r--   0        0        0      660 2024-05-17 07:27:28.907431 drawlib-0.1.6/drawlib/v0_1/private/validators/smartarts.py
--rw-r--r--   0        0        0     2276 2024-05-17 08:45:25.563109 drawlib-0.1.6/drawlib/v0_1/private/validators/style.py
--rw-r--r--   0        0        0      824 2024-05-17 07:27:54.398157 drawlib-0.1.6/drawlib/v0_1/private/validators/text.py
--rw-r--r--   0        0        0     2270 2024-05-17 08:45:46.188412 drawlib-0.1.6/drawlib/v0_1/private/validators/types.py
--rw-r--r--   0        0        0      758 2024-05-17 13:51:02.999084 drawlib-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.7/README.md
+-rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.7/drawlib/.pylintrc
+-rw-r--r--   0        0        0     1039 2024-05-17 13:51:50.749671 drawlib-0.1.7/drawlib/__init__.py
+-rw-r--r--   0        0        0      688 2024-05-21 13:52:08.835136 drawlib-0.1.7/drawlib/__main__.py
+-rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.7/drawlib/apis.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.7/drawlib/assets/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.7/drawlib/assets/v0_1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.7/drawlib/assets/v0_1/fonticons/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.7/drawlib/assets/v0_1/fonts/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.7/drawlib/v0_1/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.7/drawlib/v0_1/__main__.py
+-rw-r--r--   0        0        0     2421 2024-05-21 13:50:32.945869 drawlib-0.1.7/drawlib/v0_1/apis.py
+-rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.7/drawlib/v0_1/private/__init__.py
+-rw-r--r--   0        0        0    12860 2024-05-21 14:42:32.950675 drawlib-0.1.7/drawlib/v0_1/private/command.py
+-rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.7/drawlib/v0_1/private/core/__init__.py
+-rw-r--r--   0        0        0    12776 2024-04-23 00:24:17.718876 drawlib-0.1.7/drawlib/v0_1/private/core/colors.py
+-rw-r--r--   0        0        0    13598 2024-05-17 11:32:14.717753 drawlib-0.1.7/drawlib/v0_1/private/core/dimage.py
+-rw-r--r--   0        0        0    23775 2024-05-17 13:15:29.707391 drawlib-0.1.7/drawlib/v0_1/private/core/fonts.py
+-rw-r--r--   0        0        0    33160 2024-05-17 07:10:44.348191 drawlib-0.1.7/drawlib/v0_1/private/core/model.py
+-rw-r--r--   0        0        0    18865 2024-05-19 04:26:51.380337 drawlib-0.1.7/drawlib/v0_1/private/core/theme.py
+-rw-r--r--   0        0        0    12272 2024-05-19 00:50:29.097717 drawlib-0.1.7/drawlib/v0_1/private/core/theme_officials.py
+-rw-r--r--   0        0        0    51534 2024-05-17 08:42:26.352080 drawlib-0.1.7/drawlib/v0_1/private/core/theme_styles.py
+-rw-r--r--   0        0        0    28300 2024-05-17 11:42:16.612394 drawlib-0.1.7/drawlib/v0_1/private/core/util.py
+-rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/__init__.py
+-rw-r--r--   0        0        0    15589 2024-05-17 11:33:32.642807 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/base.py
+-rw-r--r--   0        0        0     7992 2024-05-17 04:55:01.315534 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/canvas.py
+-rw-r--r--   0        0        0     4950 2024-05-17 04:01:16.413350 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/image.py
+-rw-r--r--   0        0        0     6593 2024-05-17 04:01:22.784734 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/line.py
+-rw-r--r--   0        0        0     4297 2024-05-17 04:01:28.386700 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/original_arrow.py
+-rw-r--r--   0        0        0    12132 2024-05-17 12:08:03.060649 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/original_polygon.py
+-rw-r--r--   0        0        0    16466 2024-05-17 04:01:43.093731 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/patches.py
+-rw-r--r--   0        0        0     3264 2024-05-17 04:02:22.095588 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/text.py
+-rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.7/drawlib/v0_1/private/download.py
+-rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.7/drawlib/v0_1/private/dutil.py
+-rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.7/drawlib/v0_1/private/icons/__init__.py
+-rw-r--r--   0        0        0   902368 2024-05-17 00:56:51.813460 drawlib-0.1.7/drawlib/v0_1/private/icons/phosphor.py
+-rw-r--r--   0        0        0     1998 2024-05-17 04:04:01.158522 drawlib-0.1.7/drawlib/v0_1/private/icons/util.py
+-rw-r--r--   0        0        0     1206 2024-05-21 13:50:52.977426 drawlib-0.1.7/drawlib/v0_1/private/logging.py
+-rw-r--r--   0        0        0     6689 2024-05-21 13:34:20.888010 drawlib-0.1.7/drawlib/v0_1/private/settings.py
+-rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.7/drawlib/v0_1/private/smartarts/__init__.py
+-rw-r--r--   0        0        0     3482 2024-05-17 07:07:04.377539 drawlib-0.1.7/drawlib/v0_1/private/smartarts/bubblespeech.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.7/drawlib/v0_1/private/smartarts/cycle.py
+-rw-r--r--   0        0        0      686 2024-05-17 01:14:56.535422 drawlib-0.1.7/drawlib/v0_1/private/smartarts/dsart.py
+-rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.7/drawlib/v0_1/private/smartarts/groups.py
+-rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.7/drawlib/v0_1/private/smartarts/pyramid.py
+-rw-r--r--   0        0        0     5905 2024-05-17 01:19:04.280798 drawlib-0.1.7/drawlib/v0_1/private/smartarts/sourcecode.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.7/drawlib/v0_1/private/smartarts/table.py
+-rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.7/drawlib/v0_1/private/smartarts/tree.py
+-rw-r--r--   0        0        0    10163 2024-05-20 09:07:41.448465 drawlib-0.1.7/drawlib/v0_1/private/util.py
+-rw-r--r--   0        0        0      407 2024-05-17 07:28:29.821380 drawlib-0.1.7/drawlib/v0_1/private/validators/__init__.py
+-rw-r--r--   0        0        0     7382 2024-05-17 07:25:34.994200 drawlib-0.1.7/drawlib/v0_1/private/validators/args.py
+-rw-r--r--   0        0        0     1576 2024-05-17 07:25:58.475653 drawlib-0.1.7/drawlib/v0_1/private/validators/color.py
+-rw-r--r--   0        0        0     3275 2024-05-17 08:44:34.098244 drawlib-0.1.7/drawlib/v0_1/private/validators/coordinate.py
+-rw-r--r--   0        0        0      891 2024-05-17 08:44:42.485495 drawlib-0.1.7/drawlib/v0_1/private/validators/image.py
+-rw-r--r--   0        0        0     1249 2024-05-17 08:44:59.932902 drawlib-0.1.7/drawlib/v0_1/private/validators/line.py
+-rw-r--r--   0        0        0     1332 2024-05-17 08:45:07.566582 drawlib-0.1.7/drawlib/v0_1/private/validators/shape.py
+-rw-r--r--   0        0        0      660 2024-05-17 07:27:28.907431 drawlib-0.1.7/drawlib/v0_1/private/validators/smartarts.py
+-rw-r--r--   0        0        0     2276 2024-05-17 08:45:25.563109 drawlib-0.1.7/drawlib/v0_1/private/validators/style.py
+-rw-r--r--   0        0        0      824 2024-05-17 07:27:54.398157 drawlib-0.1.7/drawlib/v0_1/private/validators/text.py
+-rw-r--r--   0        0        0     2270 2024-05-17 08:45:46.188412 drawlib-0.1.7/drawlib/v0_1/private/validators/types.py
+-rw-r--r--   0        0        0      712 2024-05-21 14:45:13.302199 drawlib-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.7/PKG-INFO
```

### Comparing `drawlib-0.1.6/LICENSE.txt` & `drawlib-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/README.md` & `drawlib-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/__init__.py` & `drawlib-0.1.7/drawlib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 - drawlib.v0_1: API v0.1 interface (latest)
 
 """
 
 from typing import Final
 
 # please update here when you release new version
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 
 # might not be changed
 LIB_NAME: Final[str] = "drawlib"
 AUTHOR: Final[str] = "Yuichi Ito"
 CONTACT: Final[str] = "yuichi@yuichi.com"
 __version__: Final[str] = VERSION
```

### Comparing `drawlib-0.1.6/drawlib/__main__.py` & `drawlib-0.1.7/drawlib/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/apis.py` & `drawlib-0.1.7/drawlib/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/__init__.py` & `drawlib-0.1.7/drawlib/v0_1/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/__main__.py` & `drawlib-0.1.7/drawlib/v0_1/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/apis.py` & `drawlib-0.1.7/drawlib/v0_1/apis.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,17 +113,14 @@
     phosphor as icon_phosphor,
 )
 
 #################
 ### Utilities ###
 #################
 
-from drawlib.v0_1.private.tools import (
-    dexec,
-)
 from drawlib.v0_1.private import (
     dutil,
 )
 from drawlib.v0_1.private.settings import (
     dsettings,
 )
 from drawlib.v0_1.private.smartarts import (
```

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/__init__.py` & `drawlib-0.1.7/drawlib/v0_1/private/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core/__init__.py` & `drawlib-0.1.7/drawlib/v0_1/private/core/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core/colors.py` & `drawlib-0.1.7/drawlib/v0_1/private/core/colors.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core/dimage.py` & `drawlib-0.1.7/drawlib/v0_1/private/core/dimage.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core/fonts.py` & `drawlib-0.1.7/drawlib/v0_1/private/core/fonts.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core/model.py` & `drawlib-0.1.7/drawlib/v0_1/private/core/model.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core/theme.py` & `drawlib-0.1.7/drawlib/v0_1/private/core/theme.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,26 +89,33 @@
     * define theme here
     * provide theme access methods
 
     """
 
     @dataclasses.dataclass
     class ThemeStyle:
+        # mandatory for default
         backgroundcolor: Union[Tuple[int, int, int], Tuple[int, int, int, float], None] = None
         sourcecodefont: Optional[FontSourceCode] = None
         iconstyle: Optional[IconStyle] = None
         imagestyle: Optional[ImageStyle] = None
         linestyle: Optional[LineStyle] = None
         linearrowstyle: Optional[LineArrowStyle] = None
         shapestyle: Optional[ShapeStyle] = None
         shapetextstyle: Optional[ShapeTextStyle] = None
         textstyle: Optional[TextStyle] = None
 
+        # optional for default
+        arcstyle: Optional[ShapeStyle] = None
+        arttextstyle: Optional[ShapeTextStyle] = None
+
     @error_handler
     def __init__(self):
+        self._style_names: List[str] = []
+
         self.backgroundcolors = BackgroundColors()
         self.sourcecodefonts = SourceCodeFonts()
         self.iconstyles = IconStyles()
         self.imagestyles = ImageStyles()
         self.linestyles = LineStyles()
         self.linearrowstyles = LineArrowStyles()
         self.shapestyles = ShapeStyles()
@@ -170,14 +177,16 @@
         This method need to be called before setting manual theme.
 
         Returns:
             None
 
         """
 
+        self._style_names: List[str] = []
+
         self.backgroundcolors = BackgroundColors()
         self.sourcecodefonts = SourceCodeFonts()
         self.iconstyles = IconStyles()
         self.imagestyles = ImageStyles()
         self.linestyles = LineStyles()
         self.linearrowstyles = LineArrowStyles()
         self.shapestyles = ShapeStyles()
@@ -287,14 +296,16 @@
             ]
         ],
     ) -> None:
 
         # initialize
         self._initialize()
 
+        self._style_names.append("")
+
         # set default background color
         _check_color(
             default_style.backgroundcolor,
             "default_style.backgroundcolor is mandatory. "
             "Format is (R, G, B) or (R, G, B, A). Where R,G,B is 0~255 and A is 0.0~1.0.",
         )
         self.backgroundcolors.set(default_style.backgroundcolor)
@@ -331,14 +342,16 @@
 
         if not isinstance(default_style.textstyle, TextStyle):
             raise ValueError("default_style.textstyle is mandatory. Type must be TextStyle.")
         self.textstyles.set(default_style.textstyle)
 
         # named styles
         for name, styles in named_styles:
+            self._style_names.append(name)
+
             if styles.backgroundcolor is not None:
                 _check_color(
                     styles.backgroundcolor,
                     f"name={name}, ThemeStyle.backgroundcolor format must be (R,G,B) or (R,G,B,A). "
                     "Format is (R, G, B) or (R, G, B, A). Where R,G,B is 0~255 and A is 0.0~1.0.",
                 )
                 self.backgroundcolors.set(styles.backgroundcolor, name)
@@ -379,14 +392,84 @@
                 self.shapetextstyles.set(styles.shapetextstyle, name)
 
             if styles.textstyle is not None:
                 if not isinstance(styles.textstyle, TextStyle):
                     raise ValueError(f"name={name}, ThemeStyle.textstyle type must be TextStyle.")
                 self.textstyles.set(styles.textstyle, name)
 
+    @error_handler
+    def print_style_table(self) -> None:
+        print(self._get_style_table())
+
+    def _get_style_table(self) -> str:
+        lines: List[str] = []
+
+        col1: List[str] = [
+            "",
+            "IconStyle",
+            "ImageStyle",
+            "LineStyle",
+            "LineArrowStyle",
+            "ShapeStyle",
+            "ShapeTextStyle",
+            "TextStyle",
+        ]
+
+        row_objects = [
+            self.iconstyles,
+            self.imagestyles,
+            self.linestyles,
+            self.linearrowstyles,
+            self.shapestyles,
+            self.shapetextstyles,
+            self.textstyles,
+        ]
+
+        # create columns
+        cols: List[List[str]] = [col1]
+        for style_name in self._style_names:
+            col: List[str] = [style_name]
+            for row_object in row_objects:
+                if row_object.has(style_name):
+                    col.append("x")
+                else:
+                    col.append("")
+            cols.append(col)
+
+        # modify text length
+        cols2 = []
+        for col in cols:
+            max_length = max(len(s) for s in col)
+            padded_strings = [s.ljust(max_length) for s in col]
+            cols2.append(padded_strings)
+
+        def draw_border():
+            text = "+"
+            for col in cols2:
+                t = "-" * (len(col[0]) + 2)
+                text += f"{t}+"
+            lines.append(text)
+
+        for i in range(len(col1)):
+            if i == 0:
+                draw_border()
+
+            text = "|"
+            for col in cols2:
+                text += f" {col[i]} |"
+            lines.append(text)
+
+            if i == 0:
+                draw_border()
+
+            if i == len(col1) - 1:
+                draw_border()
+
+        return "\n".join(lines).strip()
+
 
 def _check_color(color, error_message: str):
 
     if not isinstance(color, tuple):
         raise ValueError(error_message)
     if len(color) not in [3, 4]:
         raise ValueError(error_message)
```

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core/theme_officials.py` & `drawlib-0.1.7/drawlib/v0_1/private/core/theme_officials.py`

 * *Files 3% similar despite different names*

```diff
@@ -403,35 +403,46 @@
                 ShapeTextStyle,
                 TextStyle,
             ]
         ],
     ]
 ]:
     new_named_styles = deepcopy(named_styles)
-    default_shapetextstyle = default_styles[5]
 
     # add white ShapeTextStyle
-    if not isinstance(default_shapetextstyle, ShapeTextStyle):
-        raise ValueError()
-    white_shapetextstyle = default_shapetextstyle.copy()
-    white_shapetextstyle.color = Colors.White
-    new_named_styles.append(("white", [white_shapetextstyle]))
+    has_named_style_white = False
+    for named_style in new_named_styles:
+        name = named_style[0]
+        if name == "white":
+            has_named_style_white = True
+
+    if not has_named_style_white:
+        default_shapetextstyle = default_styles[5]
+        if not isinstance(default_shapetextstyle, ShapeTextStyle):
+            raise ValueError()
+        white_shapetextstyle = default_shapetextstyle.copy()
+        white_shapetextstyle.color = Colors.White
+        new_named_styles.append(("white", [white_shapetextstyle]))
 
     # add IconStyle and LineArrowStyle with new names
-    for name, styles in named_styles:
+    inserted = 0
+    for i, (name, styles) in enumerate(named_styles, start=1):
         icon, image, line, linearrow, shape, shapetext, text = styles
         if isinstance(icon, IconStyle) and isinstance(shape, ShapeStyle):
             icon_lcolor = icon.copy()
             icon_lcolor.color = shape.lcolor
             icon_fcolor = icon.copy()
             icon_fcolor.color = shape.fcolor
-            new_named_styles.append((f"lcolor-{name}", [icon_lcolor]))
-            new_named_styles.append((f"fcolor-{name}", [icon_fcolor]))
+            new_named_styles.insert(i + inserted, (f"lc-{name}", [icon_lcolor]))
+            inserted += 1
+            new_named_styles.insert(i + inserted, (f"fc-{name}", [icon_fcolor]))
+            inserted += 1
         else:
             raise ValueError()
 
         if isinstance(linearrow, LineArrowStyle):
-            new_named_styles.append((f"linearrow-{name}", [linearrow]))
+            new_named_styles.insert(i + inserted, (f"la-{name}", [linearrow]))
+            inserted += 1
         else:
             raise ValueError()
 
     return new_named_styles
```

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core/theme_styles.py` & `drawlib-0.1.7/drawlib/v0_1/private/core/theme_styles.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core/util.py` & `drawlib-0.1.7/drawlib/v0_1/private/core/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core_canvas/__init__.py` & `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core_canvas/base.py` & `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/base.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core_canvas/canvas.py` & `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core_canvas/image.py` & `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/image.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core_canvas/line.py` & `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/line.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core_canvas/original_arrow.py` & `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/original_arrow.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core_canvas/original_polygon.py` & `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/original_polygon.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core_canvas/patches.py` & `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/patches.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/core_canvas/text.py` & `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/text.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/download.py` & `drawlib-0.1.7/drawlib/v0_1/private/download.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/dutil.py` & `drawlib-0.1.7/drawlib/v0_1/private/dutil.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/icons/__init__.py` & `drawlib-0.1.7/drawlib/v0_1/private/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/icons/phosphor.py` & `drawlib-0.1.7/drawlib/v0_1/private/icons/phosphor.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/icons/util.py` & `drawlib-0.1.7/drawlib/v0_1/private/icons/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/logging.py` & `drawlib-0.1.7/drawlib/v0_1/private/logging.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/settings.py` & `drawlib-0.1.7/drawlib/v0_1/private/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         elif mode in ["verbose", "developer"]:
             logger.setLevel(logging.DEBUG)
         elif mode == "quiet":
             logger.setLevel(logging.CRITICAL)
         else:
             logger.critical(f'logging mode "{mode}" is not supported.')
             sys.exit(1)
-        logger.debug(f'set_log_mode(): "{mode}"')
+        # logger.debug(f'set_log_mode(): "{mode}"')
 
         self._logging_mode = mode
 
     def get_suppress_warning(self) -> bool:
         """Get supressing-warning is enabled or not.
 
         Matplot warnings are shown when it detects small troubles.
```

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/smartarts/__init__.py` & `drawlib-0.1.7/drawlib/v0_1/private/smartarts/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/smartarts/bubblespeech.py` & `drawlib-0.1.7/drawlib/v0_1/private/smartarts/bubblespeech.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/smartarts/dsart.py` & `drawlib-0.1.7/drawlib/v0_1/private/smartarts/dsart.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/smartarts/groups.py` & `drawlib-0.1.7/drawlib/v0_1/private/smartarts/groups.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/smartarts/pyramid.py` & `drawlib-0.1.7/drawlib/v0_1/private/smartarts/pyramid.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/smartarts/sourcecode.py` & `drawlib-0.1.7/drawlib/v0_1/private/smartarts/sourcecode.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/smartarts/tree.py` & `drawlib-0.1.7/drawlib/v0_1/private/smartarts/tree.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/util.py` & `drawlib-0.1.7/drawlib/v0_1/private/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/args.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/args.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/color.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/color.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/coordinate.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/coordinate.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/image.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/image.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/line.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/line.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/shape.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/shape.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/smartarts.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/smartarts.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/style.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/style.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/text.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/text.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/drawlib/v0_1/private/validators/types.py` & `drawlib-0.1.7/drawlib/v0_1/private/validators/types.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.6/pyproject.toml` & `drawlib-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "drawlib"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python drawing library. Illustration as Code."
 homepage = "https://www.drawlib.com"
 repository = "https://github.com/yuichi110/drawlib"
 authors = [ "Yuichi Ito <yuichi@yuichi.com>",]
 readme = "README.md"
 
 [tool.black]
@@ -25,10 +25,8 @@
 mypy = "^1.9.0"
 pylint = "^3.1.0"
 types-pillow = "^10.2.0.20240311"
 radon = "^6.0.1"
 bandit = "^1.7.8"
 pytest-cov = "^5.0.0"
 pydocstyle = "^6.3.0"
-sphinx = "^7.2.6"
-sphinx-rtd-theme = "^2.0.0"
 toml = "^0.10.2"
```

### Comparing `drawlib-0.1.6/PKG-INFO` & `drawlib-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drawlib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python drawing library. Illustration as Code.
 Home-page: https://www.drawlib.com
 Author: Yuichi Ito
 Author-email: yuichi@yuichi.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

