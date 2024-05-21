# Comparing `tmp/sage_lib-0.1.5.2.tar.gz` & `tmp/sage_lib-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sage_lib-0.1.5.2.tar", last modified: Fri May 17 08:26:29 2024, max compression
+gzip compressed data, was "sage_lib-0.1.5.3.tar", last modified: Tue May 21 16:03:15 2024, max compression
```

## Comparing `sage_lib-0.1.5.2.tar` & `sage_lib-0.1.5.3.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.179460 sage_lib-0.1.5.2/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-17 08:26:29.179257 sage_lib-0.1.5.2/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.2/README.md
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.157737 sage_lib-0.1.5.2/sage_lib/
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.161800 sage_lib-0.1.5.2/sage_lib/IO/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.2/sage_lib/IO/BashScriptManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.2/sage_lib/IO/BinaryDataHandler.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.2/sage_lib/IO/ChargeFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.2/sage_lib/IO/DOSManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.2/sage_lib/IO/EigenvalueFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.2/sage_lib/IO/ForceFieldManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.2/sage_lib/IO/KPointsManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    17982 2024-05-14 11:48:21.000000 sage_lib-0.1.5.2/sage_lib/IO/OutFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.2/sage_lib/IO/PROFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.2/sage_lib/IO/PotentialManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.2/sage_lib/IO/WaveFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/IO/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.163128 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputClassic.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputFile.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.165962 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPosition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5381 2024-05-16 15:28:23.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24115 2024-05-16 15:36:29.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    47828 2024-04-29 15:23:19.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    31224 2024-05-02 06:40:23.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/plot.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.168505 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
--rw-r--r--   0 dimitry    (501) staff       (20)     9849 2024-05-16 15:55:52.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5328 2024-05-16 15:26:28.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.2/sage_lib/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.169386 sage_lib-0.1.5.2/sage_lib/descriptor/
--rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.2/sage_lib/descriptor/MBTR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.2/sage_lib/descriptor/MDTR_rev.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/descriptor/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.170185 sage_lib-0.1.5.2/sage_lib/ensemble/
--rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.2/sage_lib/ensemble/DFTEnsemble.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.2/sage_lib/ensemble/FFEnsembleManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/ensemble/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    60970 2024-05-16 15:27:57.000000 sage_lib-0.1.5.2/sage_lib/main.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.171139 sage_lib-0.1.5.2/sage_lib/master/
--rw-rw-r--   0 dimitry    (501) staff       (20)    56879 2024-05-16 12:31:55.000000 sage_lib-0.1.5.2/sage_lib/master/AtomicProperties.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12849 2024-05-16 15:37:20.000000 sage_lib-0.1.5.2/sage_lib/master/FileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/master/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.172075 sage_lib-0.1.5.2/sage_lib/miscellaneous/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.2/sage_lib/miscellaneous/BandPathGenerator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.2/sage_lib/miscellaneous/MD_tools.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/miscellaneous/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.2/sage_lib/miscellaneous/periodic_kdtree.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.172951 sage_lib-0.1.5.2/sage_lib/partition/
--rw-rw-r--   0 dimitry    (501) staff       (20)    18091 2024-03-31 12:51:40.000000 sage_lib-0.1.5.2/sage_lib/partition/Partition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    28251 2024-05-16 15:06:54.000000 sage_lib-0.1.5.2/sage_lib/partition/PartitionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/partition/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.177692 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/BandStructure_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Blender_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Config_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/CrystalDefect_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Crystal_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Dataset_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Filter_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13519 2024-03-15 18:00:18.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Molecule_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/PositionEditor_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/SurfaceStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/VacuumStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.178854 sage_lib-0.1.5.2/sage_lib/single_run/
--rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.2/sage_lib/single_run/FF_Gap.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.2/sage_lib/single_run/SingleRun.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.2/sage_lib/single_run/SingleRunDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.2/sage_lib/single_run/SingleRunManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/single_run/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.179033 sage_lib-0.1.5.2/sage_lib.egg-info/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)     3726 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/entry_points.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/requires.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/top_level.txt
--rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-17 08:26:29.179506 sage_lib-0.1.5.2/setup.cfg
--rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-17 07:20:53.000000 sage_lib-0.1.5.2/setup.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.126714 sage_lib-0.1.5.3/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-21 16:03:15.126521 sage_lib-0.1.5.3/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.3/README.md
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.103764 sage_lib-0.1.5.3/sage_lib/
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.108462 sage_lib-0.1.5.3/sage_lib/IO/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.3/sage_lib/IO/BashScriptManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.3/sage_lib/IO/BinaryDataHandler.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.3/sage_lib/IO/ChargeFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.3/sage_lib/IO/DOSManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.3/sage_lib/IO/EigenvalueFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.3/sage_lib/IO/ForceFieldManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.3/sage_lib/IO/KPointsManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    17982 2024-05-14 11:48:21.000000 sage_lib-0.1.5.3/sage_lib/IO/OutFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.3/sage_lib/IO/PROFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.3/sage_lib/IO/PotentialManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.3/sage_lib/IO/WaveFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/IO/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.110196 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputClassic.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputFile.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.112903 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPosition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5789 2024-05-21 15:53:34.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24115 2024-05-21 15:51:02.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    47828 2024-04-29 15:23:19.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    31224 2024-05-02 06:40:23.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/plot.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.115824 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
+-rw-r--r--   0 dimitry    (501) staff       (20)     8851 2024-05-21 15:56:27.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
+-rw-r--r--   0 dimitry    (501) staff       (20)    12680 2024-05-21 15:56:28.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5328 2024-05-16 15:26:28.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.3/sage_lib/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.116618 sage_lib-0.1.5.3/sage_lib/descriptor/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.3/sage_lib/descriptor/MBTR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.3/sage_lib/descriptor/MDTR_rev.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/descriptor/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.117736 sage_lib-0.1.5.3/sage_lib/ensemble/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.3/sage_lib/ensemble/DFTEnsemble.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.3/sage_lib/ensemble/FFEnsembleManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/ensemble/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    60980 2024-05-21 15:52:17.000000 sage_lib-0.1.5.3/sage_lib/main.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.118744 sage_lib-0.1.5.3/sage_lib/master/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    56879 2024-05-16 12:31:55.000000 sage_lib-0.1.5.3/sage_lib/master/AtomicProperties.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12849 2024-05-16 15:37:20.000000 sage_lib-0.1.5.3/sage_lib/master/FileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/master/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.119626 sage_lib-0.1.5.3/sage_lib/miscellaneous/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.3/sage_lib/miscellaneous/BandPathGenerator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.3/sage_lib/miscellaneous/MD_tools.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/miscellaneous/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.3/sage_lib/miscellaneous/periodic_kdtree.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.120429 sage_lib-0.1.5.3/sage_lib/partition/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    18091 2024-03-31 12:51:40.000000 sage_lib-0.1.5.3/sage_lib/partition/Partition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    28251 2024-05-16 15:06:54.000000 sage_lib-0.1.5.3/sage_lib/partition/PartitionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/partition/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.124933 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/BandStructure_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Blender_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Config_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/CrystalDefect_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Crystal_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Dataset_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Filter_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13519 2024-03-15 18:00:18.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Molecule_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/PositionEditor_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/SurfaceStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/VacuumStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.126001 sage_lib-0.1.5.3/sage_lib/single_run/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.3/sage_lib/single_run/FF_Gap.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.3/sage_lib/single_run/SingleRun.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.3/sage_lib/single_run/SingleRunDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.3/sage_lib/single_run/SingleRunManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/single_run/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.126166 sage_lib-0.1.5.3/sage_lib.egg-info/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3797 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/requires.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/top_level.txt
+-rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-21 16:03:15.126761 sage_lib-0.1.5.3/setup.cfg
+-rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-21 16:00:25.000000 sage_lib-0.1.5.3/setup.py
```

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/BashScriptManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/BashScriptManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/BinaryDataHandler.py` & `sage_lib-0.1.5.3/sage_lib/IO/BinaryDataHandler.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/ChargeFileManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/ChargeFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/DOSManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/DOSManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/EigenvalueFileManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/EigenvalueFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/ForceFieldManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/ForceFieldManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/KPointsManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/KPointsManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/OutFileManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/OutFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/PROFileManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/PROFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/PotentialManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/PotentialManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/WaveFileManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/WaveFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputClassic.py` & `sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputClassic.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputDFT.py` & `sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputFile.py` & `sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputFile.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputFileManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPosition.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPosition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,18 +61,25 @@
     sys.stderr.write(f"An error occurred while importing sage_lib.IO.structure_handling_tools.structural_file_readers.GEN: {str(e)}\n")
     del sys
 
 try:
     from sage_lib.IO.structure_handling_tools.structural_file_readers.DUMP import DUMP
 except ImportError as e:
     import sys
-    sys.stderr.write(f"An error occurred while importing sage_lib.IO.structure_handling_tools.structural_file_readers.GEN: {str(e)}\n")
+    sys.stderr.write(f"An error occurred while importing sage_lib.IO.structure_handling_tools.structural_file_readers.DUMP: {str(e)}\n")
+    del sys
+
+try:
+    from sage_lib.IO.structure_handling_tools.structural_file_readers.LAMMPS import LAMMPS
+except ImportError as e:
+    import sys
+    sys.stderr.write(f"An error occurred while importing sage_lib.IO.structure_handling_tools.structural_file_readers.LAMMPS: {str(e)}\n")
     del sys
 
-class AtomPositionLoader(CIF, POSCAR, XYZ, SI, PDB, ASE, AIMS, GEN, DUMP):
+class AtomPositionLoader(CIF, POSCAR, XYZ, SI, PDB, ASE, AIMS, GEN, DUMP, LAMMPS):
     def __init__(self, file_location:str=None, name:str=None, **kwargs):
         CIF.__init__(self, name=name, file_location=file_location)
         POSCAR.__init__(self, name=name, file_location=file_location)
         XYZ.__init__(self, name=name, file_location=file_location)
         SI.__init__(self, name=name, file_location=file_location)
         PDB.__init__(self, name=name, file_location=file_location)
         ASE.__init__(self, name=name, file_location=file_location)
@@ -88,26 +95,28 @@
                             'XYZ': 'export_as_XYZ',
                             'SI': 'export_as_SI',
                             'PDB': 'export_as_PDB',
                             'ASE': 'export_as_ASE',
                             'AIMS': 'export_as_AIMS',
                             'GEN': 'export_as_GEN',
                             'DUMP': 'export_as_DUMP',
+                            'LAMMPS': 'export_as_LAMMPS',
                             }
 
         self.import_dict = {
                             'CIF': 'read_AIMS',
                             'POSCAR': 'read_POSCAR',
                             'XYZ': 'read_XYZ',
                             'SI': 'read_SI',
                             'PDB': 'read_PDB',
                             'ASE': 'read_ASE',
                             'AIMS': 'read_AIMS',
                             'GEN': 'read_GEN',
                             'DUMP': 'read_DUMP',
+                            'LAMMPS': 'read_LAMMPS',
                             }
 
                             
     def read(self, source:str='VASP', file_location:str=None):
         metodo = getattr(self, self.import_dict[source.upper()], None)
         if callable(metodo):
             metodo(file_location)
```

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionManager.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/PeriodicSystem.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/PeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/plot.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,44 +44,14 @@
         Parameters:
             file_location (str, optional): Path to the dump file. Defaults to None.
             name (str, optional): Name of the file. Defaults to None.
         """
         super().__init__(name=name, file_location=file_location)
         AtomicProperties.__init__(self)
 
-    @staticmethod   
-    def latticeVectors_2_triclinic_box(lattice_vectors: np.ndarray) -> list:
-        """
-        Transforms VASP lattice vectors to LAMMPS triclinic box bounds.
-
-        Parameters:
-            lattice_vectors (np.ndarray): 3x3 matrix representing the lattice vectors for VASP.
-        
-        Returns:
-            list: List representing the box bounds in LAMMPS.
-                  It includes (xlo, xhi), (ylo, yhi), (zlo, zhi), xy, xz, yz.
-        """
-        if lattice_vectors.shape != (3, 3):
-            raise ValueError("lattice_vectors must be a 3x3 matrix")
-        
-        # Extracting lattice vectors
-        a1, a2, a3 = lattice_vectors
-        
-        # Calculating box bounds
-        xlo, xhi = 0.0, a1[0]
-        ylo, yhi = 0.0, a2[1]
-        zlo, zhi = 0.0, a3[2]
-        
-        # Calculating tilt factors for triclinic box
-        xy = a2[0]
-        xz = a3[0]
-        yz = a3[1]
-        
-        return [(xlo, xhi), (ylo, yhi), (zlo, zhi), xy, xz, yz]
-
     @staticmethod
     def box_2_latticeVectors(box_bounds: list) -> np.ndarray:
         """
         Transforms LAMMPS box bounds to VASP lattice vectors.
 
         Parameters:
             box_bounds (list of tuple): List of 3 tuples representing the box bounds in LAMMPS.
```

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py` & `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/__init__.py` & `sage_lib-0.1.5.3/sage_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/descriptor/MBTR.py` & `sage_lib-0.1.5.3/sage_lib/descriptor/MBTR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/descriptor/MDTR_rev.py` & `sage_lib-0.1.5.3/sage_lib/descriptor/MDTR_rev.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/ensemble/DFTEnsemble.py` & `sage_lib-0.1.5.3/sage_lib/ensemble/DFTEnsemble.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/ensemble/FFEnsembleManager.py` & `sage_lib-0.1.5.3/sage_lib/ensemble/FFEnsembleManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/main.py` & `sage_lib-0.1.5.3/sage_lib/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,15 +615,15 @@
     PT.handleBLENDER( values={f'{plot}':values}  )
 
 def add_arguments(parser):
     """
     Adds common arguments to the given subparser. This includes arguments for file paths, 
     verbosity, and other common settings used across various sub-commands.
     """
-    structure_list = ['VASP', 'OUTCAR', 'xyz', 'traj', 'cif', 'AIMS', 'gen', 'POSCAR', 'AIMS', 'ASE', 'PDB', 'DUMP']
+    structure_list = ['VASP', 'OUTCAR', 'xyz', 'traj', 'cif', 'AIMS', 'gen', 'POSCAR', 'AIMS', 'ASE', 'PDB', 'DUMP', 'LAMMPS']
     parser.add_argument('--path', type=str, default='.', help='Path to the files directory')
     parser.add_argument('--source', type=str, choices=structure_list, help='Source of calculation from which the files originate: VASP, molecular_dynamics, or force_field (default: VASP)')
     
     parser.add_argument('--forces-tag', type=str, default='forces', help='')
     parser.add_argument('--energy-tag', type=str, default='E', help='')
 
     parser.add_argument('--output_path', type=str, default='.', help='Path for exporting VASP partition and scripts')
```

### Comparing `sage_lib-0.1.5.2/sage_lib/master/AtomicProperties.py` & `sage_lib-0.1.5.3/sage_lib/master/AtomicProperties.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/master/FileManager.py` & `sage_lib-0.1.5.3/sage_lib/master/FileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/miscellaneous/BandPathGenerator.py` & `sage_lib-0.1.5.3/sage_lib/miscellaneous/BandPathGenerator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/miscellaneous/MD_tools.py` & `sage_lib-0.1.5.3/sage_lib/miscellaneous/MD_tools.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/miscellaneous/periodic_kdtree.py` & `sage_lib-0.1.5.3/sage_lib/miscellaneous/periodic_kdtree.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/Partition.py` & `sage_lib-0.1.5.3/sage_lib/partition/Partition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/PartitionManager.py` & `sage_lib-0.1.5.3/sage_lib/partition/PartitionManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/BandStructure_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/BandStructure_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Blender_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Blender_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Config_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Config_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/CrystalDefect_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/CrystalDefect_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Crystal_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Crystal_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Dataset_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Dataset_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Filter_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Filter_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/MolecularDynamic_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/MolecularDynamic_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/MoleculeCluster_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/MoleculeCluster_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Molecule_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Molecule_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/PositionEditor_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/PositionEditor_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/SurfaceStates_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/SurfaceStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/VacuumStates_builder.py` & `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/VacuumStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/single_run/FF_Gap.py` & `sage_lib-0.1.5.3/sage_lib/single_run/FF_Gap.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/single_run/SingleRun.py` & `sage_lib-0.1.5.3/sage_lib/single_run/SingleRun.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/single_run/SingleRunDFT.py` & `sage_lib-0.1.5.3/sage_lib/single_run/SingleRunDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib/single_run/SingleRunManager.py` & `sage_lib-0.1.5.3/sage_lib/single_run/SingleRunManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.2/sage_lib.egg-info/SOURCES.txt` & `sage_lib-0.1.5.3/sage_lib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 sage_lib/IO/structure_handling_tools/__init__.py
 sage_lib/IO/structure_handling_tools/plot.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
+sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
 sage_lib/descriptor/MBTR.py
 sage_lib/descriptor/MDTR_rev.py
```

