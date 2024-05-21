# Comparing `tmp/newport_laser_diode_driver-1.0.0.tar.gz` & `tmp/newport_laser_diode_driver-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newport_laser_diode_driver-1.0.0.tar", last modified: Tue May 21 17:10:56 2024, max compression
+gzip compressed data, was "newport_laser_diode_driver-1.0.1.tar", last modified: Tue May 21 17:19:00 2024, max compression
```

## Comparing `newport_laser_diode_driver-1.0.0.tar` & `newport_laser_diode_driver-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:10:56.815382 newport_laser_diode_driver-1.0.0/
--rw-r--r--   0 next       (501) staff       (20)     1093 2024-05-21 16:56:31.000000 newport_laser_diode_driver-1.0.0/LICENSE.txt
--rw-r--r--   0 next       (501) staff       (20)     2358 2024-05-21 17:10:56.815053 newport_laser_diode_driver-1.0.0/PKG-INFO
--rw-r--r--   0 next       (501) staff       (20)     2187 2024-05-21 17:10:17.000000 newport_laser_diode_driver-1.0.0/README.md
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:10:56.814076 newport_laser_diode_driver-1.0.0/newport_laser_diode_driver.egg-info/
--rw-r--r--   0 next       (501) staff       (20)     2358 2024-05-21 17:10:56.000000 newport_laser_diode_driver-1.0.0/newport_laser_diode_driver.egg-info/PKG-INFO
--rw-r--r--   0 next       (501) staff       (20)      368 2024-05-21 17:10:56.000000 newport_laser_diode_driver-1.0.0/newport_laser_diode_driver.egg-info/SOURCES.txt
--rw-r--r--   0 next       (501) staff       (20)        1 2024-05-21 17:10:56.000000 newport_laser_diode_driver-1.0.0/newport_laser_diode_driver.egg-info/dependency_links.txt
--rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:10:56.000000 newport_laser_diode_driver-1.0.0/newport_laser_diode_driver.egg-info/requires.txt
--rw-r--r--   0 next       (501) staff       (20)       10 2024-05-21 17:10:56.000000 newport_laser_diode_driver-1.0.0/newport_laser_diode_driver.egg-info/top_level.txt
--rw-r--r--   0 next       (501) staff       (20)       38 2024-05-21 17:10:56.815440 newport_laser_diode_driver-1.0.0/setup.cfg
--rw-r--r--   0 next       (501) staff       (20)      466 2024-05-21 17:05:59.000000 newport_laser_diode_driver-1.0.0/setup.py
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:10:56.814415 newport_laser_diode_driver-1.0.0/src/
--rw-r--r--   0 next       (501) staff       (20)       52 2024-05-21 16:16:52.000000 newport_laser_diode_driver-1.0.0/src/__init__.py
--rw-r--r--   0 next       (501) staff       (20)    11106 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.0/src/newport_laser_driver.py
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:10:56.814779 newport_laser_diode_driver-1.0.0/tests/
--rw-r--r--   0 next       (501) staff       (20)        0 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.0/tests/__init__.py
--rw-r--r--   0 next       (501) staff       (20)     1780 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.0/tests/test_laser_driver.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:19:00.221501 newport_laser_diode_driver-1.0.1/
+-rw-r--r--   0 next       (501) staff       (20)     1093 2024-05-21 16:56:31.000000 newport_laser_diode_driver-1.0.1/LICENSE.txt
+-rw-r--r--   0 next       (501) staff       (20)     2543 2024-05-21 17:19:00.221238 newport_laser_diode_driver-1.0.1/PKG-INFO
+-rw-r--r--   0 next       (501) staff       (20)     2372 2024-05-21 17:18:35.000000 newport_laser_diode_driver-1.0.1/README.md
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:19:00.220663 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/
+-rw-r--r--   0 next       (501) staff       (20)     2543 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/PKG-INFO
+-rw-r--r--   0 next       (501) staff       (20)      324 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 next       (501) staff       (20)        1 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/requires.txt
+-rw-r--r--   0 next       (501) staff       (20)        6 2024-05-21 17:19:00.000000 newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/top_level.txt
+-rw-r--r--   0 next       (501) staff       (20)       38 2024-05-21 17:19:00.221570 newport_laser_diode_driver-1.0.1/setup.cfg
+-rw-r--r--   0 next       (501) staff       (20)      466 2024-05-21 17:18:52.000000 newport_laser_diode_driver-1.0.1/setup.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 17:19:00.220956 newport_laser_diode_driver-1.0.1/tests/
+-rw-r--r--   0 next       (501) staff       (20)        0 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.1/tests/__init__.py
+-rw-r--r--   0 next       (501) staff       (20)     1780 2024-05-21 16:16:27.000000 newport_laser_diode_driver-1.0.1/tests/test_laser_driver.py
```

### Comparing `newport_laser_diode_driver-1.0.0/LICENSE.txt` & `newport_laser_diode_driver-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newport_laser_diode_driver-1.0.0/PKG-INFO` & `newport_laser_diode_driver-1.0.1/newport_laser_diode_driver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: newport_laser_diode_driver
-Version: 1.0.0
+Name: newport-laser-diode-driver
+Version: 1.0.1
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyusb
 
 # Newport Model 300-500B Series Laser Diode Driver USB Package (for Linux)
 
@@ -56,20 +56,26 @@
 ```shell
 pip install pyusb  # should be already installed by default
 ```
 
 
 ## Usage
 
+In your desired Python environment, run the following shell command:
+
+```shell
+pip install newport-laser-diode-driver
+```
+
 Here is an example snippet of how a Laser Driver object could be instantiated:
 
 ```python
-from 
+from newport_laser_diode_driver import NewportLaserDiodeDriver
 
-model_535B = NewportLaserDriver(idVendor=0x104d, idProduct=0x1001)
+model_535B = NewportLaserDiodeDriver(idVendor=0x104d, idProduct=0x1001)
 
 identifier = model_535B.get_identification()  # obtain the identification
 print(identifier)
 
 model_535B.set_current_set_point(10.0)  # set current set point to be 10.0 mA
 current = model_535B.get_current_set_point()  # get the current set point
 print(current)  # 10.0
```

### Comparing `newport_laser_diode_driver-1.0.0/README.md` & `newport_laser_diode_driver-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,20 +48,26 @@
 ```shell
 pip install pyusb  # should be already installed by default
 ```
 
 
 ## Usage
 
+In your desired Python environment, run the following shell command:
+
+```shell
+pip install newport-laser-diode-driver
+```
+
 Here is an example snippet of how a Laser Driver object could be instantiated:
 
 ```python
-from 
+from newport_laser_diode_driver import NewportLaserDiodeDriver
 
-model_535B = NewportLaserDriver(idVendor=0x104d, idProduct=0x1001)
+model_535B = NewportLaserDiodeDriver(idVendor=0x104d, idProduct=0x1001)
 
 identifier = model_535B.get_identification()  # obtain the identification
 print(identifier)
 
 model_535B.set_current_set_point(10.0)  # set current set point to be 10.0 mA
 current = model_535B.get_current_set_point()  # get the current set point
 print(current)  # 10.0
```

### Comparing `newport_laser_diode_driver-1.0.0/newport_laser_diode_driver.egg-info/PKG-INFO` & `newport_laser_diode_driver-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: newport-laser-diode-driver
-Version: 1.0.0
+Name: newport_laser_diode_driver
+Version: 1.0.1
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyusb
 
 # Newport Model 300-500B Series Laser Diode Driver USB Package (for Linux)
 
@@ -56,20 +56,26 @@
 ```shell
 pip install pyusb  # should be already installed by default
 ```
 
 
 ## Usage
 
+In your desired Python environment, run the following shell command:
+
+```shell
+pip install newport-laser-diode-driver
+```
+
 Here is an example snippet of how a Laser Driver object could be instantiated:
 
 ```python
-from 
+from newport_laser_diode_driver import NewportLaserDiodeDriver
 
-model_535B = NewportLaserDriver(idVendor=0x104d, idProduct=0x1001)
+model_535B = NewportLaserDiodeDriver(idVendor=0x104d, idProduct=0x1001)
 
 identifier = model_535B.get_identification()  # obtain the identification
 print(identifier)
 
 model_535B.set_current_set_point(10.0)  # set current set point to be 10.0 mA
 current = model_535B.get_current_set_point()  # get the current set point
 print(current)  # 10.0
```

### Comparing `newport_laser_diode_driver-1.0.0/tests/test_laser_driver.py` & `newport_laser_diode_driver-1.0.1/tests/test_laser_driver.py`

 * *Files identical despite different names*

