# Comparing `tmp/bblib-2.0.0.tar.gz` & `tmp/bblib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblib-2.0.0.tar", max compression
+gzip compressed data, was "bblib-2.0.1.tar", max compression
```

## Comparing `bblib-2.0.0.tar` & `bblib-2.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35146 2024-04-26 13:21:02.375355 bblib-2.0.0/LICENSE
--rw-r--r--   0        0        0     3753 2024-04-26 13:21:02.375355 bblib-2.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-26 13:21:02.375355 bblib-2.0.0/bblib/__init__.py
--rwxr-xr-x   0        0        0    37001 2024-04-26 13:21:02.375355 bblib-2.0.0/bblib/methods.py
--rwxr-xr-x   0        0        0     9961 2024-04-26 13:21:02.379356 bblib-2.0.0/bblib/models.py
--rwxr-xr-x   0        0        0    18198 2024-04-26 13:21:02.379356 bblib-2.0.0/bblib/utils.py
--rw-r--r--   0        0        0     2104 2024-04-26 13:21:22.327287 bblib-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 bblib-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-05-21 15:13:38.063589 bblib-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3906 2024-05-21 15:13:38.063589 bblib-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 15:13:38.063589 bblib-2.0.1/bblib/__init__.py
+-rwxr-xr-x   0        0        0    37211 2024-05-21 15:13:38.063589 bblib-2.0.1/bblib/methods.py
+-rwxr-xr-x   0        0        0     9961 2024-05-21 15:13:38.063589 bblib-2.0.1/bblib/models.py
+-rwxr-xr-x   0        0        0    18198 2024-05-21 15:13:38.063589 bblib-2.0.1/bblib/utils.py
+-rw-r--r--   0        0        0     2104 2024-05-21 15:13:45.871545 bblib-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7437 1970-01-01 00:00:00.000000 bblib-2.0.1/PKG-INFO
```

### Comparing `bblib-2.0.0/LICENSE` & `bblib-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bblib-2.0.0/README.md` & `bblib-2.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,23 @@
 ```
 
 The methods `FriedelPairs`, `MinimizePeakFWHM` and  `CircleDetection ` need a `plots_info` parameter if you want to save plots:
 ```python
 plots_info =  {
 	"file_name": ...,
 	"folder_name": ...,
-	"root_path": ...
+	"root_path": ...,
+	"value_auto": ...,
+	"value_max": ...,
+	"value_min": ...,
+	"axis_lim_auto": ...,
+	"xlim_min": ...,
+	"xlim_max": ...,
+	"ylim_min": ...,
+	"ylim_max": ...
 }
 ```
 To calculate the refined detector center of raw data frame as a numpy array using the following methods: 
 
 ```python
 from bblib.methods import CenterOfMass
 center_of_mass_method = CenterOfMass(config=config, PF8Config=PF8Config, plots_info=plots_info)
```

### Comparing `bblib-2.0.0/bblib/methods.py` & `bblib-2.0.1/bblib/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -768,15 +768,15 @@
         ## Calculcate the beam center shift
         
         self.peaks_list_original = [x for x, y in pairs_list]
         self.peaks_list_inverted = [y for x, y in pairs_list]
 
         if len(pairs_list)>0:
             print(f"--------------  Friedel pairs search --------------\nNumber of Friedel Pairs in frame: {len(pairs_list)/2}")
-            print(f"Pairs list for debug:")
+            print(f"Pairs list for analysis:")
             print(pairs_list)
 
             friedel_coordinates_in_x = [x for x, y in self.peaks_list_original]
             friedel_coordinates_in_y = [y for x, y in self.peaks_list_original]
             
             print(f"Friedel pairs position before center correction in pixels:")
             print(self.peaks_list_original)
@@ -786,14 +786,18 @@
             print("Center shift in x", shift_x)
             print("Center shift in y", shift_y)
             center = [self.initial_guess[0]+shift_x, self.initial_guess[1]+shift_y]
 
             print(f"Friedel pairs position after center correction in pixels:")
             pairs_list_after_correction=[(x[0]-shift_x, x[1]-shift_y) for x in self.peaks_list_original]
             print(pairs_list_after_correction)
+            print(f"All reflections after center correction in pixels:")
+            peaks_list_after_correction=[(x[0]-shift_x, x[1]-shift_y) for x in peaks]
+            print(peaks_list_after_correction)
+
         else:
             center = [-1, -1]
 
         if self.config["plots_flag"] and self.centering_converged(center):
 
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
             if self.plots_info["value_auto"]:
```

### Comparing `bblib-2.0.0/bblib/models.py` & `bblib-2.0.1/bblib/models.py`

 * *Files identical despite different names*

### Comparing `bblib-2.0.0/bblib/utils.py` & `bblib-2.0.1/bblib/utils.py`

 * *Files identical despite different names*

### Comparing `bblib-2.0.0/pyproject.toml` & `bblib-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblib"
-version = "2.0.0"
+version = "2.0.1"
 description = "beambusters library to refine the detector center for crystallography data processing."
 authors = ["Ana Rodrigues <ana.rodrigues@desy.de>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bblib-2.0.0/PKG-INFO` & `bblib-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblib
-Version: 2.0.0
+Version: 2.0.1
 Summary: beambusters library to refine the detector center for crystallography data processing.
 License: GNU
 Author: Ana Rodrigues
 Author-email: ana.rodrigues@desy.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -198,15 +198,23 @@
 ```
 
 The methods `FriedelPairs`, `MinimizePeakFWHM` and  `CircleDetection ` need a `plots_info` parameter if you want to save plots:
 ```python
 plots_info =  {
 	"file_name": ...,
 	"folder_name": ...,
-	"root_path": ...
+	"root_path": ...,
+	"value_auto": ...,
+	"value_max": ...,
+	"value_min": ...,
+	"axis_lim_auto": ...,
+	"xlim_min": ...,
+	"xlim_max": ...,
+	"ylim_min": ...,
+	"ylim_max": ...
 }
 ```
 To calculate the refined detector center of raw data frame as a numpy array using the following methods: 
 
 ```python
 from bblib.methods import CenterOfMass
 center_of_mass_method = CenterOfMass(config=config, PF8Config=PF8Config, plots_info=plots_info)
```

