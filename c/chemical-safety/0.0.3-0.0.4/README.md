# Comparing `tmp/chemical_safety-0.0.3.tar.gz` & `tmp/chemical_safety-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemical_safety-0.0.3.tar", last modified: Tue May 21 16:17:41 2024, max compression
+gzip compressed data, was "chemical_safety-0.0.4.tar", last modified: Tue May 21 16:22:30 2024, max compression
```

## Comparing `chemical_safety-0.0.3.tar` & `chemical_safety-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/
--rw-rw-rw-   0        0        0     1095 2024-02-03 21:17:28.000000 chemical_safety-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      679 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-05-21 16:01:33.000000 chemical_safety-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety/
--rw-rw-rw-   0        0        0       66 2024-05-18 17:22:12.000000 chemical_safety-0.0.3/chemical_safety/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety/chemical/
--rw-rw-rw-   0        0        0       30 2024-05-18 16:55:19.000000 chemical_safety-0.0.3/chemical_safety/chemical/__init__.py
--rw-rw-rw-   0        0        0    38858 2024-05-21 15:58:58.000000 chemical_safety-0.0.3/chemical_safety/chemical/chemical.py
--rw-rw-rw-   0        0        0    11694 2024-05-03 04:13:48.000000 chemical_safety-0.0.3/chemical_safety/chemical/molecule.py
--rw-rw-rw-   0        0        0     5474 2024-03-11 02:03:14.000000 chemical_safety-0.0.3/chemical_safety/chemical/periodictable.py
--rw-rw-rw-   0        0        0    14908 2024-05-03 04:14:07.000000 chemical_safety-0.0.3/chemical_safety/chemical/sigfig.py
--rw-rw-rw-   0        0        0     8223 2024-02-12 03:32:32.000000 chemical_safety-0.0.3/chemical_safety/chemical/units.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety/dashboard/
--rw-rw-rw-   0        0        0       26 2024-05-18 17:22:03.000000 chemical_safety-0.0.3/chemical_safety/dashboard/__init__.py
--rw-rw-rw-   0        0        0    11776 2024-05-20 22:51:02.000000 chemical_safety-0.0.3/chemical_safety/dashboard/app.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety.egg-info/
--rw-rw-rw-   0        0        0      679 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      825 2024-05-21 16:17:19.000000 chemical_safety-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:22:30.000000 chemical_safety-0.0.4/
+-rw-rw-rw-   0        0        0     1095 2024-02-03 21:17:28.000000 chemical_safety-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      317 2024-05-21 16:21:24.000000 chemical_safety-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      679 2024-05-21 16:22:30.000000 chemical_safety-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2024-05-21 16:01:33.000000 chemical_safety-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 16:22:30.000000 chemical_safety-0.0.4/chemical_safety/
+-rw-rw-rw-   0        0        0       66 2024-05-18 17:22:12.000000 chemical_safety-0.0.4/chemical_safety/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:22:28.000000 chemical_safety-0.0.4/chemical_safety/chemical/
+-rw-rw-rw-   0        0        0       30 2024-05-18 16:55:19.000000 chemical_safety-0.0.4/chemical_safety/chemical/__init__.py
+-rw-rw-rw-   0        0        0    38858 2024-05-21 15:58:58.000000 chemical_safety-0.0.4/chemical_safety/chemical/chemical.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:22:25.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/
+-rw-rw-rw-   0        0        0     1219 2024-04-23 16:19:23.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/EPA_D_List.csv
+-rw-rw-rw-   0        0        0    25593 2024-04-23 16:19:39.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/EPA_P_List.csv
+-rw-rw-rw-   0        0        0    46891 2024-04-23 16:20:09.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/EPA_U_List.csv
+-rw-rw-rw-   0        0        0    83466 2024-02-02 04:14:29.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/IARC_classification.csv
+-rw-rw-rw-   0        0        0     5163 2024-02-01 23:04:11.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/NTP_anticipated_carcinogens.csv
+-rw-rw-rw-   0        0        0      941 2024-02-01 23:03:51.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/NTP_known_carcinogens.csv
+-rw-rw-rw-   0        0        0      349 2024-02-02 00:04:46.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/OSHA_carcinogens.csv
+-rw-rw-rw-   0        0        0     2610 2024-04-21 20:25:07.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/UMN_peroxide_formers.csv
+-rw-rw-rw-   0        0        0    10379 2024-04-15 20:21:48.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/p_statements.csv
+-rw-rw-rw-   0        0        0    11694 2024-05-03 04:13:48.000000 chemical_safety-0.0.4/chemical_safety/chemical/molecule.py
+-rw-rw-rw-   0        0        0     5474 2024-03-11 02:03:14.000000 chemical_safety-0.0.4/chemical_safety/chemical/periodictable.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:22:28.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/
+-rw-rw-rw-   0        0        0    12588 2023-11-06 22:41:50.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Acute Toxic.svg
+-rw-rw-rw-   0        0        0     1446 2023-11-06 22:41:50.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Compressed Gas.svg
+-rw-rw-rw-   0        0        0    13531 2023-11-06 22:41:50.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Corrosive.svg
+-rw-rw-rw-   0        0        0     5466 2023-11-06 22:41:52.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Environmental Hazard.svg
+-rw-rw-rw-   0        0        0    11902 2023-11-06 22:41:48.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Explosive.svg
+-rw-rw-rw-   0        0        0     2526 2023-11-06 22:41:48.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Flammable.svg
+-rw-rw-rw-   0        0        0    15192 2023-11-06 22:41:52.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Health Hazard.svg
+-rw-rw-rw-   0        0        0     1675 2023-11-06 22:41:52.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Irritant.svg
```

### Comparing `chemical_safety-0.0.3/LICENSE` & `chemical_safety-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.3/PKG-INFO` & `chemical_safety-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemical_safety
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for retreiving chemical safety information
 Author: Demetrios Pagonis
 Author-email: demetriospagonis@weber.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chemical_safety
```

### Comparing `chemical_safety-0.0.3/chemical_safety/chemical/chemical.py` & `chemical_safety-0.0.4/chemical_safety/chemical/chemical.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.3/chemical_safety/chemical/molecule.py` & `chemical_safety-0.0.4/chemical_safety/chemical/molecule.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.3/chemical_safety/chemical/periodictable.py` & `chemical_safety-0.0.4/chemical_safety/chemical/periodictable.py`

 * *Files identical despite different names*

