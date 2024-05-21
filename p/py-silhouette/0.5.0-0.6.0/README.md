# Comparing `tmp/py_silhouette-0.5.0.tar.gz` & `tmp/py_silhouette-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_silhouette-0.5.0.tar", last modified: Thu Jun  8 05:41:04 2023, max compression
+gzip compressed data, was "py_silhouette-0.6.0.tar", last modified: Tue May 21 20:46:55 2024, max compression
```

## Comparing `py_silhouette-0.5.0.tar` & `py_silhouette-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-08 05:41:04.417069 py_silhouette-0.5.0/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2023-06-08 05:41:04.417069 py_silhouette-0.5.0/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2670 2019-01-20 19:51:33.000000 py_silhouette-0.5.0/README.md
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-08 05:41:04.413735 py_silhouette-0.5.0/py_silhouette/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      202 2019-01-20 19:37:22.000000 py_silhouette-0.5.0/py_silhouette/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    25201 2023-06-08 05:36:01.000000 py_silhouette-0.5.0/py_silhouette/device.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       23 2023-06-08 05:39:41.000000 py_silhouette-0.5.0/py_silhouette/version.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-08 05:41:04.413735 py_silhouette-0.5.0/py_silhouette.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      296 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       27 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       14 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2023-06-08 05:41:04.417069 py_silhouette-0.5.0/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1086 2022-08-26 13:23:43.000000 py_silhouette-0.5.0/setup.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-08 05:41:04.417069 py_silhouette-0.5.0/test/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4367 2020-09-01 13:44:40.000000 py_silhouette-0.5.0/test/test_sheet.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-21 20:46:55.445984 py_silhouette-0.6.0/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      847 2024-05-21 20:46:55.445984 py_silhouette-0.6.0/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2670 2019-01-20 19:51:33.000000 py_silhouette-0.6.0/README.md
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-21 20:46:55.445984 py_silhouette-0.6.0/py_silhouette/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      202 2019-01-20 19:37:22.000000 py_silhouette-0.6.0/py_silhouette/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    26134 2024-05-21 20:44:55.000000 py_silhouette-0.6.0/py_silhouette/device.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       23 2024-05-21 20:46:01.000000 py_silhouette-0.6.0/py_silhouette/version.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-21 20:46:55.445984 py_silhouette-0.6.0/py_silhouette.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      847 2024-05-21 20:46:55.000000 py_silhouette-0.6.0/py_silhouette.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      296 2024-05-21 20:46:55.000000 py_silhouette-0.6.0/py_silhouette.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-05-21 20:46:55.000000 py_silhouette-0.6.0/py_silhouette.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       27 2024-05-21 20:46:55.000000 py_silhouette-0.6.0/py_silhouette.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       14 2024-05-21 20:46:55.000000 py_silhouette-0.6.0/py_silhouette.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-05-21 20:46:55.445984 py_silhouette-0.6.0/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1086 2022-08-26 13:23:43.000000 py_silhouette-0.6.0/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-21 20:46:55.445984 py_silhouette-0.6.0/test/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4367 2020-09-01 13:44:40.000000 py_silhouette-0.6.0/test/test_sheet.py
```

### Comparing `py_silhouette-0.5.0/PKG-INFO` & `py_silhouette-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_silhouette
-Version: 0.5.0
+Version: 0.6.0
 Summary: A USB driver and Python API to control the Silhouette Portrait plotter.
 Home-page: https://github.com/mossblaser/py_silhouette
 Author: Jonathan Heathcote
 License: LGPLv3
 Keywords: plotter cutter driver usb silhouette
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,7 +12,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
+Requires-Dist: pyusb>=1.0.0
+Requires-Dist: attrs>=18.0.0
```

### Comparing `py_silhouette-0.5.0/README.md` & `py_silhouette-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `py_silhouette-0.5.0/py_silhouette/device.py` & `py_silhouette-0.6.0/py_silhouette/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,14 +252,42 @@
         area_width_max=inch2mm(12.0),
         area_height_min=inch2mm(3.0),
         area_height_max=inch2mm(40.0),
         tool_depth_min=0,
         tool_depth_max=10,
         tool_speed_max=3000.0,
     ),
+    # Contributed by Gabriel Davison (@gabrieldavison on GitHub, see
+    # mossblaser/plottie#10)
+    DeviceParameters(
+        product_name='Silhouette Cameo4 Plus',
+        usb_vendor_id=0x0B4D,
+        usb_product_id=0x1138,
+        area_width_min=inch2mm(3.0),
+        area_width_max=inch2mm(15.0),
+        area_height_min=inch2mm(3.0),
+        area_height_max=inch2mm(40.0),
+        tool_depth_min=0,
+        tool_depth_max=10,
+        tool_speed_max=3000.0,
+    ),
+    # Contributed by Arthur Masson (@arthursw on GitHub, see
+    # mossblaser/plottie#10)
+    DeviceParameters(
+        product_name='Silhouette Cameo4 Pro',
+        usb_vendor_id=0x0B4D,
+        usb_product_id=0x1139,
+        area_width_min=inch2mm(3.0),
+        area_width_max=inch2mm(24.0),
+        area_height_min=inch2mm(3.0),
+        area_height_max=inch2mm(40.0),
+        tool_depth_min=0,
+        tool_depth_max=10,
+        tool_speed_max=3000.0,
+    ),
 ]
 
 
 def enumerate_devices(supported_device_parameters=SUPPORTED_DEVICE_PARAMETERS):
     """
     Generator which produces a series of ``(device, device_params)`` pairs for
     all currently connected devices.
```

### Comparing `py_silhouette-0.5.0/py_silhouette.egg-info/PKG-INFO` & `py_silhouette-0.6.0/py_silhouette.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-silhouette
-Version: 0.5.0
+Name: py_silhouette
+Version: 0.6.0
 Summary: A USB driver and Python API to control the Silhouette Portrait plotter.
 Home-page: https://github.com/mossblaser/py_silhouette
 Author: Jonathan Heathcote
 License: LGPLv3
 Keywords: plotter cutter driver usb silhouette
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,7 +12,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
+Requires-Dist: pyusb>=1.0.0
+Requires-Dist: attrs>=18.0.0
```

### Comparing `py_silhouette-0.5.0/setup.py` & `py_silhouette-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `py_silhouette-0.5.0/test/test_sheet.py` & `py_silhouette-0.6.0/test/test_sheet.py`

 * *Files identical despite different names*

