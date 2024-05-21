# Comparing `tmp/iot_protocols-2.1.0.1.tar.gz` & `tmp/iot_protocols-2.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iot_protocols-2.1.0.1.tar", last modified: Mon Apr 15 11:28:48 2024, max compression
+gzip compressed data, was "iot_protocols-2.1.0.2.tar", last modified: Tue May 21 06:48:40 2024, max compression
```

## Comparing `iot_protocols-2.1.0.1.tar` & `iot_protocols-2.1.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.529352 iot_protocols-2.1.0.1/
--rw-rw-rw-   0        0        0     1093 2024-03-21 09:14:47.000000 iot_protocols-2.1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3887 2024-04-15 11:28:48.524746 iot_protocols-2.1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3150 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.372434 iot_protocols-2.1.0.1/iot_protocols/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/__init__.py
--rw-rw-rw-   0        0        0     1937 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/data.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.419158 iot_protocols-2.1.0.1/iot_protocols/devices/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/devices/__init__.py
--rw-rw-rw-   0        0        0     2402 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/devices/basics.py
--rw-rw-rw-   0        0        0     5140 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/iot_protocols/devices/iec62056_meter.py
--rw-rw-rw-   0        0        0     1138 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/iot_protocols/devices/interfaces.py
--rw-rw-rw-   0        0        0     1135 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/devices/models.py
--rw-rw-rw-   0        0        0     5891 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/devices/moxa_iologik_r1214.py
--rw-rw-rw-   0        0        0     6978 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/iot_protocols/devices/socomec.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.422157 iot_protocols-2.1.0.1/iot_protocols/protocols/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.435158 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/
--rw-rw-rw-   0        0        0       39 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/__init__.py
--rw-rw-rw-   0        0        0    10568 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/client.py
--rw-rw-rw-   0        0        0      315 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.462164 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/
--rw-rw-rw-   0        0        0       65 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/__init__.py
--rw-rw-rw-   0        0        0    12431 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/client.py
--rw-rw-rw-   0        0        0      318 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/constants.py
--rw-rw-rw-   0        0        0     1387 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/exceptions.py
--rw-rw-rw-   0        0        0    11468 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/messages.py
--rw-rw-rw-   0        0        0    12642 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/transports.py
--rw-rw-rw-   0        0        0     1872 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.483233 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/
--rw-rw-rw-   0        0        0      541 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/__init__.py
--rw-rw-rw-   0        0        0     8706 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/client.py
--rw-rw-rw-   0        0        0     1905 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/decoder.py
--rw-rw-rw-   0        0        0      331 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/exceptions.py
--rw-rw-rw-   0        0        0      981 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/requests.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.507676 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/__init__.py
--rw-rw-rw-   0        0        0     2738 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/client.py
--rw-rw-rw-   0        0        0      198 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/exceptions.py
--rw-rw-rw-   0        0        0      232 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/requests.py
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/responses.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.521389 iot_protocols-2.1.0.1/iot_protocols.egg-info/
--rw-rw-rw-   0        0        0     3887 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1518 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      890 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 11:28:48.530678 iot_protocols-2.1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.515016 iot_protocols-2.1.0.1/test/
--rw-rw-rw-   0        0        0     2058 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/test/test_iologik_r1214.py
--rw-rw-rw-   0        0        0     1416 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/test/tests_iec62056.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.305883 iot_protocols-2.1.0.2/
+-rw-rw-rw-   0        0        0     1093 2024-03-21 09:14:47.000000 iot_protocols-2.1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3887 2024-05-21 06:48:40.301258 iot_protocols-2.1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3150 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.137653 iot_protocols-2.1.0.2/iot_protocols/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/__init__.py
+-rw-rw-rw-   0        0        0     1937 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/data.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.181653 iot_protocols-2.1.0.2/iot_protocols/devices/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/devices/__init__.py
+-rw-rw-rw-   0        0        0     2402 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/devices/basics.py
+-rw-rw-rw-   0        0        0     5140 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.2/iot_protocols/devices/iec62056_meter.py
+-rw-rw-rw-   0        0        0     1138 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.2/iot_protocols/devices/interfaces.py
+-rw-rw-rw-   0        0        0     1135 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/devices/models.py
+-rw-rw-rw-   0        0        0     5891 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/devices/moxa_iologik_r1214.py
+-rw-rw-rw-   0        0        0     6978 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.2/iot_protocols/devices/socomec.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.184652 iot_protocols-2.1.0.2/iot_protocols/protocols/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.195664 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/
+-rw-rw-rw-   0        0        0       39 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/__init__.py
+-rw-rw-rw-   0        0        0    10568 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/client.py
+-rw-rw-rw-   0        0        0      315 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.232657 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/
+-rw-rw-rw-   0        0        0       65 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/__init__.py
+-rw-rw-rw-   0        0        0    12431 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/client.py
+-rw-rw-rw-   0        0        0      318 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/constants.py
+-rw-rw-rw-   0        0        0     1387 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/exceptions.py
+-rw-rw-rw-   0        0        0    11468 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/messages.py
+-rw-rw-rw-   0        0        0    12642 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/transports.py
+-rw-rw-rw-   0        0        0     1872 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.256667 iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/
+-rw-rw-rw-   0        0        0      541 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/__init__.py
+-rw-rw-rw-   0        0        0     8706 2024-05-21 06:47:59.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/client.py
+-rw-rw-rw-   0        0        0     1905 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/decoder.py
+-rw-rw-rw-   0        0        0      331 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/exceptions.py
+-rw-rw-rw-   0        0        0      981 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/requests.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.281954 iot_protocols-2.1.0.2/iot_protocols/protocols/snap7/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/snap7/__init__.py
+-rw-rw-rw-   0        0        0     2738 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/snap7/client.py
+-rw-rw-rw-   0        0        0      198 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/snap7/exceptions.py
+-rw-rw-rw-   0        0        0      232 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/snap7/requests.py
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/iot_protocols/protocols/snap7/responses.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.295883 iot_protocols-2.1.0.2/iot_protocols.egg-info/
+-rw-rw-rw-   0        0        0     3887 2024-05-21 06:48:40.000000 iot_protocols-2.1.0.2/iot_protocols.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1518 2024-05-21 06:48:40.000000 iot_protocols-2.1.0.2/iot_protocols.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:48:40.000000 iot_protocols-2.1.0.2/iot_protocols.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-21 06:48:40.000000 iot_protocols-2.1.0.2/iot_protocols.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 06:48:40.000000 iot_protocols-2.1.0.2/iot_protocols.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      890 2024-05-21 06:48:07.000000 iot_protocols-2.1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:48:40.306879 iot_protocols-2.1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 06:48:40.289222 iot_protocols-2.1.0.2/test/
+-rw-rw-rw-   0        0        0     2058 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.2/test/test_iologik_r1214.py
+-rw-rw-rw-   0        0        0     1416 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.2/test/tests_iec62056.py
```

### Comparing `iot_protocols-2.1.0.1/LICENSE` & `iot_protocols-2.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/PKG-INFO` & `iot_protocols-2.1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iot-protocols
-Version: 2.1.0.1
+Version: 2.1.0.2
 Summary: Generic IIoT protocols package
 Author-email: Adrien Delhaye <adrien.delhaye@memoco.eu>
 Project-URL: Homepage, https://pypi.org/manage/project/iot-protocols
 Keywords: python,iiot,protocols
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `iot_protocols-2.1.0.1/README.md` & `iot_protocols-2.1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/data.py` & `iot_protocols-2.1.0.2/iot_protocols/data.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/devices/basics.py` & `iot_protocols-2.1.0.2/iot_protocols/devices/basics.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/devices/iec62056_meter.py` & `iot_protocols-2.1.0.2/iot_protocols/devices/iec62056_meter.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/devices/interfaces.py` & `iot_protocols-2.1.0.2/iot_protocols/devices/interfaces.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/devices/models.py` & `iot_protocols-2.1.0.2/iot_protocols/devices/models.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/devices/moxa_iologik_r1214.py` & `iot_protocols-2.1.0.2/iot_protocols/devices/moxa_iologik_r1214.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/devices/socomec.py` & `iot_protocols-2.1.0.2/iot_protocols/devices/socomec.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/client.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/client.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/client.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/client.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/exceptions.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/messages.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/messages.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/transports.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/transports.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/utils.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/iec62056/tools/utils.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/__init__.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/client.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/client.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/decoder.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/decoder.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/requests.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/modbus/requests.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/client.py` & `iot_protocols-2.1.0.2/iot_protocols/protocols/snap7/client.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/iot_protocols.egg-info/PKG-INFO` & `iot_protocols-2.1.0.2/iot_protocols.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iot-protocols
-Version: 2.1.0.1
+Version: 2.1.0.2
 Summary: Generic IIoT protocols package
 Author-email: Adrien Delhaye <adrien.delhaye@memoco.eu>
 Project-URL: Homepage, https://pypi.org/manage/project/iot-protocols
 Keywords: python,iiot,protocols
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `iot_protocols-2.1.0.1/iot_protocols.egg-info/SOURCES.txt` & `iot_protocols-2.1.0.2/iot_protocols.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/pyproject.toml` & `iot_protocols-2.1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iot-protocols"
-version = "2.1.0.1"
+version = "2.1.0.2"
 authors = [
   { name="Adrien Delhaye", email="adrien.delhaye@memoco.eu" },
 ]
 description = "Generic IIoT protocols package"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `iot_protocols-2.1.0.1/test/test_iologik_r1214.py` & `iot_protocols-2.1.0.2/test/test_iologik_r1214.py`

 * *Files identical despite different names*

### Comparing `iot_protocols-2.1.0.1/test/tests_iec62056.py` & `iot_protocols-2.1.0.2/test/tests_iec62056.py`

 * *Files identical despite different names*

