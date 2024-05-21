# Comparing `tmp/chemical_safety-0.0.6.tar.gz` & `tmp/chemical_safety-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemical_safety-0.0.6.tar", last modified: Tue May 21 18:36:13 2024, max compression
+gzip compressed data, was "chemical_safety-0.0.7.tar", last modified: Tue May 21 19:57:55 2024, max compression
```

## Comparing `chemical_safety-0.0.6.tar` & `chemical_safety-0.0.7.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:13.000000 chemical_safety-0.0.6/
--rw-rw-rw-   0        0        0     1095 2024-02-03 21:17:28.000000 chemical_safety-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      389 2024-05-21 18:30:23.000000 chemical_safety-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      735 2024-05-21 18:36:13.000000 chemical_safety-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-05-21 16:01:33.000000 chemical_safety-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:13.000000 chemical_safety-0.0.6/chemical_safety/
--rw-rw-rw-   0        0        0       66 2024-05-18 17:22:12.000000 chemical_safety-0.0.6/chemical_safety/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:11.000000 chemical_safety-0.0.6/chemical_safety/chemical/
--rw-rw-rw-   0        0        0       30 2024-05-18 16:55:19.000000 chemical_safety-0.0.6/chemical_safety/chemical/__init__.py
--rw-rw-rw-   0        0        0    39290 2024-05-21 18:28:35.000000 chemical_safety-0.0.6/chemical_safety/chemical/chemical.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:11.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/
--rw-rw-rw-   0        0        0     1219 2024-04-23 16:19:23.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/EPA_D_List.csv
--rw-rw-rw-   0        0        0    25593 2024-04-23 16:19:39.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/EPA_P_List.csv
--rw-rw-rw-   0        0        0    46891 2024-04-23 16:20:09.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/EPA_U_List.csv
--rw-rw-rw-   0        0        0    83466 2024-02-02 04:14:29.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/IARC_classification.csv
--rw-rw-rw-   0        0        0     5163 2024-02-01 23:04:11.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/NTP_anticipated_carcinogens.csv
--rw-rw-rw-   0        0        0      941 2024-02-01 23:03:51.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/NTP_known_carcinogens.csv
--rw-rw-rw-   0        0        0      349 2024-02-02 00:04:46.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/OSHA_carcinogens.csv
--rw-rw-rw-   0        0        0     2610 2024-04-21 20:25:07.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/UMN_peroxide_formers.csv
--rw-rw-rw-   0        0        0     1948 2024-04-21 20:24:51.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/convert_UMN_peroxide_list.py
--rw-rw-rw-   0        0        0     1094 2024-04-15 20:21:47.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/convert_p_statements.py
--rw-rw-rw-   0        0        0    10379 2024-04-15 20:21:48.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/p_statements.csv
--rw-rw-rw-   0        0        0     1309 2024-04-23 16:07:29.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/process_EPA_lists.py
--rw-rw-rw-   0        0        0      317 2024-02-03 21:21:07.000000 chemical_safety-0.0.6/chemical_safety/chemical/lists/process_lists.py
--rw-rw-rw-   0        0        0    11694 2024-05-03 04:13:48.000000 chemical_safety-0.0.6/chemical_safety/chemical/molecule.py
--rw-rw-rw-   0        0        0     5474 2024-03-11 02:03:14.000000 chemical_safety-0.0.6/chemical_safety/chemical/periodictable.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:11.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/
--rw-rw-rw-   0        0        0    12588 2023-11-06 22:41:50.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Acute Toxic.svg
--rw-rw-rw-   0        0        0     1446 2023-11-06 22:41:50.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Compressed Gas.svg
--rw-rw-rw-   0        0        0    13531 2023-11-06 22:41:50.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Corrosive.svg
--rw-rw-rw-   0        0        0     5466 2023-11-06 22:41:52.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Environmental Hazard.svg
--rw-rw-rw-   0        0        0    11902 2023-11-06 22:41:48.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Explosive.svg
--rw-rw-rw-   0        0        0     2526 2023-11-06 22:41:48.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Flammable.svg
--rw-rw-rw-   0        0        0    15192 2023-11-06 22:41:52.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Health Hazard.svg
--rw-rw-rw-   0        0        0     1675 2023-11-06 22:41:52.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Irritant.svg
--rw-rw-rw-   0        0        0     3336 2023-11-06 22:41:50.000000 chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Oxidizing.svg
--rw-rw-rw-   0        0        0    14908 2024-05-03 04:14:07.000000 chemical_safety-0.0.6/chemical_safety/chemical/sigfig.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:11.000000 chemical_safety-0.0.6/chemical_safety/chemical/tables/
--rw-rw-rw-   0        0        0 15139689 2023-04-13 19:24:30.000000 chemical_safety-0.0.6/chemical_safety/chemical/tables/elements.csv
--rw-rw-rw-   0        0        0     8223 2024-02-12 03:32:32.000000 chemical_safety-0.0.6/chemical_safety/chemical/units.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:13.000000 chemical_safety-0.0.6/chemical_safety/dashboard/
--rw-rw-rw-   0        0        0       26 2024-05-18 17:22:03.000000 chemical_safety-0.0.6/chemical_safety/dashboard/__init__.py
--rw-rw-rw-   0        0        0    11776 2024-05-20 22:51:02.000000 chemical_safety-0.0.6/chemical_safety/dashboard/app.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:13.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:12.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:12.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/
--rw-rw-rw-   0        0        0       57 2024-05-01 15:05:10.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/1 Crystallization & Melting Points.txt
--rw-rw-rw-   0        0        0      131 2024-05-01 15:26:01.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/10 Oxidation of Cyclohexanol.txt
--rw-rw-rw-   0        0        0      222 2024-05-01 15:08:11.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/2 Identification of Unkown Alkanes and Alkenes.txt
--rw-rw-rw-   0        0        0      223 2024-05-01 15:14:23.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/3 Free Radical Chlorination of 1-Chlorobutane.txt
--rw-rw-rw-   0        0        0      101 2024-05-01 15:26:11.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/30 Separation of Binary Mixtures by Fractional Distillation.txt
--rw-rw-rw-   0        0        0       30 2024-05-01 15:09:04.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/4 Optical Activity of Caraway and Spearmint Oils.txt
--rw-rw-rw-   0        0        0       68 2024-05-01 15:15:28.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/5 Preparation of Phenacetin by the Williamson Ether Synthesis.txt
--rw-rw-rw-   0        0        0      103 2024-05-01 15:23:36.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/6 Synthesis of 3_3-Dimethyl-2-Butanol.txt
--rw-rw-rw-   0        0        0      110 2024-05-01 15:17:39.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/7 Dehydration of 3_3-Dimethyl-2-butanol.txt
--rw-rw-rw-   0        0        0      124 2024-05-01 15:18:00.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/8 Identification of an Unknown by Infrared Spectroscopy.txt
--rw-rw-rw-   0        0        0       18 2024-05-01 15:21:45.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2315/9 Steam Distillation of Orange Oil.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:12.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2325/
--rw-rw-rw-   0        0        0      121 2024-04-24 14:50:11.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM2325/16 Preparation of Benzoic Acid from Phenylmagnesium Bromide and Carbon Dioxide.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:12.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM3000/
--rw-rw-rw-   0        0        0        5 2024-04-24 14:27:57.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM3000/1 Calibration of glassware.txt
--rw-rw-rw-   0        0        0       35 2024-04-24 14:28:54.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM3000/2 Determination of total acidity.txt
--rw-rw-rw-   0        0        0       93 2024-04-24 14:28:52.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM3000/4 Determination of chloride.txt
--rw-rw-rw-   0        0        0       22 2024-04-24 14:29:10.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM3000/5 Beers law.txt
--rw-rw-rw-   0        0        0      100 2024-04-24 14:30:13.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM3000/6 Determination of manganese in steel.txt
--rw-rw-rw-   0        0        0       26 2024-04-24 14:31:57.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM3000/7 GCMS of gasoline.txt
--rw-rw-rw-   0        0        0       32 2024-04-24 14:31:34.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/courses/CHEM3000/8 Simultaneous determination of a two-component mixture.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:12.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/css/
--rw-rw-rw-   0        0        0     2318 2024-05-21 15:02:17.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/css/style.css
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:13.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/
--rw-rw-rw-   0        0        0    12588 2023-11-06 22:41:50.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Acute Toxic.svg
--rw-rw-rw-   0        0        0     1446 2023-11-06 22:41:50.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Compressed Gas.svg
--rw-rw-rw-   0        0        0    13531 2023-11-06 22:41:50.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Corrosive.svg
--rw-rw-rw-   0        0        0     5466 2023-11-06 22:41:52.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Environmental Hazard.svg
--rw-rw-rw-   0        0        0    11902 2023-11-06 22:41:48.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Explosive.svg
--rw-rw-rw-   0        0        0     2526 2023-11-06 22:41:48.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Flammable.svg
--rw-rw-rw-   0        0        0    15192 2023-11-06 22:41:52.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Health Hazard.svg
--rw-rw-rw-   0        0        0     1675 2023-11-06 22:41:52.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Irritant.svg
--rw-rw-rw-   0        0        0     3336 2023-11-06 22:41:50.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Oxidizer.svg
--rw-rw-rw-   0        0        0     3336 2023-11-06 22:41:50.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Oxidizing.svg
--rw-rw-rw-   0        0        0    26469 2024-04-12 12:02:11.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/PHS.png
--rw-rw-rw-   0        0        0    62940 2018-08-07 13:52:30.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/chembio_horiz.png
--rw-rw-rw-   0        0        0    10665 2024-02-08 21:28:49.000000 chemical_safety-0.0.6/chemical_safety/dashboard/static/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:13.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/
--rw-rw-rw-   0        0        0     4405 2024-05-21 15:52:31.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/chemical_lookup.html
--rw-rw-rw-   0        0        0     4289 2024-05-01 16:04:04.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/course_lookup.html
--rw-rw-rw-   0        0        0      884 2024-04-22 11:55:12.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/emergency_info.html
--rw-rw-rw-   0        0        0     3125 2024-05-01 16:03:54.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/experiment_lookup.html
--rw-rw-rw-   0        0        0     1482 2024-04-24 20:47:41.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/index.html
--rw-rw-rw-   0        0        0     3129 2024-05-20 22:51:03.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/multi_chemical_lookup.html
--rw-rw-rw-   0        0        0      897 2024-04-22 11:55:40.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/phs_list.html
--rw-rw-rw-   0        0        0      889 2024-04-22 11:55:49.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/room_lookup.html
--rw-rw-rw-   0        0        0     1519 2024-04-24 20:55:34.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/search_form.html
--rw-rw-rw-   0        0        0     2343 2024-05-20 22:51:03.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/secondary_label.html
--rw-rw-rw-   0        0        0     3722 2024-05-20 22:51:03.000000 chemical_safety-0.0.6/chemical_safety/dashboard/templates/secondary_label_builder.html
-drwxrwxrwx   0        0        0        0 2024-05-21 18:36:10.000000 chemical_safety-0.0.6/chemical_safety.egg-info/
--rw-rw-rw-   0        0        0      735 2024-05-21 18:36:06.000000 chemical_safety-0.0.6/chemical_safety.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4957 2024-05-21 18:36:10.000000 chemical_safety-0.0.6/chemical_safety.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 18:36:06.000000 chemical_safety-0.0.6/chemical_safety.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-21 18:36:06.000000 chemical_safety-0.0.6/chemical_safety.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2024-05-21 18:36:06.000000 chemical_safety-0.0.6/chemical_safety.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-21 18:36:06.000000 chemical_safety-0.0.6/chemical_safety.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10665 2024-02-08 21:28:49.000000 chemical_safety-0.0.6/logo.png
--rw-rw-rw-   0        0        0       42 2024-05-21 18:36:13.000000 chemical_safety-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      883 2024-05-21 18:34:10.000000 chemical_safety-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:55.000000 chemical_safety-0.0.7/
+-rw-rw-rw-   0        0        0     1095 2024-02-03 21:17:28.000000 chemical_safety-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      389 2024-05-21 18:30:23.000000 chemical_safety-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      781 2024-05-21 19:57:55.000000 chemical_safety-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-05-21 19:00:17.000000 chemical_safety-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:55.000000 chemical_safety-0.0.7/chemical_safety/
+-rw-rw-rw-   0        0        0       66 2024-05-18 17:22:12.000000 chemical_safety-0.0.7/chemical_safety/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:54.000000 chemical_safety-0.0.7/chemical_safety/chemical/
+-rw-rw-rw-   0        0        0       30 2024-05-18 16:55:19.000000 chemical_safety-0.0.7/chemical_safety/chemical/__init__.py
+-rw-rw-rw-   0        0        0    39290 2024-05-21 18:28:35.000000 chemical_safety-0.0.7/chemical_safety/chemical/chemical.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:53.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/
+-rw-rw-rw-   0        0        0     1219 2024-04-23 16:19:23.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/EPA_D_List.csv
+-rw-rw-rw-   0        0        0    25593 2024-04-23 16:19:39.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/EPA_P_List.csv
+-rw-rw-rw-   0        0        0    46891 2024-04-23 16:20:09.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/EPA_U_List.csv
+-rw-rw-rw-   0        0        0    83466 2024-02-02 04:14:29.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/IARC_classification.csv
+-rw-rw-rw-   0        0        0     5163 2024-02-01 23:04:11.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/NTP_anticipated_carcinogens.csv
+-rw-rw-rw-   0        0        0      941 2024-02-01 23:03:51.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/NTP_known_carcinogens.csv
+-rw-rw-rw-   0        0        0      349 2024-02-02 00:04:46.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/OSHA_carcinogens.csv
+-rw-rw-rw-   0        0        0     2610 2024-04-21 20:25:07.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/UMN_peroxide_formers.csv
+-rw-rw-rw-   0        0        0     1948 2024-04-21 20:24:51.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/convert_UMN_peroxide_list.py
+-rw-rw-rw-   0        0        0     1094 2024-04-15 20:21:47.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/convert_p_statements.py
+-rw-rw-rw-   0        0        0    10379 2024-04-15 20:21:48.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/p_statements.csv
+-rw-rw-rw-   0        0        0     1309 2024-04-23 16:07:29.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/process_EPA_lists.py
+-rw-rw-rw-   0        0        0      317 2024-02-03 21:21:07.000000 chemical_safety-0.0.7/chemical_safety/chemical/lists/process_lists.py
+-rw-rw-rw-   0        0        0    11694 2024-05-03 04:13:48.000000 chemical_safety-0.0.7/chemical_safety/chemical/molecule.py
+-rw-rw-rw-   0        0        0     5474 2024-03-11 02:03:14.000000 chemical_safety-0.0.7/chemical_safety/chemical/periodictable.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:53.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/
+-rw-rw-rw-   0        0        0    12588 2023-11-06 22:41:50.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Acute Toxic.svg
+-rw-rw-rw-   0        0        0     1446 2023-11-06 22:41:50.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Compressed Gas.svg
+-rw-rw-rw-   0        0        0    13531 2023-11-06 22:41:50.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Corrosive.svg
+-rw-rw-rw-   0        0        0     5466 2023-11-06 22:41:52.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Environmental Hazard.svg
+-rw-rw-rw-   0        0        0    11902 2023-11-06 22:41:48.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Explosive.svg
+-rw-rw-rw-   0        0        0     2526 2023-11-06 22:41:48.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Flammable.svg
+-rw-rw-rw-   0        0        0    15192 2023-11-06 22:41:52.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Health Hazard.svg
+-rw-rw-rw-   0        0        0     1675 2023-11-06 22:41:52.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Irritant.svg
+-rw-rw-rw-   0        0        0     3336 2023-11-06 22:41:50.000000 chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Oxidizing.svg
+-rw-rw-rw-   0        0        0    14908 2024-05-03 04:14:07.000000 chemical_safety-0.0.7/chemical_safety/chemical/sigfig.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:54.000000 chemical_safety-0.0.7/chemical_safety/chemical/tables/
+-rw-rw-rw-   0        0        0 15139689 2023-04-13 19:24:30.000000 chemical_safety-0.0.7/chemical_safety/chemical/tables/elements.csv
+-rw-rw-rw-   0        0        0     8223 2024-02-12 03:32:32.000000 chemical_safety-0.0.7/chemical_safety/chemical/units.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:55.000000 chemical_safety-0.0.7/chemical_safety/dashboard/
+-rw-rw-rw-   0        0        0       26 2024-05-18 17:22:03.000000 chemical_safety-0.0.7/chemical_safety/dashboard/__init__.py
+-rw-rw-rw-   0        0        0    13366 2024-05-21 19:53:41.000000 chemical_safety-0.0.7/chemical_safety/dashboard/app.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:55.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:54.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:54.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/
+-rw-rw-rw-   0        0        0       57 2024-05-01 15:05:10.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/1 Crystallization & Melting Points.txt
+-rw-rw-rw-   0        0        0      131 2024-05-01 15:26:01.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/10 Oxidation of Cyclohexanol.txt
+-rw-rw-rw-   0        0        0      222 2024-05-01 15:08:11.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/2 Identification of Unkown Alkanes and Alkenes.txt
+-rw-rw-rw-   0        0        0      223 2024-05-01 15:14:23.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/3 Free Radical Chlorination of 1-Chlorobutane.txt
+-rw-rw-rw-   0        0        0      101 2024-05-01 15:26:11.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/30 Separation of Binary Mixtures by Fractional Distillation.txt
+-rw-rw-rw-   0        0        0       30 2024-05-01 15:09:04.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/4 Optical Activity of Caraway and Spearmint Oils.txt
+-rw-rw-rw-   0        0        0       68 2024-05-01 15:15:28.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/5 Preparation of Phenacetin by the Williamson Ether Synthesis.txt
+-rw-rw-rw-   0        0        0      103 2024-05-01 15:23:36.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/6 Synthesis of 3_3-Dimethyl-2-Butanol.txt
+-rw-rw-rw-   0        0        0      110 2024-05-01 15:17:39.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/7 Dehydration of 3_3-Dimethyl-2-butanol.txt
+-rw-rw-rw-   0        0        0      124 2024-05-01 15:18:00.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/8 Identification of an Unknown by Infrared Spectroscopy.txt
+-rw-rw-rw-   0        0        0       18 2024-05-01 15:21:45.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2315/9 Steam Distillation of Orange Oil.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:54.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2325/
+-rw-rw-rw-   0        0        0      121 2024-04-24 14:50:11.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM2325/16 Preparation of Benzoic Acid from Phenylmagnesium Bromide and Carbon Dioxide.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:54.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM3000/
+-rw-rw-rw-   0        0        0        5 2024-04-24 14:27:57.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM3000/1 Calibration of glassware.txt
+-rw-rw-rw-   0        0        0       35 2024-04-24 14:28:54.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM3000/2 Determination of total acidity.txt
+-rw-rw-rw-   0        0        0       93 2024-04-24 14:28:52.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM3000/4 Determination of chloride.txt
+-rw-rw-rw-   0        0        0       22 2024-04-24 14:29:10.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM3000/5 Beers law.txt
+-rw-rw-rw-   0        0        0      100 2024-04-24 14:30:13.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM3000/6 Determination of manganese in steel.txt
+-rw-rw-rw-   0        0        0       26 2024-04-24 14:31:57.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM3000/7 GCMS of gasoline.txt
+-rw-rw-rw-   0        0        0       32 2024-04-24 14:31:34.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/courses/CHEM3000/8 Simultaneous determination of a two-component mixture.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:54.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/css/
+-rw-rw-rw-   0        0        0     2318 2024-05-21 15:02:17.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/css/style.css
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:55.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/
+-rw-rw-rw-   0        0        0    12588 2023-11-06 22:41:50.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Acute Toxic.svg
+-rw-rw-rw-   0        0        0     1446 2023-11-06 22:41:50.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Compressed Gas.svg
+-rw-rw-rw-   0        0        0    13531 2023-11-06 22:41:50.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Corrosive.svg
+-rw-rw-rw-   0        0        0     5466 2023-11-06 22:41:52.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Environmental Hazard.svg
+-rw-rw-rw-   0        0        0    11902 2023-11-06 22:41:48.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Explosive.svg
+-rw-rw-rw-   0        0        0     2526 2023-11-06 22:41:48.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Flammable.svg
+-rw-rw-rw-   0        0        0    15192 2023-11-06 22:41:52.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Health Hazard.svg
+-rw-rw-rw-   0        0        0     1675 2023-11-06 22:41:52.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Irritant.svg
+-rw-rw-rw-   0        0        0     3336 2023-11-06 22:41:50.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Oxidizer.svg
+-rw-rw-rw-   0        0        0     3336 2023-11-06 22:41:50.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Oxidizing.svg
+-rw-rw-rw-   0        0        0    26469 2024-04-12 12:02:11.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/PHS.png
+-rw-rw-rw-   0        0        0    62940 2018-08-07 13:52:30.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/chembio_horiz.png
+-rw-rw-rw-   0        0        0    10665 2024-02-08 21:28:49.000000 chemical_safety-0.0.7/chemical_safety/dashboard/static/img/logo.png
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:55.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/
+-rw-rw-rw-   0        0        0     4405 2024-05-21 15:52:31.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/chemical_lookup.html
+-rw-rw-rw-   0        0        0     4289 2024-05-01 16:04:04.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/course_lookup.html
+-rw-rw-rw-   0        0        0      884 2024-04-22 11:55:12.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/emergency_info.html
+-rw-rw-rw-   0        0        0     3125 2024-05-01 16:03:54.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/experiment_lookup.html
+-rw-rw-rw-   0        0        0     1482 2024-04-24 20:47:41.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/index.html
+-rw-rw-rw-   0        0        0     3129 2024-05-20 22:51:03.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/multi_chemical_lookup.html
+-rw-rw-rw-   0        0        0      897 2024-04-22 11:55:40.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/phs_list.html
+-rw-rw-rw-   0        0        0      889 2024-04-22 11:55:49.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/room_lookup.html
+-rw-rw-rw-   0        0        0     1519 2024-04-24 20:55:34.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/search_form.html
+-rw-rw-rw-   0        0        0     2343 2024-05-20 22:51:03.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/secondary_label.html
+-rw-rw-rw-   0        0        0     3722 2024-05-20 22:51:03.000000 chemical_safety-0.0.7/chemical_safety/dashboard/templates/secondary_label_builder.html
+drwxrwxrwx   0        0        0        0 2024-05-21 19:57:52.000000 chemical_safety-0.0.7/chemical_safety.egg-info/
+-rw-rw-rw-   0        0        0      781 2024-05-21 19:57:47.000000 chemical_safety-0.0.7/chemical_safety.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4957 2024-05-21 19:57:52.000000 chemical_safety-0.0.7/chemical_safety.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:57:47.000000 chemical_safety-0.0.7/chemical_safety.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-21 19:57:47.000000 chemical_safety-0.0.7/chemical_safety.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2024-05-21 19:57:47.000000 chemical_safety-0.0.7/chemical_safety.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-21 19:57:47.000000 chemical_safety-0.0.7/chemical_safety.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10665 2024-02-08 21:28:49.000000 chemical_safety-0.0.7/logo.png
+-rw-rw-rw-   0        0        0       42 2024-05-21 19:57:55.000000 chemical_safety-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      883 2024-05-21 19:54:03.000000 chemical_safety-0.0.7/setup.py
```

### Comparing `chemical_safety-0.0.6/LICENSE` & `chemical_safety-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/PKG-INFO` & `chemical_safety-0.0.7/chemical_safety.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
-Name: chemical_safety
-Version: 0.0.6
+Name: chemical-safety
+Version: 0.0.7
 Summary: A package for retreiving chemical safety information
 Home-page: https://github.com/dpagonis/chemical_safety
 Author: Demetrios Pagonis
 Author-email: demetriospagonis@weber.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chemical_safety
 This package retrieves and displays SDS, GHS, and regulatory information for chemicals in an academic setting.
 
-## `chemical` class
-chemical_safety.chemical
-stores all GHS info
-recommended for custom applications and development
+`pip install chemical-safety`
+
 
 ## dashboard
 recommended for users who only want to view information
+
 enter command prompt: `chemical-dashboard`
-then access in your browswer at localhost:5000
+
+then access in your browser at http://localhost:5000
+
+## chemical class
+chemical_safety.chemical stores all GHS info
+
+recommended for custom applications and development
+
```

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/chemical.py` & `chemical_safety-0.0.7/chemical_safety/chemical/chemical.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/EPA_D_List.csv` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/EPA_D_List.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/EPA_P_List.csv` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/EPA_P_List.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/EPA_U_List.csv` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/EPA_U_List.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/IARC_classification.csv` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/IARC_classification.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/NTP_anticipated_carcinogens.csv` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/NTP_anticipated_carcinogens.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/NTP_known_carcinogens.csv` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/NTP_known_carcinogens.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/UMN_peroxide_formers.csv` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/UMN_peroxide_formers.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/convert_UMN_peroxide_list.py` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/convert_UMN_peroxide_list.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/convert_p_statements.py` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/convert_p_statements.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/p_statements.csv` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/p_statements.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/lists/process_EPA_lists.py` & `chemical_safety-0.0.7/chemical_safety/chemical/lists/process_EPA_lists.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/molecule.py` & `chemical_safety-0.0.7/chemical_safety/chemical/molecule.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/periodictable.py` & `chemical_safety-0.0.7/chemical_safety/chemical/periodictable.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Acute Toxic.svg` & `chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Acute Toxic.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Compressed Gas.svg` & `chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Compressed Gas.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Corrosive.svg` & `chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Corrosive.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Environmental Hazard.svg` & `chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Environmental Hazard.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Explosive.svg` & `chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Explosive.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Flammable.svg` & `chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Flammable.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Health Hazard.svg` & `chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Health Hazard.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Irritant.svg` & `chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Irritant.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/pictograms/Oxidizing.svg` & `chemical_safety-0.0.7/chemical_safety/chemical/pictograms/Oxidizing.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/sigfig.py` & `chemical_safety-0.0.7/chemical_safety/chemical/sigfig.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/tables/elements.csv` & `chemical_safety-0.0.7/chemical_safety/chemical/tables/elements.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/chemical/units.py` & `chemical_safety-0.0.7/chemical_safety/chemical/units.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/app.py` & `chemical_safety-0.0.7/chemical_safety/dashboard/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,34 @@
 from flask import Flask, render_template, request, redirect, url_for
 import os
+import shutil
 import re
+import json
 from difflib import SequenceMatcher
 from natsort import natsorted
 from datetime import date
 
 from chemical_safety.chemical import chemical
 
+# Define the paths
+package_config_path = os.path.join(os.path.dirname(__file__), 'config.json')
+user_config_dir = os.path.expanduser('~/.chemical_safety')
+user_config_path = os.path.join(user_config_dir, 'config.json')
+
+# Ensure the user config directory exists
+os.makedirs(user_config_dir, exist_ok=True)
+
+# Copy default config to user directory if it doesn't exist
+if not os.path.exists(user_config_path):
+    shutil.copyfile(package_config_path, user_config_path)
+
+# Load configuration
+with open(user_config_path) as config_file:
+    CONFIG = json.load(config_file)
+
 def create_app():
     app = Flask(__name__)
 
     @app.route('/')
     def home():
         return render_template('index.html')
 
@@ -179,15 +197,23 @@
             if chem.hazardous_waste:
                 disposal.add(chem.hazardous_waste_info) 
         exp_summary.append({'name' : file, 'PHS' : phs, 'disposal' : list(disposal), 'PPE' : ppe, 'chem_data': experiment_chemical_data})
 
     return exp_summary, best_course
         
 def get_course_list():
-    directory_path = 'static/courses'
+
+    user_static_dir = CONFIG.get('user_courses_dir', 'None')
+
+    # Check if user has set a valid directory
+    if user_static_dir == "None" or not os.path.exists(os.path.expanduser(user_static_dir)):
+        directory_path = 'static/courses'
+    else:
+        directory_path = user_static_dir
+    
     course_list = []
 
     pattern = re.compile(r'^([A-Z]{4})(\d{4})$')
 
     if os.path.exists(directory_path):
         for entry in os.listdir(directory_path):
             if os.path.isdir(os.path.join(directory_path, entry)):
@@ -197,15 +223,25 @@
                     course_list.append(course_name)
     else:
         print(f"Directory not found: {directory_path}")
 
     return natsorted(course_list)
 
 def list_experiments(course):
-    directory_path = os.path.join('static/courses', course.replace(' ', ''))
+    
+    course = course.replace(' ', '')
+
+    user_static_dir = CONFIG.get('user_courses_dir', 'None')
+
+    # Check if user has set a valid directory
+    if user_static_dir == "None" or not os.path.exists(os.path.expanduser(user_static_dir)):
+        directory_path = os.path.join('static/courses', course)
+    else:
+        directory_path = os.path.join(os.path.expanduser(user_static_dir), course)
+    
     txt_files = []
     if os.path.exists(directory_path):
         for filename in os.listdir(directory_path):
             if filename.endswith('.txt'):
                 txt_files.append(os.path.splitext(filename)[0])
     else:
         print(f"Directory not found: {directory_path}")
@@ -219,21 +255,29 @@
     pattern = re.compile(r'([A-Z]{4})\s*(\d{4})')
     match = pattern.search(search_term)
 
     if match:
         best_course, _ = custom_match(f"{match.group(0)} {match.group(1)}", course_list)[0]
         search_term = search_term.replace(match.group(0), '')
 
+    user_static_dir = CONFIG.get('user_courses_dir', 'None')
+
+    # Check if user has set a valid directory
+    if user_static_dir == "None" or not os.path.exists(os.path.expanduser(user_static_dir)):
+        directory_path = os.path.join('static/courses', course)
+    else:
+        directory_path = os.path.join(os.path.expanduser(user_static_dir), course)
+    
     if best_course:
-        directory_path = os.path.join('static/courses', best_course.replace(' ', ''))
+        directory_path = os.path.join(directory_path, best_course.replace(' ', ''))
         txt_files = [os.path.splitext(f)[0] for f in os.listdir(directory_path) if f.endswith('.txt')]
     else:
         txt_files_dict = {}
         for course in course_list:
-            directory_path = os.path.join('static/courses', course.replace(' ', ''))
+            directory_path = os.path.join(directory_path, course.replace(' ', ''))
             for f in os.listdir(directory_path): 
                 if f.endswith('.txt'):
                     f_name = os.path.splitext(f)[0]
                     txt_files_dict[f_name] = directory_path
         txt_files = txt_files_dict.keys()
 
     best_experiment, _ = custom_match(search_term, txt_files)[0]
```

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/css/style.css` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/css/style.css`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Acute Toxic.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Acute Toxic.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Compressed Gas.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Compressed Gas.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Corrosive.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Corrosive.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Environmental Hazard.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Environmental Hazard.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Explosive.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Explosive.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Flammable.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Flammable.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Health Hazard.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Health Hazard.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Irritant.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Irritant.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Oxidizer.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Oxidizer.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/Oxidizing.svg` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/Oxidizing.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/PHS.png` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/PHS.png`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/chembio_horiz.png` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/chembio_horiz.png`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/static/img/logo.png` & `chemical_safety-0.0.7/chemical_safety/dashboard/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/chemical_lookup.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/chemical_lookup.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/course_lookup.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/course_lookup.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/emergency_info.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/emergency_info.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/experiment_lookup.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/experiment_lookup.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/index.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/multi_chemical_lookup.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/multi_chemical_lookup.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/phs_list.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/phs_list.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/room_lookup.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/room_lookup.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/search_form.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/search_form.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/secondary_label.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/secondary_label.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety/dashboard/templates/secondary_label_builder.html` & `chemical_safety-0.0.7/chemical_safety/dashboard/templates/secondary_label_builder.html`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/chemical_safety.egg-info/SOURCES.txt` & `chemical_safety-0.0.7/chemical_safety.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/logo.png` & `chemical_safety-0.0.7/logo.png`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.6/setup.py` & `chemical_safety-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chemical_safety",
-    version="0.0.6",
+    version="0.0.7",
     description="A package for retreiving chemical safety information",
     author="Demetrios Pagonis",
     author_email="demetriospagonis@weber.edu",
 
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(include=['chemical_safety', 'chemical_safety.*']),
```

