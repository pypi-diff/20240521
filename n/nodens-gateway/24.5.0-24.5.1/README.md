# Comparing `tmp/nodens_gateway-24.5.0.tar.gz` & `tmp/nodens_gateway-24.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodens_gateway-24.5.0.tar", last modified: Tue May 21 12:46:02 2024, max compression
+gzip compressed data, was "nodens_gateway-24.5.1.tar", last modified: Tue May 21 13:05:14 2024, max compression
```

## Comparing `nodens_gateway-24.5.0.tar` & `nodens_gateway-24.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.806703 nodens_gateway-24.5.0/
--rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4326 2024-05-21 12:46:02.796864 nodens_gateway-24.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.0/README.md
--rw-rw-rw-   0        0        0      817 2024-05-21 12:44:51.000000 nodens_gateway-24.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 12:46:02.809255 nodens_gateway-24.5.0/setup.cfg
--rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.407829 nodens_gateway-24.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.405465 nodens_gateway-24.5.0/src/nodens/
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.549810 nodens_gateway-24.5.0/src/nodens/gateway/
--rw-rw-rw-   0        0        0    13316 2024-05-21 12:44:58.000000 nodens_gateway-24.5.0/src/nodens/gateway/__init__.py
--rw-rw-rw-   0        0        0     8677 2024-03-02 16:51:04.000000 nodens_gateway-24.5.0/src/nodens/gateway/__main__.py
--rw-rw-rw-   0        0        0    84960 2024-05-21 10:54:01.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_fns.py
--rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_insight_hub.py
--rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_mesh.py
--rw-rw-rw-   0        0        0    25146 2024-05-21 10:51:38.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_serv.py
--rw-rw-rw-   0        0        0    10888 2024-05-21 10:52:10.000000 nodens_gateway-24.5.0/src/nodens/gateway/nodens_thingsboard.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:02.789179 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/
--rw-rw-rw-   0        0        0     4326 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/PKG-INFO-Hawk
--rw-rw-rw-   0        0        0      640 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/requires-Hawk.txt
--rw-rw-rw-   0        0        0       70 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 12:46:02.000000 nodens_gateway-24.5.0/src/nodens_gateway.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 13:05:14.601169 nodens_gateway-24.5.1/
+-rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4326 2024-05-21 13:05:14.598152 nodens_gateway-24.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.1/README.md
+-rw-rw-rw-   0        0        0      817 2024-05-21 13:04:39.000000 nodens_gateway-24.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:05:14.603176 nodens_gateway-24.5.1/setup.cfg
+-rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:05:14.479149 nodens_gateway-24.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 13:05:14.478571 nodens_gateway-24.5.1/src/nodens/
+drwxrwxrwx   0        0        0        0 2024-05-21 13:05:14.520906 nodens_gateway-24.5.1/src/nodens/gateway/
+-rw-rw-rw-   0        0        0    13316 2024-05-21 13:04:36.000000 nodens_gateway-24.5.1/src/nodens/gateway/__init__.py
+-rw-rw-rw-   0        0        0     8677 2024-03-02 16:51:04.000000 nodens_gateway-24.5.1/src/nodens/gateway/__main__.py
+-rw-rw-rw-   0        0        0    84961 2024-05-21 13:03:56.000000 nodens_gateway-24.5.1/src/nodens/gateway/nodens_fns.py
+-rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.1/src/nodens/gateway/nodens_insight_hub.py
+-rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.1/src/nodens/gateway/nodens_mesh.py
+-rw-rw-rw-   0        0        0    25146 2024-05-21 10:51:38.000000 nodens_gateway-24.5.1/src/nodens/gateway/nodens_serv.py
+-rw-rw-rw-   0        0        0    11078 2024-05-21 12:58:30.000000 nodens_gateway-24.5.1/src/nodens/gateway/nodens_thingsboard.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:05:14.595182 nodens_gateway-24.5.1/src/nodens_gateway.egg-info/
+-rw-rw-rw-   0        0        0     4326 2024-05-21 13:05:14.000000 nodens_gateway-24.5.1/src/nodens_gateway.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.1/src/nodens_gateway.egg-info/PKG-INFO-Hawk
+-rw-rw-rw-   0        0        0      640 2024-05-21 13:05:14.000000 nodens_gateway-24.5.1/src/nodens_gateway.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:05:14.000000 nodens_gateway-24.5.1/src/nodens_gateway.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-21 13:05:14.000000 nodens_gateway-24.5.1/src/nodens_gateway.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.1/src/nodens_gateway.egg-info/requires-Hawk.txt
+-rw-rw-rw-   0        0        0       70 2024-05-21 13:05:14.000000 nodens_gateway-24.5.1/src/nodens_gateway.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 13:05:14.000000 nodens_gateway-24.5.1/src/nodens_gateway.egg-info/top_level.txt
```

### Comparing `nodens_gateway-24.5.0/LICENSE` & `nodens_gateway-24.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.0/PKG-INFO` & `nodens_gateway-24.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.0
+Version: 24.5.1
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.0/README.md` & `nodens_gateway-24.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.0/pyproject.toml` & `nodens_gateway-24.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodens-gateway"
-version = "24.5.0"
+version = "24.5.1"
 description = "Run the NodeNs gateway"
 readme = "README.md"
 authors = [{ name = "Khalid Z Rajab", email = "khalid@nodens.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `nodens_gateway-24.5.0/src/nodens/gateway/__init__.py` & `nodens_gateway-24.5.1/src/nodens/gateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 global APPNAME
 global APPAUTHOR
 global CWD
 
 # Some information
 __title__ = "nodens-gateway"
-__version__ = "24.5.0"
+__version__ = "24.5.1"
 __author__ = "Khalid Z Rajab"
 __author_email__ = "khalid@nodens.eu"
 __copyright__ = "Copyright (c) 2024 " + __author__
 __license__ = "MIT"
 
 APPNAME = "Gateway"
 APPAUTHOR = "NodeNs"
```

### Comparing `nodens_gateway-24.5.0/src/nodens/gateway/__main__.py` & `nodens_gateway-24.5.1/src/nodens/gateway/__main__.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.0/src/nodens/gateway/nodens_fns.py` & `nodens_gateway-24.5.1/src/nodens/gateway/nodens_fns.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,15 +630,15 @@
         self.Yres = Yres
 
         self.Xrange = Xrange
         self.Yrange = Yrange
 
         Xn = np.ceil(Xrange[1]/Xres)-np.floor(Xrange[0]/Xres)
         Yn = np.ceil(Yrange[1]/Yres)-np.floor(Yrange[0]/Yres)
-        self.heatmap = np.zero((Xn,Yn))
+        self.heatmap = np.zeros((Xn,Yn))
         self.heatmap_string = ""
 
     def reset_heatmap(self):
         self.heatmap = 0*self.heatmap
         self.heatmap_string = ""
     
     def update_heatmap(self, X, Y):
```

### Comparing `nodens_gateway-24.5.0/src/nodens/gateway/nodens_insight_hub.py` & `nodens_gateway-24.5.1/src/nodens/gateway/nodens_insight_hub.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.0/src/nodens/gateway/nodens_mesh.py` & `nodens_gateway-24.5.1/src/nodens/gateway/nodens_mesh.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.0/src/nodens/gateway/nodens_serv.py` & `nodens_gateway-24.5.1/src/nodens/gateway/nodens_serv.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.0/src/nodens/gateway/nodens_thingsboard.py` & `nodens_gateway-24.5.1/src/nodens/gateway/nodens_thingsboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,22 +162,28 @@
                 self.payload["pc_energy"] = f"{input_data['PC energy']:.2f}"
                 # self.payload["most_inactive_track"] = input_data['Most inactive track']
                 # self.payload["most_inactive_time"] = input_data['Most inactive time']
 
                 # ~~~~~~~~~~~ SLEEP ~~~~~~~~~~~~~ #
                 self.payload["rest_zone_presence"] = f"{input_data['Presence detected']}"
 
-                # ~~~~~~~~~~~ HEATMAP ~~~~~~~~~~~~~ #
-                self.payload["room_occ_heatmap"] = f"{input_data['Occupancy heatmap']}"
-
                 # ~~~~~~~~~~~ GAIT ~~~~~~~~~~~~~ #
                 self.payload["gait_distribution"] = f"{input_data['Gait distribution']}"
 
             except Exception as e:
                 nodens.logger.debug(f"THINGSBOARD: occupant error: {e.args}")
+
+        # ~~~~~~~~~~~ ENERGY ~~~~~~~~~~~~~ #
+        self.payload["track_ud_energy"] = f"{input_data['UD energy']:.2f}"
+        self.payload["pc_energy"] = f"{input_data['PC energy']:.2f}"
+        
+        # ~~~~~~~~~~~ HEATMAP ~~~~~~~~~~~~~ #
+        self.payload["room_occ_heatmap"] = f"{input_data['Occupancy heatmap']}"
+
+
                 # self.payload["occ_1_X"] = "-"
                 # self.payload["occ_1_Y"] = "-"
                 # self.payload["most_inactive_track"] = "-"
                 # self.payload["most_inactive_time"] = "-"
         # Don't send anything if no occupants.
         # else:
```

### Comparing `nodens_gateway-24.5.0/src/nodens_gateway.egg-info/PKG-INFO` & `nodens_gateway-24.5.1/src/nodens_gateway.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.0
+Version: 24.5.1
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.0/src/nodens_gateway.egg-info/PKG-INFO-Hawk` & `nodens_gateway-24.5.1/src/nodens_gateway.egg-info/PKG-INFO-Hawk`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.0/src/nodens_gateway.egg-info/SOURCES.txt` & `nodens_gateway-24.5.1/src/nodens_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

