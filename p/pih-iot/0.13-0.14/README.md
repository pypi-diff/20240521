# Comparing `tmp/pih-iot-0.13.tar.gz` & `tmp/pih-iot-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-iot-0.13.tar", last modified: Thu Apr 18 04:22:43 2024, max compression
+gzip compressed data, was "pih-iot-0.14.tar", last modified: Mon May 20 22:56:25 2024, max compression
```

## Comparing `pih-iot-0.13.tar` & `pih-iot-0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 04:22:43.818305 pih-iot-0.13/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:22:43.376426 pih-iot-0.13/IOTDevicesService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-iot-0.13/IOTDevicesService/__init__.py
--rw-rw-rw-   0        0        0      152 2024-04-17 04:59:58.000000 pih-iot-0.13/IOTDevicesService/__main__.py
--rw-rw-rw-   0        0        0      599 2024-04-18 04:12:40.000000 pih-iot-0.13/IOTDevicesService/const.py
--rw-rw-rw-   0        0        0     1381 2024-04-17 15:27:11.000000 pih-iot-0.13/IOTDevicesService/service.py
--rw-rw-rw-   0        0        0      296 2024-04-18 04:22:43.802680 pih-iot-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 04:22:43.752830 pih-iot-0.13/pih_iot.egg-info/
--rw-rw-rw-   0        0        0      296 2024-04-18 04:22:42.000000 pih-iot-0.13/pih_iot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-04-18 04:22:43.000000 pih-iot-0.13/pih_iot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 04:22:42.000000 pih-iot-0.13/pih_iot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-18 04:22:42.000000 pih-iot-0.13/pih_iot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-18 04:22:42.000000 pih-iot-0.13/pih_iot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-18 04:22:42.000000 pih-iot-0.13/pih_iot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 04:22:43.833928 pih-iot-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:56:25.136288 pih-iot-0.14/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:56:23.727005 pih-iot-0.14/IOTDevicesService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-iot-0.14/IOTDevicesService/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-04-17 04:59:58.000000 pih-iot-0.14/IOTDevicesService/__main__.py
+-rw-rw-rw-   0        0        0      599 2024-05-20 22:55:47.000000 pih-iot-0.14/IOTDevicesService/const.py
+-rw-rw-rw-   0        0        0     1381 2024-04-17 15:27:11.000000 pih-iot-0.14/IOTDevicesService/service.py
+-rw-rw-rw-   0        0        0      296 2024-05-20 22:56:25.089410 pih-iot-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:56:24.665133 pih-iot-0.14/pih_iot.egg-info/
+-rw-rw-rw-   0        0        0      296 2024-05-20 22:56:22.000000 pih-iot-0.14/pih_iot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-05-20 22:56:22.000000 pih-iot-0.14/pih_iot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:56:22.000000 pih-iot-0.14/pih_iot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-20 22:56:22.000000 pih-iot-0.14/pih_iot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 22:56:22.000000 pih-iot-0.14/pih_iot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-20 22:56:22.000000 pih-iot-0.14/pih_iot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:56:25.183554 pih-iot-0.14/setup.cfg
```

### Comparing `pih-iot-0.13/IOTDevicesService/const.py` & `pih-iot-0.14/IOTDevicesService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME: str = "IOTDevices"
 
 HOST = Hosts.WS255
 
 MODULES: tuple[str, ...] = ("tinytuya",)
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 API_REGION: str = "eu"
 API_KEY: str = "ss88c577cc4nex5sqf8u"
 API_SECRET: str = "b3eb6c41acf2465cb48bb366ba6c0fd2"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-iot-0.13/IOTDevicesService/service.py` & `pih-iot-0.14/IOTDevicesService/service.py`

 * *Files identical despite different names*

