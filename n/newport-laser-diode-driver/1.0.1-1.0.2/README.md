# Comparing `tmp/newport_laser_diode_driver-1.0.1.tar.gz` & `tmp/newport_laser_diode_driver-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newport_laser_diode_driver-1.0.1.tar", last modified: Tue May 21 17:19:00 2024, max compression
+gzip compressed data, was "newport_laser_diode_driver-1.0.2.tar", last modified: Tue May 21 17:32:00 2024, max compression
```

## Comparing `newport_laser_diode_driver-1.0.1.tar` & `newport_laser_diode_driver-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:19:00.221501 newport_laser_diode_driver-1.0.1/
--rw-r--r--   0 next       (501) staff       (20)     1093 2024-05-21 16:56:31.000000 newport_laser_diode_driver-1.0.1/LICENSE.txt
--rw-r--r--   0 next       (501) staff       (20)     2543 2024-05-21 17:19:00.221238 newport_laser_diode_driver-1.0.1/PKG-INFO
--rw-r--r--   0 next       (501) staff       (20)     2372 2024-05-21 17:18:35.000000 newport_laser_diode_driver-1.0.1/README.md
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:19:00.220663 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/
--rw-r--r--   0 next       (501) staff       (20)     2543 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/PKG-INFO
--rw-r--r--   0 next       (501) staff       (20)      324 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/SOURCES.txt
--rw-r--r--   0 next       (501) staff       (20)        1 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/dependency_links.txt
--rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/requires.txt
--rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/top_level.txt
--rw-r--r--   0 next       (501) staff       (20)       38 2024-05-21 17:19:00.221570 newport_laser_diode_driver-1.0.1/setup.cfg
--rw-r--r--   0 next       (501) staff       (20)      466 2024-05-21 17:18:52.000000 newport_laser_diode_driver-1.0.1/setup.py
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:19:00.220956 newport_laser_diode_driver-1.0.1/tests/
--rw-r--r--   0 next       (501) staff       (20)        0 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.1/tests/__init__.py
--rw-r--r--   0 next       (501) staff       (20)     1780 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.1/tests/test_laser_driver.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:32:00.045317 newport_laser_diode_driver-1.0.2/
+-rw-r--r--   0 next       (501) staff       (20)     1093 2024-05-21 16:56:31.000000 newport_laser_diode_driver-1.0.2/LICENSE.txt
+-rw-r--r--   0 next       (501) staff       (20)     2543 2024-05-21 17:32:00.045022 newport_laser_diode_driver-1.0.2/PKG-INFO
+-rw-r--r--   0 next       (501) staff       (20)     2372 2024-05-21 17:18:35.000000 newport_laser_diode_driver-1.0.2/README.md
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:32:00.044445 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/
+-rw-r--r--   0 next       (501) staff       (20)     2543 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/PKG-INFO
+-rw-r--r--   0 next       (501) staff       (20)      322 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 next       (501) staff       (20)        1 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/requires.txt
+-rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:32:00.000000 newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/top_level.txt
+-rw-r--r--   0 next       (501) staff       (20)       38 2024-05-21 17:32:00.045381 newport_laser_diode_driver-1.0.2/setup.cfg
+-rw-r--r--   0 next       (501) staff       (20)      466 2024-05-21 17:30:36.000000 newport_laser_diode_driver-1.0.2/setup.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:32:00.044715 newport_laser_diode_driver-1.0.2/tests/
+-rw-r--r--   0 next       (501) staff       (20)        0 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.2/tests/__init__.py
+-rw-r--r--   0 next       (501) staff       (20)     1807 2024-05-21 17:31:13.000000 newport_laser_diode_driver-1.0.2/tests/test_model_535b.py
```

### Comparing `newport_laser_diode_driver-1.0.1/LICENSE.txt` & `newport_laser_diode_driver-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newport_laser_diode_driver-1.0.1/PKG-INFO` & `newport_laser_diode_driver-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newport_laser_diode_driver
-Version: 1.0.1
+Version: 1.0.2
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyusb
 
 # Newport Model 300-500B Series Laser Diode Driver USB Package (for Linux)
```

### Comparing `newport_laser_diode_driver-1.0.1/README.md` & `newport_laser_diode_driver-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/PKG-INFO` & `newport_laser_diode_driver-1.0.2/newport_laser_diode_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newport-laser-diode-driver
-Version: 1.0.1
+Version: 1.0.2
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyusb
 
 # Newport Model 300-500B Series Laser Diode Driver USB Package (for Linux)
```

### Comparing `newport_laser_diode_driver-1.0.1/tests/test_laser_driver.py` & `newport_laser_diode_driver-1.0.2/tests/test_model_535b.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from ..newport_laser_driver import NewportLaserDriver
+from ..src.newport_laser_diode_driver import NewportLaserDiodeDriver
 
-model_535B = NewportLaserDriver(idVendor=0x104d, idProduct=0x1001)
-model_535B.clear_buffer()
+model_535b = NewportLaserDiodeDriver(idVendor=0x104d, idProduct=0x1001)
+model_535b.clear_buffer()
 
 def test_identity():
-    assert model_535B._dev.manufacturer == "Newport"
-    assert model_535B._dev.product == "Model 300/500"
-    assert model_535B.get_identification().__contains__("NEWPORT")
+    assert model_535b._dev.manufacturer == "Newport"
+    assert model_535b._dev.product == "Model 300/500"
+    assert model_535b.get_identification().__contains__("NEWPORT")
 
 
 #? Getting error message leads to timeout error
 # def test_no_error():
 #     assert model_535B.get_error() == ("0", "No error")
 
 
 def test_key_status_on():
-    model_535B.get_key_switch_status() == 1
+    assert model_535b.get_key_switch_status() == 1
 
 
 def test_set_and_get_current_set_point():
-    model_535B.set_current_set_point(5.0)
-    assert round(model_535B.get_current_set_point(), 1) == 5.0
+    model_535b.set_current_set_point(5.0)
+    assert round(model_535b.get_current_set_point(), 1) == 5.0
 
 
 def test_set_and_get_photodiode_current_set_point():
-    model_535B.set_photodiode_current_set_point(5.0)
-    assert round(model_535B.get_photodiode_current_set_point(), 1) == 5.0
+    model_535b.set_photodiode_current_set_point(5.0)
+    assert round(model_535b.get_photodiode_current_set_point(), 1) == 5.0
 
 
 def test_set_and_get_current_limit():
-    model_535B.set_current_limit(50.0)
-    assert round(model_535B.get_current_limit(), 0) == 50
+    model_535b.set_current_limit(50.0)
+    assert round(model_535b.get_current_limit(), 0) == 50
 
 
 def test_constanst_current_mode():
-    model_535B.enter_constant_current_mode()
-    assert model_535B.get_laser_mode() == "Ilbw" or model_535B.get_laser_mode() == "Ihbw"
+    model_535b.enter_constant_current_mode()
+    assert model_535b.get_laser_mode() == "Ilbw" or model_535b.get_laser_mode() == "Ihbw"
 
 
 def test_constanst_photodiode_current_mode():
-    model_535B.enter_constant_photodiode_current_mode()
-    assert model_535B.get_laser_mode() == "Mdi"
+    model_535b.enter_constant_photodiode_current_mode()
+    assert model_535b.get_laser_mode() == "Mdi"
 
 
 def test_enable_laser_output():
-    model_535B.enable_laser_output()
-    assert model_535B.get_laser_output_enable() == 1
+    model_535b.enable_laser_output()
+    assert model_535b.get_laser_output_enable() == 1
 
 
 def test_disable_laser_output():
-    model_535B.disable_laser_output()
-    assert model_535B.get_laser_output_enable() == 0
+    model_535b.disable_laser_output()
+    assert model_535b.get_laser_output_enable() == 0
 
 
 def test_laser_range():
-    model_535B.set_laser_range_low()
-    assert model_535B.get_laser_range() == 0
+    model_535b.set_laser_range_low()
+    assert model_535b.get_laser_range() == 0
 
-    model_535B.set_laser_range_high()
-    assert model_535B.get_laser_range() == 1
+    model_535b.set_laser_range_high()
+    assert model_535b.get_laser_range() == 1
```

