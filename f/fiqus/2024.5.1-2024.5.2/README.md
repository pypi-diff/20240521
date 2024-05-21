# Comparing `tmp/fiqus-2024.5.1.tar.gz` & `tmp/fiqus-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiqus-2024.5.1.tar", last modified: Tue May 21 12:39:30 2024, max compression
+gzip compressed data, was "fiqus-2024.5.2.tar", last modified: Tue May 21 16:33:58 2024, max compression
```

## Comparing `fiqus-2024.5.1.tar` & `fiqus-2024.5.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.841556 fiqus-2024.5.1/
--rw-rw-rw-   0        0        0     4607 2024-05-21 12:39:30.840556 fiqus-2024.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1719 2024-04-30 14:27:57.000000 fiqus-2024.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.769564 fiqus-2024.5.1/fiqus/
--rw-rw-rw-   0        0        0    13700 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/MainFiQuS.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.782559 fiqus-2024.5.1/fiqus/data/
--rw-rw-rw-   0        0        0     6396 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/data/DataFiQuS.py
--rw-rw-rw-   0        0        0     7287 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/data/DataFiQuSCCT.py
--rw-rw-rw-   0        0        0     2403 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/data/DataFiQuSMultipole.py
--rw-rw-rw-   0        0        0   109844 2024-05-21 12:38:19.000000 fiqus-2024.5.1/fiqus/data/DataFiQuSPancake3D.py
--rw-rw-rw-   0        0        0     2304 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/data/DataMultipole.py
--rw-rw-rw-   0        0        0     9036 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     1709 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/data/DataWindingsCCT.py
--rw-rw-rw-   0        0        0     7162 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/data/RegionsModelFiQuS.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.786558 fiqus-2024.5.1/fiqus/geom_generators/
--rw-rw-rw-   0        0        0    49745 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/geom_generators/GeometryCCT.py
--rw-rw-rw-   0        0        0    24171 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/geom_generators/GeometryMultipole.py
--rw-rw-rw-   0        0        0   167791 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/geom_generators/GeometryPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/geom_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.790558 fiqus-2024.5.1/fiqus/getdp_runners/
--rw-rw-rw-   0        0        0     3012 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/getdp_runners/RunGetdpCCT.py
--rw-rw-rw-   0        0        0     4172 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/getdp_runners/RunGetdpMultipole.py
--rw-rw-rw-   0        0        0     9744 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/getdp_runners/RunGetdpPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/getdp_runners/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.795559 fiqus-2024.5.1/fiqus/mains/
--rw-rw-rw-   0        0        0     4414 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/mains/MainCCT.py
--rw-rw-rw-   0        0        0     5075 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/mains/MainMultipole.py
--rw-rw-rw-   0        0        0    21524 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/mains/MainPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/mains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.801558 fiqus-2024.5.1/fiqus/mesh_generators/
--rw-rw-rw-   0        0        0    11338 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/mesh_generators/MeshCCT.py
--rw-rw-rw-   0        0        0    14221 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/mesh_generators/MeshMultipole.py
--rw-rw-rw-   0        0        0   120547 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/mesh_generators/MeshPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/mesh_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.808557 fiqus-2024.5.1/fiqus/parsers/
--rw-rw-rw-   0        0        0      675 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/parsers/ParserDAT.py
--rw-rw-rw-   0        0        0     8408 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/parsers/ParserGetDPOnSection.py
--rw-rw-rw-   0        0        0     5098 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/parsers/ParserGetDPTimeTable.py
--rw-rw-rw-   0        0        0     1912 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/parsers/ParserMSH.py
--rw-rw-rw-   0        0        0    10121 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/parsers/ParserPOS.py
--rw-rw-rw-   0        0        0     5984 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/parsers/ParserRES.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.811558 fiqus-2024.5.1/fiqus/plotters/
--rw-rw-rw-   0        0        0     6333 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/plotters/PlotPythonCCT.py
--rw-rw-rw-   0        0        0      481 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/plotters/PlotPythonMultipole.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.814557 fiqus-2024.5.1/fiqus/post_processors/
--rw-rw-rw-   0        0        0    28443 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/post_processors/PostProcessCCT.py
--rw-rw-rw-   0        0        0    15649 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/post_processors/PostProcessMultipole.py
--rw-rw-rw-   0        0        0    13195 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/post_processors/PostProcessPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/post_processors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.816558 fiqus-2024.5.1/fiqus/pre_processors/
--rw-rw-rw-   0        0        0     9217 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pre_processors/PreProcessCCT.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pre_processors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.818557 fiqus-2024.5.1/fiqus/pro_assemblers/
--rw-rw-rw-   0        0        0     2770 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_assemblers/ProAssembler.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_assemblers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.819560 fiqus-2024.5.1/fiqus/pro_material_functions/
--rw-rw-rw-   0        0        0    17835 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_material_functions/ironBHcurves.pro
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.820571 fiqus-2024.5.1/fiqus/pro_templates/
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.825558 fiqus-2024.5.1/fiqus/pro_templates/combined/
--rw-rw-rw-   0        0        0    13524 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_templates/combined/CCT_template.pro
--rw-rw-rw-   0        0        0     7956 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_templates/combined/Multipole_template.pro
--rw-rw-rw-   0        0        0   146175 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_templates/combined/Pancake3D_template.pro
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_templates/combined/__init__.py
--rw-rw-rw-   0        0        0     5525 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_templates/combined/materials.pro
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.826557 fiqus-2024.5.1/fiqus/pro_templates/separated/
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/pro_templates/separated/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.828558 fiqus-2024.5.1/fiqus/utils/
--rw-rw-rw-   0        0        0    18489 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/utils/Utils.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/fiqus/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.773558 fiqus-2024.5.1/fiqus.egg-info/
--rw-rw-rw-   0        0        0     4607 2024-05-21 12:39:29.000000 fiqus-2024.5.1/fiqus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2233 2024-05-21 12:39:29.000000 fiqus-2024.5.1/fiqus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 12:39:29.000000 fiqus-2024.5.1/fiqus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1003 2024-05-21 12:39:29.000000 fiqus-2024.5.1/fiqus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 12:39:29.000000 fiqus-2024.5.1/fiqus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 12:39:30.841556 fiqus-2024.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1595 2024-05-21 12:39:07.000000 fiqus-2024.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.833561 fiqus-2024.5.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.1/tests/__init__.py
--rw-rw-rw-   0        0        0    15537 2024-04-30 14:28:07.000000 fiqus-2024.5.1/tests/test_FiQuS.py
--rw-rw-rw-   0        0        0     2034 2024-04-30 14:28:07.000000 fiqus-2024.5.1/tests/test_geometry_generators.py
--rw-rw-rw-   0        0        0     2112 2024-04-30 14:28:07.000000 fiqus-2024.5.1/tests/test_mesh_generators.py
--rw-rw-rw-   0        0        0     4224 2024-04-30 14:28:07.000000 fiqus-2024.5.1/tests/test_solvers.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:30.835558 fiqus-2024.5.1/tests/utils/
--rw-rw-rw-   0        0        0        0 2024-04-30 14:28:07.000000 fiqus-2024.5.1/tests/utils/__init__.py
--rw-rw-rw-   0        0        0    24891 2024-04-30 14:28:07.000000 fiqus-2024.5.1/tests/utils/fiqus_test_classes.py
--rw-rw-rw-   0        0        0     4149 2024-04-30 14:28:07.000000 fiqus-2024.5.1/tests/utils/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.915187 fiqus-2024.5.2/
+-rw-rw-rw-   0        0        0     4607 2024-05-21 16:33:58.914183 fiqus-2024.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1719 2024-05-21 14:29:13.000000 fiqus-2024.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.853558 fiqus-2024.5.2/fiqus/
+-rw-rw-rw-   0        0        0    13700 2024-02-01 14:04:54.000000 fiqus-2024.5.2/fiqus/MainFiQuS.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.863071 fiqus-2024.5.2/fiqus/data/
+-rw-rw-rw-   0        0        0     6396 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0     7287 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/data/DataFiQuSCCT.py
+-rw-rw-rw-   0        0        0     2403 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/data/DataFiQuSMultipole.py
+-rw-rw-rw-   0        0        0   110178 2024-05-21 14:44:57.000000 fiqus-2024.5.2/fiqus/data/DataFiQuSPancake3D.py
+-rw-rw-rw-   0        0        0     2304 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/data/DataMultipole.py
+-rw-rw-rw-   0        0        0     9036 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     1709 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/data/DataWindingsCCT.py
+-rw-rw-rw-   0        0        0     7162 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/data/RegionsModelFiQuS.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.867073 fiqus-2024.5.2/fiqus/geom_generators/
+-rw-rw-rw-   0        0        0    49745 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/geom_generators/GeometryCCT.py
+-rw-rw-rw-   0        0        0    24171 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/geom_generators/GeometryMultipole.py
+-rw-rw-rw-   0        0        0   167791 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/geom_generators/GeometryPancake3D.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/geom_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.870073 fiqus-2024.5.2/fiqus/getdp_runners/
+-rw-rw-rw-   0        0        0     3012 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/getdp_runners/RunGetdpCCT.py
+-rw-rw-rw-   0        0        0     4172 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/getdp_runners/RunGetdpMultipole.py
+-rw-rw-rw-   0        0        0     9744 2024-02-01 14:04:54.000000 fiqus-2024.5.2/fiqus/getdp_runners/RunGetdpPancake3D.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/getdp_runners/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.872585 fiqus-2024.5.2/fiqus/mains/
+-rw-rw-rw-   0        0        0     4414 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/mains/MainCCT.py
+-rw-rw-rw-   0        0        0     5075 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/mains/MainMultipole.py
+-rw-rw-rw-   0        0        0    21524 2024-05-21 14:31:10.000000 fiqus-2024.5.2/fiqus/mains/MainPancake3D.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/mains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.876584 fiqus-2024.5.2/fiqus/mesh_generators/
+-rw-rw-rw-   0        0        0    11338 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/mesh_generators/MeshCCT.py
+-rw-rw-rw-   0        0        0    14221 2023-11-20 18:57:57.000000 fiqus-2024.5.2/fiqus/mesh_generators/MeshMultipole.py
+-rw-rw-rw-   0        0        0   120547 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/mesh_generators/MeshPancake3D.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/mesh_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.885099 fiqus-2024.5.2/fiqus/parsers/
+-rw-rw-rw-   0        0        0      675 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/parsers/ParserDAT.py
+-rw-rw-rw-   0        0        0     8408 2023-11-20 18:57:57.000000 fiqus-2024.5.2/fiqus/parsers/ParserGetDPOnSection.py
+-rw-rw-rw-   0        0        0     5098 2023-11-20 18:57:57.000000 fiqus-2024.5.2/fiqus/parsers/ParserGetDPTimeTable.py
+-rw-rw-rw-   0        0        0     1912 2023-11-20 18:57:57.000000 fiqus-2024.5.2/fiqus/parsers/ParserMSH.py
+-rw-rw-rw-   0        0        0    10121 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/parsers/ParserPOS.py
+-rw-rw-rw-   0        0        0     5984 2023-11-20 18:57:57.000000 fiqus-2024.5.2/fiqus/parsers/ParserRES.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.887098 fiqus-2024.5.2/fiqus/plotters/
+-rw-rw-rw-   0        0        0     6333 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/plotters/PlotPythonCCT.py
+-rw-rw-rw-   0        0        0      481 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/plotters/PlotPythonMultipole.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.890098 fiqus-2024.5.2/fiqus/post_processors/
+-rw-rw-rw-   0        0        0    28443 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/post_processors/PostProcessCCT.py
+-rw-rw-rw-   0        0        0    15649 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/post_processors/PostProcessMultipole.py
+-rw-rw-rw-   0        0        0    13195 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/post_processors/PostProcessPancake3D.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/post_processors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.891601 fiqus-2024.5.2/fiqus/pre_processors/
+-rw-rw-rw-   0        0        0     9217 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/pre_processors/PreProcessCCT.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/pre_processors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.893613 fiqus-2024.5.2/fiqus/pro_assemblers/
+-rw-rw-rw-   0        0        0     2770 2023-11-20 18:57:57.000000 fiqus-2024.5.2/fiqus/pro_assemblers/ProAssembler.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/pro_assemblers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.895614 fiqus-2024.5.2/fiqus/pro_material_functions/
+-rw-rw-rw-   0        0        0    17835 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/pro_material_functions/ironBHcurves.pro
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.896615 fiqus-2024.5.2/fiqus/pro_templates/
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/pro_templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.901119 fiqus-2024.5.2/fiqus/pro_templates/combined/
+-rw-rw-rw-   0        0        0    13524 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/pro_templates/combined/CCT_template.pro
+-rw-rw-rw-   0        0        0     7956 2023-11-20 18:57:57.000000 fiqus-2024.5.2/fiqus/pro_templates/combined/Multipole_template.pro
+-rw-rw-rw-   0        0        0   146568 2024-05-21 14:37:50.000000 fiqus-2024.5.2/fiqus/pro_templates/combined/Pancake3D_template.pro
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/pro_templates/combined/__init__.py
+-rw-rw-rw-   0        0        0     5525 2023-11-20 18:57:57.000000 fiqus-2024.5.2/fiqus/pro_templates/combined/materials.pro
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.901119 fiqus-2024.5.2/fiqus/pro_templates/separated/
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/pro_templates/separated/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.902660 fiqus-2024.5.2/fiqus/utils/
+-rw-rw-rw-   0        0        0    18489 2024-05-21 14:29:13.000000 fiqus-2024.5.2/fiqus/utils/Utils.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:38:58.000000 fiqus-2024.5.2/fiqus/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.909666 fiqus-2024.5.2/fiqus.egg-info/
+-rw-rw-rw-   0        0        0     4607 2024-05-21 16:33:58.000000 fiqus-2024.5.2/fiqus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2233 2024-05-21 16:33:58.000000 fiqus-2024.5.2/fiqus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:33:58.000000 fiqus-2024.5.2/fiqus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1003 2024-05-21 16:33:58.000000 fiqus-2024.5.2/fiqus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 16:33:58.000000 fiqus-2024.5.2/fiqus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:33:58.916185 fiqus-2024.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1595 2024-05-21 16:33:55.000000 fiqus-2024.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.906666 fiqus-2024.5.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-01 14:04:54.000000 fiqus-2024.5.2/tests/__init__.py
+-rw-rw-rw-   0        0        0    15537 2024-02-01 14:04:54.000000 fiqus-2024.5.2/tests/test_FiQuS.py
+-rw-rw-rw-   0        0        0     2034 2024-05-21 14:29:19.000000 fiqus-2024.5.2/tests/test_geometry_generators.py
+-rw-rw-rw-   0        0        0     2112 2024-05-21 14:29:19.000000 fiqus-2024.5.2/tests/test_mesh_generators.py
+-rw-rw-rw-   0        0        0     4224 2024-05-21 14:29:19.000000 fiqus-2024.5.2/tests/test_solvers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:33:58.908667 fiqus-2024.5.2/tests/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-01 14:04:54.000000 fiqus-2024.5.2/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0    24891 2024-05-21 14:29:19.000000 fiqus-2024.5.2/tests/utils/fiqus_test_classes.py
+-rw-rw-rw-   0        0        0     4149 2023-07-16 19:38:58.000000 fiqus-2024.5.2/tests/utils/helpers.py
```

### Comparing `fiqus-2024.5.1/PKG-INFO` & `fiqus-2024.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiqus
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: Source code for STEAM FiQuS tool
 Home-page: https://gitlab.cern.ch/steam/fiqus
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 Keywords: STEAM,FiQuS,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
```

### Comparing `fiqus-2024.5.1/README.md` & `fiqus-2024.5.2/README.md`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/MainFiQuS.py` & `fiqus-2024.5.2/fiqus/MainFiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/data/DataFiQuS.py` & `fiqus-2024.5.2/fiqus/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/data/DataFiQuSCCT.py` & `fiqus-2024.5.2/fiqus/data/DataFiQuSCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/data/DataFiQuSMultipole.py` & `fiqus-2024.5.2/fiqus/data/DataFiQuSMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/data/DataFiQuSPancake3D.py` & `fiqus-2024.5.2/fiqus/data/DataFiQuSPancake3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,18 +149,20 @@
     "thermalConductivity",
     "specificHeatCapacity",
     "debug",
 ]
 quantityProperNames = {
     "axialComponentOfTheMagneticField": "Axila Component of the Magnetic Field",
     "magneticField": "Magnetic Field",
+    "magneticEnergy": "Magnetic Energy",
     "magnitudeOfMagenticField": "Magnitude of Magnetic Field",
     "currentDensity": "Current Density",
     "magnitudeOfCurrentDensity": "Magnitude of Current Density",
     "resistiveHeating": "Resistive Heating",
+    "totalResistiveHeating": "Total Resistive Heating",
     "temperature": "Temperature",
     "currentThroughCoil": "Current Through Coil",
     "voltageBetweenTerminals": "Voltage Between Terminals",
     "criticalCurrentDensity": "Critical Current Density",
     "heatFlux": "Heat Flux",
     "resistivity": "Resistivity",
     "thermalConductivity": "Thermal Conductivity",
@@ -171,18 +173,20 @@
     "inductance": "Inductance",
     "timeConstant": "Time Constant",
 }
 
 quantityUnits = {
     "axialComponentOfTheMagneticField": "T",
     "magneticField": "T",
+    "magneticEnergy": "J",
     "magnitudeOfMagneticField": "T",
     "currentDensity": "$A/m^2$",
     "magnitudeOfCurrentDensity": "$A/m^2$",
     "resistiveHeating": "W",
+    "totalResistiveHeating": "W",
     "temperature": "K",
     "currentThroughCoil": "A",
     "voltageBetweenTerminals": "V",
     "criticalCurrentDensity": "$A/m^2$",
     "heatFlux": "$W/m^2$",
     "resistivity": "Ohm*m",
     "thermalConductivity": "W/m*K",
@@ -198,14 +202,15 @@
     "axialComponentOfTheMagneticField": "RESULT_axialComponentOfTheMagneticField",
     "magneticField": "RESULT_magneticField",
     "magneticEnergy": "RESULT_magneticEnergy",
     "magnitudeOfMagneticField": "RESULT_magnitudeOfMagneticField",
     "currentDensity": "RESULT_currentDensity",
     "magnitudeOfCurrentDensity": "RESULT_magnitudeOfCurrentDensity",
     "resistiveHeating": "RESULT_resistiveHeating",
+    "totalResistiveHeating": "RESULT_totalResistiveHeating",
     "temperature": "RESULT_temperature",
     "currentThroughCoil": "RESULT_currentThroughCoil",
     "voltageBetweenTerminals": "RESULT_voltageBetweenTerminals",
     "criticalCurrentDensity": "RESULT_criticalCurrentDensity",
     "heatFlux": "RESULT_heatFlux",
     "resistivity": "RESULT_resistivity",
     "thermalConductivity": "RESULT_thermalConductivity",
@@ -216,18 +221,20 @@
     "inductance": "RESULT_inductance",
     "timeConstant": "RESULT_timeConstant",
 }
 
 getdpPostOperationNames = {
     "axialComponentOfTheMagneticField": "POSTOP_axialComponentOfTheMagneticField",
     "magneticField": "POSTOP_magneticField",
+    "magneticEnergy": "RESULT_magneticEnergy",
     "magnitudeOfMagneticField": "POSTOP_magnitudeOfMagneticField",
     "currentDensity": "POSTOP_currentDensity",
     "magnitudeOfCurrentDensity": "POSTOP_magnitudeOfCurrentDensity",
     "resistiveHeating": "POSTOP_resistiveHeating",
+    "totalResistiveHeating": "POSTOP_totalResistiveHeating",
     "temperature": "POSTOP_temperature",
     "currentThroughCoil": "POSTOP_currentThroughCoil",
     "voltageBetweenTerminals": "POSTOP_voltageBetweenTerminals",
     "criticalCurrentDensity": "POSTOP_criticalCurrentDensity",
     "heatFlux": "POSTOP_heatFlux",
     "resistivity": "POSTOP_resistivity",
     "thermalConductivity": "POSTOP_thermalConductivity",
```

### Comparing `fiqus-2024.5.1/fiqus/data/DataMultipole.py` & `fiqus-2024.5.2/fiqus/data/DataMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/data/DataRoxieParser.py` & `fiqus-2024.5.2/fiqus/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/data/DataWindingsCCT.py` & `fiqus-2024.5.2/fiqus/data/DataWindingsCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/data/RegionsModelFiQuS.py` & `fiqus-2024.5.2/fiqus/data/RegionsModelFiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/geom_generators/GeometryCCT.py` & `fiqus-2024.5.2/fiqus/geom_generators/GeometryCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/geom_generators/GeometryMultipole.py` & `fiqus-2024.5.2/fiqus/geom_generators/GeometryMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/geom_generators/GeometryPancake3D.py` & `fiqus-2024.5.2/fiqus/geom_generators/GeometryPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/getdp_runners/RunGetdpCCT.py` & `fiqus-2024.5.2/fiqus/getdp_runners/RunGetdpCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/getdp_runners/RunGetdpMultipole.py` & `fiqus-2024.5.2/fiqus/getdp_runners/RunGetdpMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/getdp_runners/RunGetdpPancake3D.py` & `fiqus-2024.5.2/fiqus/getdp_runners/RunGetdpPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/mains/MainCCT.py` & `fiqus-2024.5.2/fiqus/mains/MainCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/mains/MainMultipole.py` & `fiqus-2024.5.2/fiqus/mains/MainMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/mains/MainPancake3D.py` & `fiqus-2024.5.2/fiqus/mains/MainPancake3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             }
             inductance = None
             inductance_solution_folder = os.path.join(
                 self.solution_folder,
                 "inductance",
             )
             inductance_file = os.path.join(
-                inductance_solution_folder, "Inductance-TimeTableFormat.txt"
+                inductance_solution_folder, "Inductance-TimeTableFormat.csv"
             )
             if "inductance" in save_list:
                 # to calculate inductance and time constant, we should run the simulation
                 # with specigic power supply and material settings.
                 copy_fdm = deepcopy(self.fdm)
 
                 new_solve_object_for_inductance_and_time_constant["time"]["start"] = 0
@@ -427,19 +427,19 @@
                     time_constant_solution_folder,
                 )
                 solve.assemble_pro()
 
                 solve.run_getdp(solve=True, postOperation=True)
 
                 # then compute the time constant and write it to a file:
-                # read axialComponentOfTheMagneticFieldForTimeConstant-TimeTableFormat.txt
+                # read axialComponentOfTheMagneticFieldForTimeConstant-TimeTableFormat.csv
 
                 time_constant_file = os.path.join(
                     time_constant_solution_folder,
-                    "axialComponentOfTheMagneticFieldForTimeConstant-TimeTableFormat.txt",
+                    "axialComponentOfTheMagneticFieldForTimeConstant-TimeTableFormat.csv",
                 )
                 times = []
                 Bzs = []
                 isNegative = False
                 with open(time_constant_file, "r") as f:
                     for line in f.readlines():
                         time = float(line.split()[1])
@@ -478,15 +478,15 @@
 
                 time_constant = (
                     x1 + (0.368 - y1) * (x2 - x1) / (y2 - y1) - times[peak_index]
                 )
 
                 # write the time constant to a file:
                 time_constant_file = os.path.join(
-                    time_constant_solution_folder, "time_constant.txt"
+                    time_constant_solution_folder, "time_constant.csv"
                 )
                 with open(time_constant_file, "w") as f:
                     f.write(str(time_constant))
 
         # main solver:
         solve = Solve(
             self.fdm,
```

### Comparing `fiqus-2024.5.1/fiqus/mesh_generators/MeshCCT.py` & `fiqus-2024.5.2/fiqus/mesh_generators/MeshCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/mesh_generators/MeshMultipole.py` & `fiqus-2024.5.2/fiqus/mesh_generators/MeshMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/mesh_generators/MeshPancake3D.py` & `fiqus-2024.5.2/fiqus/mesh_generators/MeshPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/parsers/ParserDAT.py` & `fiqus-2024.5.2/fiqus/parsers/ParserDAT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/parsers/ParserGetDPOnSection.py` & `fiqus-2024.5.2/fiqus/parsers/ParserGetDPOnSection.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/parsers/ParserGetDPTimeTable.py` & `fiqus-2024.5.2/fiqus/parsers/ParserGetDPTimeTable.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/parsers/ParserMSH.py` & `fiqus-2024.5.2/fiqus/parsers/ParserMSH.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/parsers/ParserPOS.py` & `fiqus-2024.5.2/fiqus/parsers/ParserPOS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/parsers/ParserRES.py` & `fiqus-2024.5.2/fiqus/parsers/ParserRES.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/plotters/PlotPythonCCT.py` & `fiqus-2024.5.2/fiqus/plotters/PlotPythonCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/post_processors/PostProcessCCT.py` & `fiqus-2024.5.2/fiqus/post_processors/PostProcessCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/post_processors/PostProcessMultipole.py` & `fiqus-2024.5.2/fiqus/post_processors/PostProcessMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/post_processors/PostProcessPancake3D.py` & `fiqus-2024.5.2/fiqus/post_processors/PostProcessPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/pre_processors/PreProcessCCT.py` & `fiqus-2024.5.2/fiqus/pre_processors/PreProcessCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/pro_assemblers/ProAssembler.py` & `fiqus-2024.5.2/fiqus/pro_assemblers/ProAssembler.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/pro_material_functions/ironBHcurves.pro` & `fiqus-2024.5.2/fiqus/pro_material_functions/ironBHcurves.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/pro_templates/combined/CCT_template.pro` & `fiqus-2024.5.2/fiqus/pro_templates/combined/CCT_template.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/pro_templates/combined/Multipole_template.pro` & `fiqus-2024.5.2/fiqus/pro_templates/combined/Multipole_template.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/pro_templates/combined/Pancake3D_template.pro` & `fiqus-2024.5.2/fiqus/pro_templates/combined/Pancake3D_template.pro`

 * *Files 0% similar despite different names*

```diff
@@ -3386,14 +3386,21 @@
     {% if timeSeriesPlot.quantity in ["currentThroughCoil", "voltageBetweenTerminals"] %}
             <<POSTOPERATION_printResults(
                 quantity=timeSeriesPlot.getdpQuantityName,
                 onRegion="DOM_terminalCut",
                 format="TimeTable",
                 fileName=timeSeriesPlot.fileName
             )|indent(12)>>
+                {% elif timeSeriesPlot.quantity in ["totalResistiveHeating", "magneticEnergy"] %}
+                <<POSTOPERATION_printResults(
+                    quantity=timeSeriesPlot.getdpQuantityName,
+                    onGlobal=True,
+                    format="TimeTable",
+                    fileName=timeSeriesPlot.fileName
+                )|indent(12)>>
                 {% elif timeSeriesPlot.position.x is none %}
             <<POSTOPERATION_printResults(
                 quantity=timeSeriesPlot.getdpQuantityName,
                 onGlobal=True,
                 format="TimeTable",
                 fileName=timeSeriesPlot.fileName
             )|indent(12)>>
@@ -3435,15 +3442,15 @@
             )|indent(12)>>
         }
     }
 {% endif %}
 {% endif %}
     // convergence criteria as postoperations:
 {% for tolerance in (dm.magnet.solve.nls.postOperationTolerances + dm.magnet.solve.t.adaptive.postOperationTolerances)|unique(attribute="quantity") %}
-    {% if tolerance.quantity == "totalResistiveHeating" %}
+    {% if tolerance.quantity in ["totalResistiveHeating", "magneticEnergy"] %}
     {
         Name POSTOP_CONV_totalResistiveHeating;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         LastTimeStepOnly 1;
         Operation {
             Print[RESULT_totalResistiveHeating, OnGlobal];
         }
```

### Comparing `fiqus-2024.5.1/fiqus/pro_templates/combined/materials.pro` & `fiqus-2024.5.2/fiqus/pro_templates/combined/materials.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus/utils/Utils.py` & `fiqus-2024.5.2/fiqus/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus.egg-info/PKG-INFO` & `fiqus-2024.5.2/fiqus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiqus
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: Source code for STEAM FiQuS tool
 Home-page: https://gitlab.cern.ch/steam/fiqus
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 Keywords: STEAM,FiQuS,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
```

### Comparing `fiqus-2024.5.1/fiqus.egg-info/SOURCES.txt` & `fiqus-2024.5.2/fiqus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/fiqus.egg-info/requires.txt` & `fiqus-2024.5.2/fiqus.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/setup.py` & `fiqus-2024.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "setuptools==65.3.0"
 ]
 
 all_requirements = required + docs_require + tests_require + build_require
 
 setup(
     name="fiqus",
-    version="2024.5.1",
+    version="2024.5.2",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for STEAM FiQuS tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/fiqus",
     keywords=["STEAM", "FiQuS", "CERN"],
```

### Comparing `fiqus-2024.5.1/tests/test_FiQuS.py` & `fiqus-2024.5.2/tests/test_FiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/tests/test_geometry_generators.py` & `fiqus-2024.5.2/tests/test_geometry_generators.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/tests/test_mesh_generators.py` & `fiqus-2024.5.2/tests/test_mesh_generators.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/tests/test_solvers.py` & `fiqus-2024.5.2/tests/test_solvers.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/tests/utils/fiqus_test_classes.py` & `fiqus-2024.5.2/tests/utils/fiqus_test_classes.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.5.1/tests/utils/helpers.py` & `fiqus-2024.5.2/tests/utils/helpers.py`

 * *Files identical despite different names*

