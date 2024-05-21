# Comparing `tmp/nansat-1.6.1.tar.gz` & `tmp/nansat-1.6.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nansat-1.6.1.tar", last modified: Thu Apr 11 12:34:28 2024, max compression
+gzip compressed data, was "nansat-1.6.2rc1.tar", last modified: Tue May 21 09:53:01 2024, max compression
```

## Comparing `nansat-1.6.1.tar` & `nansat-1.6.2rc1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.088415 nansat-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35127 2024-04-11 12:34:26.000000 nansat-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 12:34:26.000000 nansat-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-11 12:34:28.088415 nansat-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-11 12:34:26.000000 nansat-1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.068415 nansat-1.6.1/nansat/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32792 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21060 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    35475 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/figure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.068415 nansat-1.6.1/nansat/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   720012 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/fonts/DejaVuSans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/geolocation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.076415 nansat-1.6.1/nansat/mappers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19395 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/envisat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3439 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/get_grib.pl
--rwxr-xr-x   0 runner    (1001) docker     (127)     3150 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/get_inv.pl
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/globcolour.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/hdf4_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_aapp_l1b.py
--rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_aapp_l1c.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_amsr2_l1r.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_amsr2_l3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_amsre_uham_leadfraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_arome.py
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_asar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ascat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_aster_l1a.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_aster_l1b.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_case2reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_cmems.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_csks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ecmwf_metno.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_emodnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    24579 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_geostationary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_globcolour_l3b.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_globcolour_l3m.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_goci_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_hirlam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_hirlam_wind_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_kmss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_landsat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_meris_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_meris_l2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_metno_hfr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_metno_hires_seaice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_metno_local_hires_seaice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_mod44w.py
--rw-r--r--   0 runner    (1001) docker     (127)    20692 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_modis_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ncep.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ncep_wind.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ncep_wind_online.py
--rw-r--r--   0 runner    (1001) docker     (127)    19296 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_netcdf_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_netcdf_cf_sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_nora10_local_vpv.py
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_obpg_l2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_obpg_l2_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_obpg_l3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ocean_productivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_arome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_globcurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_globcurrent_thredds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_mywave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_occci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_osisaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_ostia.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel1_wind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_siwtacsst.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_sstcci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_pathfinder52.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_quikscat.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_radarsat2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25487 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_sentinel1_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_sentinel1_l2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_topography.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_viirs_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/obpg.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/opendap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/scatterometers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (127)    60463 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/nansat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/nsr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.076415 nansat-1.6.1/nansat/pixelfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/MakefileWin
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/README_Nansat
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/_pixfun_py2.c
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/_pixfun_py3.c
--rw-r--r--   0 runner    (1001) docker     (127)    57315 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/pixelfunctions.c
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/pixfunplugin.c
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pointbrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.080415 nansat-1.6.1/nansat/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.084415 nansat-1.6.1/nansat/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   350912 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/arctic.nc
--rw-r--r--   0 runner    (1001) docker     (127)   327344 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/complex.nc
--rw-r--r--   0 runner    (1001) docker     (127)   126224 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/gcps.tif
--rw-r--r--   0 runner    (1001) docker     (127)  2164298 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/map.tif
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/nansat_logo_s.png
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/points.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/points.shp
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/points.shx
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/some_xml_file.xml
--rw-r--r--   0 runner    (1001) docker     (127)   218690 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/stere.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.084415 nansat-1.6.1/nansat/tests/mappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_netcdf_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap_arome.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap_mywave.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap_ostia.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/nansat_test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/nansat_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    26206 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_geolocation.py
--rw-r--r--   0 runner    (1001) docker     (127)    34081 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_nansat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_nsr.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_pixelfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_pointbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29775 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_vrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    71148 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/vrt.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.068415 nansat-1.6.1/nansat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.088415 nansat-1.6.1/nansat_integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/mapper_test_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/test_mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/test_netcdf_cf_mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/test_open_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/test_radarsat2.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:34:28.088415 nansat-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-11 12:34:26.000000 nansat-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.088415 nansat-1.6.1/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1653 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansat_add_coastline
--rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansat_geotiffimage
--rwxr-xr-x   0 runner    (1001) docker     (127)      814 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansat_show
--rwxr-xr-x   0 runner    (1001) docker     (127)      728 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansat_translate
--rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansatinfo
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.666633 nansat-1.6.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    35127 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      121 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1413 2024-05-21 09:53:01.666633 nansat-1.6.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5302 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.642633 nansat-1.6.2rc1/nansat/
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32792 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/domain.py
+-rw-r--r--   0 root         (0) root         (0)      978 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    21060 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/exporter.py
+-rw-r--r--   0 root         (0) root         (0)    35475 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/figure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.642633 nansat-1.6.2rc1/nansat/fonts/
+-rw-r--r--   0 root         (0) root         (0)   720012 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/fonts/DejaVuSans.ttf
+-rw-r--r--   0 root         (0) root         (0)     4573 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/geolocation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.654633 nansat-1.6.2rc1/nansat/mappers/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19395 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/envisat.py
+-rwxr-xr-x   0 root         (0) root         (0)     3439 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/get_grib.pl
+-rwxr-xr-x   0 root         (0) root         (0)     3150 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/get_inv.pl
+-rw-r--r--   0 root         (0) root         (0)     2974 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/globcolour.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/hdf4_mapper.py
+-rw-r--r--   0 root         (0) root         (0)    10643 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_aapp_l1b.py
+-rw-r--r--   0 root         (0) root         (0)     9490 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_aapp_l1c.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_amsr2_l1r.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_amsr2_l3.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_amsre_uham_leadfraction.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_arome.py
+-rw-r--r--   0 root         (0) root         (0)    13280 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_asar.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_ascat.py
+-rw-r--r--   0 root         (0) root         (0)     5647 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_aster_l1a.py
+-rw-r--r--   0 root         (0) root         (0)     5494 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_aster_l1b.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_case2reg.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_cmems.py
+-rw-r--r--   0 root         (0) root         (0)     7937 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_csks.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_ecmwf_metno.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_emodnet.py
+-rw-r--r--   0 root         (0) root         (0)    15618 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_generic.py
+-rw-r--r--   0 root         (0) root         (0)    24579 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_geostationary.py
+-rw-r--r--   0 root         (0) root         (0)     7125 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_globcolour_l3b.py
+-rw-r--r--   0 root         (0) root         (0)     6271 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_globcolour_l3m.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_goci_l1.py
+-rw-r--r--   0 root         (0) root         (0)     4095 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_hirlam.py
+-rw-r--r--   0 root         (0) root         (0)     4217 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_hirlam_wind_netcdf.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_kmss.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_landsat.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_meris_l1.py
+-rw-r--r--   0 root         (0) root         (0)     9725 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_meris_l2.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_metno_hfr.py
+-rw-r--r--   0 root         (0) root         (0)     3882 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_metno_hires_seaice.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_metno_local_hires_seaice.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_mod44w.py
+-rw-r--r--   0 root         (0) root         (0)    20692 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_modis_l1.py
+-rw-r--r--   0 root         (0) root         (0)     5439 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_ncep.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_ncep_wind.py
+-rw-r--r--   0 root         (0) root         (0)     6319 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_ncep_wind_online.py
+-rw-r--r--   0 root         (0) root         (0)    19296 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_netcdf_cf.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_netcdf_cf_sentinel1.py
+-rw-r--r--   0 root         (0) root         (0)     5106 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_nora10_local_vpv.py
+-rw-r--r--   0 root         (0) root         (0)    13311 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_obpg_l2.py
+-rw-r--r--   0 root         (0) root         (0)     6122 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_obpg_l2_nc.py
+-rw-r--r--   0 root         (0) root         (0)     8499 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_obpg_l3.py
+-rw-r--r--   0 root         (0) root         (0)     5327 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_ocean_productivity.py
+-rw-r--r--   0 root         (0) root         (0)     3837 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_arome.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_globcurrent.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_globcurrent_thredds.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_mywave.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_occci.py
+-rw-r--r--   0 root         (0) root         (0)     3073 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_osisaf.py
+-rw-r--r--   0 root         (0) root         (0)     6131 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_ostia.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_sentinel1.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_sentinel1_wind.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_sentinel2.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_siwtacsst.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_opendap_sstcci.py
+-rw-r--r--   0 root         (0) root         (0)     3711 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_pathfinder52.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_quikscat.py
+-rw-r--r--   0 root         (0) root         (0)    15452 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_radarsat2.py
+-rw-r--r--   0 root         (0) root         (0)    25487 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_sentinel1_l1.py
+-rw-r--r--   0 root         (0) root         (0)     8233 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_sentinel1_l2.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_topography.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/mapper_viirs_l1.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/obpg.py
+-rw-r--r--   0 root         (0) root         (0)    13143 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/opendap.py
+-rw-r--r--   0 root         (0) root         (0)     4262 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/scatterometers.py
+-rw-r--r--   0 root         (0) root         (0)     7613 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/mappers/sentinel1.py
+-rw-r--r--   0 root         (0) root         (0)    60463 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/nansat.py
+-rw-r--r--   0 root         (0) root         (0)    11570 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/node.py
+-rw-r--r--   0 root         (0) root         (0)     3332 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/nsr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.654633 nansat-1.6.2rc1/nansat/pixelfunctions/
+-rw-r--r--   0 root         (0) root         (0)      793 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/pixelfunctions/Makefile
+-rw-r--r--   0 root         (0) root         (0)      574 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/pixelfunctions/MakefileWin
+-rw-r--r--   0 root         (0) root         (0)      783 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/pixelfunctions/README.txt
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/pixelfunctions/README_Nansat
+-rw-r--r--   0 root         (0) root         (0)      836 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/pixelfunctions/_pixfun_py2.c
+-rw-r--r--   0 root         (0) root         (0)     2713 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/pixelfunctions/_pixfun_py3.c
+-rw-r--r--   0 root         (0) root         (0)    57315 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/pixelfunctions/pixelfunctions.c
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/pixelfunctions/pixfunplugin.c
+-rw-r--r--   0 root         (0) root         (0)     6428 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/pointbrowser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.658633 nansat-1.6.2rc1/nansat/tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.662633 nansat-1.6.2rc1/nansat/tests/data/
+-rw-r--r--   0 root         (0) root         (0)   350912 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/arctic.nc
+-rw-r--r--   0 root         (0) root         (0)   327344 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/complex.nc
+-rw-r--r--   0 root         (0) root         (0)   126224 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/gcps.tif
+-rw-r--r--   0 root         (0) root         (0)  2164298 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/map.tif
+-rw-r--r--   0 root         (0) root         (0)     7534 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/nansat_logo_s.png
+-rw-r--r--   0 root         (0) root         (0)      113 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/points.dbf
+-rw-r--r--   0 root         (0) root         (0)      212 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/points.shp
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/points.shx
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/some_xml_file.xml
+-rw-r--r--   0 root         (0) root         (0)   218690 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/data/stere.tif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.662633 nansat-1.6.2rc1/nansat/tests/mappers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/mappers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16960 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/mappers/test_mapper_netcdf_cf.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/mappers/test_mapper_opendap.py
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/mappers/test_mapper_opendap_arome.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/mappers/test_mapper_opendap_mywave.py
+-rw-r--r--   0 root         (0) root         (0)      489 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/mappers/test_mapper_opendap_ostia.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/nansat_test_base.py
+-rw-r--r--   0 root         (0) root         (0)      811 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/nansat_test_data.py
+-rw-r--r--   0 root         (0) root         (0)    26206 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_domain.py
+-rw-r--r--   0 root         (0) root         (0)    21366 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_exporter.py
+-rw-r--r--   0 root         (0) root         (0)     5203 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_figure.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_geolocation.py
+-rw-r--r--   0 root         (0) root         (0)    34081 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_nansat.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_node.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_nsr.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_pixelfunctions.py
+-rw-r--r--   0 root         (0) root         (0)     3888 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_pointbrowser.py
+-rw-r--r--   0 root         (0) root         (0)     3948 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_tools.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    29775 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tests/test_vrt.py
+-rw-r--r--   0 root         (0) root         (0)     7406 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/tools.py
+-rw-r--r--   0 root         (0) root         (0)     9266 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/utils.py
+-rw-r--r--   0 root         (0) root         (0)    71259 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/vrt.py
+-rw-r--r--   0 root         (0) root         (0)      357 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.642633 nansat-1.6.2rc1/nansat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1413 2024-05-21 09:53:01.000000 nansat-1.6.2rc1/nansat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4667 2024-05-21 09:53:01.000000 nansat-1.6.2rc1/nansat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:53:01.000000 nansat-1.6.2rc1/nansat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-21 09:53:01.000000 nansat-1.6.2rc1/nansat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-21 09:53:01.000000 nansat-1.6.2rc1/nansat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.662633 nansat-1.6.2rc1/nansat_integration_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat_integration_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat_integration_tests/mapper_test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat_integration_tests/test_mappers.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat_integration_tests/test_netcdf_cf_mappers.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat_integration_tests/test_open_issues.py
+-rw-r--r--   0 root         (0) root         (0)     4314 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/nansat_integration_tests/test_radarsat2.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 09:53:01.666633 nansat-1.6.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9444 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:53:01.666633 nansat-1.6.2rc1/utilities/
+-rwxr-xr-x   0 root         (0) root         (0)     1653 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/utilities/nansat_add_coastline
+-rwxr-xr-x   0 root         (0) root         (0)      697 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/utilities/nansat_geotiffimage
+-rwxr-xr-x   0 root         (0) root         (0)      814 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/utilities/nansat_show
+-rwxr-xr-x   0 root         (0) root         (0)      728 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/utilities/nansat_translate
+-rwxr-xr-x   0 root         (0) root         (0)      416 2024-05-21 09:52:37.000000 nansat-1.6.2rc1/utilities/nansatinfo
```

### Comparing `nansat-1.6.1/LICENSE` & `nansat-1.6.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/PKG-INFO` & `nansat-1.6.2rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nansat
-Version: 1.6.1
+Version: 1.6.2rc1
 Summary: A scientist friendly Python toolbox for processing 2D satellite Earth observation data
 Home-page: https://github.com/nansencenter/nansat
 Download-URL: https://github.com/nansencenter/nansat
 Author: Anton Korosov, Morten W. Hansen, Kunt-Frode Dagestad, Aleksander Vines, Asuka Yamakawa, Artem Moiseev, Mohamed Babiker
 Author-email: nansat-dev@googlegroups.com
 Maintainer: Nansat Developers
 Maintainer-email: nansat-dev@googlegroups.com
```

### Comparing `nansat-1.6.1/README.rst` & `nansat-1.6.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/__init__.py` & `nansat-1.6.2rc1/nansat/__init__.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/domain.py` & `nansat-1.6.2rc1/nansat/domain.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/exceptions.py` & `nansat-1.6.2rc1/nansat/exceptions.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/exporter.py` & `nansat-1.6.2rc1/nansat/exporter.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/figure.py` & `nansat-1.6.2rc1/nansat/figure.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/fonts/DejaVuSans.ttf` & `nansat-1.6.2rc1/nansat/fonts/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/geolocation.py` & `nansat-1.6.2rc1/nansat/geolocation.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/envisat.py` & `nansat-1.6.2rc1/nansat/mappers/envisat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/get_grib.pl` & `nansat-1.6.2rc1/nansat/mappers/get_grib.pl`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/get_inv.pl` & `nansat-1.6.2rc1/nansat/mappers/get_inv.pl`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/globcolour.py` & `nansat-1.6.2rc1/nansat/mappers/globcolour.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/hdf4_mapper.py` & `nansat-1.6.2rc1/nansat/mappers/hdf4_mapper.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_aapp_l1b.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_aapp_l1b.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_aapp_l1c.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_aapp_l1c.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_amsr2_l1r.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_amsr2_l1r.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_amsr2_l3.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_amsr2_l3.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_amsre_uham_leadfraction.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_amsre_uham_leadfraction.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_arome.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_arome.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_asar.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_asar.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_ascat.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_ascat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_aster_l1a.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_aster_l1a.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_aster_l1b.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_aster_l1b.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_case2reg.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_case2reg.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_cmems.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_cmems.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_csks.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_csks.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_ecmwf_metno.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_ecmwf_metno.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_emodnet.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_emodnet.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_generic.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_generic.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_geostationary.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_geostationary.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_globcolour_l3b.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_globcolour_l3b.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_globcolour_l3m.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_globcolour_l3m.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_goci_l1.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_goci_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_hirlam.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_hirlam.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_hirlam_wind_netcdf.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_hirlam_wind_netcdf.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_kmss.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_kmss.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_landsat.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_landsat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_meris_l1.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_meris_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_meris_l2.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_meris_l2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_metno_hfr.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_metno_hfr.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_metno_hires_seaice.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_metno_hires_seaice.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_metno_local_hires_seaice.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_metno_local_hires_seaice.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_mod44w.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_mod44w.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_modis_l1.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_modis_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_ncep.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_ncep.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_ncep_wind.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_ncep_wind.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_ncep_wind_online.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_ncep_wind_online.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_netcdf_cf.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_netcdf_cf.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_netcdf_cf_sentinel1.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_netcdf_cf_sentinel1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_nora10_local_vpv.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_nora10_local_vpv.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_obpg_l2.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_obpg_l2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_obpg_l2_nc.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_obpg_l2_nc.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_obpg_l3.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_obpg_l3.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_ocean_productivity.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_ocean_productivity.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_arome.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_arome.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_globcurrent.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_globcurrent.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_globcurrent_thredds.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_globcurrent_thredds.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_mywave.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_mywave.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_occci.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_occci.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_osisaf.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_osisaf.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_ostia.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_ostia.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel1.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_sentinel1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel1_wind.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_sentinel1_wind.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel2.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_sentinel2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_siwtacsst.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_siwtacsst.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_opendap_sstcci.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_opendap_sstcci.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_pathfinder52.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_pathfinder52.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_quikscat.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_quikscat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_radarsat2.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_radarsat2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_sentinel1_l1.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_sentinel1_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_sentinel1_l2.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_sentinel1_l2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_topography.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_topography.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/mapper_viirs_l1.py` & `nansat-1.6.2rc1/nansat/mappers/mapper_viirs_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/obpg.py` & `nansat-1.6.2rc1/nansat/mappers/obpg.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/opendap.py` & `nansat-1.6.2rc1/nansat/mappers/opendap.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/scatterometers.py` & `nansat-1.6.2rc1/nansat/mappers/scatterometers.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/mappers/sentinel1.py` & `nansat-1.6.2rc1/nansat/mappers/sentinel1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/nansat.py` & `nansat-1.6.2rc1/nansat/nansat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/node.py` & `nansat-1.6.2rc1/nansat/node.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/nsr.py` & `nansat-1.6.2rc1/nansat/nsr.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/pixelfunctions/Makefile` & `nansat-1.6.2rc1/nansat/pixelfunctions/Makefile`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/pixelfunctions/MakefileWin` & `nansat-1.6.2rc1/nansat/pixelfunctions/MakefileWin`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/pixelfunctions/README.txt` & `nansat-1.6.2rc1/nansat/pixelfunctions/README.txt`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/pixelfunctions/README_Nansat` & `nansat-1.6.2rc1/nansat/pixelfunctions/README_Nansat`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/pixelfunctions/_pixfun_py2.c` & `nansat-1.6.2rc1/nansat/pixelfunctions/_pixfun_py2.c`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/pixelfunctions/_pixfun_py3.c` & `nansat-1.6.2rc1/nansat/pixelfunctions/_pixfun_py3.c`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/pixelfunctions/pixelfunctions.c` & `nansat-1.6.2rc1/nansat/pixelfunctions/pixelfunctions.c`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/pixelfunctions/pixfunplugin.c` & `nansat-1.6.2rc1/nansat/pixelfunctions/pixfunplugin.c`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/pointbrowser.py` & `nansat-1.6.2rc1/nansat/pointbrowser.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/data/arctic.nc` & `nansat-1.6.2rc1/nansat/tests/data/arctic.nc`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/data/complex.nc` & `nansat-1.6.2rc1/nansat/tests/data/complex.nc`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/data/gcps.tif` & `nansat-1.6.2rc1/nansat/tests/data/gcps.tif`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/data/map.tif` & `nansat-1.6.2rc1/nansat/tests/data/map.tif`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/data/nansat_logo_s.png` & `nansat-1.6.2rc1/nansat/tests/data/nansat_logo_s.png`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/data/stere.tif` & `nansat-1.6.2rc1/nansat/tests/data/stere.tif`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/mappers/test_mapper_netcdf_cf.py` & `nansat-1.6.2rc1/nansat/tests/mappers/test_mapper_netcdf_cf.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap.py` & `nansat-1.6.2rc1/nansat/tests/mappers/test_mapper_opendap.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/nansat_test_base.py` & `nansat-1.6.2rc1/nansat/tests/nansat_test_base.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/nansat_test_data.py` & `nansat-1.6.2rc1/nansat/tests/nansat_test_data.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_domain.py` & `nansat-1.6.2rc1/nansat/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_exporter.py` & `nansat-1.6.2rc1/nansat/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_figure.py` & `nansat-1.6.2rc1/nansat/tests/test_figure.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_geolocation.py` & `nansat-1.6.2rc1/nansat/tests/test_geolocation.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_nansat.py` & `nansat-1.6.2rc1/nansat/tests/test_nansat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_node.py` & `nansat-1.6.2rc1/nansat/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_nsr.py` & `nansat-1.6.2rc1/nansat/tests/test_nsr.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_pointbrowser.py` & `nansat-1.6.2rc1/nansat/tests/test_pointbrowser.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_tools.py` & `nansat-1.6.2rc1/nansat/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_utils.py` & `nansat-1.6.2rc1/nansat/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tests/test_vrt.py` & `nansat-1.6.2rc1/nansat/tests/test_vrt.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/tools.py` & `nansat-1.6.2rc1/nansat/tools.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/utils.py` & `nansat-1.6.2rc1/nansat/utils.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat/vrt.py` & `nansat-1.6.2rc1/nansat/vrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1725,15 +1725,18 @@
                'SourceType': 'ComplexSource',
                'ScaleRatio': 1.0,
                'ScaleOffset': 0.0}
         src.update(src_in)
 
         # find DataType of source (if not given in src)
         if src['SourceBand'] > 0 and 'DataType' not in src:
-            raster_band = gdal.Open(src['SourceFilename']).GetRasterBand(src['SourceBand'])
+            # prevent Python from releasing the dataset's handle
+            # prematurely
+            ds = gdal.Open(src['SourceFilename'])
+            raster_band = ds.GetRasterBand(src['SourceBand'])
             src['DataType'] = raster_band.DataType
 
         if 'xSize' not in src or 'ySize' not in src:
             ds = gdal.Open(src['SourceFilename'])
             src['xSize'] = ds.RasterXSize
             src['ySize'] = ds.RasterYSize
```

### Comparing `nansat-1.6.1/nansat.egg-info/PKG-INFO` & `nansat-1.6.2rc1/nansat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nansat
-Version: 1.6.1
+Version: 1.6.2rc1
 Summary: A scientist friendly Python toolbox for processing 2D satellite Earth observation data
 Home-page: https://github.com/nansencenter/nansat
 Download-URL: https://github.com/nansencenter/nansat
 Author: Anton Korosov, Morten W. Hansen, Kunt-Frode Dagestad, Aleksander Vines, Asuka Yamakawa, Artem Moiseev, Mohamed Babiker
 Author-email: nansat-dev@googlegroups.com
 Maintainer: Nansat Developers
 Maintainer-email: nansat-dev@googlegroups.com
```

### Comparing `nansat-1.6.1/nansat.egg-info/SOURCES.txt` & `nansat-1.6.2rc1/nansat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat_integration_tests/mapper_test_archive.py` & `nansat-1.6.2rc1/nansat_integration_tests/mapper_test_archive.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat_integration_tests/test_mappers.py` & `nansat-1.6.2rc1/nansat_integration_tests/test_mappers.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat_integration_tests/test_netcdf_cf_mappers.py` & `nansat-1.6.2rc1/nansat_integration_tests/test_netcdf_cf_mappers.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat_integration_tests/test_open_issues.py` & `nansat-1.6.2rc1/nansat_integration_tests/test_open_issues.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/nansat_integration_tests/test_radarsat2.py` & `nansat-1.6.2rc1/nansat_integration_tests/test_radarsat2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/setup.py` & `nansat-1.6.2rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,14 @@
     # remove mapper_tests from installed packages
     packages = find_packages()
     #if 'mapper_tests' in packages:
     #    packages.remove('mapper_tests')
 
     setup(
         name=NAME,
-        version=VERSION,
         maintainer=MAINTAINER,
         maintainer_email=MAINTAINER_EMAIL,
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         url=URL,
         download_url=DOWNLOAD_URL,
         license=LICENSE,
@@ -233,14 +232,16 @@
                      'nansat_geotiffimage',
                      'nansat_show',
                      'nansat_translate',
                      ]],
         cmdclass = {'install_scripts': my_install_scripts},
         install_requires=REQS,
         test_suite="nansat.tests",
+        use_scm_version=True,
+        setup_requires=['setuptools_scm'],
         **kw
     )
 
 try:
     run_setup(skip_compile)
 except ext_errors:
     BUILD_EXT_WARNING = ("WARNING: The C extension could not be compiled, "
```

### Comparing `nansat-1.6.1/utilities/nansat_add_coastline` & `nansat-1.6.2rc1/utilities/nansat_add_coastline`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/utilities/nansat_geotiffimage` & `nansat-1.6.2rc1/utilities/nansat_geotiffimage`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/utilities/nansat_show` & `nansat-1.6.2rc1/utilities/nansat_show`

 * *Files identical despite different names*

### Comparing `nansat-1.6.1/utilities/nansat_translate` & `nansat-1.6.2rc1/utilities/nansat_translate`

 * *Files identical despite different names*

