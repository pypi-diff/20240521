# Comparing `tmp/ecoviewer-0.1.2.tar.gz` & `tmp/ecoviewer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoviewer-0.1.2.tar", last modified: Mon May 13 22:36:56 2024, max compression
+gzip compressed data, was "ecoviewer-0.1.3.tar", last modified: Tue May 21 18:46:57 2024, max compression
```

## Comparing `ecoviewer-0.1.2.tar` & `ecoviewer-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:36:56.224863 ecoviewer-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 22:36:56.224863 ecoviewer-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-13 22:36:56.228863 ecoviewer-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:36:56.224863 ecoviewer-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:36:56.224863 ecoviewer-0.1.2/src/ecoviewer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/src/ecoviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:36:56.224863 ecoviewer-0.1.2/src/ecoviewer/config/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/src/ecoviewer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/src/ecoviewer/config/configutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:36:56.224863 ecoviewer-0.1.2/src/ecoviewer/display/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/src/ecoviewer/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/src/ecoviewer/display/displayutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23365 2024-05-13 22:36:30.000000 ecoviewer-0.1.2/src/ecoviewer/display/graphutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:36:56.224863 ecoviewer-0.1.2/src/ecoviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 22:36:56.000000 ecoviewer-0.1.2/src/ecoviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-13 22:36:56.000000 ecoviewer-0.1.2/src/ecoviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:36:56.000000 ecoviewer-0.1.2/src/ecoviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 22:36:56.000000 ecoviewer-0.1.2/src/ecoviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 22:36:56.000000 ecoviewer-0.1.2/src/ecoviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:46:57.454235 ecoviewer-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-21 18:46:57.454235 ecoviewer-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-21 18:46:57.454235 ecoviewer-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:46:57.450235 ecoviewer-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:46:57.450235 ecoviewer-0.1.3/src/ecoviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/src/ecoviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:46:57.454235 ecoviewer-0.1.3/src/ecoviewer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/src/ecoviewer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/src/ecoviewer/config/configutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:46:57.454235 ecoviewer-0.1.3/src/ecoviewer/display/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/src/ecoviewer/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/src/ecoviewer/display/displayutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23365 2024-05-21 18:46:30.000000 ecoviewer-0.1.3/src/ecoviewer/display/graphutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:46:57.454235 ecoviewer-0.1.3/src/ecoviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-21 18:46:57.000000 ecoviewer-0.1.3/src/ecoviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-21 18:46:57.000000 ecoviewer-0.1.3/src/ecoviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:46:57.000000 ecoviewer-0.1.3/src/ecoviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 18:46:57.000000 ecoviewer-0.1.3/src/ecoviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 18:46:57.000000 ecoviewer-0.1.3/src/ecoviewer.egg-info/top_level.txt
```

### Comparing `ecoviewer-0.1.2/LICENSE` & `ecoviewer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.1.2/PKG-INFO` & `ecoviewer-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecoviewer-0.1.2/setup.cfg` & `ecoviewer-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoviewer
-version = 0.1.2
+version = 0.1.3
 authors = ["Ecotope"]
 description = Contains functions for use in HVAC Dash applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoviewer-0.1.2/src/ecoviewer/config/configutils.py` & `ecoviewer-0.1.3/src/ecoviewer/config/configutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         if exclude_csv_only_fields:
             field_query = f"{field_query} AND graph_id IS NOT NULL" 
         
         cursor.execute(field_query, table_names)
         result = cursor.fetchall()
         column_names = [desc[0] for desc in cursor.description]
         field_df = pd.DataFrame(result, columns=column_names)
-        print("field df length", len(field_df.index))
 
     cursor.close()
     cnx.close()
 
     display_drop_down = []
     for name in table_names:
         display_drop_down.append({'label': site_df.loc[name, "pretty_name"], 'value' : name})
```

### Comparing `ecoviewer-0.1.2/src/ecoviewer/display/displayutils.py` & `ecoviewer-0.1.3/src/ecoviewer/display/displayutils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,44 @@
 import plotly.graph_objects as go
 from dash import dcc, html, Dash, dash_table
 from ecoviewer.config import get_organized_mapping
 
 def create_meta_data_table(site_df : pd.DataFrame, selected_table : str, app : Dash, anonymize_data : bool = True):
     wh_unit_name = site_df.loc[selected_table, 'wh_unit_name']
     wh_manufacturer = site_df.loc[selected_table, 'wh_manufacturer']
+    primary_model = None
+    if not wh_manufacturer is None and not wh_unit_name is None:
+        primary_model = f"{wh_manufacturer} {wh_unit_name}"
+    elif not wh_manufacturer is None:
+         primary_model = f"{wh_manufacturer}"
+    elif not wh_unit_name is None:
+         primary_model = f"{wh_unit_name}"
     swing_tank_volume = site_df.loc[selected_table, 'swing_tank_volume']
     zip_code = site_df.loc[selected_table, 'zip_code']
     swing_t_elem = site_df.loc[selected_table, 'swing_element_kw']
     primary_volume = site_df.loc[selected_table, 'tank_size_gallons']
+    installation_year = site_df.loc[selected_table, 'unit_installation_year']
+    building_specs = "Unknown"
+    if site_df.loc[selected_table, 'building_specs'] is not None:
+        building_specs = site_df.loc[selected_table, 'building_specs']
+    elif site_df.loc[selected_table, 'building_type'] is not None:
+        building_specs = site_df.loc[selected_table, 'building_type']
 
     mapping = {
         "Address" : site_df.loc[selected_table, 'address'] if site_df.loc[selected_table, 'address'] is not None else "Unknown", 
         "Zip Code" : zip_code if not (zip_code is None or pd.isna(zip_code)) else "Unknown",
-        "Building Specifications" : site_df.loc[selected_table, 'building_specs'] if site_df.loc[selected_table, 'building_specs'] is not None else "Unknown", 
-        "Primary System Model" : f"{wh_manufacturer} {wh_unit_name}" if not wh_manufacturer is None and not wh_unit_name is None else None, 
+        "Building Specifications/Type" : building_specs, 
+        "Primary System Model" : primary_model, 
         "Primary HPWHs" : site_df.loc[selected_table, 'number_heat_pumps'], 
         "Primary Tank Volume" : f"{primary_volume} Gallons" if not (primary_volume is None or pd.isna(primary_volume)) else None, 
         "Swing Tank Element" : f"{swing_t_elem} kW" if not (swing_t_elem is None or pd.isna(swing_t_elem)) else None, 
         "Temperature Maintenance Storage Volume" : f"{swing_tank_volume} Gallons" if not (swing_tank_volume is None or pd.isna(swing_tank_volume)) else None,
-        "Schematic Drawing": f"![]({app.get_asset_url('schematic-swingtank.jpg')})" if not (swing_tank_volume is None or pd.isna(swing_tank_volume)) else None
+        "Schematic Drawing": f"![]({app.get_asset_url('schematic-swingtank.jpg')})" if not (swing_tank_volume is None or pd.isna(swing_tank_volume)) else None,
+        "Installation Year" : installation_year if not (installation_year is None or pd.isna(installation_year)) else None,
+        "Operation Hours" : site_df.loc[selected_table, 'operation_hours'] if site_df.loc[selected_table, 'operation_hours'] is not None else None,
     }
 
     if anonymize_data:
         mapping['Address'] = None
 
 
     detail = []
```

### Comparing `ecoviewer-0.1.2/src/ecoviewer/display/graphutils.py` & `ecoviewer-0.1.3/src/ecoviewer/display/graphutils.py`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.1.2/src/ecoviewer.egg-info/PKG-INFO` & `ecoviewer-0.1.3/src/ecoviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

