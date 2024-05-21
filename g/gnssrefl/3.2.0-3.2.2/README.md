# Comparing `tmp/gnssrefl-3.2.0.tar.gz` & `tmp/gnssrefl-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-3.2.0.tar", last modified: Wed May  8 15:26:45 2024, max compression
+gzip compressed data, was "gnssrefl-3.2.2.tar", last modified: Tue May 21 15:47:01 2024, max compression
```

## Comparing `gnssrefl-3.2.0.tar` & `gnssrefl-3.2.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.088953 gnssrefl-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 15:26:37.000000 gnssrefl-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 15:26:37.000000 gnssrefl-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-08 15:26:45.088953 gnssrefl-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-08 15:26:37.000000 gnssrefl-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.060953 gnssrefl-3.2.0/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.060953 gnssrefl-3.2.0/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/filesizes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnssir_cl_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    21055 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44620 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    50903 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)    50899 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (127)   199307 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)    40525 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/make_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/max_resolve_RH_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/mjd.py
--rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18818 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    43423 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57267 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    25224 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex_coords.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    38571 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/sd_libs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    61269 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.060953 gnssrefl-3.2.0/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:26:45.088953 gnssrefl-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.088953 gnssrefl-3.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.937650 gnssrefl-3.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 15:46:54.000000 gnssrefl-3.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 15:46:54.000000 gnssrefl-3.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-21 15:47:01.937650 gnssrefl-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-21 15:46:54.000000 gnssrefl-3.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.913650 gnssrefl-3.2.2/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.913650 gnssrefl-3.2.2/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/filesizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnssir_cl_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22239 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44629 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50903 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)    50899 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (127)   202799 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40525 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    20209 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/make_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/max_resolve_RH_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/mjd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18818 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20890 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43423 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57682 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25343 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex_coords.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38571 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/sd_libs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61269 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.913650 gnssrefl-3.2.2/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:47:01.941650 gnssrefl-3.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.937650 gnssrefl-3.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/test/test_rinex2snr.py
```

### Comparing `gnssrefl-3.2.0/LICENSE` & `gnssrefl-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/PKG-INFO` & `gnssrefl-3.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.2.0
+Version: 3.2.2
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.2.0 
+# gnssrefl v3.2.2 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494) 
@@ -26,14 +26,16 @@
 
 ![](docs/myAnimation.gif)
 
 I made this animation ages ago - so it is in Matlab.  I would be happy to host a link to 
 a version in python.  The main code is [snr_simulation](docs/pages/snr_simulation.m) 
 and the helper function is [setFrame.m](docs/pages/set_Frame.m). 
 
+High-rate data from CDDIS that are more than six months old can now be downloaded.
+
 Documentation:
 
 - [online](https://gnssrefl.readthedocs.io/en/latest/)
 
 - [pdf](https://gnssrefl.readthedocs.io/_/downloads/en/latest/pdf/)
 
 - [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `gnssrefl-3.2.0/README.md` & `gnssrefl-3.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gnssrefl v3.2.0 
+# gnssrefl v3.2.2 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494) 
@@ -12,14 +12,16 @@
 
 ![](docs/myAnimation.gif)
 
 I made this animation ages ago - so it is in Matlab.  I would be happy to host a link to 
 a version in python.  The main code is [snr_simulation](docs/pages/snr_simulation.m) 
 and the helper function is [setFrame.m](docs/pages/set_Frame.m). 
 
+High-rate data from CDDIS that are more than six months old can now be downloaded.
+
 Documentation:
 
 - [online](https://gnssrefl.readthedocs.io/en/latest/)
 
 - [pdf](https://gnssrefl.readthedocs.io/_/downloads/en/latest/pdf/)
 
 - [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `gnssrefl-3.2.0/gnssrefl/EGM96.py` & `gnssrefl-3.2.2/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/check_rinex_file.py` & `gnssrefl-3.2.2/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/computemp1mp2.py` & `gnssrefl-3.2.2/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/daily_avg.py` & `gnssrefl-3.2.2/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/daily_avg_cl.py` & `gnssrefl-3.2.2/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-3.2.2/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/decipher_argt.py` & `gnssrefl-3.2.2/gnssrefl/decipher_argt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/download_ioc.py` & `gnssrefl-3.2.2/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/download_noaa.py` & `gnssrefl-3.2.2/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/download_orbits.py` & `gnssrefl-3.2.2/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/download_psmsl.py` & `gnssrefl-3.2.2/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/download_rinex.py` & `gnssrefl-3.2.2/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/download_teqc.py` & `gnssrefl-3.2.2/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/download_tides.py` & `gnssrefl-3.2.2/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/download_unr.py` & `gnssrefl-3.2.2/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/download_wsv.py` & `gnssrefl-3.2.2/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/filesizes.py` & `gnssrefl-3.2.2/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/gnssir_cl.py` & `gnssrefl-3.2.2/gnssrefl/gnssir_cl.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,17 @@
         periodograms are computed. 1 sec is default (i.e. no decimating)
     newarcs : bool, optional
         this input no longer has any meaning 
     par : int, optional
         number of parallel processing jobs. 
 
     """
+    vers = 'gnssrefl version ' + str(g.version('gnssrefl'))
+    print('You are running ', vers)
+
 
 #   make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
     xdir = str(os.environ['REFL_CODE'])
 
     exitS = g.check_inputs(station, year, doy, snr)
 
@@ -302,15 +305,15 @@
             url='https://github.com/kristinemlarson/gnssrefl/raw/master/gnssrefl/gpt_1wA.pickle'
             wget.download(url, picklefile)
             subprocess.call(['mv', '-f', picklefile, xdir + '/input/'])
 
     args = {'station': station.lower(), 'year': year, 'doy': doy, 'snr_type': snr, 'extension': extension, 'lsp': lsp}
 
     print(lsp['pele'], ' direct signal elevation angle limits')
-    print(lsp['e1'], lsp['e2'], ' min and max elevation angles')
+    #print(lsp['e1'], lsp['e2'], ' min and max elevation angles')
     # added this because ellist is a new option and was not necessarily created in old json files
     if 'ellist' not in lsp:
         #print('did not find ellist')
         if float(lsp['e1']) < float(lsp['pele'][0]):
             print('emin is smaller than the minimum eangle (pele) used for direct signal removed.')
             print('This is Forbidden. Fix the records set in the json created by gnssir_analysis')
             sys.exit()
```

### Comparing `gnssrefl-3.2.0/gnssrefl/gnssir_cl_old.py` & `gnssrefl-3.2.2/gnssrefl/gnssir_cl_old.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/gnssir_input.py` & `gnssrefl-3.2.2/gnssrefl/gnssir_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     parser.add_argument("-refraction", default=None, type=str, help="Set to False to turn off refraction correction")
     parser.add_argument("-extension", default=None,type=str, help="Provide extension name so you can try different strategies")
     parser.add_argument("-ediff", default=None, type=float, help="Allowed min/max elevation diff from obs min/max elev angle (degrees) default is 2")
     parser.add_argument("-delTmax", default=None, type=float, help="max arc length (min) default is 75. Shorten for tides.")
     parser.add_argument("-frlist", nargs="*",type=int,  help="User defined frequencies using our nomenclature")
     parser.add_argument("-azlist2", nargs="*",type=float,  default=None,help="list of azimuth regions, default is 0-360") 
     parser.add_argument("-ellist", nargs="*",type=float,  default=None,help="List of elevation angles, advanced users only!") 
-    parser.add_argument("-refr_model", default=1, type=int, help="refraction model. default is 1, zero turns it off)")
+    parser.add_argument("-refr_model", default="1", type=str, help="refraction model. default is 1, zero turns it off)")
     parser.add_argument("-apriori_rh", default=None, type=float, help="apriori reflector height (m) used by NITE model")
     parser.add_argument("-Hortho", default=None, type=float, help="station orthometric height (m)")
     parser.add_argument("-pele", nargs="*", type=float, help="min and max elevation angle in direct signal removal, default is 5-30")
     parser.add_argument("-daily_avg_medfilter", default=None, type=float, help="daily_avg, median filter, meters")
     parser.add_argument("-daily_avg_reqtracks", default=None, type=int, help="daily_avg, ReqTracks parameter ")
     parser.add_argument("-subdaily_alt_sigma", default=None, type=str, help="subdaily, Nievinski sigma")
     parser.add_argument("-subdaily_sigma", default=None, type=str, help="subdaily, sigma for part 1")
@@ -62,15 +62,15 @@
     return {key: value for key, value in args.items() if value is not None}
 
 
 def make_gnssir_input(station: str, lat: float=0, lon: float=0, height: float=0, e1: float = 5.0, e2: float = 25.0,
        h1: float = 0.5, h2: float = 8.0, nr1: float = None, nr2: float = None, peak2noise: float = 2.8, 
        ampl: float = 5.0, allfreq: bool = False, l1: bool = False, l2c: bool = False, 
        xyz: bool = False, refraction: bool = True, extension: str = '', ediff: float=2.0, 
-       delTmax: float=75.0, frlist: list=[], azlist2: list=[0,360], ellist : list=[], refr_model : int=1, 
+       delTmax: float=75.0, frlist: list=[], azlist2: list=[0,360], ellist : list=[], refr_model : str="1", 
                       apriori_rh: float=None, Hortho : float = None, pele: list=[5,30], daily_avg_reqtracks: int=None, 
                       daily_avg_medfilter: float =None, subdaily_alt_sigma : bool=None, 
                       subdaily_ampl : float=None, subdaily_delta_out : float=None, 
                       subdaily_knots : int=None, subdaily_sigma: float=None, subdaily_subdir: str=None, 
                       subdaily_spline_outlier1: float=None, subdaily_spline_outlier2: float=None):
 
     """
@@ -86,31 +86,43 @@
 
     Note: you can keep using your old json files - you just need to add this new -azlist2 setting manually.
 
     Latitude, longitude, and height are assumed to be stored in the UNR database.  If they are not, you should
     set them manually.
 
     Originally we had refraction as a boolean, i.e. on or off. This was stored in the gnssir 
-    analysis json. The code however, uses an integer 1 (for a simple non-time-varying 
-    Bennett correction) and integer 0 for no correction.
-    From version 1.8.4 we begin to implement more refraction models.  1 (and Bennett) will continue to be 
-    the default.  The "1" is written to the LSP results file so that people can keep track easily of whether
+    analysis description json. The code however, uses a 1 for a simple non-time-varying 
+    Bennett correction and 0 for no correction.
+
+    From version 1.8.4 we begin to implement more refraction models.  Model 1 (Bennett) will continue to be 
+    the default.  The model number is written (as an integer) to the LSP results file so that people can keep track easily of whether
     they are inadvertently mixing files with different strategies. And that is why it is an integer, because
     all results in the LSP results files are numbers.  Going forward, we are adding a time-varying capability.
 
-        Model 1: Bennett, static
-        Model 2: Bennett and time-varying
-        Model 3: Ulich, static
+        Model 1: Bennett, non-time-varying
+
+        Model 2: Bennett, time-varying
+
+        Model 3: Ulich, non-time-varying
+
         Model 4: Ulich, time-varying
+
         Model 5: NITE, Feng et al. 2023 DOI: 10.1109/TGRS.2023.3332422, time-varying
+
         Model 6: MPF, Williams and Nievinski, 2017,  DOI: 10.1002/2016JB013612, time-varying
 
-    gnssir_input will have a new parameter for the json output, refr_model. If it is not set, i.e. you 
-    have an old json, it is assumed to be 1. You can change the refraction model by 
-    hand editting the file if you like. And you can certainly test out the impact by using -extension option.
+
+    We allow users to input the model names NITE and MPF (nite and mpf also allowed).  The other models do not allow that.
+    If you want model 2, you have to ask for model 2. We thank Peng Feng for providing python code to be used for some of these models.
+
+    If you want to test the effect of different refraction models, you are encouraged to create
+    two json files using the extension option. You can then run gnssir using those two extensions.
+    In general I think the refraction default is fine for soil moisture and snow accumulation.
+    If you are going to look at tall sites, you most definitely need the refraction correction. If you
+    plan to look at very tall sites, you should pick the best one.
 
     Examples
     --------
     gnssir_input p041 
         uses only GPS frequencies and all azimuths and the coordinates in the UNR database
 
     gnssir_input p041   -azlist2 0 180 -fr 1 101
@@ -118,14 +130,15 @@
 
     gnssir_input p041 -lat 39.9494 -lon -105.19426 -height 1728.85  -l2c T -e1 5 -e2 15
         uses only L2C GPS data between elevation angles of 5 and 15 degrees.
         user input lat/long/height
 
     gnssir_input p041  -h1 0.5 -h2 10 -e1 5 -e2 25
         uses UNR database, only GPS data between elevation angles of 5-25 degrees and reflector heights of 0.5-10 meters
+
     gnssir_input p041 -ediff 1
         uses UNR database, only GPS data, default station coordinates, enforces elevation angles to be 
         within 1 degrees of default elevation angle limits (5-25)
 
     gnssir_input sc02 -ellist 5 10 7 12
         let's say you want to compute smaller arcs than just a single set of elevation angles.
         you can use this to set this up, so instead of 5 and 12, you could set it up to 
@@ -213,19 +226,19 @@
         Default is 0 to 360. list of azimuth limits as subquadrants are no longer required.
 
     ellist: list of floats
         min and max elevation angles to be used with the azimuth regions you listed, i.e.
         [5 10 6 11 7 12 8 13] would allow overlapping regions - all five degrees long 
         Default is empty list. 
 
-    refr_model : int
-        refraction model. we are keeping this as integer as it is written to a file withonly
-        numbers in it.  1 is the default simple refraction (just correct elevation angles
-        using standard bending models).  0 is no refraction correction.  As we add more
-        models, they will receiver their own number. 
+    refr_model : str
+        refraction model. While defined as a string (so that people can specify names of models)
+        we convert this to an integer for book-keeping. 1 is the default refraction model 
+        (it corrects elevation angles using standard bending models).  0 is no refraction correction.  
+        The other models are defined in the summary section of this code.
 
     apriori_rh : float
         apriori reflector height (meters). only used in NITE model 
 
     Hortho : float
         station orthometric height, in meters. Currently only used in subdaily.  If not provided on the command line, 
         it will use ellipsoidal height and EGM96 to compute.
@@ -442,15 +455,34 @@
  
     # gzip SNR files after running the code
     # this really should be set to True.  the code is obviously ignoring it
     lsp['gzip'] = False   
 
     lsp['ellist'] = ellist
 
+    if refr_model[0] == '-':
+         print('You selected a negative refraction model. Exiting')
+         sys.exit()
+
+    if refr_model.isnumeric():
+        # number has been input
+        refr_model = int(refr_model)
+        if (refr_model > 6) :
+            print('We only have six refraction models and you selected ', refr_model, ' Exiting')
+            sys.exit()
+    else:
+        if refr_model.upper() == 'NITE':
+            refr_model = 5
+        elif refr_model.upper() == 'MPF':
+            refr_model = 6
+        else:
+            print('Your refraction model ', refr_model, ' is not recognized by the code. Exiting')
+
     lsp['refr_model'] = refr_model
+    print('refraction model ', refr_model)
 
     # added for people that want to save their daily average and subdaily strategies.
     # if not set, then they are saved as None.
     lsp['daily_avg_reqtracks'] = daily_avg_reqtracks
     lsp['daily_avg_medfilter'] = daily_avg_medfilter
 
     lsp['subdaily_alt_sigma'] = subdaily_alt_sigma
```

### Comparing `gnssrefl-3.2.0/gnssrefl/gnssir_v2.py` & `gnssrefl-3.2.2/gnssrefl/gnssir_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             # and apply
             snrD = snrD[iss,:]
             # not sure nrows and ncols is being used ... so not redoing it
 
 
         snr.compress_snr_files(lsp['wantCompression'], obsfile, obsfile2,twoDays,gzip) 
     if (allGood == 1):
-        print('Reading from: ', obsfile)
+        print('Reading SNR data from: ', obsfile)
         #print('Results will be written to:', fname)
         minObsE = min(snrD[:,1])
         print('Min observed elev. angle ', station, year, doy, minObsE, '/requested e1 and e2 ', e1,e2)
         # only apply this test for simple e1 and e2
         if len(ellist) == 0:
             if minObsE > (e1 + ediff):
                 print('You literally have no data above the minimum elevation angle setting')
```

### Comparing `gnssrefl-3.2.0/gnssrefl/gnsssnr.f` & `gnssrefl-3.2.2/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/gnsssnrbigger.f` & `gnssrefl-3.2.2/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/gps.py` & `gnssrefl-3.2.2/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import os
 import pickle
 import re
 import requests
 import subprocess
 import sys
 import sqlite3
+import zipfile
 from urllib.parse import urlparse
 import time
 from ftplib import FTP #import FTP commands from python's built-in ftp library
 from ftplib import FTP_TLS
 from random import seed
 from random import random
 
@@ -33,14 +34,15 @@
 import wget
 from numpy import array
 
 import gnssrefl.read_snr_files as snr
 import gnssrefl.karnak_libraries as k
 import gnssrefl.EGM96 as EGM96
 import gnssrefl.rinex2snr as rnx
+import gnssrefl.sd_libs as sd
 import gnssrefl.kelly as kelly
 
 # for future ref
 #import urllib.request
 
 
 # various numbers you need in the GNSS world
@@ -6397,16 +6399,16 @@
     # input date
     idate = iyear + idoy/365.25
 
     if (tdate - idate) > 0.5:
         # i.e. half a year is six months
         bad_day =  True
         print(archive.upper() + ' does not allow direct access to their high-rate data for this day and year. ')
-        print('They now tar files six months after the data archived. If you are willing to ')
-        print('submit a pull request to fix this issue, we would be very willing to host it.')
+        print('They now tar files six months after the data archived - but force you to merge them. I have installed a solution for CDDIS.')
+        print('It would be nice if someone would make a similar fix for BKG')
 
     else:
         bad_day = False
 
 
     return bad_day
 
@@ -6855,7 +6857,135 @@
         subprocess.call(['mkdir', '-p',logdir])
 
     logname = cdoy + '_translation.txt'
 
     return logdir, logname
 
 
+def noaa2me(date1):
+    """
+    converts NOAA type of date string to simple integers
+
+    Parameters
+    ----------
+    date1 : string
+        time in format YYYYMMDD for year month and day
+
+    Returns
+    -------
+    year1 : integer
+        full year
+
+    month1 : integer
+        month
+
+    day1 : integer
+        day of the month
+
+    doy : integer
+        day of year
+
+    modjulday : float
+        modified julian date
+
+    """
+    year1 = int(date1[0:4]);
+    month1=int(date1[4:6]);
+    day1=int(date1[6:8])
+    doy, cdoy, cyyyy, cyy =ymd2doy(year1, month1, day1)
+
+    mj, fj = mjd(year1, month1, day1, 0, 0, 0)
+    modjulday = mj + fj;
+
+    return year1, month1, day1, doy, modjulday
+
+def noaatime_to_obstime(noaa):
+    """
+    stitching together something to convert string
+    with year, month, day and returning obstime
+
+    Parameters
+    ----------
+    noaa : str
+        year, month, day (e.g. 20220115)
+
+    Returns
+    -------
+    obstime : datetime
+        time in datetime format
+
+    """
+    year1, month1, day1, doy1, modjulday1 = noaa2me(noaa)
+    obstime =  sd.mjd_to_obstimes(modjulday1)
+
+    return obstime
+
+
+def trignet(station,year,doy):
+    """
+    tries to pick up 30 sec RINEX 2.11 data from TRIGNET
+
+    Parameters
+    ----------
+    station : str
+        station name
+    year : int
+        full year
+    doy : int
+        day of year
+    Returns
+    -------
+    fexist : bool
+        whether you succeeded
+
+    """
+    cyyyy,cyy,cdoy = ydoych(year,doy)
+    data_server = 'ftp.trignet.co.za'
+    fexist = False
+
+    try:
+        ftp=FTP(data_server) #log in to server
+        ftp.login(user='anonymous', passwd='kristine@colorado.edu')
+        rinex_dirc = 'RefData.' + cyy + '/' + cdoy + '/L1L2_30sec/'
+        ftp.cwd(rinex_dirc) #change to the directory
+        files=ftp.nlst() #list files in the directory
+        for f in files:
+            if station.upper() in f:
+                print(f)
+                ftp.retrbinary('RETR '+f, open(f,'wb').write)
+        ftp.close()
+    except:
+        print('no file found ', cyyyy, cdoy)
+    the_zipfile = station.upper() + cdoy + 'Z.zip'
+
+    if os.path.exists(the_zipfile):
+        station_u = station.upper() + cdoy + 'z.' + cyy 
+        station_l = station.lower() + cdoy + '0.' + cyy 
+    # in case they are there
+        subprocess.call(['rm', '-f','unpack.bat'])
+        subprocess.call(['rm', '-f','CRX2RNX.EXE'])
+        try:
+            archive = zipfile.ZipFile(the_zipfile, 'r')
+            subprocess.call(['unzip', the_zipfile])
+            subprocess.call(['rm', '-f',station.upper() + cdoy + 'Z.' + cyy + 'q'])
+            subprocess.call(['rm', '-f',station.upper() + cdoy + 'Z.' + cyy + 'n'])
+            subprocess.call(['rm', '-f',station.upper() + cdoy + 'Z.zip'])
+            if os.path.exists(station_u +'d'):
+                subprocess.call(['mv', station_u + 'd', station_l + 'd' ])
+                subprocess.call(['rm', '-f','unpack.bat'])
+                subprocess.call(['rm', '-f','CRX2RNX.EXE'])
+
+                crnxpath = hatanaka_version()
+                subprocess.call([crnxpath, station_l + 'd'])
+                subprocess.call(['rm', '-f',station_l + 'd'])
+
+        except:
+            print('probably a corrupt zipfile, but who knows')
+    # remove crap
+        if os.path.exists(station_l + 'o'):
+            fexist = True
+            print('Found RINEX ', station_l + 'o')
+
+    return fexist
+
+
+
```

### Comparing `gnssrefl-3.2.0/gnssrefl/gpssnr.f` & `gnssrefl-3.2.2/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/gpsweek.py` & `gnssrefl-3.2.2/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/gpt_1wA.pickle` & `gnssrefl-3.2.2/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/highrate.py` & `gnssrefl-3.2.2/gnssrefl/highrate.py`

 * *Files 12% similar despite different names*

```diff
@@ -296,16 +296,16 @@
                         subprocess.call(['rm',crnx_name]) # remove old file
                 except:
                     okok = 1
                     print('Could not find ', file_name, ' at BKG')
                 if os.path.isfile(oname):
                     #print('successful download ', oname)
                     fileF = fileF + 1
-                #else:
-                #    print('unsuccessful download ', oname)
+                else:
+                    print('Unsuccessful download ', oname)
 
     searchP = station.upper() + streamID + cyyyy + cdoy + '*15M*MO.rnx'
     print('Found ', fileF,' 15 minute files')
 
     outfile = station.upper() + cyyyy + cdoy + '.tmp'
     crate = '{:02d}'.format(dec_rate)
 
@@ -434,7 +434,144 @@
 
     # remove one hour files
     cm = 'rm ' + station.upper() + streamID + cyyyy + cdoy + '*01H_01S_MO.rnx'
     if fexist:
         subprocess.call(cm,shell=True)
 
     return file_name24,  fexist
+
+
+def cddis_highrate_tar(station, year, month, day,stream,dec_rate):
+    """
+    picks up a tar'ed highrate RINEX files from CDDIS, untars it, and merges.
+
+    Parameters
+    ----------
+    station : str
+        4 char or 9 char station name
+        Rinex 2.11 for the first and rinex 3 for the latter
+    year : int
+        full year
+    month : int
+        calendar month
+    day : int 
+        calendar day
+    stream : str
+        rinex3 ID, S or R
+    dec_rate : int
+        decimation rate, seconds
+
+    Returns
+    -------
+    rinexname : str
+        name of the merged/uncompressed outputfile
+    fexist : bool
+        whether the Rinex file was successfully retrieved
+
+    requires hatanaka code and gfzrnx
+    """
+    s1=time.time()
+    fexist  = False
+    version = 3 # only version 3
+    crnxpath = g.hatanaka_version()
+    gfzpath = g.gfz_version()
+    alpha='abcdefghijklmnopqrstuvwxyz'
+    # if doy is input
+    if day == 0:
+        doy=month
+        d = g.doy2ymd(year,doy);
+        month = d.month; day = d.day
+    doy,cdoy,cyyyy,cyy = g.ymd2doy(year,month,day); 
+
+    if not os.path.isfile(gfzpath):
+        print('You need to install gfzrnx to use high-rate RINEX data in gnssrefl.')
+        return
+
+    gns = 'https://cddis.nasa.gov/archive/gnss/data/highrate/' 
+    gns = gns + cyyyy + '/'+ cdoy + '/' +cyy + 'd/'
+
+    streamID  = '_' + stream + '_'
+
+    new_way_dir = 'gnss/data/highrate/' + cyyyy + '/' + cdoy + '/'
+    file_name = station.upper() +  streamID + cyyyy + cdoy + '0000_01D_01S_MO.crx.tar'
+    #print(new_way_dir,file_name)
+    if os.path.isfile(file_name):
+        print('already have the tar file - so it has probably been un tarred')
+    else:
+        g.cddis_download_2022B(file_name,new_way_dir)
+        if os.path.isfile(file_name):
+            subprocess.call(['tar','-xf', file_name])
+            print('Now remove the tar file')
+            subprocess.call(['rm', file_name])
+
+    fileF = 0
+    for h in range(0,24):
+        # subdirectory
+        ch = '{:02d}'.format(h)
+        print('Hour: ', ch)
+        #gnss/data/highrate/2023/199/23d/22
+        new_way_dir = 'gnss/data/highrate/' + cyyyy + '/' + cdoy + '/' + cyy + 'd/' + ch + '/'
+        for e in ['00', '15', '30', '45']:
+            file_name = station.upper() + streamID + cyyyy + cdoy + ch + e + '_15M_01S_MO.crx.gz'
+            crnx_name = file_name[:-3] 
+            oname = station.upper() + streamID + cyyyy + cdoy + ch + e + '_15M_01S_MO.rnx' # do we need this?
+            if os.path.isfile(new_way_dir + oname):
+                #print('Found rnx file', oname)
+                subprocess.call(['mv',new_way_dir + oname, 'gnss/data'])
+                fileF = fileF + 1
+            elif os.path.isfile(new_way_dir + file_name):
+                #print('Found file:', new_way_dir,file_name)
+                subprocess.call(['gunzip',new_way_dir + file_name])
+                subprocess.call([crnxpath, new_way_dir + crnx_name])
+                subprocess.call(['rm',new_way_dir + crnx_name])
+                subprocess.call(['mv',new_way_dir + oname, 'gnss/data'])
+                if os.path.isfile('gnss/data/' + oname):
+                    fileF = fileF + 1
+            else:
+                print('did not find  file:', new_way_dir,file_name)
+    # moved the files to 'gnss/data/'
+    searchpath = 'gnss/data/' + station.upper() + streamID + cyyyy + cdoy + '*.rnx'
+    #print(searchpath)
+    rinexname = station.upper() + streamID + cyyyy + cdoy + '0000_01D_01S_MO.rnx'
+    tmpname = rinexname + 'tmp'
+
+    print('Attempt to merge the 15 minute files using gfzrnx and move to ', rinexname)
+    if (fileF > 0): # files exist
+        if (dec_rate == 1):
+            subprocess.call([gfzpath,'-finp', searchpath, '-fout', tmpname, '-vo',str(version),'-f','-q'])
+        else:
+            print('Am decimating with gfzrnx')
+            crate = str(dec_rate)
+            subprocess.call([gfzpath,'-finp', searchpath, '-fout', tmpname, '-vo',str(version),'-sei','out','-smp',crate,'-f','-q'])
+
+        cm = 'rm ' + searchpath 
+        if os.path.isfile(tmpname): # clean up
+            ok = 1
+            subprocess.call(cm,shell=True)
+            subprocess.call(['mv',tmpname,rinexname])
+            print('File created ', rinexname)
+            fexist = True
+
+        # remove unneeded 15 minute files
+        #new_way_dir = 'gnss/data/highrate/' + cyyyy + '/' + cdoy + '/' + cyy + 'd/' + ch + '/'
+        new_dir =      'gnss/data/highrate/' + cyyyy + '/' + cdoy + '/' + cyy + 'd/*'
+        print('remove compressed 15 minute files')
+        cm = 'rm -rf ' + new_dir
+        subprocess.call(cm,shell=True)
+
+        print('remove converted 15 minute files')
+        searchpath = 'gnss/data/' + station.upper() + streamID + cyyyy + cdoy + '*.rnx'
+        cm = 'rm -rf ' + searchpath
+        subprocess.call(cm,shell=True)
+
+        # remove junk from CDDIS
+        searchpath = station.upper() + streamID + cyyyy + cdoy + '*.md5.txt'
+        cm = 'rm -rf ' + searchpath
+        subprocess.call(cm,shell=True)
+
+        searchpath = station.upper() + streamID + cyyyy + cdoy + '*.sha512.txt'
+        cm = 'rm -rf ' + searchpath
+        subprocess.call(cm,shell=True)
+
+    s2=time.time()
+    print('That download/merge experience took ', int(s2-s1), ' seconds.')
+    return rinexname,  fexist
```

### Comparing `gnssrefl-3.2.0/gnssrefl/installexe_cl.py` & `gnssrefl-3.2.2/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/invsnr_cl.py` & `gnssrefl-3.2.2/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/invsnr_input.py` & `gnssrefl-3.2.2/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/karnak_libraries.py` & `gnssrefl-3.2.2/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/kelly.py` & `gnssrefl-3.2.2/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/llh2xyz.py` & `gnssrefl-3.2.2/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/make_meta.py` & `gnssrefl-3.2.2/gnssrefl/make_meta.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/max_resolve_RH_cl.py` & `gnssrefl-3.2.2/gnssrefl/max_resolve_RH_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/nmea2snr.py` & `gnssrefl-3.2.2/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/nmea2snr_cl.py` & `gnssrefl-3.2.2/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/nyquist_libs.py` & `gnssrefl-3.2.2/gnssrefl/nyquist_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/phase_functions.py` & `gnssrefl-3.2.2/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/prn2gps.py` & `gnssrefl-3.2.2/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/query_unr.py` & `gnssrefl-3.2.2/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/quickLook_cl.py` & `gnssrefl-3.2.2/gnssrefl/quickLook_cl.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,18 @@
         maximum allowed arc length, in minutes
         default is 75 minutes.
 
     hires_figs : bool, optional
         eps instead of png files
     """
 
+    vers = 'gnssrefl version ' + str(g.version('gnssrefl'))
+    print('You are running ', vers)
+
+
 #   make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
 
     # checks for output
     g.checkFiles(station, '')
 
     exitS = g.check_inputs(station, year, doy, snr)
```

### Comparing `gnssrefl-3.2.0/gnssrefl/quickLook_function2.py` & `gnssrefl-3.2.2/gnssrefl/quickLook_function2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/quickPhase.py` & `gnssrefl-3.2.2/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/quicklib.py` & `gnssrefl-3.2.2/gnssrefl/quicklib.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,24 +53,24 @@
         print('You asked to plot column', ycol+1, ' and that column does not exist in the file')
         sys.exit()
     if (xcol+1 > nc):
         print('You asked to plot column', xcol+1, ' and that column does not exist in the file')
         sys.exit()
 
     if ymd :
+        yval = tvd[:,ycol] # ??
         for i in range(0,len(tvd)):
             bigT = datetime.datetime(year=int(tvd[i,0]), month=int(tvd[i,1]), day=int(tvd[i,2]) )
             tval.append(bigT)
-            yval.append( tvd[i,ycol])
     elif ymdhm:
+        yval = tvd[:,ycol] # ??
         for i in range(0,len(tvd)):
             bigT = datetime.datetime(year=int(tvd[i,0]), month=int(tvd[i,1]), 
                                      day=int(tvd[i,2]), hour=int(tvd[i,3]), minute=int(tvd[i,4]), second=0)
             tval.append(bigT)
-            yval.append( tvd[i,ycol])
     else:
         if convert_mjd:
             mm = tvd[:,xcol]
             if utc_offset is not None :
                 if utc_offset != 0:
                     print('Apply local time offset')
                     mm = mm + utc_offset*3600/86400
```

### Comparing `gnssrefl-3.2.0/gnssrefl/quickplt.py` & `gnssrefl-3.2.2/gnssrefl/quickplt.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     parser.add_argument("-ymd", help="True/T for when columns 1-3 are year month day ", type=str,default=None)
     parser.add_argument("-ymdhm", help="True/T for when columns 1-5 are year month day hour minute", type=str,default=None)
     parser.add_argument("-xlabel", type=str, help="optional x-axis label", default=None)
     parser.add_argument("-ylabel", type=str, help="optional y-axis label", default=None)
     parser.add_argument("-symbol", help="plot symbol, e.g. o or -", type=str,default=None)
     parser.add_argument("-title", help="optional title", type=str,default=None)
     parser.add_argument("-outfile", help="optional filename for plot. Must end in png", type=str,default=None)
-    parser.add_argument("-xlimits", nargs="*",type=float, help="optional x-axis limits", default=None)
+    parser.add_argument("-xlimits", nargs="*",type=str, help="optional x-axis limits, use yyyyMMdd", default=None)
     parser.add_argument("-ylimits", nargs="*",type=float, help="optional y-axis limits", default=None)
     parser.add_argument("-ydoy", help="True/T for when columns 1-2 are year and doy", type=str,default=None)
     parser.add_argument("-filename2", help="second filename", type=str, default=None)
     parser.add_argument("-freq", help="spec freq, column 11 in a LSP file ", type=int,default=None)
     parser.add_argument("-utc_offset", help="offset from UTC, hours  ", type=int,default=None)
     parser.add_argument("-yoffset", help="offset for y-axis values", type=float,default=None)
     parser.add_argument("-yoffset2", help="offset for y-axis values in file 2", type=float,default=None)
@@ -55,15 +55,15 @@
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def run_quickplt (filename: str, xcol: str, ycol: str, errorcol: int=None, mjd: bool=False, xlabel: str=None, 
                   ylabel: str=None, symbol: str=None, reverse:bool=False,title:str=None,outfile: str=None,
-                  xlimits: float=[], ylimits: float=[], ydoy:bool=False, ymd:bool=False, ymdhm:bool=False, 
+                  xlimits: str=None, ylimits: float=[], ydoy:bool=False, ymd:bool=False, ymdhm:bool=False, 
                   filename2: str=None, freq:int=None, utc_offset: int=None, yoffset: float=None, 
                   keepzeros: bool=False, sat: str=None,yoffset2: float=None,scale: float=1.0, 
                   scale2: float=1.0, elimits: float=[0], azlimits:float=[0], plt:bool=True):
 
     """
     quick file plotting using matplotlib
 
@@ -169,16 +169,18 @@
         'b.' or 'b^'
     reverse : bool, optional
         to reverse y-axis limits
     title : str, optional
         title for plot 
     outfile : str, optional
         name of png file to store plot 
-    xlimits: list of floats, optional
+    xlimits: list of str, 
         xaxis limits  
+        if you selected any time options (ymd, mjd, ydoy,mjd), the code assumes
+        a format of yyyyMMdd (year,month,day) 
     ylimits: list of floats, optional
         yaxis limits  
     ydoy : bool, optional
         if columns 1 and 2 are year and doy, the x-axis will be plotted in obstimes
         you should select column 1 to plot
     ymd : bool, optional
         if columns 1,2,3 are year, month, date. So meant for plots with daily measurements -
@@ -212,14 +214,17 @@
     azlimits : list of floats
         if SNR file is plotted, azimuth angle limits are applied
     plt: bool
          whether you want the plot to be displayed on the screen.
          png file is always created.
 
     """
+    if xlimits is None:
+        xlimits = []
+
     snrfile = False
     if sat is not None:
         snrfile = True
 
         if xcol == 'elevation':
             xcol = 1 # python column
         elif xcol == 'time':
@@ -263,15 +268,14 @@
 
     secondFile = False
 
     if yoffset is None:
         yoffset = 0
     if yoffset2 is None:
         yoffset2 = 0
-
     reverse_sign = reverse
 
     convert_mjd = mjd
     commentsign = '%'
 
     basename = os.path.basename(filename)
     station = basename[0:4]
@@ -460,35 +464,50 @@
 
 
     if len(ylimits) == 2:
         print('found y-axis limits')
         myplt.ylim((ylimits))
     if len(xlimits) == 2:
         print('found x-axis limits')
+        if (convert_mjd | ymd | ydoy | ymdhm):
+            if (len(xlimits[0]) != 8):
+                print('xlimit format is YYYYMMDD, but you said: ', xlimits[0], ' Exiting'); sys.exit()
+            if (len(xlimits[1]) != 8):
+                print('xlimit format is YYYYMMDD, but you said: ', xlimits[1], ' Exiting'); sys.exit()
+        else:
+            # make sure you change from string to numbers
+            xlimits[0] = float(xlimits[0])
+            xlimits[1] = float(xlimits[1])
+
         if convert_mjd:
-            t1 = Time(xlimits[0],format='mjd')
+            # need to just get MJD so you can use the local UTC offset
+            year1, month1, day1, doy1, mjd1 = g.noaa2me(xlimits[0])
+            year2, month2, day2, doy2, mjd2 = g.noaa2me(xlimits[1])
+
+            t1 = Time(mjd1,format='mjd')
             t1_utc = t1.utc # change to UTC
             tvalues1 =  t1_utc.datetime # change to datetime
-            t2 = Time(xlimits[1],format='mjd')
+            t2 = Time(mjd2,format='mjd')
             t2_utc = t2.utc # change to UTC
             tvalues2 =  t2_utc.datetime # change to datetime
             myplt.xlim((tvalues1,tvalues2))
             if utc_offset is not None:
                 cc = '{:02d}'.format(abs(utc_offset)) + ':00'
                 if utc_offset < 0:
                     myplt.xlabel('UTC-' + cc)
                 else:
                     myplt.xlabel('UTC+' + cc)
         else:
-            if ydoy:
-                t1,t2 = q.set_xlimits_ydoy(xlimits)
+            if ymd | ydoy | ymdhm :
+                t1 = g.noaatime_to_obstime(xlimits[0])
+                t2 = g.noaatime_to_obstime(xlimits[1])
                 myplt.xlim((t1,t2))
-            else:
-                myplt.xlim((xlimits))
-
+            else: 
+                # this is for when you are plotting something that isn't time
+                myplt.xlim((xlimits[0], xlimits[1]))
 
     if reverse_sign:
         ax.invert_yaxis()
     fig.autofmt_xdate() # obstimes
 
     q.save_plot(outfile)
     if plt:
```

### Comparing `gnssrefl-3.2.0/gnssrefl/read_snr_files.py` & `gnssrefl-3.2.2/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/refl_zones.py` & `gnssrefl-3.2.2/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/refl_zones_cl.py` & `gnssrefl-3.2.2/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/refraction.py` & `gnssrefl-3.2.2/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/rh_plot.py` & `gnssrefl-3.2.2/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/rinex2snr.py` & `gnssrefl-3.2.2/gnssrefl/rinex2snr.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,21 +288,26 @@
                                 if screenstats:
                                     print('RINEX 2 file derived from the GA archive should now exist:', r2)
                             if archive == 'cddis':
                                 bad_day = g.cddis_restriction(year, doy,'cddis')
                                 if not bad_day:
                                     rnx_filename,foundit = ch.cddis_highrate(station9ch, year, doy, 0,stream,dec_rate)
                                 else: 
+                                    print('Check the tar version')
+                                    rnx_filename,foundit = ch.cddis_highrate_tar(station9ch, year, doy, 0,stream,dec_rate)
+                                    print(rnx_filename, ' returned from tar version')
+                                if not foundit:
                                     print('No high-rate RINEX data will be downloaded')
                                     foundit = False; fexists = False; rnx_file = ''
-                                if foundit:
+                                else:
                                     if screenstats:
                                         print('The RINEX 3 file has been downloaded from CDDIS . Try to make ', r2)
                                     fexists = g.new_rinex3_rinex2(rnx_filename,r2,dec_rate)
                             if archive == 'bkg':
+                                # this is confusing - so the bkg variable is either IGS or EUREF
                                 bad_day = g.cddis_restriction(year, doy,'bkg')
                                 if not bad_day:
                                     rnx_filename,foundit = ch.bkg_highrate(station9ch, year, doy, 0,stream,dec_rate,bkg)
                                 else:
                                     print('No high-rate RINEX data will be downloaded')
                                     foundit = False; fexists = False; rnx_file = ''
                                 if foundit:
```

### Comparing `gnssrefl-3.2.0/gnssrefl/rinex2snr_cl.py` & `gnssrefl-3.2.2/gnssrefl/rinex2snr_cl.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,14 +334,17 @@
         default is false. snr files created every 30 days instead of every day
 
     par : int, optional
         default is NOne.  parallel processing, valid up to 10
 
     """
 
+    vers = 'gnssrefl version ' + str(g.version('gnssrefl'))
+    print('You are running ', vers)
+
     archive_list_rinex3 = ['unavco', 'epn','cddis', 'bev', 'bkg', 'ga', 'epn', 'bfg','sonel','all','unavco2','nrcan','gfz','ignes']
     archive_list = ['sopac', 'unavco', 'sonel',  'nz', 'ga', 'bkg', 'jeff',
                     'ngs', 'nrcan', 'special', 'bev', 'jp', 'all','unavco2','cddis']
 
     archive_list_no_parallel = ['sopac','cddis','jeff']
 
     if False:
@@ -479,15 +482,15 @@
         else:
             bkg = 'IGS'
         # change archive name back to original name
         archive = 'bkg'
 
 
     # adding spanish archive
-    highrate_list = ['unavco', 'nrcan', 'ga','bkg','cddis','ignes']  
+    highrate_list = ['unavco', 'nrcan', 'ga','bkg','cddis','ignes','bkg-igs','bkg-euref']  
     if ns == 9:
         # rinex3
         if rate == 'high':
             if (archive not in highrate_list) and (nolook == False):
                 print('You have chosen an archive not supported by the code.')
                 print(highrate_list)
                 sys.exit()
```

### Comparing `gnssrefl-3.2.0/gnssrefl/rinex3_rinex2.py` & `gnssrefl-3.2.2/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/rinex3_snr.py` & `gnssrefl-3.2.2/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/rinex_coords.py` & `gnssrefl-3.2.2/gnssrefl/rinex_coords.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/rinpy.py` & `gnssrefl-3.2.2/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-3.2.2/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/sd_libs.py` & `gnssrefl-3.2.2/gnssrefl/sd_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/smoosh.py` & `gnssrefl-3.2.2/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/smoosh_snr.py` & `gnssrefl-3.2.2/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/snow_functions.py` & `gnssrefl-3.2.2/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/snowdepth_cl.py` & `gnssrefl-3.2.2/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/spline_functions.py` & `gnssrefl-3.2.2/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/subdaily.py` & `gnssrefl-3.2.2/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/subdaily_cl.py` & `gnssrefl-3.2.2/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/utils.py` & `gnssrefl-3.2.2/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/veg_multiyr.py` & `gnssrefl-3.2.2/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/vwc_cl.py` & `gnssrefl-3.2.2/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/vwc_input.py` & `gnssrefl-3.2.2/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/xnmeasnr.f` & `gnssrefl-3.2.2/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/xyz2llh.py` & `gnssrefl-3.2.2/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/ydoy.py` & `gnssrefl-3.2.2/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl/ymd.py` & `gnssrefl-3.2.2/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-3.2.2/gnssrefl.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.2.0
+Version: 3.2.2
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.2.0 
+# gnssrefl v3.2.2 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494) 
@@ -26,14 +26,16 @@
 
 ![](docs/myAnimation.gif)
 
 I made this animation ages ago - so it is in Matlab.  I would be happy to host a link to 
 a version in python.  The main code is [snr_simulation](docs/pages/snr_simulation.m) 
 and the helper function is [setFrame.m](docs/pages/set_Frame.m). 
 
+High-rate data from CDDIS that are more than six months old can now be downloaded.
+
 Documentation:
 
 - [online](https://gnssrefl.readthedocs.io/en/latest/)
 
 - [pdf](https://gnssrefl.readthedocs.io/_/downloads/en/latest/pdf/)
 
 - [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `gnssrefl-3.2.0/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-3.2.2/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-3.2.2/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/pyproject.toml` & `gnssrefl-3.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.0/setup.py` & `gnssrefl-3.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "simplekml",
     "earthscope-sdk",
     "jupyterlab",
     "ipywidgets"
 ]
 setup(
     name="gnssrefl",
-    version="3.2.0",
+    version="3.2.2",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-3.2.0/test/test_gps.py` & `gnssrefl-3.2.2/test/test_gps.py`

 * *Files identical despite different names*

