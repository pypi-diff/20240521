# Comparing `tmp/chemical_safety-0.0.4.tar.gz` & `tmp/chemical_safety-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemical_safety-0.0.4.tar", last modified: Tue May 21 16:22:30 2024, max compression
+gzip compressed data, was "chemical_safety-0.0.5.tar", last modified: Tue May 21 16:28:14 2024, max compression
```

## Comparing `chemical_safety-0.0.4.tar` & `chemical_safety-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 16:22:30.000000 chemical_safety-0.0.4/
--rw-rw-rw-   0        0        0     1095 2024-02-03 21:17:28.000000 chemical_safety-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      317 2024-05-21 16:21:24.000000 chemical_safety-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      679 2024-05-21 16:22:30.000000 chemical_safety-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-05-21 16:01:33.000000 chemical_safety-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 16:22:30.000000 chemical_safety-0.0.4/chemical_safety/
--rw-rw-rw-   0        0        0       66 2024-05-18 17:22:12.000000 chemical_safety-0.0.4/chemical_safety/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:22:28.000000 chemical_safety-0.0.4/chemical_safety/chemical/
--rw-rw-rw-   0        0        0       30 2024-05-18 16:55:19.000000 chemical_safety-0.0.4/chemical_safety/chemical/__init__.py
--rw-rw-rw-   0        0        0    38858 2024-05-21 15:58:58.000000 chemical_safety-0.0.4/chemical_safety/chemical/chemical.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:22:25.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/
--rw-rw-rw-   0        0        0     1219 2024-04-23 16:19:23.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/EPA_D_List.csv
--rw-rw-rw-   0        0        0    25593 2024-04-23 16:19:39.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/EPA_P_List.csv
--rw-rw-rw-   0        0        0    46891 2024-04-23 16:20:09.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/EPA_U_List.csv
--rw-rw-rw-   0        0        0    83466 2024-02-02 04:14:29.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/IARC_classification.csv
--rw-rw-rw-   0        0        0     5163 2024-02-01 23:04:11.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/NTP_anticipated_carcinogens.csv
--rw-rw-rw-   0        0        0      941 2024-02-01 23:03:51.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/NTP_known_carcinogens.csv
--rw-rw-rw-   0        0        0      349 2024-02-02 00:04:46.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/OSHA_carcinogens.csv
--rw-rw-rw-   0        0        0     2610 2024-04-21 20:25:07.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/UMN_peroxide_formers.csv
--rw-rw-rw-   0        0        0    10379 2024-04-15 20:21:48.000000 chemical_safety-0.0.4/chemical_safety/chemical/lists/p_statements.csv
--rw-rw-rw-   0        0        0    11694 2024-05-03 04:13:48.000000 chemical_safety-0.0.4/chemical_safety/chemical/molecule.py
--rw-rw-rw-   0        0        0     5474 2024-03-11 02:03:14.000000 chemical_safety-0.0.4/chemical_safety/chemical/periodictable.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:22:28.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/
--rw-rw-rw-   0        0        0    12588 2023-11-06 22:41:50.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Acute Toxic.svg
--rw-rw-rw-   0        0        0     1446 2023-11-06 22:41:50.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Compressed Gas.svg
--rw-rw-rw-   0        0        0    13531 2023-11-06 22:41:50.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Corrosive.svg
--rw-rw-rw-   0        0        0     5466 2023-11-06 22:41:52.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Environmental Hazard.svg
--rw-rw-rw-   0        0        0    11902 2023-11-06 22:41:48.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Explosive.svg
--rw-rw-rw-   0        0        0     2526 2023-11-06 22:41:48.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Flammable.svg
--rw-rw-rw-   0        0        0    15192 2023-11-06 22:41:52.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Health Hazard.svg
--rw-rw-rw-   0        0        0     1675 2023-11-06 22:41:52.000000 chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Irritant.svg
+drwxrwxrwx   0        0        0        0 2024-05-21 16:28:14.000000 chemical_safety-0.0.5/
+-rw-rw-rw-   0        0        0     1095 2024-02-03 21:17:28.000000 chemical_safety-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      393 2024-05-21 16:26:45.000000 chemical_safety-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      679 2024-05-21 16:28:14.000000 chemical_safety-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2024-05-21 16:01:33.000000 chemical_safety-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:05.000000 chemical_safety-0.0.5/chemical_safety/
+-rw-rw-rw-   0        0        0       66 2024-05-18 17:22:12.000000 chemical_safety-0.0.5/chemical_safety/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:04.000000 chemical_safety-0.0.5/chemical_safety/chemical/
+-rw-rw-rw-   0        0        0       30 2024-05-18 16:55:19.000000 chemical_safety-0.0.5/chemical_safety/chemical/__init__.py
+-rw-rw-rw-   0        0        0    38858 2024-05-21 15:58:58.000000 chemical_safety-0.0.5/chemical_safety/chemical/chemical.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:03.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/
+-rw-rw-rw-   0        0        0     1219 2024-04-23 16:19:23.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/EPA_D_List.csv
+-rw-rw-rw-   0        0        0    25593 2024-04-23 16:19:39.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/EPA_P_List.csv
+-rw-rw-rw-   0        0        0    46891 2024-04-23 16:20:09.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/EPA_U_List.csv
+-rw-rw-rw-   0        0        0    83466 2024-02-02 04:14:29.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/IARC_classification.csv
+-rw-rw-rw-   0        0        0     5163 2024-02-01 23:04:11.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/NTP_anticipated_carcinogens.csv
+-rw-rw-rw-   0        0        0      941 2024-02-01 23:03:51.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/NTP_known_carcinogens.csv
+-rw-rw-rw-   0        0        0      349 2024-02-02 00:04:46.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/OSHA_carcinogens.csv
+-rw-rw-rw-   0        0        0     2610 2024-04-21 20:25:07.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/UMN_peroxide_formers.csv
+-rw-rw-rw-   0        0        0     1948 2024-04-21 20:24:51.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/convert_UMN_peroxide_list.py
+-rw-rw-rw-   0        0        0     1094 2024-04-15 20:21:47.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/convert_p_statements.py
+-rw-rw-rw-   0        0        0    10379 2024-04-15 20:21:48.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/p_statements.csv
+-rw-rw-rw-   0        0        0     1309 2024-04-23 16:07:29.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/process_EPA_lists.py
+-rw-rw-rw-   0        0        0      317 2024-02-03 21:21:07.000000 chemical_safety-0.0.5/chemical_safety/chemical/lists/process_lists.py
+-rw-rw-rw-   0        0        0    11694 2024-05-03 04:13:48.000000 chemical_safety-0.0.5/chemical_safety/chemical/molecule.py
+-rw-rw-rw-   0        0        0     5474 2024-03-11 02:03:14.000000 chemical_safety-0.0.5/chemical_safety/chemical/periodictable.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:03.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/
+-rw-rw-rw-   0        0        0    12588 2023-11-06 22:41:50.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Acute Toxic.svg
+-rw-rw-rw-   0        0        0     1446 2023-11-06 22:41:50.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Compressed Gas.svg
+-rw-rw-rw-   0        0        0    13531 2023-11-06 22:41:50.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Corrosive.svg
+-rw-rw-rw-   0        0        0     5466 2023-11-06 22:41:52.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Environmental Hazard.svg
+-rw-rw-rw-   0        0        0    11902 2023-11-06 22:41:48.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Explosive.svg
+-rw-rw-rw-   0        0        0     2526 2023-11-06 22:41:48.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Flammable.svg
+-rw-rw-rw-   0        0        0    15192 2023-11-06 22:41:52.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Health Hazard.svg
+-rw-rw-rw-   0        0        0     1675 2023-11-06 22:41:52.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Irritant.svg
+-rw-rw-rw-   0        0        0     3336 2023-11-06 22:41:50.000000 chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Oxidizing.svg
+-rw-rw-rw-   0        0        0    14908 2024-05-03 04:14:07.000000 chemical_safety-0.0.5/chemical_safety/chemical/sigfig.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:04.000000 chemical_safety-0.0.5/chemical_safety/chemical/tables/
+-rw-rw-rw-   0        0        0 15139689 2023-04-13 19:24:30.000000 chemical_safety-0.0.5/chemical_safety/chemical/tables/elements.csv
+-rw-rw-rw-   0        0        0     8223 2024-02-12 03:32:32.000000 chemical_safety-0.0.5/chemical_safety/chemical/units.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:05.000000 chemical_safety-0.0.5/chemical_safety/dashboard/
+-rw-rw-rw-   0        0        0       26 2024-05-18 17:22:03.000000 chemical_safety-0.0.5/chemical_safety/dashboard/__init__.py
+-rw-rw-rw-   0        0        0    11776 2024-05-20 22:51:02.000000 chemical_safety-0.0.5/chemical_safety/dashboard/app.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:05.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:04.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:04.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/
+-rw-rw-rw-   0        0        0       57 2024-05-01 15:05:10.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/1 Crystallization & Melting Points.txt
+-rw-rw-rw-   0        0        0      131 2024-05-01 15:26:01.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/10 Oxidation of Cyclohexanol.txt
+-rw-rw-rw-   0        0        0      222 2024-05-01 15:08:11.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/2 Identification of Unkown Alkanes and Alkenes.txt
+-rw-rw-rw-   0        0        0      223 2024-05-01 15:14:23.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/3 Free Radical Chlorination of 1-Chlorobutane.txt
+-rw-rw-rw-   0        0        0      101 2024-05-01 15:26:11.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/30 Separation of Binary Mixtures by Fractional Distillation.txt
+-rw-rw-rw-   0        0        0       30 2024-05-01 15:09:04.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/4 Optical Activity of Caraway and Spearmint Oils.txt
+-rw-rw-rw-   0        0        0       68 2024-05-01 15:15:28.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/5 Preparation of Phenacetin by the Williamson Ether Synthesis.txt
+-rw-rw-rw-   0        0        0      103 2024-05-01 15:23:36.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/6 Synthesis of 3_3-Dimethyl-2-Butanol.txt
+-rw-rw-rw-   0        0        0      110 2024-05-01 15:17:39.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/7 Dehydration of 3_3-Dimethyl-2-butanol.txt
+-rw-rw-rw-   0        0        0      124 2024-05-01 15:18:00.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/8 Identification of an Unknown by Infrared Spectroscopy.txt
+-rw-rw-rw-   0        0        0       18 2024-05-01 15:21:45.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2315/9 Steam Distillation of Orange Oil.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:04.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2325/
+-rw-rw-rw-   0        0        0      121 2024-04-24 14:50:11.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM2325/16 Preparation of Benzoic Acid from Phenylmagnesium Bromide and Carbon Dioxide.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:04.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM3000/
+-rw-rw-rw-   0        0        0        5 2024-04-24 14:27:57.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM3000/1 Calibration of glassware.txt
+-rw-rw-rw-   0        0        0       35 2024-04-24 14:28:54.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM3000/2 Determination of total acidity.txt
+-rw-rw-rw-   0        0        0       93 2024-04-24 14:28:52.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM3000/4 Determination of chloride.txt
+-rw-rw-rw-   0        0        0       22 2024-04-24 14:29:10.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM3000/5 Beers law.txt
+-rw-rw-rw-   0        0        0      100 2024-04-24 14:30:13.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM3000/6 Determination of manganese in steel.txt
+-rw-rw-rw-   0        0        0       26 2024-04-24 14:31:57.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM3000/7 GCMS of gasoline.txt
+-rw-rw-rw-   0        0        0       32 2024-04-24 14:31:34.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/courses/CHEM3000/8 Simultaneous determination of a two-component mixture.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:05.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/css/
+-rw-rw-rw-   0        0        0     2318 2024-05-21 15:02:17.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/css/style.css
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:05.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/
+-rw-rw-rw-   0        0        0    12588 2023-11-06 22:41:50.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Acute Toxic.svg
+-rw-rw-rw-   0        0        0     1446 2023-11-06 22:41:50.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Compressed Gas.svg
+-rw-rw-rw-   0        0        0    13531 2023-11-06 22:41:50.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Corrosive.svg
+-rw-rw-rw-   0        0        0     5466 2023-11-06 22:41:52.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Environmental Hazard.svg
+-rw-rw-rw-   0        0        0    11902 2023-11-06 22:41:48.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Explosive.svg
+-rw-rw-rw-   0        0        0     2526 2023-11-06 22:41:48.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Flammable.svg
+-rw-rw-rw-   0        0        0    15192 2023-11-06 22:41:52.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Health Hazard.svg
+-rw-rw-rw-   0        0        0     1675 2023-11-06 22:41:52.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Irritant.svg
+-rw-rw-rw-   0        0        0     3336 2023-11-06 22:41:50.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Oxidizer.svg
+-rw-rw-rw-   0        0        0     3336 2023-11-06 22:41:50.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/Oxidizing.svg
+-rw-rw-rw-   0        0        0    26469 2024-04-12 12:02:11.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/PHS.png
+-rw-rw-rw-   0        0        0    62940 2018-08-07 13:52:30.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/chembio_horiz.png
+-rw-rw-rw-   0        0        0    10665 2024-02-08 21:28:49.000000 chemical_safety-0.0.5/chemical_safety/dashboard/static/img/logo.png
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:05.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/
+-rw-rw-rw-   0        0        0     4405 2024-05-21 15:52:31.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/chemical_lookup.html
+-rw-rw-rw-   0        0        0     4289 2024-05-01 16:04:04.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/course_lookup.html
+-rw-rw-rw-   0        0        0      884 2024-04-22 11:55:12.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/emergency_info.html
+-rw-rw-rw-   0        0        0     3125 2024-05-01 16:03:54.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/experiment_lookup.html
+-rw-rw-rw-   0        0        0     1482 2024-04-24 20:47:41.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/index.html
+-rw-rw-rw-   0        0        0     3129 2024-05-20 22:51:03.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/multi_chemical_lookup.html
+-rw-rw-rw-   0        0        0      897 2024-04-22 11:55:40.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/phs_list.html
+-rw-rw-rw-   0        0        0      889 2024-04-22 11:55:49.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/room_lookup.html
+-rw-rw-rw-   0        0        0     1519 2024-04-24 20:55:34.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/search_form.html
+-rw-rw-rw-   0        0        0     2343 2024-05-20 22:51:03.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/secondary_label.html
+-rw-rw-rw-   0        0        0     3722 2024-05-20 22:51:03.000000 chemical_safety-0.0.5/chemical_safety/dashboard/templates/secondary_label_builder.html
+drwxrwxrwx   0        0        0        0 2024-05-21 16:28:13.000000 chemical_safety-0.0.5/chemical_safety.egg-info/
+-rw-rw-rw-   0        0        0      679 2024-05-21 16:28:09.000000 chemical_safety-0.0.5/chemical_safety.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4957 2024-05-21 16:28:12.000000 chemical_safety-0.0.5/chemical_safety.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:28:09.000000 chemical_safety-0.0.5/chemical_safety.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-21 16:28:09.000000 chemical_safety-0.0.5/chemical_safety.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2024-05-21 16:28:09.000000 chemical_safety-0.0.5/chemical_safety.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-21 16:28:09.000000 chemical_safety-0.0.5/chemical_safety.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10665 2024-02-08 21:28:49.000000 chemical_safety-0.0.5/logo.png
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:28:14.000000 chemical_safety-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      825 2024-05-21 16:26:52.000000 chemical_safety-0.0.5/setup.py
```

### Comparing `chemical_safety-0.0.4/LICENSE` & `chemical_safety-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/PKG-INFO` & `chemical_safety-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemical_safety
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for retreiving chemical safety information
 Author: Demetrios Pagonis
 Author-email: demetriospagonis@weber.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chemical_safety
```

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/chemical.py` & `chemical_safety-0.0.5/chemical_safety/chemical/chemical.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/lists/EPA_D_List.csv` & `chemical_safety-0.0.5/chemical_safety/chemical/lists/EPA_D_List.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/lists/EPA_P_List.csv` & `chemical_safety-0.0.5/chemical_safety/chemical/lists/EPA_P_List.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/lists/EPA_U_List.csv` & `chemical_safety-0.0.5/chemical_safety/chemical/lists/EPA_U_List.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/lists/IARC_classification.csv` & `chemical_safety-0.0.5/chemical_safety/chemical/lists/IARC_classification.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/lists/NTP_anticipated_carcinogens.csv` & `chemical_safety-0.0.5/chemical_safety/chemical/lists/NTP_anticipated_carcinogens.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/lists/NTP_known_carcinogens.csv` & `chemical_safety-0.0.5/chemical_safety/chemical/lists/NTP_known_carcinogens.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/lists/UMN_peroxide_formers.csv` & `chemical_safety-0.0.5/chemical_safety/chemical/lists/UMN_peroxide_formers.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/lists/p_statements.csv` & `chemical_safety-0.0.5/chemical_safety/chemical/lists/p_statements.csv`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/molecule.py` & `chemical_safety-0.0.5/chemical_safety/chemical/molecule.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/periodictable.py` & `chemical_safety-0.0.5/chemical_safety/chemical/periodictable.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Acute Toxic.svg` & `chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Acute Toxic.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Compressed Gas.svg` & `chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Compressed Gas.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Corrosive.svg` & `chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Corrosive.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Environmental Hazard.svg` & `chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Environmental Hazard.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Explosive.svg` & `chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Explosive.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Flammable.svg` & `chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Flammable.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Health Hazard.svg` & `chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Health Hazard.svg`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.4/chemical_safety/chemical/pictograms/Irritant.svg` & `chemical_safety-0.0.5/chemical_safety/chemical/pictograms/Irritant.svg`

 * *Files identical despite different names*

