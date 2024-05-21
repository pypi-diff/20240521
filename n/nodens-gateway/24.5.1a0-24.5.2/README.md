# Comparing `tmp/nodens_gateway-24.5.1a0.tar.gz` & `tmp/nodens_gateway-24.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodens_gateway-24.5.1a0.tar", last modified: Tue May 21 15:10:17 2024, max compression
+gzip compressed data, was "nodens_gateway-24.5.2.tar", last modified: Tue May 21 15:58:35 2024, max compression
```

## Comparing `nodens_gateway-24.5.1a0.tar` & `nodens_gateway-24.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 15:10:17.867598 nodens_gateway-24.5.1a0/
--rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.1a0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.1a0/MANIFEST.in
--rw-rw-rw-   0        0        0     4328 2024-05-21 15:10:17.859603 nodens_gateway-24.5.1a0/PKG-INFO
--rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.1a0/README.md
--rw-rw-rw-   0        0        0      819 2024-05-21 13:17:05.000000 nodens_gateway-24.5.1a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 15:10:17.868597 nodens_gateway-24.5.1a0/setup.cfg
--rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.1a0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:10:17.310962 nodens_gateway-24.5.1a0/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:10:17.307964 nodens_gateway-24.5.1a0/src/nodens/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:10:17.632429 nodens_gateway-24.5.1a0/src/nodens/gateway/
--rw-rw-rw-   0        0        0    13492 2024-05-21 13:40:23.000000 nodens_gateway-24.5.1a0/src/nodens/gateway/__init__.py
--rw-rw-rw-   0        0        0     8583 2024-05-21 13:43:36.000000 nodens_gateway-24.5.1a0/src/nodens/gateway/__main__.py
--rw-rw-rw-   0        0        0    85301 2024-05-21 15:09:04.000000 nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_fns.py
--rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_insight_hub.py
--rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_mesh.py
--rw-rw-rw-   0        0        0    25387 2024-05-21 14:23:09.000000 nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_serv.py
--rw-rw-rw-   0        0        0    11078 2024-05-21 12:58:30.000000 nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_thingsboard.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:10:17.853052 nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/
--rw-rw-rw-   0        0        0     4328 2024-05-21 15:10:17.000000 nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/PKG-INFO-Hawk
--rw-rw-rw-   0        0        0      640 2024-05-21 15:10:17.000000 nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 15:10:17.000000 nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-21 15:10:17.000000 nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/requires-Hawk.txt
--rw-rw-rw-   0        0        0       70 2024-05-21 15:10:17.000000 nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 15:10:17.000000 nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.611402 nodens_gateway-24.5.2/
+-rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.2/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4326 2024-05-21 15:58:35.606017 nodens_gateway-24.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.2/README.md
+-rw-rw-rw-   0        0        0      817 2024-05-21 15:57:40.000000 nodens_gateway-24.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:58:35.612410 nodens_gateway-24.5.2/setup.cfg
+-rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.370823 nodens_gateway-24.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.368822 nodens_gateway-24.5.2/src/nodens/
+drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.444689 nodens_gateway-24.5.2/src/nodens/gateway/
+-rw-rw-rw-   0        0        0    13490 2024-05-21 15:57:30.000000 nodens_gateway-24.5.2/src/nodens/gateway/__init__.py
+-rw-rw-rw-   0        0        0     8583 2024-05-21 13:43:36.000000 nodens_gateway-24.5.2/src/nodens/gateway/__main__.py
+-rw-rw-rw-   0        0        0    86570 2024-05-21 15:56:35.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_fns.py
+-rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_insight_hub.py
+-rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_mesh.py
+-rw-rw-rw-   0        0        0    25387 2024-05-21 14:23:09.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_serv.py
+-rw-rw-rw-   0        0        0    11078 2024-05-21 12:58:30.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_thingsboard.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.599072 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/
+-rw-rw-rw-   0        0        0     4326 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/PKG-INFO-Hawk
+-rw-rw-rw-   0        0        0      640 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/requires-Hawk.txt
+-rw-rw-rw-   0        0        0       70 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/top_level.txt
```

### Comparing `nodens_gateway-24.5.1a0/LICENSE` & `nodens_gateway-24.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.1a0/PKG-INFO` & `nodens_gateway-24.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.1a0
+Version: 24.5.2
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.1a0/README.md` & `nodens_gateway-24.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.1a0/pyproject.toml` & `nodens_gateway-24.5.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodens-gateway"
-version = "24.5.1.a"
+version = "24.5.2"
 description = "Run the NodeNs gateway"
 readme = "README.md"
 authors = [{ name = "Khalid Z Rajab", email = "khalid@nodens.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `nodens_gateway-24.5.1a0/src/nodens/gateway/__init__.py` & `nodens_gateway-24.5.2/src/nodens/gateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 global APPNAME
 global APPAUTHOR
 global CWD
 
 # Some information
 __title__ = "nodens-gateway"
-__version__ = "24.5.1.a"
+__version__ = "24.5.2"
 __author__ = "Khalid Z Rajab"
 __author_email__ = "khalid@nodens.eu"
 __copyright__ = "Copyright (c) 2024 " + __author__
 __license__ = "MIT"
 
 APPNAME = "Gateway"
 APPAUTHOR = "NodeNs"
```

### Comparing `nodens_gateway-24.5.1a0/src/nodens/gateway/__main__.py` & `nodens_gateway-24.5.2/src/nodens/gateway/__main__.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_fns.py` & `nodens_gateway-24.5.2/src/nodens/gateway/nodens_fns.py`

 * *Files 2% similar despite different names*

```diff
@@ -844,14 +844,17 @@
         self.room_heatmap = [] # Room heatmap showing occupancy positions
 
         # Gait parameters
         self.gait_params = []
 
         # Prepare outputs
         self.outputs = []
+
+        # List of tracks to delete
+        self.track_del_flag = []
         
     # Use this to refresh the histories
     def refresh(self, sensor_id):
         # Check for this specific sensor
         ind_s = self.sensor_id.index(sensor_id)
 
         self.id[ind_s] = [] 
@@ -935,28 +938,14 @@
         self.x1[ind_s].append(X)
         self.y1[ind_s].append(Y)
 
         self.tot_dist[ind_s].append(0)
         self.max_dist[ind_s].append(0)
         self.flag_active[ind_s].append(1)   # By default mark them as active
         self.time_inactive_start[ind_s].append(dt.datetime.now(dt.timezone.utc))
-
-        # else:
-        #     # self.id.append([track_id])
-        #     self.id[ind_s].append(track_id)
-
-        #     self.x0.append([X])
-        #     self.y0.append([Y])
-        #     self.x1.append([X])
-        #     self.y1.append([Y])
-
-        #     self.tot_dist.append([0])
-        #     self.max_dist.append([0])
-        #     self.flag_active.append([1])    # By default mark them as active
-        #     self.time_inactive_start.append([dt.datetime.now(dt.timezone.utc)])
         
         ind_t = self.id[ind_s].index(track_id)
         if ind_t > self.xh.shape[1]-1:
             new_track = np.empty((self.xh.shape[0],self.xh.shape[1],self.num_hist_frames),dtype=object)
             self.xh = np.concatenate((self.xh,new_track),axis=1)
             self.yh = np.concatenate((self.yh,new_track),axis=1)
         self.xh[ind_s][ind_t][0] = X
@@ -991,20 +980,55 @@
         self.y1.append([])
 
         self.tot_dist.append([])
         self.max_dist.append([])
         self.flag_active.append([])    # By default mark them as active
         self.time_inactive_start.append([])
 
+        self.track_del_flag.append([])
+
         # Room heatmap
         self.room_heatmap.append(OccupantHeatmap(sensor_id, Xres=0.25, Yres=0.25, Xrange=[-4.5,4.5], Yrange=[0,5]))
 
         # Gait parameters
         self.gait_params.append(GaitParameters(sensor_id, num_hist_frames=self.num_hist_frames))
 
+    # Procedure to delete a track when it has left
+    def delete_track(self,sensor_id,track_id, mark_to_delete=1):
+        """This function can be used to specific tracks, or to mark them for deletion
+        mark_to_delete=1. track_id is all *safe* tracks (i.e. tracks to keep); typically done by inputting an array of current tracks.
+        mark_to_delete=0. track_id is the track to delete."""
+
+        ind_s = self.sensor_id.index(sensor_id)
+
+        if mark_to_delete == 1:
+            for track in self.id[ind_s]:
+                if track not in track_id:
+                    self.track_del_flag[ind_s].append(track)
+        else:
+            ind_t = self.id[ind_s].index(track_id)
+
+            self.x0[ind_s].pop(ind_t)
+            self.y0[ind_s].pop(ind_t)
+            self.x1[ind_s].pop(ind_t)
+            self.y1[ind_s].pop(ind_t)
+
+            self.tot_dist[ind_s].pop(ind_t)
+            self.max_dist[ind_s].pop(ind_t)
+            self.flag_active[ind_s].pop(ind_t)   # By default mark them as active
+            self.time_inactive_start[ind_s].pop(ind_t)
+            
+            self.xh = np.delete(self.xh, ind_t, axis=1)
+            self.yh = np.delete(self.yh, ind_t, axis=1)
+
+            self.track_del_flag[ind_s].pop(track_id)
+            self.id[ind_s].pop(track_id)
+
+            # Delete gait params
+            self.gait_params[ind_s].delete_track(sensor_id, track_id)
     
     # Use this to check entryways and see if anyone has entered/left the room
     def entryway(self, sensor_id, track_id, ew):
         if (sensor_id in ew.id):
             ind_s = self.sensor_id.index(sensor_id)
             ind_e = ew.id.index(sensor_id)
             ind_t = self.id[ind_s].index(track_id)
@@ -1126,14 +1150,18 @@
             pc_e = [val for val in self.e_pc_h[idx] if val is not None]
             self.outputs[idx].pc_energy = sum(pc_e)
             
             # Room heatmaps
             self.room_heatmap[idx].prepare_heatmap_string()
             self.outputs[idx].heatmap_string = self.room_heatmap[idx].heatmap_string
 
+            # Delete tracks which have left
+            for ind_t, track in enumerate(self.id[idx]):
+                if track in self.track_del_flag[idx]:
+                    self.delete_track(sensor,track,mark_to_delete=0)
 
 
     
     # Class to define outputs
     class Outputs:
         def __init__(self) -> None:
             self.sensor_id = []
```

### Comparing `nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_insight_hub.py` & `nodens_gateway-24.5.2/src/nodens/gateway/nodens_insight_hub.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_mesh.py` & `nodens_gateway-24.5.2/src/nodens/gateway/nodens_mesh.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_serv.py` & `nodens_gateway-24.5.2/src/nodens/gateway/nodens_serv.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.1a0/src/nodens/gateway/nodens_thingsboard.py` & `nodens_gateway-24.5.2/src/nodens/gateway/nodens_thingsboard.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/PKG-INFO` & `nodens_gateway-24.5.2/src/nodens_gateway.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.1a0
+Version: 24.5.2
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/PKG-INFO-Hawk` & `nodens_gateway-24.5.2/src/nodens_gateway.egg-info/PKG-INFO-Hawk`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.1a0/src/nodens_gateway.egg-info/SOURCES.txt` & `nodens_gateway-24.5.2/src/nodens_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

