# Comparing `tmp/osml-imagery-toolkit-1.3.0.tar.gz` & `tmp/osml_imagery_toolkit-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osml-imagery-toolkit-1.3.0.tar", last modified: Fri Feb 16 13:34:10 2024, max compression
+gzip compressed data, was "osml_imagery_toolkit-1.4.0rc1.tar", last modified: Tue May 21 19:03:11 2024, max compression
```

## Comparing `osml-imagery-toolkit-1.3.0.tar` & `osml_imagery_toolkit-1.4.0rc1.tar`

### file list

```diff
@@ -1,128 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.444527 osml-imagery-toolkit-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-16 13:34:10.444527 osml-imagery-toolkit-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-16 13:34:10.444527 osml-imagery-toolkit-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.420527 osml-imagery-toolkit-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.416527 osml-imagery-toolkit-1.3.0/src/aws/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.420527 osml-imagery-toolkit-1.3.0/src/aws/osml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.420527 osml-imagery-toolkit-1.3.0/src/aws/osml/features/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/features/feature_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/features/geolocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/features/imaged_feature_property_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.424528 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.424528 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sicd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sicd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.424528 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sicd/models/
--rw-r--r--   0 runner    (1001) docker     (127)    12132 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sicd/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99182 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sicd/models/sicd_v1_2_1.py
--rw-r--r--   0 runner    (1001) docker     (127)   100834 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sicd/models/sicd_v1_3_0.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.424528 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.424528 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/
--rw-r--r--   0 runner    (1001) docker     (127)    32969 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.424528 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.424528 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.428527 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.428527 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ism25_x.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismclassification_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismcomplies_with.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismdissem.py
--rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismfgiopen.py
--rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismfgiprotected.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismnon_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismnon_uscontrols.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismowner_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismrel_to.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismscicontrols.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismsource_marked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.428527 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.428527 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.428527 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.432527 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ism25_x.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismatomic_energy_markings.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismclassification_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismcomplies_with.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismdissem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismexempt_from.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnon_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnon_uscontrols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnotice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismpoc_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismscicontrols.py
--rw-r--r--   0 runner    (1001) docker     (127)    44777 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/ic_ism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.432527 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.432527 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatfgiopen.py
--rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatfgiprotected.py
--rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatowner_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16300 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatrel_to.py
--rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    41340 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sicommon_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    49614 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sicommon_types_v1_0.py
--rw-r--r--   0 runner    (1001) docker     (127)    60087 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sidd_v1_0_0.py
--rw-r--r--   0 runner    (1001) docker     (127)   101811 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sidd_v2_0_0.py
--rw-r--r--   0 runner    (1001) docker     (127)   100999 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sidd_v3_0_0.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.436527 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/dynamic_range_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/gdal_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/gdal_dem_tile_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/gdal_sensor_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/gdal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/nitf_des_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/projective_sensor_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/rpc_sensor_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/rsm_sensor_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/sensor_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/sensor_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/sicd_sensor_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/sidd_sensor_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/xmltre_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.436527 osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/gdal_tile_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/sar_complex_imageop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/sicd_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/sidd_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.440528 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/chipped_image_sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/composite_sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/digital_elevation_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/elevation_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/gdal_sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/generic_dem_tile_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/projective_sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    38607 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/replacement_sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/rpc_sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    55446 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/sicd_sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/srtm_dem_tile_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-02-16 13:33:57.000000 osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 13:34:10.440528 osml-imagery-toolkit-1.3.0/src/osml_imagery_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-16 13:34:10.000000 osml-imagery-toolkit-1.3.0/src/osml_imagery_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-02-16 13:34:10.000000 osml-imagery-toolkit-1.3.0/src/osml_imagery_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 13:34:10.000000 osml-imagery-toolkit-1.3.0/src/osml_imagery_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 13:34:10.000000 osml-imagery-toolkit-1.3.0/src/osml_imagery_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-16 13:34:10.000000 osml-imagery-toolkit-1.3.0/src/osml_imagery_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-16 13:34:10.000000 osml-imagery-toolkit-1.3.0/src/osml_imagery_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.952661 osml_imagery_toolkit-1.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/PACKAGE_DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-21 19:03:11.952661 osml_imagery_toolkit-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-21 19:03:11.952661 osml_imagery_toolkit-1.4.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.928661 osml_imagery_toolkit-1.4.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.928661 osml_imagery_toolkit-1.4.0rc1/src/aws/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.928661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.932661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/features/feature_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/features/geolocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/features/imaged_feature_property_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.932661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.932661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sicd/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sicd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.932661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sicd/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sicd/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99242 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sicd/models/sicd_v1_2_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100894 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sicd/models/sicd_v1_3_0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.932661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.936661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    33029 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.936661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.936661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.936661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.936661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ism25_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismclassification_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismcomplies_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismdissem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16358 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismfgiopen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismfgiprotected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismnon_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismnon_uscontrols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16424 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismowner_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismrel_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismscicontrols.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismsource_marked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.936661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.940661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.940661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.940661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ism25_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismatomic_energy_markings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismclassification_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismcomplies_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismdissem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismexempt_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnon_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnon_uscontrols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnotice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismpoc_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismscicontrols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44837 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/ic_ism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.940661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.944661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16358 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatfgiopen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16391 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatfgiprotected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatowner_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatrel_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sicommon_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49674 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sicommon_types_v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60147 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sidd_v1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101871 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sidd_v2_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101059 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sidd_v3_0_0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.944661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/dynamic_range_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/gdal_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/gdal_dem_tile_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/gdal_sensor_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/gdal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/nitf_des_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/projective_sensor_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/rpc_sensor_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/rsm_sensor_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/sensor_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/sensor_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/sicd_sensor_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/sidd_sensor_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/xmltre_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.948661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21556 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/gdal_tile_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/map_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/map_tileset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/map_tileset_wmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/sar_complex_imageop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/sicd_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/sidd_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.948661 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/chipped_image_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/composite_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/digital_elevation_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/elevation_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/gdal_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/generic_dem_tile_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/projective_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38667 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/replacement_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12598 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/rpc_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55506 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/sicd_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/srtm_dem_tile_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-21 19:03:02.000000 osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:03:11.952661 osml_imagery_toolkit-1.4.0rc1/src/osml_imagery_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-21 19:03:11.000000 osml_imagery_toolkit-1.4.0rc1/src/osml_imagery_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-21 19:03:11.000000 osml_imagery_toolkit-1.4.0rc1/src/osml_imagery_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:03:11.000000 osml_imagery_toolkit-1.4.0rc1/src/osml_imagery_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:03:11.000000 osml_imagery_toolkit-1.4.0rc1/src/osml_imagery_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-21 19:03:11.000000 osml_imagery_toolkit-1.4.0rc1/src/osml_imagery_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 19:03:11.000000 osml_imagery_toolkit-1.4.0rc1/src/osml_imagery_toolkit.egg-info/top_level.txt
```

### Comparing `osml-imagery-toolkit-1.3.0/LICENSE` & `osml_imagery_toolkit-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `osml-imagery-toolkit-1.3.0/PKG-INFO` & `osml_imagery_toolkit-1.4.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-imagery-toolkit
-Version: 1.3.0
+Version: 1.4.0rc1
 Summary: Toolkit to work with imagery collected by satellites and UAVs
 Author: Amazon Web Services
 Author-email: aws-osml-admin@amazon.com
 License: 
         MIT No Attribution
         
         Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
@@ -26,44 +26,44 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: scikit-optimize>=0.9.0
+Requires-Dist: opencv-python-headless>=4.9.0
 Requires-Dist: cachetools>=5.3.2
 Requires-Dist: geojson>=3.1.0
 Requires-Dist: pyproj>=3.6.1
 Requires-Dist: shapely>=2.0.2
 Requires-Dist: omegaconf==2.3.0; python_version < "3.10.0"
 Requires-Dist: xsdata>=24.1
 Requires-Dist: defusedxml>=0.7.1
 Provides-Extra: gdal
 Requires-Dist: gdal>=3.7.0; extra == "gdal"
 Provides-Extra: test
 Requires-Dist: tox; extra == "test"
 
-# OversightML Imagery Toolkit
-
 The OversightML Imagery Toolkit is a Python package that contains image processing and photogrammetry routines commonly
 used during the analysis of imagery collected by satellites and unmanned aerial vehicles (UAVs). It builds upon GDAL
 by providing additional support for images compliant with the National Imagery Transmission Format (NITF), Sensor
 Independent Complex Data (SICD), and Sensor Independent Derived Data (SIDD) standards.
 
 This library contains four core packages under the `aws.osml` namespace:
 * **photogrammetry**: convert locations between the image (x, y) and geodetic (lon, lat, elev) coordinate systems
 * **gdal**: utilities to work with datasets loaded by GDAL
 * **image_processing**: common image manipulation routines
 * **features**: common geospatial feature manipulation routines
 
 ## Documentation
 
-* **APIs**: You can find API documentation for the OSML Imagery Toolkit hosted on our [GitHub project page](https://aws-solutions-library-samples.github.io/osml-imagery-toolkit/).
-If you are working from the source code running `tox -e docs` will trigger the Sphinx documentation build.
+* **APIs**: You can find the latest API documentation for the OSML Imagery Toolkit hosted [here](https://aws-solutions-library-samples.github.io/osml-imagery-toolkit/).
+  If you are working from the source code running `tox -e docs` will trigger the Sphinx documentation build.
 * **Example Notebooks**: Example notebooks for some operations are in the `examples` directory
+
 ## Installation
 
 This software is available through a Python Package Index.
 If your environment has a distribution, you should be able to install it using pip:
 ```shell
 pip install osml-imagery-toolkit[gdal]
 ```
@@ -74,18 +74,9 @@
 pip install .[gdal]
 ```
 Note that GDAL is listed as an extra dependency for this package. This is done to facilitate environments that either
 don't want to use GDAL or those that have their own custom installation steps for that library. Future versions of
 this package will include image IO backbones that have fewer dependencies.
 
 ## Contributing
-
-This project welcomes contributions and suggestions. If you would like to submit a pull request, see our
-[Contribution Guide](CONTRIBUTING.md) for more information.
-
-## Security
-
-See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
-
-## License
-
-This library is licensed under the MIT-0 License. See the [LICENSE](LICENSE) file.
+We welcome contributions and suggestions. If you would like to submit a pull request please do so using a GitHub pull
+request [here](https://github.com/aws-solutions-library-samples/osml-imagery-toolkit/pulls).
```

### Comparing `osml-imagery-toolkit-1.3.0/README.md` & `osml_imagery_toolkit-1.4.0rc1/PACKAGE_DESCRIPTION.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# OversightML Imagery Toolkit
-
 The OversightML Imagery Toolkit is a Python package that contains image processing and photogrammetry routines commonly
 used during the analysis of imagery collected by satellites and unmanned aerial vehicles (UAVs). It builds upon GDAL
 by providing additional support for images compliant with the National Imagery Transmission Format (NITF), Sensor
 Independent Complex Data (SICD), and Sensor Independent Derived Data (SIDD) standards.
 
 This library contains four core packages under the `aws.osml` namespace:
 * **photogrammetry**: convert locations between the image (x, y) and geodetic (lon, lat, elev) coordinate systems
 * **gdal**: utilities to work with datasets loaded by GDAL
 * **image_processing**: common image manipulation routines
 * **features**: common geospatial feature manipulation routines
 
 ## Documentation
 
-* **APIs**: You can find API documentation for the OSML Imagery Toolkit hosted on our [GitHub project page](https://aws-solutions-library-samples.github.io/osml-imagery-toolkit/).
-If you are working from the source code running `tox -e docs` will trigger the Sphinx documentation build.
+* **APIs**: You can find the latest API documentation for the OSML Imagery Toolkit hosted [here](https://aws-solutions-library-samples.github.io/osml-imagery-toolkit/).
+  If you are working from the source code running `tox -e docs` will trigger the Sphinx documentation build.
 * **Example Notebooks**: Example notebooks for some operations are in the `examples` directory
+
 ## Installation
 
 This software is available through a Python Package Index.
 If your environment has a distribution, you should be able to install it using pip:
 ```shell
 pip install osml-imagery-toolkit[gdal]
 ```
@@ -30,18 +29,9 @@
 pip install .[gdal]
 ```
 Note that GDAL is listed as an extra dependency for this package. This is done to facilitate environments that either
 don't want to use GDAL or those that have their own custom installation steps for that library. Future versions of
 this package will include image IO backbones that have fewer dependencies.
 
 ## Contributing
-
-This project welcomes contributions and suggestions. If you would like to submit a pull request, see our
-[Contribution Guide](CONTRIBUTING.md) for more information.
-
-## Security
-
-See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
-
-## License
-
-This library is licensed under the MIT-0 License. See the [LICENSE](LICENSE) file.
+We welcome contributions and suggestions. If you would like to submit a pull request please do so using a GitHub pull
+request [here](https://github.com/aws-solutions-library-samples/osml-imagery-toolkit/pulls).
```

### Comparing `osml-imagery-toolkit-1.3.0/setup.cfg` & `osml_imagery_toolkit-1.4.0rc1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = osml-imagery-toolkit
-version = 1.3.0
+version = 1.4.0rc1
 description = Toolkit to work with imagery collected by satellites and UAVs
-long_description = file: README.md
+long_description = file: PACKAGE_DESCRIPTION.md
 long_description_content_type = text/markdown
 author = Amazon Web Services
 author_email = aws-osml-admin@amazon.com
 license = 
 	MIT No Attribution
 	
 	Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
@@ -36,14 +36,15 @@
 	=src
 packages = find_namespace:
 python_requires = >=3.9
 include_package_data = True
 install_requires = 
 	numpy>=1.23.0
 	scikit-optimize>=0.9.0
+	opencv-python-headless>=4.9.0
 	cachetools>=5.3.2
 	geojson>=3.1.0
 	pyproj>=3.6.1
 	shapely>=2.0.2
 	omegaconf==2.3.0;python_version<'3.10.0'
 	xsdata>=24.1
 	defusedxml>=0.7.1
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/features/feature_index.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/features/feature_index.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from abc import ABC, abstractmethod
 from typing import Iterable, Optional
 
 import geojson
 import shapely
 
 from .imaged_feature_property_accessor import ImagedFeaturePropertyAccessor
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/features/geolocation.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/features/geolocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 import math
 from typing import List, Optional, Tuple, Union
 
 import geojson
 import numpy as np
 import shapely
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/features/imaged_feature_property_accessor.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/features/imaged_feature_property_accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import json
 from typing import Optional
 
 import geojson
 import shapely
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sicd/models/__init__.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sicd/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-08-30 17:21:13
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from .sicd_v1_2_1 import SICD as Type21SICD
 from .sicd_v1_2_1 import AntennaType as Type21AntennaType
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sicd/models/sicd_v1_2_1.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sicd/models/sicd_v1_2_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-08-30 17:21:13
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sicd/models/sicd_v1_3_0.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sicd/models/sicd_v1_3_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-08-30 17:21:13
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/__init__.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from .sfa import (
     AbstractReferenceSystemType,
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/__init__.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from .cvenum_ism25_x import CVEnumISM25X
 from .cvenum_ismclassification_all import CVEnumISMClassificationAll
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ism25_x.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ism25_x.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismclassification_all.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismclassification_all.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismcomplies_with.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismcomplies_with.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismdissem.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismdissem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismfgiopen.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismfgiopen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismfgiprotected.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismfgiprotected.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismnon_ic.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismnon_ic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismnon_uscontrols.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismnon_uscontrols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismowner_producer.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismowner_producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismrel_to.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismrel_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismsource_marked.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism/schema/cvegenerated/cvenum_ismsource_marked.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/__init__.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from .ic_ism import (
     LongStringWithSecurityType,
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/__init__.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from .cvenum_ism25_x import CVEnumISM25X
 from .cvenum_ismatomic_energy_markings import CVEnumISMatomicEnergyMarkingsValuesvalue
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ism25_x.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ism25_x.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismatomic_energy_markings.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismatomic_energy_markings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismclassification_all.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismclassification_all.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismcomplies_with.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismcomplies_with.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismdissem.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismdissem.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismexempt_from.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismexempt_from.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnon_ic.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnon_ic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnotice.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismnotice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismpoc_type.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismpoc_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismscicontrols.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/cvegenerated/cvenum_ismscicontrols.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/ic_ism.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ism/ic_ism.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from typing import List, Optional, Union
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/__init__.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from .cvenum_ismcatfgiopen import CVEnumISMCATFGIOpenValuesvalue
 from .cvenum_ismcatfgiprotected import CVEnumISMCATFGIProtectedValuesvalue
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatfgiopen.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatfgiopen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatfgiprotected.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatfgiprotected.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatowner_producer.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatowner_producer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatrel_to.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/external/ism_v13/schema/ismcat/cvegenerated/cvenum_ismcatrel_to.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sfa.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sfa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from typing import List, Optional
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sicommon_types.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sicommon_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sicommon_types_v1_0.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sicommon_types_v1_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sidd_v1_0_0.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sidd_v1_0_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sidd_v2_0_0.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sidd_v2_0_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/formats/sidd/models/sidd_v3_0_0.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/formats/sidd/models/sidd_v3_0_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 """This file was generated by xsdata, v23.8, on 2023-10-05 09:59:45
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/__init__.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 # Telling flake8 to not flag errors in this file. It is normal that these classes are imported but not used in an
 # __init__.py file.
 # flake8: noqa
 """
 The gdal package contains utilities that assist with loading imagery and metadata using the OSGeo GDAL library.
 
 Loading Imagery and Sensor Models with OSML
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/dynamic_range_adjustment.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/dynamic_range_adjustment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from typing import List, Optional
 
 
 class DRAParameters:
     """
     This class manages a set of parameters used to perform a Dynamic Range Adjustment that is applied when
     converting imagery pixel values (e.g. 11-bit per pixel panchromatic imagery to an 8-bit per pixel grayscale).
@@ -66,20 +68,20 @@
             cumulative_counts[i] = cumulative_counts[i] + cumulative_counts[i - 1]
 
         # Find the values that exclude the lowest and highest percentages of the counts.
         # This identifies the range that contains most of the pixels while excluding outliers.
         max_counts = cumulative_counts[-1]
         low_threshold = min_percentage * max_counts
         e_min = 0
-        while cumulative_counts[e_min] < low_threshold:
+        while cumulative_counts[e_min] < low_threshold and e_min < len(cumulative_counts) - 1:
             e_min += 1
 
         high_threshold = max_percentage * max_counts
         e_max = num_histogram_bins - 1
-        while cumulative_counts[e_max] > high_threshold:
+        while cumulative_counts[e_max] > high_threshold and e_max > 0:
             e_max -= 1
 
         min_value = max([actual_min_value, e_min - a * (e_max - e_min)])
         max_value = min([actual_max_value, e_max + b * (e_max - e_min)])
 
         value_step = (last_bucket_value - first_bucket_value) / num_histogram_bins
         return DRAParameters(
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/gdal_config.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/gdal_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from typing import Dict, Optional
 
 from osgeo import gdal
 
 logger = logging.getLogger(__name__)
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/gdal_dem_tile_factory.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/gdal_dem_tile_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from typing import Any, Optional, Tuple
 
 import numpy as np
 from osgeo import gdal
 
 from aws.osml.photogrammetry import (
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/gdal_sensor_model_builder.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/gdal_sensor_model_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from math import radians
 from typing import List, Optional
 
 from osgeo import gdal
 
 from aws.osml.photogrammetry import GDALAffineSensorModel, GeodeticWorldCoordinate, ImageCoordinate, ProjectiveSensorModel
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/gdal_utils.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/gdal_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 import re
 from typing import Dict, List, Optional, Tuple
 
 from defusedxml import ElementTree
 from osgeo import gdal, gdalconst
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/nitf_des_accessor.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/nitf_des_accessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from io import StringIO
 from typing import Callable, List, TypeVar
 from xml.etree import ElementTree as ET
 
 from defusedxml import ElementTree
 
 # This is a type placeholder needed by the _get_tre_field_value() type hints
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/projective_sensor_model_builder.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/projective_sensor_model_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from math import radians
 from typing import Optional
 from xml.etree import ElementTree as ET
 
 from aws.osml.photogrammetry import GeodeticWorldCoordinate, ImageCoordinate, ProjectiveSensorModel
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/rpc_sensor_model_builder.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/rpc_sensor_model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from typing import Optional
 from xml.etree import ElementTree as ET
 
 from aws.osml.photogrammetry import RPCPolynomial, RPCSensorModel
 
 from .sensor_model_builder import SensorModelBuilder
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/rsm_sensor_model_builder.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/rsm_sensor_model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from typing import List, Optional
 from xml.etree import ElementTree as ET
 
 from aws.osml.photogrammetry import (
     RSMContext,
     RSMGroundDomain,
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/sensor_model_builder.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/sensor_model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from abc import ABC, abstractmethod
 from typing import Optional
 
 from aws.osml.photogrammetry import SensorModel
 
 
 class SensorModelBuilder(ABC):
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/sensor_model_factory.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/sensor_model_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import base64
 import logging
 from enum import Enum
 from typing import List, Optional
 from xml.etree import ElementTree as ET
 
 from osgeo import gdal
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/sicd_sensor_model_builder.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/sicd_sensor_model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from typing import Optional, Union
 
 import numpy as np
 from xsdata.formats.dataclass.parsers import XmlParser
 
 import aws.osml.formats.sicd.models.sicd_v1_2_1 as sicd121
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/sidd_sensor_model_builder.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/sidd_sensor_model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from typing import Optional, Union
 
 from xsdata.formats.dataclass.parsers import XmlParser
 
 import aws.osml.formats.sidd.models.sidd_v1_0_0 as sidd100
 import aws.osml.formats.sidd.models.sidd_v2_0_0 as sidd200
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/typing.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/typing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from enum import Enum
 
 
 class GDALCompressionOptions(str, Enum):
     """
     Enumeration defining compression algorithms for image.
     """
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/gdal/xmltre_utils.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/gdal/xmltre_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from typing import Callable, List, TypeVar
 from xml.etree import ElementTree as ET
 
 # This is a type placeholder needed by the _get_tre_field_value() type hints
 T = TypeVar("T")
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/__init__.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 # Telling flake8 to not flag errors in this file. It is normal that these classes are imported but not used in an
 # __init__.py file.
 # flake8: noqa
 """
 The image_processing package contains various utilities for manipulating overhead imagery.
 
 Image Tiling: Tiling With Updated Image Metadata
@@ -44,14 +46,43 @@
                                        GDALImageFormats.PNG,
                                        GDALCompressionOptions.NONE,
                                        output_type=gdalconst.GDT_Byte,
                                        range_adjustment=RangeAdjustmentType.DRA)
 
     viz_tile = viz_tile_factory.create_encoded_tile([0, 0, 1024, 1024], output_size=(512, 512))
 
+Image Tiling: Map Tiles / Orthophotos
+*************************************
+
+The TileFactory supports creation of tiles suitable for use by geographic information systems (GIS) or map-based
+visualization tools. Given a north-east aligned bounding box in geographic coordinates the tile factory can use
+the sensor models to orthorectify imagery to remove the perspective and terrain effects.
+
+.. code-block:: python
+    :caption: Example showing creation of a map tile from the WebMercatorQuad tile set
+
+    # Look up the tile boundary for a tile in a well known tile set
+    tile_set = MapTileSetFactory.get_for_id("WebMercatorQuad")
+    tile_id = MapTileId(tile_matrix=16, tile_row=37025, tile_col=54816)
+    tile = tile_set.get_tile(tile_id)
+
+    # Create an orthophoto for this tile
+    image_bytes = viz_tile_factory.create_orthophoto_tile(geo_bbox=tile.bounds, tile_size=tile.size)
+
+.. figure:: ../images/MapTileExample-BeforeAfter.png
+    :width: 600
+    :alt: Original image with perspective effects and same area after orthorectification
+
+    Example showing original image with perspective effects and same area after orthorectification.
+
+.. figure:: ../images/MapTileExample-MapOverlay.png
+    :width: 400
+    :alt: Orthophoto tile overlaid on Google Maps
+
+    Example showing map tile overlaid on Google Maps
 
 Complex SAR Data Display
 ************************
 
 There are a variety of different techniques to convert complex SAR data to a simple image suitable for human display.
 The toolkit contains two helper functions that can convert complex image data into an 8-bit grayscle representation
 The equations implemented are described in Sections 3.1 and 3.2 of SAR Image Scaling, Dynamic Range, Radiometric
@@ -87,10 +118,21 @@
 -------------------------
 
 APIs
 ****
 """
 
 from .gdal_tile_factory import GDALTileFactory
+from .map_tileset import MapTile, MapTileId, MapTileSet
+from .map_tileset_factory import MapTileSetFactory, WellKnownMapTileSet
 from .sar_complex_imageop import histogram_stretch, quarter_power_image
 
-__all__ = ["GDALTileFactory", "histogram_stretch", "quarter_power_image"]
+__all__ = [
+    "GDALTileFactory",
+    "MapTile",
+    "MapTileId",
+    "MapTileSet",
+    "MapTileSetFactory",
+    "WellKnownMapTileSet",
+    "histogram_stretch",
+    "quarter_power_image",
+]
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/sar_complex_imageop.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/sar_complex_imageop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from typing import Optional, Tuple
 
 import numpy as np
 
 TWO_PI = np.pi * 2.0
 
@@ -75,15 +77,15 @@
     :param magnitude_values: SAR magnitude values
     :return: the scaled values in range [0:1]
     """
     min_value, max_value = get_value_bounds(magnitude_values)
     if max_value == min_value:
         return np.full(magnitude_values.shape, 0.5)
 
-    return np.clip((magnitude_values - min_value) / (max_value - min_value), 0, 1.0)
+    return np.clip((magnitude_values.astype(np.float32) - min_value) / (np.float32(max_value) - min_value), 0, 1.0)
 
 
 def histogram_stretch_mag_values(magnitude_values: np.ndarray, scale_factor: float = 8.0):
     """
     This function converts image pixel magnitudes to an 8-bit image by scaling the pixels and
     cropping to the desired range. This is histogram stretching without any gamma correction.
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/sicd_updater.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/sicd_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from math import floor
 from typing import List, Optional, Tuple
 
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/image_processing/sidd_updater.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/image_processing/sidd_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from typing import List, Optional, Tuple
 
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/__init__.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 # Telling flake8 to not flag errors in this file. It is normal that these classes are imported but not used in an
 # __init__.py file.
 # flake8: noqa
 """
 Many users need to estimate the geographic position of an object found in a georeferenced image. The osml-imagery-toolkit
 provides open source implementations of the image-to-world and world-to-image equations for some common replacement
 sensor models. These sensor models work with many georeferenced imagery types and do not require orthorectification of
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/chipped_image_sensor_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/chipped_image_sensor_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 
 from .coordinates import GeodeticWorldCoordinate, ImageCoordinate
 from .elevation_model import ElevationModel
 from .sensor_model import SensorModel
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/composite_sensor_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/composite_sensor_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import math
 from typing import Any, Dict, Optional
 
 from .coordinates import GeodeticWorldCoordinate, ImageCoordinate
 from .elevation_model import ElevationModel
 from .sensor_model import SensorModel, SensorModelOptions
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/coordinates.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import numpy as np
 import numpy.typing as npt
 import pyproj
 from pyproj.enums import TransformDirection
 
 
 class WorldCoordinate:
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/digital_elevation_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/digital_elevation_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 # TODO: Add typing for ArrayLike once Numpy upgraded to 1.20+
 # from numpy.typing import ArrayLike
 
 import operator
 from abc import ABC, abstractmethod
 from typing import Any, Optional, Tuple
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/elevation_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/elevation_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Optional
 
 from .coordinates import GeodeticWorldCoordinate
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/gdal_sensor_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/gdal_sensor_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from math import degrees, radians
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 import pyproj
 from pyproj.enums import TransformDirection
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/generic_dem_tile_set.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/generic_dem_tile_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from math import degrees, floor
 from typing import Optional
 
 from .coordinates import GeodeticWorldCoordinate
 from .digital_elevation_model import DigitalElevationModelTileSet
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/math_utils.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/math_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from math import sqrt
 from typing import List
 
 
 def equilateral_triangle(centroid: List[float], size: float) -> List[List[float]]:
     """
     Utility function to create an equilateral triangle with a given side length centered on a point. There
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/projective_sensor_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/projective_sensor_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 
 from .coordinates import GeodeticWorldCoordinate, ImageCoordinate
 from .elevation_model import ElevationModel
 from .sensor_model import SensorModel
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/replacement_sensor_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/replacement_sensor_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from abc import ABC
 from enum import Enum
 from math import floor, pi, radians, sqrt
 from typing import Any, Dict, List, Optional, Tuple
 
 import numpy as np
 from scipy.optimize import minimize
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/rpc_sensor_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/rpc_sensor_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from math import degrees, radians, sqrt
 from typing import Any, Dict, List, Optional, Tuple
 
 import numpy as np
 from scipy.optimize import minimize
 
 from . import ConstantElevationModel, ElevationModel, GeodeticWorldCoordinate, ImageCoordinate, WorldCoordinate
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/sensor_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/sensor_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, Dict, Optional
 
 from .coordinates import GeodeticWorldCoordinate, ImageCoordinate
 from .elevation_model import ElevationModel
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/sicd_sensor_model.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/sicd_sensor_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from abc import abstractmethod
 from enum import Enum
 from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/srtm_dem_tile_set.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/srtm_dem_tile_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from math import degrees, floor
 from typing import Optional
 
 from .coordinates import GeodeticWorldCoordinate
 from .digital_elevation_model import DigitalElevationModelTileSet
```

### Comparing `osml-imagery-toolkit-1.3.0/src/aws/osml/photogrammetry/transforms.py` & `osml_imagery_toolkit-1.4.0rc1/src/aws/osml/photogrammetry/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from __future__ import annotations
 
 import numpy as np
 import numpy.typing as npt
 
 
 class ProjectiveTransform:
```

### Comparing `osml-imagery-toolkit-1.3.0/src/osml_imagery_toolkit.egg-info/PKG-INFO` & `osml_imagery_toolkit-1.4.0rc1/src/osml_imagery_toolkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-imagery-toolkit
-Version: 1.3.0
+Version: 1.4.0rc1
 Summary: Toolkit to work with imagery collected by satellites and UAVs
 Author: Amazon Web Services
 Author-email: aws-osml-admin@amazon.com
 License: 
         MIT No Attribution
         
         Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
@@ -26,44 +26,44 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: scikit-optimize>=0.9.0
+Requires-Dist: opencv-python-headless>=4.9.0
 Requires-Dist: cachetools>=5.3.2
 Requires-Dist: geojson>=3.1.0
 Requires-Dist: pyproj>=3.6.1
 Requires-Dist: shapely>=2.0.2
 Requires-Dist: omegaconf==2.3.0; python_version < "3.10.0"
 Requires-Dist: xsdata>=24.1
 Requires-Dist: defusedxml>=0.7.1
 Provides-Extra: gdal
 Requires-Dist: gdal>=3.7.0; extra == "gdal"
 Provides-Extra: test
 Requires-Dist: tox; extra == "test"
 
-# OversightML Imagery Toolkit
-
 The OversightML Imagery Toolkit is a Python package that contains image processing and photogrammetry routines commonly
 used during the analysis of imagery collected by satellites and unmanned aerial vehicles (UAVs). It builds upon GDAL
 by providing additional support for images compliant with the National Imagery Transmission Format (NITF), Sensor
 Independent Complex Data (SICD), and Sensor Independent Derived Data (SIDD) standards.
 
 This library contains four core packages under the `aws.osml` namespace:
 * **photogrammetry**: convert locations between the image (x, y) and geodetic (lon, lat, elev) coordinate systems
 * **gdal**: utilities to work with datasets loaded by GDAL
 * **image_processing**: common image manipulation routines
 * **features**: common geospatial feature manipulation routines
 
 ## Documentation
 
-* **APIs**: You can find API documentation for the OSML Imagery Toolkit hosted on our [GitHub project page](https://aws-solutions-library-samples.github.io/osml-imagery-toolkit/).
-If you are working from the source code running `tox -e docs` will trigger the Sphinx documentation build.
+* **APIs**: You can find the latest API documentation for the OSML Imagery Toolkit hosted [here](https://aws-solutions-library-samples.github.io/osml-imagery-toolkit/).
+  If you are working from the source code running `tox -e docs` will trigger the Sphinx documentation build.
 * **Example Notebooks**: Example notebooks for some operations are in the `examples` directory
+
 ## Installation
 
 This software is available through a Python Package Index.
 If your environment has a distribution, you should be able to install it using pip:
 ```shell
 pip install osml-imagery-toolkit[gdal]
 ```
@@ -74,18 +74,9 @@
 pip install .[gdal]
 ```
 Note that GDAL is listed as an extra dependency for this package. This is done to facilitate environments that either
 don't want to use GDAL or those that have their own custom installation steps for that library. Future versions of
 this package will include image IO backbones that have fewer dependencies.
 
 ## Contributing
-
-This project welcomes contributions and suggestions. If you would like to submit a pull request, see our
-[Contribution Guide](CONTRIBUTING.md) for more information.
-
-## Security
-
-See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
-
-## License
-
-This library is licensed under the MIT-0 License. See the [LICENSE](LICENSE) file.
+We welcome contributions and suggestions. If you would like to submit a pull request please do so using a GitHub pull
+request [here](https://github.com/aws-solutions-library-samples/osml-imagery-toolkit/pulls).
```

### Comparing `osml-imagery-toolkit-1.3.0/src/osml_imagery_toolkit.egg-info/SOURCES.txt` & `osml_imagery_toolkit-1.4.0rc1/src/osml_imagery_toolkit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+PACKAGE_DESCRIPTION.md
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/aws/osml/features/__init__.py
 src/aws/osml/features/feature_index.py
 src/aws/osml/features/geolocation.py
@@ -72,14 +73,17 @@
 src/aws/osml/gdal/sensor_model_factory.py
 src/aws/osml/gdal/sicd_sensor_model_builder.py
 src/aws/osml/gdal/sidd_sensor_model_builder.py
 src/aws/osml/gdal/typing.py
 src/aws/osml/gdal/xmltre_utils.py
 src/aws/osml/image_processing/__init__.py
 src/aws/osml/image_processing/gdal_tile_factory.py
+src/aws/osml/image_processing/map_tileset.py
+src/aws/osml/image_processing/map_tileset_factory.py
+src/aws/osml/image_processing/map_tileset_wmq.py
 src/aws/osml/image_processing/sar_complex_imageop.py
 src/aws/osml/image_processing/sicd_updater.py
 src/aws/osml/image_processing/sidd_updater.py
 src/aws/osml/photogrammetry/__init__.py
 src/aws/osml/photogrammetry/chipped_image_sensor_model.py
 src/aws/osml/photogrammetry/composite_sensor_model.py
 src/aws/osml/photogrammetry/coordinates.py
```

