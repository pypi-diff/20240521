# Comparing `tmp/nodens_gateway-24.5.2a0.tar.gz` & `tmp/nodens_gateway-24.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodens_gateway-24.5.2a0.tar", last modified: Tue May 21 16:24:39 2024, max compression
+gzip compressed data, was "nodens_gateway-24.5.3.tar", last modified: Tue May 21 17:39:58 2024, max compression
```

## Comparing `nodens_gateway-24.5.2a0.tar` & `nodens_gateway-24.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.790323 nodens_gateway-24.5.2a0/
--rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.2a0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.2a0/MANIFEST.in
--rw-rw-rw-   0        0        0     4328 2024-05-21 16:24:39.767828 nodens_gateway-24.5.2a0/PKG-INFO
--rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.2a0/README.md
--rw-rw-rw-   0        0        0      819 2024-05-21 16:23:24.000000 nodens_gateway-24.5.2a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 16:24:39.791271 nodens_gateway-24.5.2a0/setup.cfg
--rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.2a0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.216928 nodens_gateway-24.5.2a0/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.194227 nodens_gateway-24.5.2a0/src/nodens/
-drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.518635 nodens_gateway-24.5.2a0/src/nodens/gateway/
--rw-rw-rw-   0        0        0    13492 2024-05-21 16:23:30.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/__init__.py
--rw-rw-rw-   0        0        0     8583 2024-05-21 13:43:36.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/__main__.py
--rw-rw-rw-   0        0        0    86284 2024-05-21 16:23:09.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_fns.py
--rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_insight_hub.py
--rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_mesh.py
--rw-rw-rw-   0        0        0    25387 2024-05-21 14:23:09.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_serv.py
--rw-rw-rw-   0        0        0    11078 2024-05-21 12:58:30.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_thingsboard.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.754935 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/
--rw-rw-rw-   0        0        0     4328 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/PKG-INFO-Hawk
--rw-rw-rw-   0        0        0      640 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/requires-Hawk.txt
--rw-rw-rw-   0        0        0       70 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 17:39:58.597991 nodens_gateway-24.5.3/
+-rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4326 2024-05-21 17:39:58.588269 nodens_gateway-24.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.3/README.md
+-rw-rw-rw-   0        0        0      817 2024-05-21 17:39:00.000000 nodens_gateway-24.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 17:39:58.599017 nodens_gateway-24.5.3/setup.cfg
+-rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:39:58.181424 nodens_gateway-24.5.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 17:39:58.176436 nodens_gateway-24.5.3/src/nodens/
+drwxrwxrwx   0        0        0        0 2024-05-21 17:39:58.333990 nodens_gateway-24.5.3/src/nodens/gateway/
+-rw-rw-rw-   0        0        0    13490 2024-05-21 17:38:59.000000 nodens_gateway-24.5.3/src/nodens/gateway/__init__.py
+-rw-rw-rw-   0        0        0     8583 2024-05-21 13:43:36.000000 nodens_gateway-24.5.3/src/nodens/gateway/__main__.py
+-rw-rw-rw-   0        0        0    86289 2024-05-21 16:58:21.000000 nodens_gateway-24.5.3/src/nodens/gateway/nodens_fns.py
+-rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.3/src/nodens/gateway/nodens_insight_hub.py
+-rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.3/src/nodens/gateway/nodens_mesh.py
+-rw-rw-rw-   0        0        0    25953 2024-05-21 16:58:37.000000 nodens_gateway-24.5.3/src/nodens/gateway/nodens_serv.py
+-rw-rw-rw-   0        0        0    11052 2024-05-21 17:00:26.000000 nodens_gateway-24.5.3/src/nodens/gateway/nodens_thingsboard.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:39:58.581670 nodens_gateway-24.5.3/src/nodens_gateway.egg-info/
+-rw-rw-rw-   0        0        0     4326 2024-05-21 17:39:58.000000 nodens_gateway-24.5.3/src/nodens_gateway.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.3/src/nodens_gateway.egg-info/PKG-INFO-Hawk
+-rw-rw-rw-   0        0        0      640 2024-05-21 17:39:58.000000 nodens_gateway-24.5.3/src/nodens_gateway.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 17:39:58.000000 nodens_gateway-24.5.3/src/nodens_gateway.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-21 17:39:58.000000 nodens_gateway-24.5.3/src/nodens_gateway.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.3/src/nodens_gateway.egg-info/requires-Hawk.txt
+-rw-rw-rw-   0        0        0       70 2024-05-21 17:39:58.000000 nodens_gateway-24.5.3/src/nodens_gateway.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 17:39:58.000000 nodens_gateway-24.5.3/src/nodens_gateway.egg-info/top_level.txt
```

### Comparing `nodens_gateway-24.5.2a0/LICENSE` & `nodens_gateway-24.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2a0/PKG-INFO` & `nodens_gateway-24.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.2a0
+Version: 24.5.3
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.2a0/README.md` & `nodens_gateway-24.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2a0/pyproject.toml` & `nodens_gateway-24.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodens-gateway"
-version = "24.5.2.a"
+version = "24.5.3"
 description = "Run the NodeNs gateway"
 readme = "README.md"
 authors = [{ name = "Khalid Z Rajab", email = "khalid@nodens.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `nodens_gateway-24.5.2a0/src/nodens/gateway/__init__.py` & `nodens_gateway-24.5.3/src/nodens/gateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 global APPNAME
 global APPAUTHOR
 global CWD
 
 # Some information
 __title__ = "nodens-gateway"
-__version__ = "24.5.2.a"
+__version__ = "24.5.3"
 __author__ = "Khalid Z Rajab"
 __author_email__ = "khalid@nodens.eu"
 __copyright__ = "Copyright (c) 2024 " + __author__
 __license__ = "MIT"
 
 APPNAME = "Gateway"
 APPAUTHOR = "NodeNs"
```

### Comparing `nodens_gateway-24.5.2a0/src/nodens/gateway/__main__.py` & `nodens_gateway-24.5.3/src/nodens/gateway/__main__.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_fns.py` & `nodens_gateway-24.5.3/src/nodens/gateway/nodens_fns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1793,15 +1793,15 @@
         self.presence = PresenceDetect()
 
     def update(self, version, data, Nud):
         if (version == 3):
             hl = 48
         self.packet_len = data[12] + 256*data[13]
         if len(data) < self.packet_len:
-            print("WARNING: Rx data size is smaller than expected. Expected: {}. Received: {}.".format(self.packet_len, len(data)))
+            nodens.logger.debug("Rx data size is smaller than expected. Expected: {}. Received: {}.".format(self.packet_len, len(data)))
             self.packet_len = len(data)
         self.num_tlv = data[44]
         self.frame = convert_4_to_1(data[20:24])
         j = hl
         flag_track = False
         flag_pc = False
         while (j < self.packet_len):
```

### Comparing `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_insight_hub.py` & `nodens_gateway-24.5.3/src/nodens/gateway/nodens_insight_hub.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_mesh.py` & `nodens_gateway-24.5.3/src/nodens/gateway/nodens_mesh.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_serv.py` & `nodens_gateway-24.5.3/src/nodens/gateway/nodens_serv.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,29 +163,34 @@
                 heartbeat = "\r" + heartbeat
                 #print(heartbeat, end='')
                 mqttDataTemp = [T.strftime("%H:%M:%S")]
                 mqttDataTemp.append(mqttData['addr'])
                 mqttDataTemp.append(mqttData['data'])
                 mqttData_SAVEFull.append(mqttDataTemp)
 
+                temp_current_occupants = []
                 try:
                     if ndns_fns.sd.track.num_tracks > 0:
                         for idx, track in enumerate(ndns_fns.sd.track.tid):
+                            temp_current_occupants.append(track)
                             ndns_fns.oh.update(mqttData['addr'],track,ndns_fns.sd.track.X[idx],ndns_fns.sd.track.Y[idx],ndns_fns.sd)
                     ndns_fns.oh.sensor_activity(mqttData['addr'])
                 except Exception as e:
                     pass
 
                 # Update time period occupancy data
                 if mqttData['addr'] not in ndns_fns.ew.id:
                     ndns_fns.ew.update(mqttData['addr'])
                 send_idx_e = ndns_fns.ew.id.index(mqttData['addr'])
 
                 ndns_fns.si.update_refresh(sen_idx, send_idx_e, T, ndns_fns.ew)
 
+                # Mark for deletion tracks which have left
+                ndns_fns.oh.delete_track(mqttData['addr'], temp_current_occupants, mark_to_delete=1)
+
                 #TODO: check cloud update
                 if ((T - ndns_fns.si.period_t[sen_idx]).total_seconds() > nodens.cp.CLOUD_WRITE_TIME):
                     # Calculate occupant history outputs
                     ndns_fns.oh.calculate_outputs()
 
                     mqttTime = json.loads("{\"Time\": \"" + str(T) + "\"}")
                     mqttClass = json.loads("{\"Activity detected\": \"" + str(int(ndns_fns.class_eng.activity_alert))
@@ -298,35 +303,40 @@
                     
 
                     # # Update max number of occupants
                     # if (ndns_fns.si.num_occ[sen_idx] > ndns_fns.si.max_occ[sen_idx]):
                     #     ndns_fns.si.max_occ[sen_idx] = ndns_fns.si.num_occ[sen_idx]
 
                     # If there are occupants, what are their locations?
+                    temp_current_occupants = []
                     if (ndns_fns.si.num_occ[sen_idx] > 0):        # NodeNs KZR FIX : need to update so oh processes when num_occ=0
                         try:
                             occ_info = mqttDataFinal['Occupancy Info']
                         except:
                             occ_info = mqttDataFinal['Occupancy Info'][0]
                         # nodens.logger.debug('OCCUPANCY INFO')
 
                         # Update occupancy history and entryways for each occupant
                         for i in range(len(occ_info)):      # NodeNs KZR FIX: update ESP to create new payload
                             temp = occ_info[i]
+                            temp_current_occupants.append(temp['Occupant ID'])
                             ndns_fns.oh.update(mqttData['addr'],temp['Occupant ID'],temp['X'],temp['Y'])
                             # Check if occupant has crossed entryway
                             ndns_fns.oh.entryway(mqttData['addr'],temp['Occupant ID'], ndns_fns.ew)
                             # nodens.logger.debug('Occupant no.: {}. X: {}. Y = {}.'.format(temp['Occupant ID'],temp['X'],temp['Y']))
 
                         # Look at general activity stats
                         ndns_fns.oh.sensor_activity(mqttData['addr'])
                     else:
                         ndns_fns.oh.update(mqttData['addr'])
                         ndns_fns.oh.sensor_activity(mqttData['addr'])
 
+                    # Mark for deletion tracks which have left
+                    ndns_fns.oh.delete_track(mqttData['addr'], temp_current_occupants, mark_to_delete=1)
+
                     # Update time period occupancy data
                     if mqttData['addr'] not in ndns_fns.ew.id:
                         ndns_fns.ew.update(mqttData['addr'])
                     send_idx_e = ndns_fns.ew.id.index(mqttData['addr'])
 
                     ndns_fns.si.update_refresh(sen_idx, send_idx_e, T, ndns_fns.ew)
```

### Comparing `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_thingsboard.py` & `nodens_gateway-24.5.3/src/nodens/gateway/nodens_thingsboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,14 @@
         global FLAG_TX_IN_PROGRESS
 
         try:
             while FLAG_TX_IN_PROGRESS == 1:
                 sleep(0.1)
             FLAG_TX_IN_PROGRESS = 1
             for i in range(len(self.subscribed_sensors)):
-                print(i)
                 self.client_sub[i].loop_stop()
                 self.client_sub[i].disconnect()
                 self.client_sub[i].unsubscribe('#')
             s_idx = self.sensor_id.index(sensor_id)
             username = self.access_token[s_idx]
             self.client.username_pw_set(username)
             TB_CONNECT = 0
```

### Comparing `nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/PKG-INFO` & `nodens_gateway-24.5.3/src/nodens_gateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.2a0
+Version: 24.5.3
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/PKG-INFO-Hawk` & `nodens_gateway-24.5.3/src/nodens_gateway.egg-info/PKG-INFO-Hawk`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/SOURCES.txt` & `nodens_gateway-24.5.3/src/nodens_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

