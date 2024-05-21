# Comparing `tmp/grass_gis_helpers-1.1.0.tar.gz` & `tmp/grass_gis_helpers-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grass_gis_helpers-1.1.0.tar", last modified: Wed Apr 24 13:39:11 2024, max compression
+gzip compressed data, was "grass_gis_helpers-1.2.0.tar", last modified: Tue May 21 11:14:57 2024, max compression
```

## Comparing `grass_gis_helpers-1.1.0.tar` & `grass_gis_helpers-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-24 13:39:06.000000 grass_gis_helpers-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.941000 grass_gis_helpers-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/mapset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/download_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/tiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:14:57.046461 grass_gis_helpers-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 11:14:57.046461 grass_gis_helpers-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-21 11:14:50.000000 grass_gis_helpers-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:14:57.046461 grass_gis_helpers-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:14:57.042461 grass_gis_helpers-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:14:57.046461 grass_gis_helpers-1.2.0/src/grass_gis_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/mapset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:14:57.046461 grass_gis_helpers-1.2.0/src/grass_gis_helpers/open_geodata_germany/
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/open_geodata_germany/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/tiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-21 11:13:53.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:14:57.046461 grass_gis_helpers-1.2.0/src/grass_gis_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 11:14:57.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-21 11:14:57.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:14:57.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 11:14:57.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 11:14:57.000000 grass_gis_helpers-1.2.0/src/grass_gis_helpers.egg-info/top_level.txt
```

### Comparing `grass_gis_helpers-1.1.0/LICENSE` & `grass_gis_helpers-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/PKG-INFO` & `grass_gis_helpers-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grass_gis_helpers
-Version: 1.1.0
+Version: 1.2.0
 Summary: This library provides functions which can be used for developing GRASS GIS addons.
 Author-email: Anika Weinmann <weinmann@mundialis.de>
 Maintainer-email: "mundialis GmbH & Co. KG" <info@mundialis.de>
 Project-URL: Homepage, https://github.com/mundialis/grass-gis-helpers
 Project-URL: Bug Tracker, https://github.com/mundialis/grass-gis-helpers/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grass_gis_helpers-1.1.0/README.md` & `grass_gis_helpers-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/pyproject.toml` & `grass_gis_helpers-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grass_gis_helpers"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Anika Weinmann", email="weinmann@mundialis.de" },
 ]
 maintainers = [{name="mundialis GmbH & Co. KG", email="info@mundialis.de"}]
 description = "This library provides functions which can be used for developing GRASS GIS addons."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/cleanup.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/cleanup.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,21 +60,23 @@
     for rmfile in rm_files:
         if os.path.isfile(rmfile):
             os.remove(rmfile)
     for rmdir in rm_dirs:
         if os.path.isdir(rmdir):
             shutil.rmtree(rmdir)
     if orig_region is not None:
-        if grass.find_file(name=orig_region, element="windows")["file"]:
+        find_reg = grass.find_file(name=orig_region, element="windows")
+        if "file" in find_reg and find_reg["file"]:
             grass.run_command("g.region", region=orig_region)
             grass.run_command(
                 "g.remove", type="region", name=orig_region, **kwargs
             )
     for rmreg in rm_regions:
-        if grass.find_file(name=rmreg, element="windows")["file"]:
+        find_reg = grass.find_file(name=rmreg, element="windows")
+        if "file" in find_reg and find_reg["file"]:
             grass.run_command("g.remove", type="region", name=rmreg, **kwargs)
     strds = grass.parse_command("t.list", type="strds")
     mapset = grass.gisenv()["MAPSET"]
     for rm_s in rm_strds:
         if f"{rm_s}@{mapset}" in strds:
             grass.run_command(
                 "t.remove",
```

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/data_import.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/data_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,19 +213,20 @@
             imported_local_data = True
     elif len(all_raster) > 0:
         imported_local_data = True
 
     return imported_local_data
 
 
-def get_xyz_file_infos(xyz_file):
+def get_xyz_file_infos(xyz_file, separator="space"):
     """Get the infos of a XYZ file to resolution, bounding box and pixelcenter
 
     Args:
         xyz_file (str): XYZ file path to import
+        separator (str): Separator of XYZ file; default is "space"
     Returns:
         res (float): Resolution of the XYZ file
         xyz_reg (dict): Dictionary with region of the XYZ file
         shift_needed (bool): Boolean if the XYZ file hat to be shifted
     """
     gdalinfo_cmd = ["gdalinfo", xyz_file]
     process = grass.Popen(gdalinfo_cmd, stdout=PIPE, stderr=PIPE)
@@ -260,65 +261,84 @@
         shift_needed = False
     # get region to xyz file
     xyz_reg_str = grass.read_command(
         "r.in.xyz",
         output="dummy",
         input=xyz_file,
         flags="sg",
-        separator="space",
+        separator=separator,
     )
     xyz_reg = {
         item.split("=")[0]: float(item.split("=")[1])
         for item in xyz_reg_str.strip().split(" ")
     }
     xyz_reg["n"] += half_res
     xyz_reg["s"] -= half_res
     xyz_reg["w"] -= half_res
     xyz_reg["e"] += half_res
     return res, xyz_reg, shift_needed
 
 
-def import_single_local_xyz_file(xyz_file, output, use_cur_reg=False):
+def import_single_local_xyz_file(
+    xyz_file, output, use_cur_reg=False, separator="space"
+):
     """Import single XYZ file
 
     Args:
         xyz_file (str): XYZ file path to import
         output (str): Output raster file name
         use_cur_reg (bool): If True the XYZ file will only be imported if it
                             overlaps with the current region, otherwise it
                             will not be imported
+        separator (str): Separator of XYZ file; default is "space"
     Returns:
         output (str): If the output is imported, otherwise return None
     """
-    res, xyz_reg, shift_needed = get_xyz_file_infos(xyz_file)
+    res, xyz_reg, shift_needed = get_xyz_file_infos(
+        xyz_file, separator=separator
+    )
     # check if aoi overlaps
     if use_cur_reg:
         cur_reg = grass.region()
         if (
             cur_reg["e"] < xyz_reg["w"]
             or xyz_reg["e"] < cur_reg["w"]
             or cur_reg["n"] < xyz_reg["s"]
             or xyz_reg["n"] < cur_reg["s"]
         ):
             return None
-    # import data
+    # set region
     grass.run_command(
         "g.region",
         n=xyz_reg["n"],
         s=xyz_reg["s"],
         w=xyz_reg["w"],
         e=xyz_reg["e"],
         res=res,
     )
+    if use_cur_reg:
+        while (cur_reg["n"] + res) < xyz_reg["n"]:
+            grass.run_command("g.region", n=f"n-{res}")
+            xyz_reg["n"] -= res
+        while (cur_reg["s"] - res) > xyz_reg["s"]:
+            grass.run_command("g.region", s=f"s+{res}")
+            xyz_reg["s"] += res
+        while (cur_reg["e"] + res) < xyz_reg["e"]:
+            grass.run_command("g.region", e=f"e-{res}")
+            xyz_reg["e"] -= res
+        while (cur_reg["w"] - res) > xyz_reg["w"]:
+            grass.run_command("g.region", w=f"w+{res}")
+            xyz_reg["w"] += res
+    # import data
     grass.run_command(
         "r.in.xyz",
         input=xyz_file,
         output=output,
         method="mean",
-        separator="space",
+        separator=separator,
         quiet=True,
         overwrite=True,
     )
     # shift data if needed
     if shift_needed:
         grass.run_command(
             "g.region",
```

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/general.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         )
         grass.warning(_(f"Set used memory to {free_ram} MB."))
         return free_ram
     else:
         return memory
 
 
-def check_installed_addon(addon, url):
+def check_installed_addon(addon, url="..."):
     """Check if addon is already installed and raise error if not.
     Args:
         addon(string): Addon to check if it is installed
         url(string): Path to addon
     """
     if not grass.find_program(addon, "--help"):
         msg = (
```

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/location.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/location.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/mapset.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/mapset.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/download_data.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/open_geodata_germany/download_data.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/parallel.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/parallel.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/raster.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/raster.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/tiling.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/tiling.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/validation.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/validation.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers/vector.py` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers/vector.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/PKG-INFO` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grass_gis_helpers
-Version: 1.1.0
+Version: 1.2.0
 Summary: This library provides functions which can be used for developing GRASS GIS addons.
 Author-email: Anika Weinmann <weinmann@mundialis.de>
 Maintainer-email: "mundialis GmbH & Co. KG" <info@mundialis.de>
 Project-URL: Homepage, https://github.com/mundialis/grass-gis-helpers
 Project-URL: Bug Tracker, https://github.com/mundialis/grass-gis-helpers/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/SOURCES.txt` & `grass_gis_helpers-1.2.0/src/grass_gis_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

