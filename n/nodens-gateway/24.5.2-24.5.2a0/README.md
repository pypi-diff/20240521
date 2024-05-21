# Comparing `tmp/nodens_gateway-24.5.2.tar.gz` & `tmp/nodens_gateway-24.5.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodens_gateway-24.5.2.tar", last modified: Tue May 21 15:58:35 2024, max compression
+gzip compressed data, was "nodens_gateway-24.5.2a0.tar", last modified: Tue May 21 16:24:39 2024, max compression
```

## Comparing `nodens_gateway-24.5.2.tar` & `nodens_gateway-24.5.2a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.611402 nodens_gateway-24.5.2/
--rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.2/LICENSE
--rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4326 2024-05-21 15:58:35.606017 nodens_gateway-24.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.2/README.md
--rw-rw-rw-   0        0        0      817 2024-05-21 15:57:40.000000 nodens_gateway-24.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 15:58:35.612410 nodens_gateway-24.5.2/setup.cfg
--rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.370823 nodens_gateway-24.5.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.368822 nodens_gateway-24.5.2/src/nodens/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.444689 nodens_gateway-24.5.2/src/nodens/gateway/
--rw-rw-rw-   0        0        0    13490 2024-05-21 15:57:30.000000 nodens_gateway-24.5.2/src/nodens/gateway/__init__.py
--rw-rw-rw-   0        0        0     8583 2024-05-21 13:43:36.000000 nodens_gateway-24.5.2/src/nodens/gateway/__main__.py
--rw-rw-rw-   0        0        0    86570 2024-05-21 15:56:35.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_fns.py
--rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_insight_hub.py
--rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_mesh.py
--rw-rw-rw-   0        0        0    25387 2024-05-21 14:23:09.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_serv.py
--rw-rw-rw-   0        0        0    11078 2024-05-21 12:58:30.000000 nodens_gateway-24.5.2/src/nodens/gateway/nodens_thingsboard.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:58:35.599072 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/
--rw-rw-rw-   0        0        0     4326 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/PKG-INFO-Hawk
--rw-rw-rw-   0        0        0      640 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/requires-Hawk.txt
--rw-rw-rw-   0        0        0       70 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 15:58:35.000000 nodens_gateway-24.5.2/src/nodens_gateway.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.790323 nodens_gateway-24.5.2a0/
+-rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.2a0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.2a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4328 2024-05-21 16:24:39.767828 nodens_gateway-24.5.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.2a0/README.md
+-rw-rw-rw-   0        0        0      819 2024-05-21 16:23:24.000000 nodens_gateway-24.5.2a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:24:39.791271 nodens_gateway-24.5.2a0/setup.cfg
+-rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.2a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.216928 nodens_gateway-24.5.2a0/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.194227 nodens_gateway-24.5.2a0/src/nodens/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.518635 nodens_gateway-24.5.2a0/src/nodens/gateway/
+-rw-rw-rw-   0        0        0    13492 2024-05-21 16:23:30.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/__init__.py
+-rw-rw-rw-   0        0        0     8583 2024-05-21 13:43:36.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/__main__.py
+-rw-rw-rw-   0        0        0    86284 2024-05-21 16:23:09.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_fns.py
+-rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_insight_hub.py
+-rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_mesh.py
+-rw-rw-rw-   0        0        0    25387 2024-05-21 14:23:09.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_serv.py
+-rw-rw-rw-   0        0        0    11078 2024-05-21 12:58:30.000000 nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_thingsboard.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:24:39.754935 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/
+-rw-rw-rw-   0        0        0     4328 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/PKG-INFO-Hawk
+-rw-rw-rw-   0        0        0      640 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/requires-Hawk.txt
+-rw-rw-rw-   0        0        0       70 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 16:24:39.000000 nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/top_level.txt
```

### Comparing `nodens_gateway-24.5.2/LICENSE` & `nodens_gateway-24.5.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2/PKG-INFO` & `nodens_gateway-24.5.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.2
+Version: 24.5.2a0
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.2/README.md` & `nodens_gateway-24.5.2a0/README.md`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2/pyproject.toml` & `nodens_gateway-24.5.2a0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodens-gateway"
-version = "24.5.2"
+version = "24.5.2.a"
 description = "Run the NodeNs gateway"
 readme = "README.md"
 authors = [{ name = "Khalid Z Rajab", email = "khalid@nodens.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `nodens_gateway-24.5.2/src/nodens/gateway/__init__.py` & `nodens_gateway-24.5.2a0/src/nodens/gateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 global APPNAME
 global APPAUTHOR
 global CWD
 
 # Some information
 __title__ = "nodens-gateway"
-__version__ = "24.5.2"
+__version__ = "24.5.2.a"
 __author__ = "Khalid Z Rajab"
 __author_email__ = "khalid@nodens.eu"
 __copyright__ = "Copyright (c) 2024 " + __author__
 __license__ = "MIT"
 
 APPNAME = "Gateway"
 APPAUTHOR = "NodeNs"
```

### Comparing `nodens_gateway-24.5.2/src/nodens/gateway/__main__.py` & `nodens_gateway-24.5.2a0/src/nodens/gateway/__main__.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2/src/nodens/gateway/nodens_fns.py` & `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_fns.py`

 * *Files 1% similar despite different names*

```diff
@@ -787,22 +787,18 @@
 
     def calculate_gait_parameters(self, track_id=[]):
         """This function calculates gait parameters for all tracks recorded with this sensor, over num_hist_frames."""
         """To calculate parameters for a specific track, specify the track_id."""
 
         if (track_id == []):
             for track_gaits in self.track_gait_params:
-                nodens.logger.info(f"GAIT. speed: {track_gaits.speed}")
-                nodens.logger.info(f"GAIT. bins: {track_gaits.gait_bins}")
                 track_gaits.gait = np.bincount(np.digitize(track_gaits.speed, track_gaits.gait_bins))
-                nodens.logger.info(f"GAIT. gait: {track_gaits.gait}")
                 if len(self.gait_str) > 0:
                     self.gait_str += ";"
                 self.gait_str += ','.join(map(str, track_gaits.gait))
-            nodens.logger.info(f"GAIT. string: {self.gait_str}")
 
         else:
             ind_t = self.track_id.index(track_id)
             self.track_gait_params[ind_t].gait = np.bincount(np.digitize(self.track_gait_params[ind_t].speed, self.track_gait_params[ind_t].gait_bins))
```

### Comparing `nodens_gateway-24.5.2/src/nodens/gateway/nodens_insight_hub.py` & `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_insight_hub.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2/src/nodens/gateway/nodens_mesh.py` & `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_mesh.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2/src/nodens/gateway/nodens_serv.py` & `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_serv.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2/src/nodens/gateway/nodens_thingsboard.py` & `nodens_gateway-24.5.2a0/src/nodens/gateway/nodens_thingsboard.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2/src/nodens_gateway.egg-info/PKG-INFO` & `nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.2
+Version: 24.5.2a0
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.2/src/nodens_gateway.egg-info/PKG-INFO-Hawk` & `nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/PKG-INFO-Hawk`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.2/src/nodens_gateway.egg-info/SOURCES.txt` & `nodens_gateway-24.5.2a0/src/nodens_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

