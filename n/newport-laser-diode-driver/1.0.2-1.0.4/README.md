# Comparing `tmp/newport_laser_diode_driver-1.0.2.tar.gz` & `tmp/newport_laser_diode_driver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newport_laser_diode_driver-1.0.2.tar", last modified: Tue May 21 17:32:00 2024, max compression
+gzip compressed data, was "newport_laser_diode_driver-1.0.4.tar", last modified: Tue May 21 17:56:27 2024, max compression
```

## Comparing `newport_laser_diode_driver-1.0.2.tar` & `newport_laser_diode_driver-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:32:00.045317 newport_laser_diode_driver-1.0.2/
--rw-r--r--   0 next       (501) staff       (20)     1093 2024-05-21 16:56:31.000000 newport_laser_diode_driver-1.0.2/LICENSE.txt
--rw-r--r--   0 next       (501) staff       (20)     2543 2024-05-21 17:32:00.045022 newport_laser_diode_driver-1.0.2/PKG-INFO
--rw-r--r--   0 next       (501) staff       (20)     2372 2024-05-21 17:18:35.000000 newport_laser_diode_driver-1.0.2/README.md
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:32:00.044445 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/
--rw-r--r--   0 next       (501) staff       (20)     2543 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/PKG-INFO
--rw-r--r--   0 next       (501) staff       (20)      322 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/SOURCES.txt
--rw-r--r--   0 next       (501) staff       (20)        1 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/dependency_links.txt
--rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/requires.txt
--rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/top_level.txt
--rw-r--r--   0 next       (501) staff       (20)       38 2024-05-21 17:32:00.045381 newport_laser_diode_driver-1.0.2/setup.cfg
--rw-r--r--   0 next       (501) staff       (20)      466 2024-05-21 17:30:36.000000 newport_laser_diode_driver-1.0.2/setup.py
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:32:00.044715 newport_laser_diode_driver-1.0.2/tests/
--rw-r--r--   0 next       (501) staff       (20)        0 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.2/tests/__init__.py
--rw-r--r--   0 next       (501) staff       (20)     1807 2024-05-21 17:31:13.000000 newport_laser_diode_driver-1.0.2/tests/test_model_535b.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:56:27.451514 newport_laser_diode_driver-1.0.4/
+-rw-r--r--   0 next       (501) staff       (20)     1093 2024-05-21 16:56:31.000000 newport_laser_diode_driver-1.0.4/LICENSE.txt
+-rw-r--r--   0 next       (501) staff       (20)     2556 2024-05-21 17:56:27.451178 newport_laser_diode_driver-1.0.4/PKG-INFO
+-rw-r--r--   0 next       (501) staff       (20)     2385 2024-05-21 17:55:32.000000 newport_laser_diode_driver-1.0.4/README.md
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:56:27.449777 newport_laser_diode_driver-1.0.4/newport_laser_diode_driver/
+-rw-r--r--   0 next       (501) staff       (20)       63 2024-05-21 17:39:51.000000 newport_laser_diode_driver-1.0.4/newport_laser_diode_driver/__init__.py
+-rw-r--r--   0 next       (501) staff       (20)    11111 2024-05-21 17:18:12.000000 newport_laser_diode_driver-1.0.4/newport_laser_diode_driver/newport_laser_diode_driver.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:56:27.450583 newport_laser_diode_driver-1.0.4/newport_laser_diode_driver.egg-info/
+-rw-r--r--   0 next       (501) staff       (20)     2556 2024-05-21 17:56:27.000000 newport_laser_diode_driver-1.0.4/newport_laser_diode_driver.egg-info/PKG-INFO
+-rw-r--r--   0 next       (501) staff       (20)      418 2024-05-21 17:56:27.000000 newport_laser_diode_driver-1.0.4/newport_laser_diode_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 next       (501) staff       (20)        1 2024-05-21 17:56:27.000000 newport_laser_diode_driver-1.0.4/newport_laser_diode_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:56:27.000000 newport_laser_diode_driver-1.0.4/newport_laser_diode_driver.egg-info/requires.txt
+-rw-r--r--   0 next       (501) staff       (20)       33 2024-05-21 17:56:27.000000 newport_laser_diode_driver-1.0.4/newport_laser_diode_driver.egg-info/top_level.txt
+-rw-r--r--   0 next       (501) staff       (20)       38 2024-05-21 17:56:27.451574 newport_laser_diode_driver-1.0.4/setup.cfg
+-rw-r--r--   0 next       (501) staff       (20)      466 2024-05-21 17:56:04.000000 newport_laser_diode_driver-1.0.4/setup.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:56:27.450855 newport_laser_diode_driver-1.0.4/tests/
+-rw-r--r--   0 next       (501) staff       (20)        0 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.4/tests/__init__.py
+-rw-r--r--   0 next       (501) staff       (20)     1803 2024-05-21 17:54:12.000000 newport_laser_diode_driver-1.0.4/tests/test_model_535b.py
```

### Comparing `newport_laser_diode_driver-1.0.2/LICENSE.txt` & `newport_laser_diode_driver-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newport_laser_diode_driver-1.0.2/PKG-INFO` & `newport_laser_diode_driver-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: newport_laser_diode_driver
-Version: 1.0.2
+Version: 1.0.4
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyusb
 
-# Newport Model 300-500B Series Laser Diode Driver USB Package (for Linux)
+# Newport Model 300-500B Series Laser Diode Driver Python USB Package (for Linux)
 
 
 ## Pre-requisites
 
 - Permission to connect to the Newport Laser Diode Driver USB device
 - Python version >= 3
 - pyusb library
@@ -80,9 +80,9 @@
 current = model_535B.get_current_set_point()  # get the current set point
 print(current)  # 10.0
 model_535B.enable_laser_output()  # enable laser output
 ```
 
 ## Troubleshooting
 
-To check if the device is recognized by the PC, run `lsusb` to list all USB devices connected to your PC. If the Newport device 
+To check if the device is recognized by the PC, run `usb-devices` to list all USB devices connected to your PC. If the Newport device 
 is not found, try connecting the USB cable from the device to your PC first and then restart the device.
```

### Comparing `newport_laser_diode_driver-1.0.2/README.md` & `newport_laser_diode_driver-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Newport Model 300-500B Series Laser Diode Driver USB Package (for Linux)
+# Newport Model 300-500B Series Laser Diode Driver Python USB Package (for Linux)
 
 
 ## Pre-requisites
 
 - Permission to connect to the Newport Laser Diode Driver USB device
 - Python version >= 3
 - pyusb library
@@ -72,9 +72,9 @@
 current = model_535B.get_current_set_point()  # get the current set point
 print(current)  # 10.0
 model_535B.enable_laser_output()  # enable laser output
 ```
 
 ## Troubleshooting
 
-To check if the device is recognized by the PC, run `lsusb` to list all USB devices connected to your PC. If the Newport device 
+To check if the device is recognized by the PC, run `usb-devices` to list all USB devices connected to your PC. If the Newport device 
 is not found, try connecting the USB cable from the device to your PC first and then restart the device.
```

### Comparing `newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/PKG-INFO` & `newport_laser_diode_driver-1.0.4/newport_laser_diode_driver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: newport-laser-diode-driver
-Version: 1.0.2
+Version: 1.0.4
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyusb
 
-# Newport Model 300-500B Series Laser Diode Driver USB Package (for Linux)
+# Newport Model 300-500B Series Laser Diode Driver Python USB Package (for Linux)
 
 
 ## Pre-requisites
 
 - Permission to connect to the Newport Laser Diode Driver USB device
 - Python version >= 3
 - pyusb library
@@ -80,9 +80,9 @@
 current = model_535B.get_current_set_point()  # get the current set point
 print(current)  # 10.0
 model_535B.enable_laser_output()  # enable laser output
 ```
 
 ## Troubleshooting
 
-To check if the device is recognized by the PC, run `lsusb` to list all USB devices connected to your PC. If the Newport device 
+To check if the device is recognized by the PC, run `usb-devices` to list all USB devices connected to your PC. If the Newport device 
 is not found, try connecting the USB cable from the device to your PC first and then restart the device.
```

### Comparing `newport_laser_diode_driver-1.0.2/tests/test_model_535b.py` & `newport_laser_diode_driver-1.0.4/tests/test_model_535b.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..src.newport_laser_diode_driver import NewportLaserDiodeDriver
+from ..newport_laser_diode_driver import NewportLaserDiodeDriver
 
 model_535b = NewportLaserDiodeDriver(idVendor=0x104d, idProduct=0x1001)
 model_535b.clear_buffer()
 
 def test_identity():
     assert model_535b._dev.manufacturer == "Newport"
     assert model_535b._dev.product == "Model 300/500"
```

