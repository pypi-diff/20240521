# Comparing `tmp/pytransportnswv2-0.3.0.tar.gz` & `tmp/pytransportnswv2-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransportnswv2-0.3.0.tar", last modified: Fri May 17 11:31:51 2024, max compression
+gzip compressed data, was "pytransportnswv2-0.3.1.tar", last modified: Mon May 20 22:06:34 2024, max compression
```

## Comparing `pytransportnswv2-0.3.0.tar` & `pytransportnswv2-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-17 11:31:51.339066 pytransportnswv2-0.3.0/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    35149 2024-05-17 11:23:48.000000 pytransportnswv2-0.3.0/LICENSE
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4500 2024-05-17 11:31:51.339066 pytransportnswv2-0.3.0/PKG-INFO
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-17 11:31:51.339066 pytransportnswv2-0.3.0/PyTransportNSWv2.egg-info/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4500 2024-05-17 11:31:51.000000 pytransportnswv2-0.3.0/PyTransportNSWv2.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      279 2024-05-17 11:31:51.000000 pytransportnswv2-0.3.0/PyTransportNSWv2.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2024-05-17 11:31:51.000000 pytransportnswv2-0.3.0/PyTransportNSWv2.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       23 2024-05-17 11:31:51.000000 pytransportnswv2-0.3.0/PyTransportNSWv2.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       13 2024-05-17 11:31:51.000000 pytransportnswv2-0.3.0/PyTransportNSWv2.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3924 2024-05-17 11:23:22.000000 pytransportnswv2-0.3.0/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-17 11:31:51.335065 pytransportnswv2-0.3.0/TransportNSW/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    12930 2024-05-17 11:28:53.000000 pytransportnswv2-0.3.0/TransportNSW/TransportNSW.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       86 2024-05-17 11:22:12.000000 pytransportnswv2-0.3.0/TransportNSW/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2024-05-17 11:31:51.339066 pytransportnswv2-0.3.0/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      804 2024-05-17 11:27:07.000000 pytransportnswv2-0.3.0/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-20 22:06:34.798767 pytransportnswv2-0.3.1/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    35149 2024-05-17 11:23:48.000000 pytransportnswv2-0.3.1/LICENSE
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5326 2024-05-20 22:06:34.798767 pytransportnswv2-0.3.1/PKG-INFO
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-20 22:06:34.798767 pytransportnswv2-0.3.1/PyTransportNSWv2.egg-info/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5326 2024-05-20 22:06:34.000000 pytransportnswv2-0.3.1/PyTransportNSWv2.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      279 2024-05-20 22:06:34.000000 pytransportnswv2-0.3.1/PyTransportNSWv2.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2024-05-20 22:06:34.000000 pytransportnswv2-0.3.1/PyTransportNSWv2.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       23 2024-05-20 22:06:34.000000 pytransportnswv2-0.3.1/PyTransportNSWv2.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       13 2024-05-20 22:06:34.000000 pytransportnswv2-0.3.1/PyTransportNSWv2.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4750 2024-05-20 22:04:42.000000 pytransportnswv2-0.3.1/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-20 22:06:34.794767 pytransportnswv2-0.3.1/TransportNSW/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    13395 2024-05-20 21:39:11.000000 pytransportnswv2-0.3.1/TransportNSW/TransportNSW.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       86 2024-05-17 11:22:12.000000 pytransportnswv2-0.3.1/TransportNSW/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2024-05-20 22:06:34.798767 pytransportnswv2-0.3.1/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      804 2024-05-20 22:06:00.000000 pytransportnswv2-0.3.1/setup.py
```

### Comparing `pytransportnswv2-0.3.0/LICENSE` & `pytransportnswv2-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransportnswv2-0.3.0/README.md` & `pytransportnswv2-0.3.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -4,56 +4,59 @@
 ## How to Use
 
 ### Get an API Key
 An OpenData account and API key is required to request the data. More information on how to create the free account can be found here:
 https://opendata.transport.nsw.gov.au/user-guide.  You need to register an application that needs both the Trip Planner and Realtime Vehicle Positions APIs
 
 ### Get the stop IDs
-The library needs the stop ID for the source and destination, and optionally how many minutes from now the departure should be.  The easiest way to get the stop ID is via https://transportnsw.info/stops#/. It provides the option to search for either a location or a specific platform, bus stop or ferry wharf.  Regardless of if you specify a general location for the origin or destination, the return information shows the stop_id for the actual arrival and destination platform, bus stop or ferry wharf.
+The function needs the stop IDs for the source and destination, and optionally how many minutes from now the departure should be, and if you want to filter trips by a specific transport type.  The easiest way to get the stop ID is via https://transportnsw.info/stops#/. It provides the option to search for either a location or a specific platform, bus stop or ferry wharf.  Regardless of if you specify a general location for the origin or destination, the return information shows the stop_id for the actual arrival and destination platform, bus stop or ferry wharf.
 
 If it's available, the general occupancy level and the latitude and longitude of the selected journey's vehicle (train, bus, etc) will be returned.
 
 ### API Documentation
 The source API details can be found here: https://opendata.transport.nsw.gov.au/sites/default/files/2023-08/Trip%20Planner%20API%20manual-opendataproduction%20v3.2.pdf
 
 ### Parameters
 ```python
-.get_trip(origin_stop_id, destination_stop_id, api_key, [trip_wait_time = 0])
+.get_trip(origin_stop_id, destination_stop_id, api_key, [trip_wait_time = 0], [transport_type = 0])
 ```
 
-TransportNSW's trip planner works much better if you use the general location IDs (eg Central Station) rather than a specific platform id (eg Central Station, Platform 19).  Forcing a specific platform sometimes results in much more complicated trips.
+TransportNSW's trip planner can work better if you use the general location IDs (eg Central Station) rather than a specific Stop ID (eg Central Station, Platform 19) for the destination, depending on the transport type.  Forcing a specific end destination sometimes results in much more complicated trips.  Also note that the API expects (and returns) the Stop IDs as strings, although so far they all appear to be numeric.
 
 ### Sample Code
-The following example will return the next trip from a bus stop in St. Ives to Central Station, without specifying a specific destination platform.
+
+The following example will return the next trip that starts from a bus stop in St. Ives (207537) five minutes from now, to Central Station's general stop ID (10101100):
 
 **Code:**
 ```python
 from TransportNSW import TransportNSW
 tnsw = TransportNSW()
-journey = tnsw.get_trip('207537', '10101100', 'YOUR_API_KEY')
+journey = tnsw.get_trip('207537', '10101100', 'YOUR_API_KEY', 5)
 print(journey)
 ```
 **Result:**
 ```python
-{'due': 23, 'origin_stop_id': '207537', 'origin_name': 'St Ives, Mona Vale Rd at Shinfield Ave', 'departure_time': '2020-06-28T10:10:00Z', 'destination_stop_id': '2000338', 'destination_name': 'Sydney, Central Station, Platform 18', 'arrival_time': '2020-06-28T11:02:00Z', 'origin_transport_type': 'Bus', 'origin_transport_name': 'Sydney Buses Network', 'origin_line_name': '195', 'origin_line_name_short': '195', 'changes': 1, 'occupancy': 'UNKNOWN', 'real_time_trip_id': '612993', 'latitude': 'n/a', 'longitude': 'n/a'}
+{"due": 3, "origin_stop_id": "207537", "origin_name": "Mona Vale Rd at Shinfield Ave, St Ives", "departure_time": "2024-05-20T21:59:48Z", "destination_stop_id": "2000338", "destination_name": "Central Station, Platform 18, Sydney", "arrival_time": "2024-05-20T22:47:36Z", "origin_transport_type": "Bus", "origin_transport_name": "Sydney Buses Network", "origin_line_name": "195", "origin_line_name_short": "195", "changes": 1, "occupancy": "MANY_SEATS", "real_time_trip_id": "2096551", "latitude": -33.72665786743164, "longitude": 151.16305541992188}
 ```
+Fun fact:  TransportNSW's raw API output calls itself JSON, but it uses single quotes for strings in defiance of the JSON standards.  When using this wrapper the output is formatted such that `jq`, for example, is happy with.
 
-* due: the time (in minutes) before the journey starts 
+* due: the time (in minutes) before the journey starts
 * origin_stop_id: the specific departure stop id
 * origin_name: the name of the departure location
-* departure_time: the departure time
+* departure_time: the departure time, in UTC
 * destination_stop_id: the specific destination stop id
 * destination_name: the name of the destination location
-* arrival_time: the arrival time at the origin
+* arrival_time: the planned arrival time at the origin, in UTC
 * origin_transport_type: the type of transport, eg train, bus, ferry etc
-* origin_transport_name: the full name of transport providere
+* origin_transport_name: the full name of the transport provider
 * origin_line_name & origin_line_name_short: the full and short names of the journey
-* changes: how many transport changes are needed
+* changes: how many transport changes are needed on the journey
 * occupancy: how full the vehicle is, if available
-* real_time_trip_id: the unique TransportNSW id for that specific journey
+* real_time_trip_id: the unique TransportNSW id for that specific journey, if available
 * latitude & longitude: The location of the vehicle, if available
 
-Please note that the origin and destination detail is just that.  We don't return any intermediate steps, transport change types etc other than the total number of changes.  The assumption is that you'll know the details of your specified trip, you just want to know when the next departure is.  If you need much more detailed information then I recommend that you use the full Transport NSW trip planner website or application.
+Please note that the origin and destination detail is just that - information about the first and last stops on the journey at the time the request was made.  We don't return any intermediate steps, transport change types etc other than the total number of changes - the assumption is that you'll know the details of your specified trip, you just want to know when the next departure is.  If you need much more detailed information then I recommend that you use the full Transport NSW trip planner website or application.
+Also note that the 'transport_type' filter, if present,  only makes sure that at least one leg of the journey includes that transport type.
 
 ## Thank you
 Thank you Dav0815 for your TransportNSW library that the vast majority of this fork is based on.  I couldn't have done it without you!
 https://github.com/Dav0815/TransportNSW
```

### Comparing `pytransportnswv2-0.3.0/TransportNSW/TransportNSW.py` & `pytransportnswv2-0.3.1/TransportNSW/TransportNSW.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from datetime import datetime, timedelta
 from google.transit import gtfs_realtime_pb2
 import requests.exceptions
 import requests
 import logging
 import re
+import json #For the output
 
 ATTR_DUE_IN = 'due'
 
 ATTR_ORIGIN_STOP_ID = 'origin_stop_id'
 ATTR_ORIGIN_NAME = 'origin_name'
 ATTR_DEPARTURE_TIME = 'departure_time'
 
@@ -127,14 +128,22 @@
         if transport_type == 0:
             # Just grab the first (and only) trip
             journey = result['journeys'][0]
         else:
             # Look for a trip with a matching class filter in at least one of its legs.  Could possibly be more stringent here, if ANY part of the journey fits the filter, it will be returned.
             journey = self.find_first_journey(result['journeys'], transport_type)
 
+        if journey is None:
+            logger.warning("No journey information returned")
+            return self.info
+
+        if journey['legs'] is None:
+            logger.warning("No journey information returned")
+            return self.info
+
         legs = journey['legs']
         first_leg = self.find_first_leg(legs, transport_type)
         last_leg = self.find_last_leg(legs, transport_type)
         changes = self.find_changes(legs, transport_type)
 
         origin = result['journeys'][0]['legs'][first_leg]['origin']
         # probably tidy this up when we start to get occupancy data back
@@ -164,16 +173,21 @@
         # RealTimeTripID info so we can try and get the current location later
         realtimetripid = 'n/a'
         if 'properties' in transportation:
             if 'RealtimeTripId' in transportation['properties']:
                 realtimetripid = transportation['properties']['RealtimeTripId']
 
         # Line info
-        origin_line_name_short = transportation['disassembledName']
-        origin_line_name = transportation['number']
+        origin_line_name_short = "unknown"
+        if 'disassembledName' in transportation:
+            origin_line_name_short = transportation['disassembledName']
+
+        origin_line_name = "unknown"
+        if 'number' in transportation:
+            origin_line_name = transportation['number']
 
         # Occupancy info, if it's there
         occupancy = 'UNKNOWN'
         if 'properties' in first_stop:
             if 'occupancy' in first_stop['properties']:
                 occupancy = first_stop['properties']['occupancy']
 
@@ -238,15 +252,15 @@
             ATTR_ORIGIN_LINE_NAME_SHORT : origin_line_name_short,
             ATTR_CHANGES: changes,
             ATTR_OCCUPANCY : occupancy,
             ATTR_REAL_TIME_TRIP_ID : realtimetripid,
             ATTR_LATITUDE : latitude,
             ATTR_LONGITUDE : longitude
             }
-        return self.info
+        return json.dumps(self.info)
 
     def find_first_journey(self, journeys, journeytype):
         # Find the first journey whose first leg is of the requested type
         journey_count = len(journeys)
         for journey in range (0, journey_count, 1):
             leg = self.find_first_leg(journeys[journey]['legs'], journeytype)
             if leg is not None:
```

### Comparing `pytransportnswv2-0.3.0/setup.py` & `pytransportnswv2-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyTransportNSWv2",
-    version="0.3.0",
+    version="0.3.1",
     author="andystewart999",
     description="Get detailed per-trip transport information from TransportNSW",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andystewart999/TransportNSW",
     packages=setuptools.find_packages(),
     install_requires=[
```

