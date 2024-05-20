# Comparing `tmp/ecoengine-1.6.1.tar.gz` & `tmp/ecoengine-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-1.6.1.tar", last modified: Fri May 17 20:23:38 2024, max compression
+gzip compressed data, was "ecoengine-1.6.2.tar", last modified: Mon May 20 22:43:36 2024, max compression
```

## Comparing `ecoengine-1.6.1.tar` & `ecoengine-1.6.2.tar`

### file list

```diff
@@ -1,300 +1,300 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.546096 ecoengine-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-17 20:21:59.000000 ecoengine-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-17 20:23:38.546096 ecoengine-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-17 20:21:59.000000 ecoengine-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-17 20:21:59.000000 ecoengine-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 20:23:38.546096 ecoengine-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 20:21:59.000000 ecoengine-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.454096 ecoengine-1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.458096 ecoengine-1.6.1/src/ecoengine/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.458096 ecoengine-1.6.1/src/ecoengine/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/constants/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.458096 ecoengine-1.6.1/src/ecoengine/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.466096 ecoengine-1.6.1/src/ecoengine/data/climate_data/
--rw-r--r--   0 runner    (1001) docker     (127)  3784790 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv
--rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/climate_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1728735 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.470096 ecoengine-1.6.1/src/ecoengine/data/load_shapes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/apartment.json
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/elementary_school.json
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/food_service_a.json
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/food_service_b.json
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/junior_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/mens_dorm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/motel.json
--rw-r--r--   0 runner    (1001) docker     (127)   262011 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/multi_family.json
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/nursing_home.json
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/office_building.json
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/senior_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/load_shapes/womens_dorm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.470096 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58109 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/maps.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.542096 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.546096 ecoengine-1.6.1/src/ecoengine/engine/
--rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/engine/BuildingCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)    44086 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/engine/EcosizerEngine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/engine/Simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/engine/SystemCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.546096 ecoengine-1.6.1/src/ecoengine/objects/
--rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/Building.py
--rw-r--r--   0 runner    (1001) docker     (127)    30767 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/PrefMapTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    34744 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/SimulationRun.py
--rw-r--r--   0 runner    (1001) docker     (127)    48934 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/SystemConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/UtilityCostTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/systemConfigUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.546096 ecoengine-1.6.1/src/ecoengine/objects/systems/
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/systems/MultiPass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/systems/MultiPassRecirc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/systems/PrimaryWithRecirc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26555 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/systems/SwingTank.py
--rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/systems/SwingTankER.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:21:59.000000 ecoengine-1.6.1/src/ecoengine/objects/systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:23:38.546096 ecoengine-1.6.1/src/ecoengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-17 20:23:38.000000 ecoengine-1.6.1/src/ecoengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-05-17 20:23:38.000000 ecoengine-1.6.1/src/ecoengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:23:38.000000 ecoengine-1.6.1/src/ecoengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-17 20:23:38.000000 ecoengine-1.6.1/src/ecoengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 20:23:38.000000 ecoengine-1.6.1/src/ecoengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.218585 ecoengine-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-20 22:41:57.000000 ecoengine-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-20 22:43:36.218585 ecoengine-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-20 22:41:57.000000 ecoengine-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 22:41:57.000000 ecoengine-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-20 22:43:36.218585 ecoengine-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 22:41:57.000000 ecoengine-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.134584 ecoengine-1.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.138584 ecoengine-1.6.2/src/ecoengine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.138584 ecoengine-1.6.2/src/ecoengine/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/constants/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.138584 ecoengine-1.6.2/src/ecoengine/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.146584 ecoengine-1.6.2/src/ecoengine/data/climate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3784790 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1728735 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.150584 ecoengine-1.6.2/src/ecoengine/data/load_shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/apartment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/junior_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/motel.json
+-rw-r--r--   0 runner    (1001) docker     (127)   262011 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/multi_family.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/office_building.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/senior_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.150584 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58109 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/maps.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.214585 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.214585 ecoengine-1.6.2/src/ecoengine/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/BuildingCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44309 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/EcosizerEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/Simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/SystemCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.214585 ecoengine-1.6.2/src/ecoengine/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/Building.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30767 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/PrefMapTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34744 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/SimulationRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48934 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/SystemConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/UtilityCostTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systemConfigUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.218585 ecoengine-1.6.2/src/ecoengine/objects/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/MultiPass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/MultiPassRecirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/PrimaryWithRecirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26555 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/SwingTank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/SwingTankER.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.218585 ecoengine-1.6.2/src/ecoengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-1.6.1/PKG-INFO` & `ecoengine-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 1.6.1
+Version: 1.6.2
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-1.6.1/README.md` & `ecoengine-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/setup.cfg` & `ecoengine-1.6.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoengine
-version = 1.6.1
+version = 1.6.2
 author = Nolan
 author_email = nolan@ecotope.com
 description = A software for sizing Heat Pump Water Heaters for buildings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://ecosizer.ecotope.com/sizer/
 project_urls =
```

### Comparing `ecoengine-1.6.1/src/ecoengine/__init__.py` & `ecoengine-1.6.2/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/constants/Constants.py` & `ecoengine-1.6.2/src/ecoengine/constants/Constants.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv` & `ecoengine-1.6.2/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv` & `ecoengine-1.6.2/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv` & `ecoengine-1.6.2/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv` & `ecoengine-1.6.2/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv` & `ecoengine-1.6.2/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/apartment.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/apartment.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/elementary_school.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/elementary_school.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/food_service_a.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/food_service_a.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/food_service_b.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/food_service_b.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/junior_high.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/junior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/mens_dorm.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/mens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/motel.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/motel.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/multi_family.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/multi_family.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/nursing_home.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/nursing_home.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/office_building.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/office_building.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/senior_high.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/senior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/load_shapes/womens_dorm.json` & `ecoengine-1.6.2/src/ecoengine/data/load_shapes/womens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/maps.json` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/maps.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-1.6.2/src/ecoengine/engine/BuildingCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-1.6.2/src/ecoengine/engine/EcosizerEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -780,36 +780,40 @@
                              kBTUhr = return_as_kW == False,
                              numHeatPumps = num_heatPumps,
                              usePkl = True)
     output_cap, input_cap = perfMap.getCapacity(outdoorAirTemp_F,inletWaterTemp_F,outletWaterTemp_F)
     return output_cap * (1.0 - defrost_derate)
 
 
-def getSizingCurvePlot(x, y, startind, loadshifting = False):
+def getSizingCurvePlot(x, y, startind, loadshifting : bool = False, er_sized : bool = False):
     """
     creates a plotly figure from a list of x and y points and starts the slider at the start index.
 
     Parameters
     ----------
     x : List
         List of x axis values of points on the sizing curve.
     y : List
         List of y axis values of points on the sizing curve.
     startind : int
         the index in x_values and y_values to start the slider on the sizing curve.
     loadshifting : boolean
         Indicates whether the resulting plot should be for a load shifting system (plotting Percent of Load Shift Days Covered vs. Storage Volume)
         or non-load shifting system (plotting Storage Volume vs. Capacity)
+    er_sized : boolean
+        Indicates whether the resulting plot should be for Electric Resistance trade off sizing
 
     Returns
     -------
     plot : plotly.Figure
         The sizing curve graph. If loadshifting parameter is set to True, the graph will label the plot as Percent of Load Shift Days Covered vs. Storage Volume.
         Otherwise, it will label the plot as Storage Volume vs. Capacity.
     """
+    if er_sized:
+        return createERSizingCurvePlot(x, y, startind)
     return createSizingCurvePlot(x, y, startind, loadshifting)
 
 def getAnnualSimLSComparison(simRun_ls : SimulationRun, simRun_nls : SimulationRun, return_as_div=True):
     """
     Returns comparison graph of the input power by hour for an annual load shifting and non loadshifting HPWH simulation
 
     Parameters
```

### Comparing `ecoengine-1.6.1/src/ecoengine/engine/Simulator.py` & `ecoengine-1.6.2/src/ecoengine/engine/Simulator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/engine/SystemCreator.py` & `ecoengine-1.6.2/src/ecoengine/engine/SystemCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/engine/__init__.py` & `ecoengine-1.6.2/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/Building.py` & `ecoengine-1.6.2/src/ecoengine/objects/Building.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/PrefMapTracker.py` & `ecoengine-1.6.2/src/ecoengine/objects/PrefMapTracker.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/SimulationRun.py` & `ecoengine-1.6.2/src/ecoengine/objects/SimulationRun.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/SystemConfig.py` & `ecoengine-1.6.2/src/ecoengine/objects/SystemConfig.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/UtilityCostTracker.py` & `ecoengine-1.6.2/src/ecoengine/objects/UtilityCostTracker.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/__init__.py` & `ecoengine-1.6.2/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-1.6.2/src/ecoengine/objects/systemConfigUtils.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/systems/MultiPass.py` & `ecoengine-1.6.2/src/ecoengine/objects/systems/MultiPass.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/systems/MultiPassRecirc.py` & `ecoengine-1.6.2/src/ecoengine/objects/systems/MultiPassRecirc.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/systems/ParallelLoopTank.py` & `ecoengine-1.6.2/src/ecoengine/objects/systems/ParallelLoopTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/systems/PrimaryWithRecirc.py` & `ecoengine-1.6.2/src/ecoengine/objects/systems/PrimaryWithRecirc.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/systems/SwingTank.py` & `ecoengine-1.6.2/src/ecoengine/objects/systems/SwingTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine/objects/systems/SwingTankER.py` & `ecoengine-1.6.2/src/ecoengine/objects/systems/SwingTankER.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.1/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-1.6.2/src/ecoengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 1.6.1
+Version: 1.6.2
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-1.6.1/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-1.6.2/src/ecoengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

