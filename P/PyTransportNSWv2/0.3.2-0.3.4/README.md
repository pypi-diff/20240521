# Comparing `tmp/pytransportnswv2-0.3.2.tar.gz` & `tmp/pytransportnswv2-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransportnswv2-0.3.2.tar", last modified: Mon May 20 22:10:46 2024, max compression
+gzip compressed data, was "pytransportnswv2-0.3.4.tar", last modified: Tue May 21 05:49:41 2024, max compression
```

## Comparing `pytransportnswv2-0.3.2.tar` & `pytransportnswv2-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-20 22:10:46.587089 pytransportnswv2-0.3.2/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    35149 2024-05-17 11:23:48.000000 pytransportnswv2-0.3.2/LICENSE
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5329 2024-05-20 22:10:46.587089 pytransportnswv2-0.3.2/PKG-INFO
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-20 22:10:46.587089 pytransportnswv2-0.3.2/PyTransportNSWv2.egg-info/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5329 2024-05-20 22:10:46.000000 pytransportnswv2-0.3.2/PyTransportNSWv2.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      279 2024-05-20 22:10:46.000000 pytransportnswv2-0.3.2/PyTransportNSWv2.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2024-05-20 22:10:46.000000 pytransportnswv2-0.3.2/PyTransportNSWv2.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       23 2024-05-20 22:10:46.000000 pytransportnswv2-0.3.2/PyTransportNSWv2.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       13 2024-05-20 22:10:46.000000 pytransportnswv2-0.3.2/PyTransportNSWv2.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4753 2024-05-20 22:09:49.000000 pytransportnswv2-0.3.2/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-20 22:10:46.583089 pytransportnswv2-0.3.2/TransportNSW/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    13395 2024-05-20 21:39:11.000000 pytransportnswv2-0.3.2/TransportNSW/TransportNSW.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       86 2024-05-17 11:22:12.000000 pytransportnswv2-0.3.2/TransportNSW/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2024-05-20 22:10:46.587089 pytransportnswv2-0.3.2/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      804 2024-05-20 22:10:36.000000 pytransportnswv2-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4881 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/TransportNSW/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13926 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/TransportNSW/TransportNSW.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       86 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/TransportNSW/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      823 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/setup.py
```

### Comparing `pytransportnswv2-0.3.2/LICENSE` & `pytransportnswv2-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransportnswv2-0.3.2/PKG-INFO` & `pytransportnswv2-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: PyTransportNSWv2
-Version: 0.3.2
+Version: 0.3.4
 Summary: Get detailed per-trip transport information from TransportNSW
 Home-page: https://github.com/andystewart999/TransportNSW
 Author: andystewart999
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gtfs-realtime-bindings
+Requires-Dist: requests
 
 # TransportNSW
 Python lib to access Transport NSW information.
 
 ## How to Use
 
 ### Get an API Key
@@ -30,17 +31,29 @@
 ### API Documentation
 The source API details can be found here: https://opendata.transport.nsw.gov.au/sites/default/files/2023-08/Trip%20Planner%20API%20manual-opendataproduction%20v3.2.pdf
 
 ### Parameters
 ```python
 .get_trip(origin_stop_id, destination_stop_id, api_key, [trip_wait_time = 0], [transport_type = 0])
 ```
-
 TransportNSW's trip planner can work better if you use the general location IDs (eg Central Station) rather than a specific Stop ID (eg Central Station, Platform 19) for the destination, depending on the transport type.  Forcing a specific end destination sometimes results in much more complicated trips.  Also note that the API expects (and returns) the Stop IDs as strings, although so far they all appear to be numeric.
 
+### transport_type filters
+```
+1: Train
+4: Light rail
+5: Bus
+7: Coach
+9: Ferry
+11: School bus
+99: Walk
+100: Walk
+107: Cycle
+```
+
 ### Sample Code
 
 The following example will return the next trip that starts from a bus stop in St. Ives (207537) five minutes from now, to Central Station's general stop ID (10101100):
 
 **Code:**
 ```python
 from TransportNSW import TransportNSW
```

### Comparing `pytransportnswv2-0.3.2/PyTransportNSWv2.egg-info/PKG-INFO` & `pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: PyTransportNSWv2
-Version: 0.3.2
+Version: 0.3.4
 Summary: Get detailed per-trip transport information from TransportNSW
 Home-page: https://github.com/andystewart999/TransportNSW
 Author: andystewart999
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gtfs-realtime-bindings
+Requires-Dist: requests
 
 # TransportNSW
 Python lib to access Transport NSW information.
 
 ## How to Use
 
 ### Get an API Key
@@ -30,17 +31,29 @@
 ### API Documentation
 The source API details can be found here: https://opendata.transport.nsw.gov.au/sites/default/files/2023-08/Trip%20Planner%20API%20manual-opendataproduction%20v3.2.pdf
 
 ### Parameters
 ```python
 .get_trip(origin_stop_id, destination_stop_id, api_key, [trip_wait_time = 0], [transport_type = 0])
 ```
-
 TransportNSW's trip planner can work better if you use the general location IDs (eg Central Station) rather than a specific Stop ID (eg Central Station, Platform 19) for the destination, depending on the transport type.  Forcing a specific end destination sometimes results in much more complicated trips.  Also note that the API expects (and returns) the Stop IDs as strings, although so far they all appear to be numeric.
 
+### transport_type filters
+```
+1: Train
+4: Light rail
+5: Bus
+7: Coach
+9: Ferry
+11: School bus
+99: Walk
+100: Walk
+107: Cycle
+```
+
 ### Sample Code
 
 The following example will return the next trip that starts from a bus stop in St. Ives (207537) five minutes from now, to Central Station's general stop ID (10101100):
 
 **Code:**
 ```python
 from TransportNSW import TransportNSW
```

### Comparing `pytransportnswv2-0.3.2/README.md` & `pytransportnswv2-0.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,29 @@
 ### API Documentation
 The source API details can be found here: https://opendata.transport.nsw.gov.au/sites/default/files/2023-08/Trip%20Planner%20API%20manual-opendataproduction%20v3.2.pdf
 
 ### Parameters
 ```python
 .get_trip(origin_stop_id, destination_stop_id, api_key, [trip_wait_time = 0], [transport_type = 0])
 ```
-
 TransportNSW's trip planner can work better if you use the general location IDs (eg Central Station) rather than a specific Stop ID (eg Central Station, Platform 19) for the destination, depending on the transport type.  Forcing a specific end destination sometimes results in much more complicated trips.  Also note that the API expects (and returns) the Stop IDs as strings, although so far they all appear to be numeric.
 
+### transport_type filters
+```
+1: Train
+4: Light rail
+5: Bus
+7: Coach
+9: Ferry
+11: School bus
+99: Walk
+100: Walk
+107: Cycle
+```
+
 ### Sample Code
 
 The following example will return the next trip that starts from a bus stop in St. Ives (207537) five minutes from now, to Central Station's general stop ID (10101100):
 
 **Code:**
 ```python
 from TransportNSW import TransportNSW
```

### Comparing `pytransportnswv2-0.3.2/TransportNSW/TransportNSW.py` & `pytransportnswv2-0.3.4/TransportNSW/TransportNSW.py`

 * *Files 6% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
 
         # Origin info
         origin_stop_id = origin['id']
         origin_name = origin['name']
         origin_departure_time = origin['departureTimeEstimated']
 
-	# How long until it leaves?
+        # How long until it leaves?
         due = self.get_due(datetime.strptime(origin_departure_time, fmt))
 
         # Destination info
         destination_stop_id = destination['id']
         destination_name = destination['name']
         destination_arrival_time = destination['arrivalTimeEstimated']
 
@@ -272,28 +272,38 @@
 
     def find_first_leg(self, legs, legtype):
         # Find the first leg of the requested type
         leg_count = len(legs)
         for leg in range (0, leg_count, 1):
             leg_class = legs[leg]['transportation']['product']['class']
 
-            if leg_class == legtype or legtype == 0:
+            # We've got a filter, and the leg type matches it, so return it
+            if legtype != 0 and leg_class == legtype:
+                return leg
+                
+            # We don't have a filter, and this is the first non-walk/cycle leg so return it
+            if  legtype == 0 and leg_class < 99:
                 return leg
 
         # Hmm, we didn't find one
         return None
 
 
     def find_last_leg(self, legs, legtype):
         # Find the last leg of the requested type
         leg_count = len(legs)
         for leg in range (leg_count - 1, -1, -1):
             leg_class = legs[leg]['transportation']['product']['class']
 
-            if leg_class == legtype or legtype == 0:
+            # We've got a filter, and the leg type matches it, so return it
+            if legtype != 0 and leg_class == legtype:
+                return leg
+                
+            # We don't have a filter, and this is the first non-walk/cycle leg so return it
+            if  legtype == 0 and leg_class < 99:
                 return leg
 
         # Hmm, we didn't find one
         return None
 
     def find_changes(self, legs, legtype):
         # Find out how often we have to change
```

### Comparing `pytransportnswv2-0.3.2/setup.py` & `pytransportnswv2-0.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyTransportNSWv2",
-    version="0.3.2",
+    version="0.3.4",
     author="andystewart999",
     description="Get detailed per-trip transport information from TransportNSW",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andystewart999/TransportNSW",
     packages=setuptools.find_packages(),
     install_requires=[
         'gtfs-realtime-bindings',
+        'requests'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

