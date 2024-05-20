# Comparing `tmp/petal_qc-0.0.0.tar.gz` & `tmp/petal_qc-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petal_qc-0.0.0.tar", last modified: Fri May 17 15:11:56 2024, max compression
+gzip compressed data, was "petal_qc-0.0.1.tar", last modified: Mon May 20 22:23:03 2024, max compression
```

## Comparing `petal_qc-0.0.0.tar` & `petal_qc-0.0.1.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-17 15:11:56.021997 petal_qc-0.0.0/
--rw-r--r--   0 lacasta    (501) staff       (20)      943 2024-05-17 15:11:56.021792 petal_qc-0.0.0/PKG-INFO
--rw-r--r--   0 lacasta    (501) staff       (20)      179 2024-05-17 07:56:57.000000 petal_qc-0.0.0/README.md
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-17 15:11:56.015646 petal_qc-0.0.0/petal_qc/
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-17 15:11:56.016611 petal_qc-0.0.0/petal_qc/BTreport/
--rw-r--r--   0 lacasta    (501) staff       (20)     8845 2024-05-17 11:44:19.000000 petal_qc-0.0.0/petal_qc/BTreport/CheckBTtests.py
--rw-r--r--   0 lacasta    (501) staff       (20)        0 2024-05-17 08:12:22.000000 petal_qc-0.0.0/petal_qc/BTreport/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)     4151 2024-05-17 11:39:20.000000 petal_qc-0.0.0/petal_qc/BTreport/bustapeReport.py
--rw-r--r--   0 lacasta    (501) staff       (20)      337 2024-05-17 15:11:38.000000 petal_qc-0.0.0/petal_qc/__init__.py
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-17 15:11:56.018730 petal_qc-0.0.0/petal_qc/metrology/
--rw-r--r--   0 lacasta    (501) staff       (20)     2105 2023-03-06 14:36:41.000000 petal_qc-0.0.0/petal_qc/metrology/Cluster.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1367 2024-05-17 08:33:02.000000 petal_qc-0.0.0/petal_qc/metrology/DataFile.py
--rw-r--r--   0 lacasta    (501) staff       (20)    11886 2024-05-17 15:09:00.000000 petal_qc-0.0.0/petal_qc/metrology/PetalMetrology.py
--rw-r--r--   0 lacasta    (501) staff       (20)        0 2024-05-17 08:12:20.000000 petal_qc-0.0.0/petal_qc/metrology/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1569 2023-09-13 15:37:58.000000 petal_qc-0.0.0/petal_qc/metrology/all2csv.py
--rwxr-xr-x   0 lacasta    (501) staff       (20)    20539 2024-05-17 14:35:44.000000 petal_qc-0.0.0/petal_qc/metrology/analyze_locking_points.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3106 2023-06-27 23:03:41.000000 petal_qc-0.0.0/petal_qc/metrology/cold_noise.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1743 2023-07-17 12:10:41.000000 petal_qc-0.0.0/petal_qc/metrology/comparisonTable.py
--rw-r--r--   0 lacasta    (501) staff       (20)     5449 2024-05-13 18:45:58.000000 petal_qc-0.0.0/petal_qc/metrology/convert_mitutoyo.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3836 2024-05-17 08:33:52.000000 petal_qc-0.0.0/petal_qc/metrology/convert_smartscope.py
--rw-r--r--   0 lacasta    (501) staff       (20)    13256 2024-05-17 10:52:54.000000 petal_qc-0.0.0/petal_qc/metrology/coreMetrology.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1809 2023-08-31 06:45:26.000000 petal_qc-0.0.0/petal_qc/metrology/data2csv.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3977 2024-05-17 08:30:55.000000 petal_qc-0.0.0/petal_qc/metrology/do_Metrology.py
--rw-r--r--   0 lacasta    (501) staff       (20)     4071 2023-09-08 15:22:08.000000 petal_qc-0.0.0/petal_qc/metrology/flatness4nigel.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3372 2024-05-14 08:23:47.000000 petal_qc-0.0.0/petal_qc/metrology/gtkutils.py
--rwxr-xr-x   0 lacasta    (501) staff       (20)    11190 2024-05-17 08:29:23.000000 petal_qc-0.0.0/petal_qc/metrology/petal_flatness.py
--rwxr-xr-x   0 lacasta    (501) staff       (20)     4057 2024-05-17 08:37:41.000000 petal_qc-0.0.0/petal_qc/metrology/show_data_file.py
--rw-r--r--   0 lacasta    (501) staff       (20)      994 2023-07-17 12:15:20.000000 petal_qc-0.0.0/petal_qc/metrology/testSummary.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1981 2023-06-29 09:43:18.000000 petal_qc-0.0.0/petal_qc/metrology/test_paralelism.py
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-17 15:11:56.020533 petal_qc-0.0.0/petal_qc/thermal/
--rw-r--r--   0 lacasta    (501) staff       (20)     2038 2023-03-06 14:36:41.000000 petal_qc-0.0.0/petal_qc/thermal/CSVImage.py
--rw-r--r--   0 lacasta    (501) staff       (20)     2119 2023-03-06 14:36:41.000000 petal_qc-0.0.0/petal_qc/thermal/DebugPlot.py
--rw-r--r--   0 lacasta    (501) staff       (20)    22225 2023-06-08 14:59:18.000000 petal_qc-0.0.0/petal_qc/thermal/IRBFile.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3029 2024-05-17 10:38:18.000000 petal_qc-0.0.0/petal_qc/thermal/IRCore.py
--rw-r--r--   0 lacasta    (501) staff       (20)     9662 2024-05-17 10:40:19.000000 petal_qc-0.0.0/petal_qc/thermal/IRDataGetter.py
--rwxr-xr-x   0 lacasta    (501) staff       (20)    38208 2024-05-17 08:53:09.000000 petal_qc-0.0.0/petal_qc/thermal/IRPetal.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3366 2023-06-10 19:01:24.000000 petal_qc-0.0.0/petal_qc/thermal/IRPetalParam.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3831 2023-03-06 14:36:41.000000 petal_qc-0.0.0/petal_qc/thermal/PetalColorMaps.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3910 2024-05-17 10:42:03.000000 petal_qc-0.0.0/petal_qc/thermal/Petal_IR_Analysis.py
--rw-r--r--   0 lacasta    (501) staff       (20)    17191 2024-05-17 10:43:12.000000 petal_qc-0.0.0/petal_qc/thermal/PipeFit.py
--rw-r--r--   0 lacasta    (501) staff       (20)        0 2023-03-06 14:33:23.000000 petal_qc-0.0.0/petal_qc/thermal/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)    13740 2024-05-17 08:48:05.000000 petal_qc-0.0.0/petal_qc/thermal/analyze_IRCore.py
--rw-r--r--   0 lacasta    (501) staff       (20)     8244 2024-05-17 08:48:22.000000 petal_qc-0.0.0/petal_qc/thermal/contours.py
--rw-r--r--   0 lacasta    (501) staff       (20)     5678 2024-05-17 08:49:46.000000 petal_qc-0.0.0/petal_qc/thermal/create_IRCore.py
--rwxr-xr-x   0 lacasta    (501) staff       (20)     5040 2024-05-17 10:42:44.000000 petal_qc-0.0.0/petal_qc/thermal/pipe_read.py
--rw-r--r--   0 lacasta    (501) staff       (20)    13029 2024-05-17 10:45:10.000000 petal_qc-0.0.0/petal_qc/thermal/show_IR_petal.py
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-17 15:11:56.021302 petal_qc-0.0.0/petal_qc/utils/
--rw-r--r--   0 lacasta    (501) staff       (20)    19765 2023-09-08 15:30:11.000000 petal_qc-0.0.0/petal_qc/utils/Geometry.py
--rw-r--r--   0 lacasta    (501) staff       (20)     4064 2023-03-06 14:36:41.000000 petal_qc-0.0.0/petal_qc/utils/Progress.py
--rw-r--r--   0 lacasta    (501) staff       (20)        0 2023-06-09 13:24:48.000000 petal_qc-0.0.0/petal_qc/utils/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1044 2023-10-20 08:59:51.000000 petal_qc-0.0.0/petal_qc/utils/all_files.py
--rw-r--r--   0 lacasta    (501) staff       (20)     5805 2023-03-06 14:36:41.000000 petal_qc-0.0.0/petal_qc/utils/docx_utils.py
--rw-r--r--   0 lacasta    (501) staff       (20)     5349 2023-03-06 14:36:41.000000 petal_qc-0.0.0/petal_qc/utils/fit_utils.py
--rw-r--r--   0 lacasta    (501) staff       (20)     4035 2024-05-15 09:50:28.000000 petal_qc-0.0.0/petal_qc/utils/utils.py
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-17 15:11:56.021554 petal_qc-0.0.0/petal_qc.egg-info/
--rw-r--r--   0 lacasta    (501) staff       (20)      943 2024-05-17 15:11:56.000000 petal_qc-0.0.0/petal_qc.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (501) staff       (20)     1699 2024-05-17 15:11:56.000000 petal_qc-0.0.0/petal_qc.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (501) staff       (20)        1 2024-05-17 15:11:56.000000 petal_qc-0.0.0/petal_qc.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (501) staff       (20)       92 2024-05-17 15:11:56.000000 petal_qc-0.0.0/petal_qc.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (501) staff       (20)      102 2024-05-17 15:11:56.000000 petal_qc-0.0.0/petal_qc.egg-info/requires.txt
--rw-r--r--   0 lacasta    (501) staff       (20)        9 2024-05-17 15:11:56.000000 petal_qc-0.0.0/petal_qc.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (501) staff       (20)      992 2024-05-17 15:11:38.000000 petal_qc-0.0.0/pyproject.toml
--rw-r--r--   0 lacasta    (501) staff       (20)       38 2024-05-17 15:11:56.022035 petal_qc-0.0.0/setup.cfg
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.807062 petal_qc-0.0.1/
+-rw-r--r--   0 lacasta    (501) staff       (20)      943 2024-05-20 22:23:03.806849 petal_qc-0.0.1/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)      179 2024-05-17 07:56:57.000000 petal_qc-0.0.1/README.md
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.798483 petal_qc-0.0.1/petal_qc/
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.799824 petal_qc-0.0.1/petal_qc/BTreport/
+-rw-r--r--   0 lacasta    (501) staff       (20)     9086 2024-05-19 10:03:41.000000 petal_qc-0.0.1/petal_qc/BTreport/CheckBTtests.py
+-rw-r--r--   0 lacasta    (501) staff       (20)        0 2024-05-17 08:12:22.000000 petal_qc-0.0.1/petal_qc/BTreport/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     6895 2024-05-19 10:14:36.000000 petal_qc-0.0.1/petal_qc/BTreport/bustapeReport.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      337 2024-05-17 15:12:21.000000 petal_qc-0.0.1/petal_qc/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      553 2024-05-17 15:29:20.000000 petal_qc-0.0.1/petal_qc/dashBoard.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.803030 petal_qc-0.0.1/petal_qc/metrology/
+-rw-r--r--   0 lacasta    (501) staff       (20)     2105 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/metrology/Cluster.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1367 2024-05-17 08:33:02.000000 petal_qc-0.0.1/petal_qc/metrology/DataFile.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    11886 2024-05-17 15:09:00.000000 petal_qc-0.0.1/petal_qc/metrology/PetalMetrology.py
+-rw-r--r--   0 lacasta    (501) staff       (20)        0 2024-05-17 08:12:20.000000 petal_qc-0.0.1/petal_qc/metrology/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1569 2023-09-13 15:37:58.000000 petal_qc-0.0.1/petal_qc/metrology/all2csv.py
+-rwxr-xr-x   0 lacasta    (501) staff       (20)    20539 2024-05-17 14:35:44.000000 petal_qc-0.0.1/petal_qc/metrology/analyze_locking_points.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3106 2023-06-27 23:03:41.000000 petal_qc-0.0.1/petal_qc/metrology/cold_noise.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1743 2023-07-17 12:10:41.000000 petal_qc-0.0.1/petal_qc/metrology/comparisonTable.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     5449 2024-05-13 18:45:58.000000 petal_qc-0.0.1/petal_qc/metrology/convert_mitutoyo.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3836 2024-05-17 08:33:52.000000 petal_qc-0.0.1/petal_qc/metrology/convert_smartscope.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    13610 2024-05-19 17:46:54.000000 petal_qc-0.0.1/petal_qc/metrology/coreMetrology.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1809 2023-08-31 06:45:26.000000 petal_qc-0.0.1/petal_qc/metrology/data2csv.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3977 2024-05-17 08:30:55.000000 petal_qc-0.0.1/petal_qc/metrology/do_Metrology.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     4071 2023-09-08 15:22:08.000000 petal_qc-0.0.1/petal_qc/metrology/flatness4nigel.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3372 2024-05-14 08:23:47.000000 petal_qc-0.0.1/petal_qc/metrology/gtkutils.py
+-rwxr-xr-x   0 lacasta    (501) staff       (20)    11190 2024-05-17 08:29:23.000000 petal_qc-0.0.1/petal_qc/metrology/petal_flatness.py
+-rwxr-xr-x   0 lacasta    (501) staff       (20)     4057 2024-05-17 08:37:41.000000 petal_qc-0.0.1/petal_qc/metrology/show_data_file.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      994 2023-07-17 12:15:20.000000 petal_qc-0.0.1/petal_qc/metrology/testSummary.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1981 2023-06-29 09:43:18.000000 petal_qc-0.0.1/petal_qc/metrology/test_paralelism.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.805651 petal_qc-0.0.1/petal_qc/thermal/
+-rw-r--r--   0 lacasta    (501) staff       (20)     2038 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/CSVImage.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     2119 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/DebugPlot.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    22225 2023-06-08 14:59:18.000000 petal_qc-0.0.1/petal_qc/thermal/IRBFile.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3029 2024-05-17 10:38:18.000000 petal_qc-0.0.1/petal_qc/thermal/IRCore.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     9662 2024-05-17 10:40:19.000000 petal_qc-0.0.1/petal_qc/thermal/IRDataGetter.py
+-rwxr-xr-x   0 lacasta    (501) staff       (20)    38208 2024-05-17 08:53:09.000000 petal_qc-0.0.1/petal_qc/thermal/IRPetal.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3516 2024-05-20 07:51:25.000000 petal_qc-0.0.1/petal_qc/thermal/IRPetalParam.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3831 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/PetalColorMaps.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3910 2024-05-17 10:42:03.000000 petal_qc-0.0.1/petal_qc/thermal/Petal_IR_Analysis.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    17191 2024-05-17 10:43:12.000000 petal_qc-0.0.1/petal_qc/thermal/PipeFit.py
+-rw-r--r--   0 lacasta    (501) staff       (20)        0 2023-03-06 14:33:23.000000 petal_qc-0.0.1/petal_qc/thermal/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    14463 2024-05-20 22:20:53.000000 petal_qc-0.0.1/petal_qc/thermal/analyze_IRCore.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     8244 2024-05-17 08:48:22.000000 petal_qc-0.0.1/petal_qc/thermal/contours.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    14428 2024-05-20 22:22:29.000000 petal_qc-0.0.1/petal_qc/thermal/coreThermal.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     5638 2024-05-20 13:04:26.000000 petal_qc-0.0.1/petal_qc/thermal/create_IRCore.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3632 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/pipe_back.npz
+-rw-r--r--   0 lacasta    (501) staff       (20)     3697 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/pipe_front.npz
+-rwxr-xr-x   0 lacasta    (501) staff       (20)     5040 2024-05-17 10:42:44.000000 petal_qc-0.0.1/petal_qc/thermal/pipe_read.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    13029 2024-05-17 10:45:10.000000 petal_qc-0.0.1/petal_qc/thermal/show_IR_petal.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.806440 petal_qc-0.0.1/petal_qc/utils/
+-rw-r--r--   0 lacasta    (501) staff       (20)    19765 2023-09-08 15:30:11.000000 petal_qc-0.0.1/petal_qc/utils/Geometry.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     4064 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/utils/Progress.py
+-rw-r--r--   0 lacasta    (501) staff       (20)        0 2023-06-09 13:24:48.000000 petal_qc-0.0.1/petal_qc/utils/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1044 2023-10-20 08:59:51.000000 petal_qc-0.0.1/petal_qc/utils/all_files.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     5805 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/utils/docx_utils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     5349 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/utils/fit_utils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     4035 2024-05-15 09:50:28.000000 petal_qc-0.0.1/petal_qc/utils/utils.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.806614 petal_qc-0.0.1/petal_qc.egg-info/
+-rw-r--r--   0 lacasta    (501) staff       (20)      943 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)     1816 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)        1 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)       92 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)      102 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)        9 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)      995 2024-05-18 10:08:12.000000 petal_qc-0.0.1/pyproject.toml
+-rw-r--r--   0 lacasta    (501) staff       (20)       38 2024-05-20 22:23:03.807099 petal_qc-0.0.1/setup.cfg
```

### Comparing `petal_qc-0.0.0/PKG-INFO` & `petal_qc-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petal_qc
-Version: 0.0.0
+Version: 0.0.1
 Summary: A collection of scripts for Petal CORE QC.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `petal_qc-0.0.0/petal_qc/BTreport/CheckBTtests.py` & `petal_qc-0.0.1/petal_qc/BTreport/CheckBTtests.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,35 +100,39 @@
         petal (Json): The petal object
 
     Returns
     -------
         dict: a dict with the bustapes. Key is the BT type.
     """
     bt_list = {}
+    bt_valid = {}
     for child in petal["children"]:
         cstage = "Missing"
         if child["component"] is None:
             continue
 
         else:
             child_sn = child["component"]["serialNumber"]
             comp_type = get_type(child)
             if "BT_PETAL" not in comp_type:
                 continue
 
             # We are left with the bus tapes
             cobj = session.get('getComponent', json={'component': child["component"]["id"]})
+            bt_list[comp_type] = cobj, child['id']
             cstage = cobj["currentStage"]['code']
             if cstage != "COMPLETED":
                 complain_func("Bus tape not in final stages", cstage)
-                continue
+                bt_valid[comp_type] = False
+                
+            else:
+                bt_valid[comp_type] = True
 
-            bt_list[comp_type] = cobj, child['id']
 
-    return bt_list
+    return bt_list, bt_valid
 
 
 def find_but_tape_tests(session, petal_date, bt_sn, complain_func=complain):
     """Find tests in bus tape.
 
     Args:
         session (itkdb.Client): The DB session
@@ -205,16 +209,22 @@
 
     # Check children
     if "children" not in petal:
         complain_func("{}[{}]".format(SerialN, id), "Not assembled")
         return None
 
     # Loop on children an find bustapes
-    bt_list = find_bus_tapes(session, petal, complain_func=complain_func)
-    if len(bt_list) == 0:
+    bt_list, bt_valid = find_bus_tapes(session, petal, complain_func=complain_func)
+    
+    nvalid = 0
+    for valid in bt_valid.values():
+        if valid:
+            nvalid += 1
+            
+    if nvalid != 2:
         complain_func("no valid bustape found", "Either not assembled or in incorrect stage.")
         return None
 
     out = {
         "component": SerialN,
         "testType": "BTTESTING",
         "institution": petal["currentLocation"]["code"],
@@ -225,15 +235,15 @@
         "results": {
             "PASS": [],
             "RUNS_ELECTRICALTEST": []
             # "RUNS_STRETCHTEST": []
         }
     }
 
-    # Check te tests in the bustapes
+    # Check the tests in the bustapes
     ngood = 0
     ntrouble = 0
     for bt, cp_id in bt_list.values():
         bt_sn = bt["serialNumber"]
         print("bus tape {}".format(bt_sn))
 
         bt_ngood = 0
```

### Comparing `petal_qc-0.0.0/petal_qc/metrology/Cluster.py` & `petal_qc-0.0.1/petal_qc/metrology/Cluster.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/DataFile.py` & `petal_qc-0.0.1/petal_qc/metrology/DataFile.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/PetalMetrology.py` & `petal_qc-0.0.1/petal_qc/metrology/PetalMetrology.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/all2csv.py` & `petal_qc-0.0.1/petal_qc/metrology/all2csv.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/analyze_locking_points.py` & `petal_qc-0.0.1/petal_qc/metrology/analyze_locking_points.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/cold_noise.py` & `petal_qc-0.0.1/petal_qc/metrology/cold_noise.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/comparisonTable.py` & `petal_qc-0.0.1/petal_qc/metrology/comparisonTable.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/convert_mitutoyo.py` & `petal_qc-0.0.1/petal_qc/metrology/convert_mitutoyo.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/convert_smartscope.py` & `petal_qc-0.0.1/petal_qc/metrology/convert_smartscope.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/coreMetrology.py` & `petal_qc-0.0.1/petal_qc/metrology/coreMetrology.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 """GUI to launch metrology analysis."""
 from pathlib import Path
 from argparse import Action
 from argparse import ArgumentParser
-import itkdb_gtk.ITkDButils
-import itkdb_gtk.dbGtkUtils
-import numpy as np
 from contextlib import redirect_stdout
+import numpy as np
 import itkdb_gtk
+import itkdb_gtk.ITkDButils
+import itkdb_gtk.dbGtkUtils
 import itkdb_gtk.UploadTest
 
 from petal_qc.metrology.do_Metrology import do_analysis
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, GObject, Gio, GLib
@@ -143,14 +143,15 @@
         grid.attach(self.btnFolder, 1, 3, 1, 1)
 
         grid.attach(self.run, 0, 4, 5, 1)
 
 
         self.mainBox.pack_start(self.message_panel.frame, True, True, 0)
 
+
     def quit(self, *args):
         """Quits the application."""
         self.hide()
         self.destroy()
 
 
     def on_file_set(self, *args):
@@ -329,14 +330,28 @@
     def upload_test(self):
         """Uploads test and attachments."""
         if self.outDB is None:
             return
         uploadW = itkdb_gtk.UploadTest.UploadTest(self.session, payload=self.outDB)
 
 
+class CoreMetrologyOptions(object):
+    """Dummy options"""
+    def __init__(self):
+        self.files = []
+        self.SN = None
+        self.desy = False
+        self.folder = None
+        self.prefix = None
+        self.locking_points = None
+        self.title = None
+        self.nbins = 25
+        self.label = "\\w+"
+        self.type = "Punto"
+
 def main():
     """Entry point."""
     parser = ArgumentParser()
     parser.add_argument('files', nargs='*', help="Input files")
     parser.add_argument("--prefix", dest='prefix', default=None)
     parser.add_argument("--SN", dest='SN', default=None)
     parser.add_argument("--save", dest='save', action="store_true", default=False)
```

### Comparing `petal_qc-0.0.0/petal_qc/metrology/data2csv.py` & `petal_qc-0.0.1/petal_qc/metrology/data2csv.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/do_Metrology.py` & `petal_qc-0.0.1/petal_qc/metrology/do_Metrology.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/flatness4nigel.py` & `petal_qc-0.0.1/petal_qc/metrology/flatness4nigel.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/gtkutils.py` & `petal_qc-0.0.1/petal_qc/metrology/gtkutils.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/petal_flatness.py` & `petal_qc-0.0.1/petal_qc/metrology/petal_flatness.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/show_data_file.py` & `petal_qc-0.0.1/petal_qc/metrology/show_data_file.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/testSummary.py` & `petal_qc-0.0.1/petal_qc/metrology/testSummary.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/metrology/test_paralelism.py` & `petal_qc-0.0.1/petal_qc/metrology/test_paralelism.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/CSVImage.py` & `petal_qc-0.0.1/petal_qc/thermal/CSVImage.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/DebugPlot.py` & `petal_qc-0.0.1/petal_qc/thermal/DebugPlot.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/IRBFile.py` & `petal_qc-0.0.1/petal_qc/thermal/IRBFile.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/IRCore.py` & `petal_qc-0.0.1/petal_qc/thermal/IRCore.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/IRDataGetter.py` & `petal_qc-0.0.1/petal_qc/thermal/IRDataGetter.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/IRPetal.py` & `petal_qc-0.0.1/petal_qc/thermal/IRPetal.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/IRPetalParam.py` & `petal_qc-0.0.1/petal_qc/thermal/IRPetalParam.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         Args:
         ----
             values: ArgParser or dict with user values-
 
         """
         self.institute = 'IFIC'   # Either IFIC or DESY to treat the different files
         self.thrs = -20.0         # the threshold
+        self.tco2 = -35.0         # Inlet temperature
         self.gauss_size = 15      # Radius of gausian filtering
         self.grad_sigma = 2.5     # Sigma of grading calculation
         self.distance = 5         # Distance in contour between slices
         self.npoints = 15         # Number of points per segment
         self.min_area = 2500      # minumum area of a valid contour.
         self.contour_cut = 0.2    # Fraction of IR image range to define contour.
         self.contour_smooth = 25  # Value to smooth contour
@@ -54,14 +55,15 @@
         # Get the default value for the parameters.
         P = IRPetalParam()
 
         parser.add_argument("--institute", type=str,
                             default=P.institute,
                             help="Either IFIC or DESY to treat the different files")
         parser.add_argument("--thrs", type=float, default=P.thrs, help="Temperature threshold")
+        parser.add_argument("--tco2", type=float, default=P.tco2, help="CO2 Inlet temperature")
         parser.add_argument("--gauss_size", type=int, default=P.gauss_size, help="Radius of gausian filtering")
         parser.add_argument("--distance", type=float, default=P.distance, help="Distance in contour beteween slices")
         parser.add_argument("--npoints", type=int, default=P.npoints, help="Number of points per segment")
         parser.add_argument("--min_area", type=float, default=P.min_area, help="minumum area of a valid contour")
         parser.add_argument("--width", type=int, default=P.width,
                             help="width of average rectangle en get_T_along_path.")
         parser.add_argument("--contour_cut", type=float, default=P.contour_cut,
```

### Comparing `petal_qc-0.0.0/petal_qc/thermal/PetalColorMaps.py` & `petal_qc-0.0.1/petal_qc/thermal/PetalColorMaps.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/Petal_IR_Analysis.py` & `petal_qc-0.0.1/petal_qc/thermal/Petal_IR_Analysis.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/PipeFit.py` & `petal_qc-0.0.1/petal_qc/thermal/PipeFit.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/analyze_IRCore.py` & `petal_qc-0.0.1/petal_qc/thermal/analyze_IRCore.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,36 +158,46 @@
         G.path_temp = compute_average([R.golden[i].path_temp for R in result_list])
         G.path_spread = compute_average([R.golden[i].path_spread for R in result_list])
         G.sensor_avg = compute_average([R.golden[i].sensor_avg for R in result_list])
         G.sensor_std = compute_average([R.golden[i].sensor_std for R in result_list])
 
     return golden, result_list
 
+def golden_from_json(js_golden):
+    """Converst a JSon golden into a Golden object."""
+    golden = [Petal_IR_Analysis.AnalysisResult() for i in range(2)]
+    for i, G in enumerate(golden):
+        G.path_length = js_golden[i]["path_length"]
+        G.path_temp = js_golden[i]["path_temp"]
+        G.path_spread = js_golden[i]["path_spread"]
+        G.sensor_avg = js_golden[i]["sensor_avg"]
+        G.sensor_std = js_golden[i]["sensor_std"]   
 
 def show_golden_average(golden, results, value):
     """Create golden average.
 
     Args:
     ----
         golden: golden values (from create_golgen_average)
         resuls: results from create_golden_average
         value: value to show, ej path_temp, path_spread, sensor_avg, sensor_std
 
     """
     tick_labels = ["R0", "R1", "R2", "R3", "R3", "R4", "R4", "R5", "R5", "EoS"]
-
+    figures = []
     factor = 1.0
     if value.find("sensor") >= 0:
         factor = 2.0
 
     # Get acceptance band
     band = get_acceptance_band()
 
     for iside in range(2):
         fig, ax = plt.subplots(2, 1, tight_layout=True, gridspec_kw={'height_ratios': (0.66, 0.34)}, figsize=(7, 6))
+        figures.append(fig)
         fig.suptitle("Golden average for {} - side {}.".format(value, iside))
         for a in ax:
             a.grid()
 
         if value.find("path") < 0:
             for i in range(2):
                 ax[i].set_xticks(range(10), labels=tick_labels)
@@ -227,14 +237,15 @@
                                label="Acceptance band")
 
         ax[1].legend(ncol=4, fontsize="x-small")
         ax[1].set_title("T$_{prof}$ - Golden avg.")
         if value.find("temp") >= 0 or value.find("_avg") >= 0:
             ax[1].set_ylim(-Tband, Tband)
 
+    return figures
 
 def compare_golden(core, golden, value):
     """Comapres petal core with golden average.
 
     Args:
     ----
         core (AnalusysResolt): The petal core
@@ -266,20 +277,23 @@
     return rc, mxval, len(outsiders)
 
 
 def analyze_petal_cores(files, golden, options):
     """Create golden average.
 
     Args:
-    ----
         files (list): List of input files
         golden: the golden object
         options: other options.
-
+    
+    Return:
+        array with JSon objects corresponding to the PDB test.
+        
     """
+    output = []
     names = get_names(files)
     for i, ifile in enumerate(files):
         ifile = find_file(options.folder, ifile)
         if not ifile.exists():
             print("+++ File {} does not exist.".format(ifile))
             continue
 
@@ -348,21 +362,25 @@
         if options.out is None:
             ofile = "{}-Thermal.json".format(core.coreID)
         else:
             ofile = options.out
 
         # Check if we are given an output folder
         ofile = output_folder(options.folder, ofile)
-        with open(ofile, 'w') as fp:
+        with open(ofile, 'w', encoding="UTF-8") as fp:
             print("writing {}".format(ofile))
             json.dump(dbOut, fp, indent=3, cls=IRCore.NumpyArrayEncoder)
 
+        output.append(dbOut)
+        
+    return output
 
 def analyze_IRCore(options):
     """Main entry."""
+    output = None
     if options.create_golden:
         golden, results = create_golden_average(options.files, options)
         if options.out is None:
             options.out = "out-golden.json"
 
         ofile = output_folder(options.folder, options.out)
         with open(ofile, 'w') as fp:
@@ -386,17 +404,18 @@
         with open(golden_file, 'r') as fp:
             J = json.load(fp)
 
         golden = [Petal_IR_Analysis.AnalysisResult() for i in range(2)]
         for i, Jside in enumerate(J):
             golden[i].from_json(Jside)
 
-        analyze_petal_cores(options.files, golden, options)
+        output = analyze_petal_cores(options.files, golden, options)
 
     plt.show()
+    return output
 
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
     # Argument parser
     parser = ArgumentParser()
     parser.add_argument('files', nargs='*', help="Input files")
```

### Comparing `petal_qc-0.0.0/petal_qc/thermal/contours.py` & `petal_qc-0.0.1/petal_qc/thermal/contours.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/create_IRCore.py` & `petal_qc-0.0.1/petal_qc/thermal/create_IRCore.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """Entry point."""
     # Obtain the Data getter.
     try:
         getter = IRDataGetter.factory(options.institute, options)
 
     except NotImplemented:
         print("*** Invalid institute name. ***")
-        return
+        return None
 
     # Set parameters from command line
     params = IRPetal.IRPetalParam(options)
     params.debug = False
 
     # Open the sequence file
     print("## ", options.files)
@@ -150,30 +150,31 @@
     core.set_files(options.files)
     core.date = get_db_date(frames[0].timestamp)
     core.institute = params.institute
     core.apply_deltaT(deltaT)
 
     # Check if we are given an output folder
     ofile = output_folder(options.folder, options.out)
-    with open(ofile, "w") as ofile:
+    with open(ofile, "w", encoding="utf-8") as ofile:
         core.to_json(ofile)
 
     if options.debug:
         plt.show()
+        
+    return core
 
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
 
     # Argument parser
     parser = ArgumentParser()
     parser.add_argument('files', nargs='*', help="Input files")
     parser.add_argument("--nframe", type=int, default=-1, help="Number of frames. (negative means all.")
     parser.add_argument('--frame', type=int, default=-1, help="First frame to start.")
-    parser.add_argument("--tco2", default=0, type=float, help="CO2 inlet temperature.")
     parser.add_argument("--out", default="core.json", help="Output file name")
     parser.add_argument("--alias", default="", help="Alias")
     parser.add_argument("--SN", default="", help="serial number")
     parser.add_argument("--folder", default=None, help="Folder to store output files. Superseeds folder in --out")
 
     IRPetalParam.add_parameters(parser)
```

### Comparing `petal_qc-0.0.0/petal_qc/thermal/pipe_read.py` & `petal_qc-0.0.1/petal_qc/thermal/pipe_read.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/thermal/show_IR_petal.py` & `petal_qc-0.0.1/petal_qc/thermal/show_IR_petal.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/utils/Geometry.py` & `petal_qc-0.0.1/petal_qc/utils/Geometry.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/utils/Progress.py` & `petal_qc-0.0.1/petal_qc/utils/Progress.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/utils/all_files.py` & `petal_qc-0.0.1/petal_qc/utils/all_files.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/utils/docx_utils.py` & `petal_qc-0.0.1/petal_qc/utils/docx_utils.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/utils/fit_utils.py` & `petal_qc-0.0.1/petal_qc/utils/fit_utils.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc/utils/utils.py` & `petal_qc-0.0.1/petal_qc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.0/petal_qc.egg-info/PKG-INFO` & `petal_qc-0.0.1/petal_qc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petal_qc
-Version: 0.0.0
+Version: 0.0.1
 Summary: A collection of scripts for Petal CORE QC.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `petal_qc-0.0.0/petal_qc.egg-info/SOURCES.txt` & `petal_qc-0.0.1/petal_qc.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 pyproject.toml
 petal_qc/__init__.py
+petal_qc/dashBoard.py
 petal_qc.egg-info/PKG-INFO
 petal_qc.egg-info/SOURCES.txt
 petal_qc.egg-info/dependency_links.txt
 petal_qc.egg-info/entry_points.txt
 petal_qc.egg-info/requires.txt
 petal_qc.egg-info/top_level.txt
 petal_qc/BTreport/CheckBTtests.py
@@ -38,15 +39,18 @@
 petal_qc/thermal/IRPetalParam.py
 petal_qc/thermal/PetalColorMaps.py
 petal_qc/thermal/Petal_IR_Analysis.py
 petal_qc/thermal/PipeFit.py
 petal_qc/thermal/__init__.py
 petal_qc/thermal/analyze_IRCore.py
 petal_qc/thermal/contours.py
+petal_qc/thermal/coreThermal.py
 petal_qc/thermal/create_IRCore.py
+petal_qc/thermal/pipe_back.npz
+petal_qc/thermal/pipe_front.npz
 petal_qc/thermal/pipe_read.py
 petal_qc/thermal/show_IR_petal.py
 petal_qc/utils/Geometry.py
 petal_qc/utils/Progress.py
 petal_qc/utils/__init__.py
 petal_qc/utils/all_files.py
 petal_qc/utils/docx_utils.py
```

### Comparing `petal_qc-0.0.0/pyproject.toml` & `petal_qc-0.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "petal_qc"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of scripts for Petal CORE QC."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -33,12 +33,12 @@
 coreMetrology = "petal_qc:coreMetrology"
 bustapeReport = "petal_qc:bustapeReport"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
-itkdb_gtk = ["*.desktop", "*.svg"]
+"*" = ["*.desktop", "*.svg", "*.npz"]
 
 [project.urls]
 "Homepage" = "https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils"
 "Bug Tracker" = "https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues"
```

