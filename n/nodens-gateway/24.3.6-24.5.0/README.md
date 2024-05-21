# Comparing `tmp/nodens-gateway-24.3.6.tar.gz` & `tmp/nodens_gateway-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodens-gateway-24.3.6.tar", last modified: Sun Mar  3 13:07:22 2024, max compression
+gzip compressed data, was "nodens_gateway-24.5.0.tar", last modified: Tue May 21 12:46:02 2024, max compression
```

## Comparing `nodens-gateway-24.3.6.tar` & `nodens_gateway-24.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-03 13:07:22.241371 nodens-gateway-24.3.6/
--rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens-gateway-24.3.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens-gateway-24.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4326 2024-03-03 13:07:22.241371 nodens-gateway-24.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens-gateway-24.3.6/README.md
--rw-rw-rw-   0        0        0      817 2024-03-03 13:07:00.000000 nodens-gateway-24.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-03 13:07:22.241371 nodens-gateway-24.3.6/setup.cfg
--rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens-gateway-24.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-03 13:07:22.022889 nodens-gateway-24.3.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-03 13:07:22.022889 nodens-gateway-24.3.6/src/nodens/
-drwxrwxrwx   0        0        0        0 2024-03-03 13:07:22.145936 nodens-gateway-24.3.6/src/nodens/gateway/
--rw-rw-rw-   0        0        0    13316 2024-03-03 13:06:56.000000 nodens-gateway-24.3.6/src/nodens/gateway/__init__.py
--rw-rw-rw-   0        0        0     8677 2024-03-02 16:51:04.000000 nodens-gateway-24.3.6/src/nodens/gateway/__main__.py
--rw-rw-rw-   0        0        0    75720 2024-03-03 13:06:40.000000 nodens-gateway-24.3.6/src/nodens/gateway/nodens_fns.py
--rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens-gateway-24.3.6/src/nodens/gateway/nodens_insight_hub.py
--rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens-gateway-24.3.6/src/nodens/gateway/nodens_mesh.py
--rw-rw-rw-   0        0        0    24418 2024-03-03 10:35:09.000000 nodens-gateway-24.3.6/src/nodens/gateway/nodens_serv.py
--rw-rw-rw-   0        0        0    10508 2024-03-03 13:06:02.000000 nodens-gateway-24.3.6/src/nodens/gateway/nodens_thingsboard.py
-drwxrwxrwx   0        0        0        0 2024-03-03 13:07:22.241371 nodens-gateway-24.3.6/src/nodens_gateway.egg-info/
--rw-rw-rw-   0        0        0     4326 2024-03-03 13:07:21.000000 nodens-gateway-24.3.6/src/nodens_gateway.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens-gateway-24.3.6/src/nodens_gateway.egg-info/PKG-INFO-Hawk
--rw-rw-rw-   0        0        0      640 2024-03-03 13:07:22.000000 nodens-gateway-24.3.6/src/nodens_gateway.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-03 13:07:21.000000 nodens-gateway-24.3.6/src/nodens_gateway.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-03-03 13:07:21.000000 nodens-gateway-24.3.6/src/nodens_gateway.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens-gateway-24.3.6/src/nodens_gateway.egg-info/requires-Hawk.txt
--rw-rw-rw-   0        0        0       70 2024-03-03 13:07:21.000000 nodens-gateway-24.3.6/src/nodens_gateway.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-03 13:07:21.000000 nodens-gateway-24.3.6/src/nodens_gateway.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.806703 nodens_gateway-24.5.0/
+-rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4326 2024-05-21 12:46:02.796864 nodens_gateway-24.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.0/README.md
+-rw-rw-rw-   0        0        0      817 2024-05-21 12:44:51.000000 nodens_gateway-24.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 12:46:02.809255 nodens_gateway-24.5.0/setup.cfg
+-rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.407829 nodens_gateway-24.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.405465 nodens_gateway-24.5.0/src/nodens/
+drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.549810 nodens_gateway-24.5.0/src/nodens/gateway/
+-rw-rw-rw-   0        0        0    13316 2024-05-21 12:44:58.000000 nodens_gateway-24.5.0/src/nodens/gateway/__init__.py
+-rw-rw-rw-   0        0        0     8677 2024-03-02 16:51:04.000000 nodens_gateway-24.5.0/src/nodens/gateway/__main__.py
+-rw-rw-rw-   0        0        0    84960 2024-05-21 10:54:01.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_fns.py
+-rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_insight_hub.py
+-rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_mesh.py
+-rw-rw-rw-   0        0        0    25146 2024-05-21 10:51:38.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_serv.py
+-rw-rw-rw-   0        0        0    10888 2024-05-21 10:52:10.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_thingsboard.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.789179 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/
+-rw-rw-rw-   0        0        0     4326 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/PKG-INFO-Hawk
+-rw-rw-rw-   0        0        0      640 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/requires-Hawk.txt
+-rw-rw-rw-   0        0        0       70 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/top_level.txt
```

### Comparing `nodens-gateway-24.3.6/LICENSE` & `nodens_gateway-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodens-gateway-24.3.6/PKG-INFO` & `nodens_gateway-24.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.3.6
+Version: 24.5.0
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens-gateway-24.3.6/README.md` & `nodens_gateway-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nodens-gateway-24.3.6/pyproject.toml` & `nodens_gateway-24.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodens-gateway"
-version = "24.3.6"
+version = "24.5.0"
 description = "Run the NodeNs gateway"
 readme = "README.md"
 authors = [{ name = "Khalid Z Rajab", email = "khalid@nodens.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `nodens-gateway-24.3.6/src/nodens/gateway/__init__.py` & `nodens_gateway-24.5.0/src/nodens/gateway/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 global APPNAME
 global APPAUTHOR
 global CWD
 
 # Some information
 __title__ = "nodens-gateway"
-__version__ = "24.3.6"
+__version__ = "24.5.0"
 __author__ = "Khalid Z Rajab"
 __author_email__ = "khalid@nodens.eu"
 __copyright__ = "Copyright (c) 2024 " + __author__
 __license__ = "MIT"
 
 APPNAME = "Gateway"
 APPAUTHOR = "NodeNs"
```

### Comparing `nodens-gateway-24.3.6/src/nodens/gateway/__main__.py` & `nodens_gateway-24.5.0/src/nodens/gateway/__main__.py`

 * *Files identical despite different names*

### Comparing `nodens-gateway-24.3.6/src/nodens/gateway/nodens_fns.py` & `nodens_gateway-24.5.0/src/nodens/gateway/nodens_fns.py`

 * *Files 4% similar despite different names*

```diff
@@ -613,20 +613,205 @@
 
     def update(self,new_id):
         self.id.append(new_id) # Add a new sensor
         self.x.append([])
         self.y.append([])
         self.count.append(0)
 
+# Heatmap class #
+class OccupantHeatmap:
+    # TODO: Set heatmap extent from radar config (requires scanning sensor config)
+    def __init__(self, sensor_id, Xres=1, Yres=[], Xrange=[-3,3], Yrange=[0,5]):
+        self.sensor_id = sensor_id
+        self.Xres = Xres
+
+        if Yres == []:
+            Yres = Xres
+        
+        self.Yres = Yres
+
+        self.Xrange = Xrange
+        self.Yrange = Yrange
+
+        Xn = np.ceil(Xrange[1]/Xres)-np.floor(Xrange[0]/Xres)
+        Yn = np.ceil(Yrange[1]/Yres)-np.floor(Yrange[0]/Yres)
+        self.heatmap = np.zero((Xn,Yn))
+        self.heatmap_string = ""
+
+    def reset_heatmap(self):
+        self.heatmap = 0*self.heatmap
+        self.heatmap_string = ""
+    
+    def update_heatmap(self, X, Y):
+        #for i in range(track.num_tracks):
+        try:
+            # X index of track
+            Xi = np.floor((X - self.Xrange[0])/self.Xres)
+            # Y index of track
+            Yi = np.floor((Y - self.Yrange[0])/self.Yres)
+            # Iterate heatmap
+            if (Xi>=0) & (Xi<np.size(self.heatmap,0)):
+                if (Yi>=0) & (Yi<np.size(self.heatmap,1)):
+                    self.heatmap[Xi,Yi] += 1
+        except Exception as e:
+            nodens.logger.warning(f"OccupantHeatmap.update_heatmap: {e}")
+
+    def prepare_heatmap_string(self):
+        string = ""
+        try:
+            for x in self.heatmap:
+                for y in x:
+                    string += chr(int(y))
+        except Exception as e:
+            nodens.logger.warning(f"OccupantHeatmap.heatmap_string: {e}")
+
+        # Base64 encoding. Could compress this by storing multiple pixels per character
+        try:
+            bytes_value = string.encode()
+            self.heatmap_string = base64.b64encode(bytes_value).decode()
+        except Exception as e:
+            nodens.logger.warning(f"OccupantHeatmap.heatmap_string: {e}")
+
+# Gait calculation #
+class GaitParameters:
+    def __init__(self, sensor_id, num_hist_frames=250, num_window_frames=4):
+        """This class records gait parameters for all tracks under a single sensor"""
+        self.sensor_id = sensor_id
+        self.track_id = []      # Record of all track ids for this sensor
+
+        self.track_gait_params = []
+        self.gait_str = ""
+
+        self.num_hist_frames = num_hist_frames
+        self.num_window_frames = num_window_frames
+
+    class TrackGait:
+        """This subclass records gait parameters for a single track"""
+        def __init__(self, sensor_id, track_id, num_hist_frames=250, num_window_frames=4, 
+                     gait_bins = [[20,0.1], [2,0.25]]):
+            self.sensor_id = sensor_id
+            self.track_id = track_id
+            self.n_window = 0
+            self.num_hist_frames = num_hist_frames
+            self.num_window_frames = num_window_frames
+
+            self.x0 = []    # previous
+            self.y0 = []
+            self.x1 = []    # current
+            self.y1 = []
+
+            self.speed = []
+            num_gait_bins = 2   # 0 and above max
+            self.gait_bins = gait_bins[0][1]
+            for vals in gait_bins:
+                if len(vals) == 2:
+                    num_gait_bins += vals[0]
+                    for i in range(vals[0]):
+                        self.gait_bins.append(self.gait_bins[-1] + vals[1])
+                else:
+                    nodens.logger.warning(f"gait bin value {vals} should be a 2-pul, [num_bins, bin_size]")
+
+            self.gait = [] # np.zeros((num_gait_bins))
+
+        def update(self, track_id, Xh, Yh):
+            if track_id == self.track_id:
+                self.n_window += 1
+                
+                if self.n_window >= self.num_window_frames:
+                    self.x0 = self.x1
+                    self.y0 = self.y1
+
+                    self.x1 = np.mean(Xh[0:self.num_window_frames])
+                    self.y1 = np.mean(Yh[0:self.num_window_frames])
+
+                    if (self.x0 != []) & (self.y0 != []):
+                        self.speed.append(np.sqrt((self.x1-self.x0)**2 + (self.y1-self.y0)**2))
+                    self.n_window = 0
+            else:
+                nodens.logger.warning(f"TrackGait.update. Track id: {track_id} does not match {self.track_id} for sensor: {self.sensor_id}")
+
+        def reset(self):
+            self.__init__(self.sensor_id, self.track_id, self.num_hist_frames, self.num_window_frames)
+            # self.n_window = 0
+
+            # self.x0 = []    # previous
+            # self.y0 = []
+            # self.x1 = []    # current
+            # self.y1 = []
+
+            # self.speed = []
+            # self.num_values = 0
+
+    def add_new_sensor(self, sensor_id):
+        self.sensor_id = sensor_id
+        self.track_id = [] 
+        self.track_gait_params = []
+
+    def add_new_track(self, sensor_id, track_id, Xh, Yh):
+        if sensor_id == self.sensor_id:
+            self.track_id.append(track_id)
+            self.track_gait_params.append(self.TrackGait(self.sensor_id, track_id, num_hist_frames=self.num_hist_frames, num_window_frames=self.num_window_frames))
+
+            self.track_gait_params[-1].update(track_id, Xh, Yh)
+        else:
+            nodens.logger.warning(f"GaitParameters.add_new_track. Sensor id: {sensor_id} does not match {self.sensor_id}")
+
+    def update_track(self, sensor_id, track_id, Xh, Yh):
+        if sensor_id == self.sensor_id:
+            ind_t = self.track_id.index(track_id)
+
+            self.track_gait_params[ind_t].update(track_id)
+        else:
+            nodens.logger.warning(f"GaitParameters.update_track. Sensor id: {sensor_id} does not match {self.sensor_id}")
+
+    def delete_track(self, sensor_id, track_id):
+        if sensor_id == self.sensor_id:
+            ind_t = self.track_id.index(track_id)
+
+            self.track_id.pop(ind_t)
+            self.track_gait_params.pop(ind_t)
+        else:
+            nodens.logger.warning(f"GaitParameters.delete_track. Sensor id: {sensor_id} does not match {self.sensor_id}")
+
+    def reset_tracks(self, sensor_id, track_id=[]):
+        if sensor_id == self.sensor_id:
+            if track_id == []:
+                for track_gaits in self.track_gait_params:
+                    track_gaits.reset()
+
+            else:
+                ind_t = self.track_id.index(track_id)
+                self.track_gait_params[ind_t].reset()
+        else:
+            nodens.logger.warning(f"GaitParameters.reset_tracks. Sensor id: {sensor_id} does not match {self.sensor_id}")
+
+
+    def calculate_gait_parameters(self, track_id=[]):
+        """This function calculates gait parameters for all tracks recorded with this sensor, over num_hist_frames."""
+        """To calculate parameters for a specific track, specify the track_id."""
+
+        if (track_id == []):
+            for track_gaits in self.track_gait_params:
+                track_gaits.gait = np.bincount(np.digitize(track_gaits.speed, track_gaits.gait_bins))
+                if len(self.gait_str) > 0:
+                    self.gait_str += ";"
+                self.gait_str += ','.join(map(str, track_gaits.gait))
+
+        else:
+            ind_t = self.track_id.index(track_id)
+            self.track_gait_params[ind_t].gait = np.bincount(np.digitize(self.track_gait_params[ind_t].speed, self.track_gait_params[ind_t].gait_bins))
+
+
+
 # Occupant track history #
 class OccupantHist:
     """Historical positions (X,Y) of occupants (tracks)."""
     def __init__(self, num_hist_frames=10, flag_time_based_record=0):
         """Initialises track histories"""
-        self.sens_idx = []
+        self.sensor_id = []
         self.id = [] # track id
         self.x0 = [] # previous
         self.y0 = []
         self.x1 = [] # current
         self.y1 = []
 
         # Save inputs internally
@@ -647,40 +832,52 @@
         self.flag_active = [] # Flag to identify whether occupant (track) is active or not (1 = active)
         self.time_inactive_start = []   # Time to mark start of inactive period
 
         # General inactivity stats per sensor
         self.most_inactive_track = []
         self.most_inactive_time = []
 
+        # Room heatmaps per sensor
+        self.room_heatmap = [] # Room heatmap showing occupancy positions
+
+        # Gait parameters
+        self.gait_params = []
+
         # Prepare outputs
-        self.outputs = self.Outputs()
+        self.outputs = []
         
     # Use this to refresh the histories
     def refresh(self, sensor_id):
         # Check for this specific sensor
-        ind_s = self.sens_idx.index(sensor_id)
+        ind_s = self.sensor_id.index(sensor_id)
 
         self.id[ind_s] = [] 
 
         self.xh[ind_s] = np.empty([self.xh.shape[1],self.xh.shape[2]], dtype=object)
         self.yh[ind_s] = np.empty([self.yh.shape[1],self.yh.shape[2]], dtype=object)
 
         self.e_ud_h[ind_s] = np.empty([self.e_ud_h.shape[1]], dtype=object)
         self.e_pc_h[ind_s] = np.empty([self.e_pc_h.shape[1]], dtype=object)
 
         self.tot_dist[ind_s] = []
         self.max_dist[ind_s] = [] 
         self.flag_active[ind_s] = []
         self.time_inactive_start[ind_s] = [] 
+
+        # Reset room heatmap
+        self.room_heatmap[ind_s].reset_heatmap()
+
+        # Reset gait parameters
+        self.gait_params[ind_s].reset_tracks(sensor_id)
     
     # Use this to update a track location everytime one is detected.
     def update(self, sensor_id, track_id=[], X=[], Y=[], sensor_data=[]):
-        if (sensor_id in self.sens_idx):
+        if (sensor_id in self.sensor_id):
             # Check for this specific sensor
-            ind_s = self.sens_idx.index(sensor_id)
+            ind_s = self.sensor_id.index(sensor_id)
 
             if (track_id == []):
                 pass
             elif (track_id in self.id[ind_s]):
                 # Check for this specific track
                 ind_t = self.id[ind_s].index(track_id)
 
@@ -703,27 +900,33 @@
                     self.e_pc_h[ind_s] = np.roll(self.e_pc_h[ind_s],1)
                     self.e_pc_h[ind_s][0] = sensor_data.pc.energy[0]
 
 
                 # Update activity statistics
                 self.activity_detection(sensor_id, track_id)
 
+                # Update heatmap
+                self.room_heatmap[ind_s].update_heatmap(X,Y)
+
+                # Update gait parameters
+                self.gait_params[ind_s].update_track(sensor_id, track_id, self.xh[ind_s][ind_t], self.yh[ind_s][ind_t])
+
             else:
                 # Record new values if track did not previously exist
                 #if track_id != []:
                 self.new_track(sensor_id,track_id,X,Y,new_sensor_flag=0)
         else:
             self.new_sensor(sensor_id)
             if track_id != []:
                 self.new_track(sensor_id,track_id,X,Y,new_sensor_flag=1)
 
 
-    # Procedure to when a new track is detected
+    # Procedure when a new track is detected
     def new_track(self,sensor_id,track_id,X,Y,new_sensor_flag):
-        ind_s = self.sens_idx.index(sensor_id)
+        ind_s = self.sensor_id.index(sensor_id)
         # if new_sensor_flag == 0:
         self.id[ind_s].append(track_id)
 
         self.x0[ind_s].append(X)
         self.y0[ind_s].append(Y)
         self.x1[ind_s].append(X)
         self.y1[ind_s].append(Y)
@@ -750,22 +953,26 @@
         ind_t = self.id[ind_s].index(track_id)
         if ind_t > self.xh.shape[1]-1:
             new_track = np.empty((self.xh.shape[0],self.xh.shape[1],self.num_hist_frames),dtype=object)
             self.xh = np.concatenate((self.xh,new_track),axis=1)
             self.yh = np.concatenate((self.yh,new_track),axis=1)
         self.xh[ind_s][ind_t][0] = X
         self.yh[ind_s][ind_t][0] = Y
+
+        # Gait paramaters sensor_id, track_id, Xh, Yh
+        self.gait_params[ind_s].add_new_track(sensor_id, track_id, self.xh[ind_s][ind_t], self.yh[ind_s][ind_t])
         
-    # Proedure when a new sensor is detected
+    # Procedure when a new sensor is detected
     def new_sensor(self,sensor_id):
         #self.max_tracks.append(0)
-        self.sens_idx.append(sensor_id)
+        self.sensor_id.append(sensor_id)
+        self.sensor_id.append(sensor_id)
         self.most_inactive_track.append(None)
         self.most_inactive_time.append(None)
-        if len(self.sens_idx) == 1:
+        if len(self.sensor_id) == 1:
             self.xh = np.array(np.empty((self.num_hist_frames,),dtype=object), ndmin=3)
             self.yh = np.array(np.empty((self.num_hist_frames,),dtype=object), ndmin=3)
             self.e_ud_h = np.array(np.empty((self.num_hist_frames,),dtype=object), ndmin=2)
             self.e_pc_h = np.array(np.empty((self.num_hist_frames,),dtype=object), ndmin=2)
         else:
             new_sensor = np.empty((1,self.xh.shape[1],self.xh.shape[2]),dtype=object)
             self.xh = np.concatenate((self.xh,new_sensor),axis=0)
@@ -780,19 +987,26 @@
         self.x1.append([])
         self.y1.append([])
 
         self.tot_dist.append([])
         self.max_dist.append([])
         self.flag_active.append([])    # By default mark them as active
         self.time_inactive_start.append([])
+
+        # Room heatmap
+        self.room_heatmap.append(OccupantHeatmap(sensor_id, Xres=0.25, Yres=0.25, Xrange=[-4.5,4.5], Yrange=[0,5]))
+
+        # Gait parameters
+        self.gait_params.append(GaitParameters(sensor_id, num_hist_frames=self.num_hist_frames))
+
     
     # Use this to check entryways and see if anyone has entered/left the room
     def entryway(self, sensor_id, track_id, ew):
         if (sensor_id in ew.id):
-            ind_s = self.sens_idx.index(sensor_id)
+            ind_s = self.sensor_id.index(sensor_id)
             ind_e = ew.id.index(sensor_id)
             ind_t = self.id[ind_s].index(track_id)
             [sx0,sx1] = [self.x0[ind_s][ind_t],self.x1[ind_s][ind_t]]
             [sy0,sy1] = [self.y0[ind_s][ind_t],self.y1[ind_s][ind_t]]
             
             try:
                 if abs(sx0-sx1)+abs(sy0-sy1) > 0:
@@ -815,25 +1029,21 @@
                                     nodens.logger.warning('Warning! Count dropped below 0 and was reset.')
                                 nodens.logger.info('Leaving room at entry {} with (t,u)=({},{}). Occupancy = {}.'.format(i,t,u,ew.count[ind_e]))
             except:
                 nodens.logger.warning('Entryway update issue. (sx0,sx1)=({},{}). (sy0,sy1)=({},{})'.format(sx0,sx1,sy0,sy1))
     
     # Track activity/inactivity statistics
     def activity_detection(self, sensor_id, track_id, tot_dist_thresh=1, max_dist_thresh=1):
-        ind_s = self.sens_idx.index(sensor_id)
+        ind_s = self.sensor_id.index(sensor_id)
         ind_t = self.id[ind_s].index(track_id)
         
         # Non-None values from history
         xh =  [val for i,val in enumerate(self.xh[ind_s][ind_t]) if val is not None]
         yh =  [val for i,val in enumerate(self.yh[ind_s][ind_t]) if val is not None]
 
-        # Take oldest values
-        xi = xh[-1]
-        yi = yh[-1]
-
         # Calculate distances for each frame
         try:
             xd = np.subtract(xh[1:],xh[0:-1])
             yd = np.subtract(yh[1:],yh[0:-1])
             rd = (xd**2 + yd**2)**0.5
 
             # Find statistics
@@ -860,69 +1070,82 @@
         # try:
         #     ud_e = [val for val in self.e_ud_h[ind_s][ind_t] if val is not None]
         #     print(f"ud: {ud_e}")
 
 
     # Calculate general activity statistics
     def sensor_activity(self, sensor_id):
-        ind_s = self.sens_idx.index(sensor_id)
+        ind_s = self.sensor_id.index(sensor_id)
         inactive_tracks = [self.time_inactive_start[ind_s][i] for i,val in enumerate(self.flag_active[ind_s]) if val==0]
         if len(inactive_tracks) == 0:
             self.most_inactive_track[ind_s] = None
             self.most_inactive_time[ind_s] = None
         else:
             inactive_idx = min(range(len(inactive_tracks)), key=inactive_tracks.__getitem__)
             self.most_inactive_track[ind_s] = self.id[ind_s][inactive_idx]
             self.most_inactive_time[ind_s] = dt.datetime.now(dt.timezone.utc) - self.time_inactive_start[ind_s][inactive_idx]
 
     # Calculate outputs
     def calculate_outputs(self, thresh_distance = 0, energy_threshold = 0):
         # Re-initialise outputs
-        self.outputs.__init__()
+        self.outputs = []
+        #self.outputs.__init__()
 
-        for idx, sensor in enumerate(self.sens_idx):    # For each sensor
+        for idx, sensor in enumerate(self.sensor_id):    # For each sensor
+            self.outputs.append(self.Outputs)
+            self.outputs.sensor_id = sensor
             if len(self.id[idx]) > 0:
                 # Determine track to send
                 if max(self.tot_dist[idx]) >= thresh_distance: # Distance threshold at 0 for now, until UD sig tid is found.
                     tid = self.tot_dist[idx].index(max(self.tot_dist[idx]))
 
                     self.outputs.track_id = self.id[idx][tid]
 
                     # Record parameters
                     self.outputs.track_X = self.x1[idx][tid]
                     self.outputs.track_Y = self.y1[idx][tid]
                     self.outputs.distance_moved = self.tot_dist[idx][tid]
-
-                    # Energy statistics (for scene not track)
-                    ud_e = [val for val in self.e_ud_h[idx] if val is not None]
-                    self.outputs.ud_energy = sum(ud_e)
-                    if self.outputs.ud_energy > energy_threshold:
-                        self.outputs.was_active = 1
-                    else:
-                        self.outputs.was_active = 0
-                    pc_e = [val for val in self.e_pc_h[idx] if val is not None]
-                    self.outputs.pc_energy = sum(pc_e)
+                    
                 else:
                     pass
                     #tid = self.ud_energy[idx].index(max(self.ud_energy[idx]))
-                    
+
+                # Gait parameters
+                self.gait_params[idx].calculate_gait_parameters()
+                self.outputs.gait_string = self.gait_params[idx].gait_string
+
+            # Energy statistics (for scene not track)
+            ud_e = [val for val in self.e_ud_h[idx] if val is not None]
+            self.outputs.ud_energy = sum(ud_e)
+            if self.outputs.ud_energy > energy_threshold:
+                self.outputs.was_active = 1
+            else:
+                self.outputs.was_active = 0
+            pc_e = [val for val in self.e_pc_h[idx] if val is not None]
+            self.outputs.pc_energy = sum(pc_e)
+            
+            # Room heatmaps
+            self.room_heatmap[idx].prepare_heatmap_string()
+            self.outputs.heatmap_string = self.room_heatmap[idx].heatmap_string
 
 
     
     # Class to define outputs
     class Outputs:
         def __init__(self) -> None:
+            self.sensor_id = []
             self.track_id = []  # tid with highest distance walked, or if under threshold then highest energy
             self.track_X = []   # corresponding location for tid
             self.track_Y = []
             self.distance_moved = []   # total distance moved
             self.was_active = []        # check if ud_energy over threshold
             self.ud_energy = []
             self.pc_energy = []
-
+            self.heatmap_string = []    # Array composed of heatmap strings
+            self.gait_string = []       # Array composed of gait speed distribution
         
                     
                 
         
 
 
 
@@ -1070,16 +1293,20 @@
 class PresenceDetect:
     """Processes radar TLV related to presence detction"""
     def __init__(self) -> None:
         self.present = 0
         self.tlv_len = []
 
     def process(self, raw):
-        self.tlv_len = np.uint8(raw[4:8]).view(np.uint32)[0]
-        self.present = raw[8]
+        try:
+            self.tlv_len = np.uint8(raw[4:8]).view(np.uint32)[0]
+            self.present = raw[8]
+        except Exception as e:
+            nodens.logger.warning(f"PresenceDetect.process: {e}. raw: {raw}")
+            self.tlv_len = 0
 
 class sensorTimeSeries:
     def __init__(self):
         self.frame = []
         self.packet_len = []
         self.num_tlv = []
         self.num_pnts = []
```

### Comparing `nodens-gateway-24.3.6/src/nodens/gateway/nodens_insight_hub.py` & `nodens_gateway-24.5.0/src/nodens/gateway/nodens_insight_hub.py`

 * *Files identical despite different names*

### Comparing `nodens-gateway-24.3.6/src/nodens/gateway/nodens_mesh.py` & `nodens_gateway-24.5.0/src/nodens/gateway/nodens_mesh.py`

 * *Files identical despite different names*

### Comparing `nodens-gateway-24.3.6/src/nodens/gateway/nodens_serv.py` & `nodens_gateway-24.5.0/src/nodens/gateway/nodens_serv.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             data_int = [data[0]]
 
             if len(data) > 6:
                 for i in range(7):
                     str_data = str_data + str(data[i+1])
                     data_int.append(data[i+1])
             else:
-                logging.warning("Data below length 8. Rx: {}".format(data))
+                nodens.logger.warning("Data below length 8. Rx: {}".format(data))
             # Check if full data packet received
             if str_data == '21436587':
                 for i in range(len(data)-8):
                     str_data = str_data + str(data[i+8])
                     data_int.append(data[i+8])
                 mqttDataFinal = mqttData
 
@@ -188,27 +188,30 @@
                     ndns_fns.oh.calculate_outputs()
 
                     mqttTime = json.loads("{\"Time\": \"" + str(T) + "\"}")
                     mqttClass = json.loads("{\"Activity detected\": \"" + str(int(ndns_fns.class_eng.activity_alert))
                                         + "\", \"Activity type\": \"" + str(int(ndns_fns.class_eng.classification))
                                         + "\"}")
                     mqttDataFinal = {**mqttData, #'addr' : mqttData['addr'],
+                                    'Sensor timestamp' : T,
                                     'Average period occupancy' : ndns_fns.si.period_sum_occ[sen_idx]/ndns_fns.si.period_N[sen_idx], 
                                     'Maximum period occupancy' : ndns_fns.si.period_max_occ[sen_idx],
                                     'Average entryway occupancy' : ndns_fns.si.ew_period_sum_occ[sen_idx]/ndns_fns.si.period_N[sen_idx], 
                                     'Maximum entryway occupancy' : ndns_fns.si.ew_period_max_occ[sen_idx],
                                     'Full data flag' : 1,
-                                    'Track id' : ndns_fns.oh.outputs.track_id,
-                                    'X' : ndns_fns.oh.outputs.track_X,
-                                    'Y' : ndns_fns.oh.outputs.track_Y,
-                                    'Distance moved' : ndns_fns.oh.outputs.distance_moved,
-                                    'Was active' : ndns_fns.oh.outputs.was_active,
-                                    'UD energy' : ndns_fns.oh.outputs.ud_energy,
-                                    'PC energy' : ndns_fns.oh.outputs.pc_energy,
+                                    'Track id' : ndns_fns.oh.outputs[sen_idx].track_id,
+                                    'X' : ndns_fns.oh.outputs[sen_idx].track_X,
+                                    'Y' : ndns_fns.oh.outputs[sen_idx].track_Y,
+                                    'Distance moved' : ndns_fns.oh.outputs[sen_idx].distance_moved,
+                                    'Was active' : ndns_fns.oh.outputs[sen_idx].was_active,
+                                    'UD energy' : ndns_fns.oh.outputs[sen_idx].ud_energy,
+                                    'PC energy' : ndns_fns.oh.outputs[sen_idx].pc_energy,
                                     'Presence detected' : ndns_fns.sd.presence.present,
+                                    'Occupancy heatmap' : ndns_fns.oh.outputs[sen_idx].heatmap_string,
+                                    'Gait distribution' : ndns_fns.oh.outputs[sen_idx].gait_string
                                     }
 
                     ndns_fns.class_eng.activity_alert = 0
                     try:
                         send_idx_o = ndns_fns.oh.sens_idx.index(mqttData['addr'])
                         mqttDataFinal = {**mqttDataFinal, 
                                     'Most inactive track' : ndns_fns.oh.most_inactive_track[send_idx_o],
@@ -236,14 +239,17 @@
                     #     ndns_tb.TB.prepare_data(mqttDataFinal)
                     #     ndns_tb.TB.multiline_payload(mqttData['addr'])
 
 
                     ndns_fns.si.cloud_send_refresh(sen_idx, send_idx_e, T, ndns_fns.ew)
                     heartbeat = ""
 
+                    # Refresh occupancy histories for next Cloud transmission frame
+                    ndns_fns.oh.refresh(mqttData['addr'])
+
             elif (mqttData['type'] == 'json'):
                 print("JSON type: {}".format(mqttData))
             # Otherwise process occupancy info
             else:
                 ndns_fns.sm.update(mqttData)
                 mqttOcc = json.loads(data)
                 mqttTime = json.loads("{\"Time\": \"" + str(T) + "\"}")
@@ -269,21 +275,23 @@
                         while 1:
                             if i < 1:
                                 for j in range(4):
                                     mqttDataTemp.append('')
                                 i += 1
                             else:
                                 break
-
-                        if 'Heatmap energy' in mqttOccInfo[-1]:
-                            mqttDataTemp.append(mqttOccInfo[-1]['Heatmap energy'])
-                            mqttDataTemp.append(mqttOccInfo[-1]['Heatmap'])
-                        else:
-                            mqttDataTemp.append(0)
-                            mqttDataTemp.append('')
+                        try:
+                            if 'Heatmap energy' in mqttOccInfo[-1]:
+                                mqttDataTemp.append(mqttOccInfo[-1]['Heatmap energy'])
+                                mqttDataTemp.append(mqttOccInfo[-1]['Heatmap'])
+                            else:
+                                mqttDataTemp.append(0)
+                                mqttDataTemp.append('')
+                        except Exception as e:
+                            nodens.logger.warning(f"{e}")
                     else:
                         for i in range(8):
                             mqttDataTemp.append('')
                         mqttDataTemp.append(0)
                         mqttDataTemp.append('')
 
                     mqttData_SAVE.append(mqttDataTemp)
@@ -363,14 +371,15 @@
                                         'X' : ndns_fns.oh.outputs.track_X,
                                         'Y' : ndns_fns.oh.outputs.track_Y,
                                         'Distance moved' : ndns_fns.oh.outputs.distance_moved,
                                         'Was active' : ndns_fns.oh.outputs.was_active,
                                         'UD energy' : ndns_fns.oh.outputs.ud_energy,
                                         'PC energy' : ndns_fns.oh.outputs.pc_energy,
                                         'Presence detected' : ndns_fns.sd.presence.present,
+                                        'Occupancy heatmap' : ndns_fns.oh.outputs.heatmap_string
                                         }
                         
                         ndns_fns.class_eng.activity_alert = 0
                         try:
                             send_idx_o = ndns_fns.oh.sens_idx.index(mqttData['addr'])
                             mqttDataFinal = {**mqttDataFinal, 
                                         'Most inactive track' : ndns_fns.oh.most_inactive_track[send_idx_o],
```

### Comparing `nodens-gateway-24.3.6/src/nodens/gateway/nodens_thingsboard.py` & `nodens_gateway-24.5.0/src/nodens/gateway/nodens_thingsboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,16 @@
         self.payload["avg_occupancy"] = input_data['Average period occupancy']
 
         # Track ID - select tid with highest energy.
         
         # Occupant positions
         if self.payload["avg_occupancy"] > 0:
             try:
+                self.payload["sensor_timestamp"] = f"{input_data['Sensor timestamp']}"
+
                 # ~~~~~~~~~~~ Occupancy ~~~~~~~~~~~~~ #
                 #temp = input_data['Occupancy Info'][0]
                 self.payload["occupant_id"] = f"{input_data['Track id']}"
                 self.payload["X"] = f"{input_data['X']:.2f}"
                 self.payload["Y"] = f"{input_data['Y']:.2f}"
 
                 # ~~~~~~~~~~~ ACTIVITY ~~~~~~~~~~~~~ #
@@ -160,14 +162,20 @@
                 self.payload["pc_energy"] = f"{input_data['PC energy']:.2f}"
                 # self.payload["most_inactive_track"] = input_data['Most inactive track']
                 # self.payload["most_inactive_time"] = input_data['Most inactive time']
 
                 # ~~~~~~~~~~~ SLEEP ~~~~~~~~~~~~~ #
                 self.payload["rest_zone_presence"] = f"{input_data['Presence detected']}"
 
+                # ~~~~~~~~~~~ HEATMAP ~~~~~~~~~~~~~ #
+                self.payload["room_occ_heatmap"] = f"{input_data['Occupancy heatmap']}"
+
+                # ~~~~~~~~~~~ GAIT ~~~~~~~~~~~~~ #
+                self.payload["gait_distribution"] = f"{input_data['Gait distribution']}"
+
             except Exception as e:
                 nodens.logger.debug(f"THINGSBOARD: occupant error: {e.args}")
                 # self.payload["occ_1_X"] = "-"
                 # self.payload["occ_1_Y"] = "-"
                 # self.payload["most_inactive_track"] = "-"
                 # self.payload["most_inactive_time"] = "-"
         # Don't send anything if no occupants.
```

### Comparing `nodens-gateway-24.3.6/src/nodens_gateway.egg-info/PKG-INFO` & `nodens_gateway-24.5.0/src/nodens_gateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.3.6
+Version: 24.5.0
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens-gateway-24.3.6/src/nodens_gateway.egg-info/PKG-INFO-Hawk` & `nodens_gateway-24.5.0/src/nodens_gateway.egg-info/PKG-INFO-Hawk`

 * *Files identical despite different names*

### Comparing `nodens-gateway-24.3.6/src/nodens_gateway.egg-info/SOURCES.txt` & `nodens_gateway-24.5.0/src/nodens_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

