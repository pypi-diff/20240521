# Comparing `tmp/napari_pixseq-1.0.2.tar.gz` & `tmp/napari_pixseq-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_pixseq-1.0.2.tar", last modified: Thu May 16 14:33:45 2024, max compression
+gzip compressed data, was "napari_pixseq-1.0.3.tar", last modified: Tue May 21 12:54:06 2024, max compression
```

## Comparing `napari_pixseq-1.0.2.tar` & `napari_pixseq-1.0.3.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 14:33:45.033755 napari_pixseq-1.0.2/
--rw-rw-rw-   0        0        0      120 2024-03-22 12:17:27.000000 napari_pixseq-1.0.2/.gitignore
--rw-rw-rw-   0        0        0     1102 2023-11-24 12:31:51.000000 napari_pixseq-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      101 2023-11-24 12:31:51.000000 napari_pixseq-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5275 2024-05-16 14:33:45.033755 napari_pixseq-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3194 2024-03-04 16:12:02.000000 napari_pixseq-1.0.2/README.md
--rw-rw-rw-   0        0        0     1306 2024-02-29 09:59:26.000000 napari_pixseq-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1983 2024-05-16 14:33:45.033755 napari_pixseq-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.917924 napari_pixseq-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 14:33:45.018133 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/
--rw-rw-rw-   0        0        0     5275 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1823 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.964762 napari_pixseq-1.0.2/src/napari_pixseq/
-drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.964762 napari_pixseq-1.0.2/src/napari_pixseq/GUI/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/GUI/__init__.py
--rw-rw-rw-   0        0        0   136082 2024-05-15 16:44:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.py
--rw-rw-rw-   0        0        0   135729 2024-05-15 16:44:26.000000 napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.ui
--rw-rw-rw-   0        0        0      197 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.964762 napari_pixseq-1.0.2/src/napari_pixseq/_tests/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/_tests/__init__.py
--rw-rw-rw-   0        0        0      667 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/_tests/test_widget.py
--rw-rw-rw-   0        0        0      427 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_pixseq/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.986887 napari_pixseq-1.0.2/src/napari_pixseq/dev/
--rw-rw-rw-   0        0        0        0 2024-05-13 10:26:25.000000 napari_pixseq-1.0.2/src/napari_pixseq/dev/__init__.py
--rw-rw-rw-   0        0        0      438 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/dev/ebfret_IO_dev.py
--rw-rw-rw-   0        0        0     1818 2024-05-15 12:30:42.000000 napari_pixseq-1.0.2/src/napari_pixseq/dev/refactor.py
--rw-rw-rw-   0        0        0     3226 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/dev/spot_mask_dev.py
-drwxrwxrwx   0        0        0        0 2024-05-16 14:33:45.018133 napari_pixseq-1.0.2/src/napari_pixseq/funcs/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/__init__.py
--rw-rw-rw-   0        0        0     9122 2024-05-15 12:25:50.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_align_utils.py
--rw-rw-rw-   0        0        0     7416 2024-05-15 12:25:50.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_cluster_utils.py
--rw-rw-rw-   0        0        0     8349 2024-05-15 12:24:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_colocalize_utils.py
--rw-rw-rw-   0        0        0    32871 2024-05-15 13:33:09.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_events.py
--rw-rw-rw-   0        0        0    20369 2024-05-15 14:00:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_export_images_utils.py
--rw-rw-rw-   0        0        0    35078 2024-05-15 14:01:09.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_export_traces_utils.py
--rw-rw-rw-   0        0        0     6602 2024-05-15 12:24:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_filter_utils.py
--rw-rw-rw-   0        0        0    32955 2024-05-15 16:14:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_import_utils.py
--rw-rw-rw-   0        0        0    35046 2024-05-15 14:44:03.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_loc_utils.py
--rw-rw-rw-   0        0        0    27024 2024-05-16 13:53:20.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_picasso_detect.py
--rw-rw-rw-   0        0        0    37770 2024-05-15 13:59:09.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_plot_utils.py
--rw-rw-rw-   0        0        0     3610 2024-05-15 11:32:04.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_segmentation_events.py
--rw-rw-rw-   0        0        0    18616 2024-05-15 10:59:04.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_segmentation_utils.py
--rw-rw-rw-   0        0        0    13712 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_simple_analysis_utils.py
--rw-rw-rw-   0        0        0    10196 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_temporal_filtering.py
--rw-rw-rw-   0        0        0    49296 2024-05-15 13:53:33.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_trace_compute_utils.py
--rw-rw-rw-   0        0        0     4548 2024-05-16 13:38:35.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_tracking_utils.py
--rw-rw-rw-   0        0        0     9379 2024-05-15 12:24:02.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_transform_utils.py
--rw-rw-rw-   0        0        0    12482 2024-05-15 12:24:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_undrift_utils.py
--rw-rw-rw-   0        0        0    11991 2024-05-15 17:17:10.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_utils_compute.py
--rw-rw-rw-   0        0        0      488 2024-03-04 16:14:23.000000 napari_pixseq-1.0.2/src/napari_pixseq/napari.yaml
--rw-rw-rw-   0        0        0    27799 2024-05-15 14:13:49.000000 napari_pixseq-1.0.2/src/napari_pixseq/pixseq_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-16 14:33:45.018133 napari_pixseq-1.0.2/src/napari_pixseq/scripts/
--rw-rw-rw-   0        0        0      232 2024-03-04 09:54:53.000000 napari_pixseq-1.0.2/src/napari_pixseq/scripts/pypi
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:06.025983 napari_pixseq-1.0.3/
+-rw-rw-rw-   0        0        0      337 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/.gitignore
+-rw-rw-rw-   0        0        0     1102 2023-11-24 12:31:51.000000 napari_pixseq-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-11-24 12:31:51.000000 napari_pixseq-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5275 2024-05-21 12:54:06.025983 napari_pixseq-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3194 2024-03-04 16:12:02.000000 napari_pixseq-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:05.936012 napari_pixseq-1.0.3/pygpufit/
+-rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/pygpufit/Gpufit.dll
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/pygpufit/__init__.py
+-rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/pygpufit/gpufit.py
+-rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/pygpufit/version.py
+-rw-rw-rw-   0        0        0     1306 2024-02-29 09:59:26.000000 napari_pixseq-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1983 2024-05-21 12:54:06.031018 napari_pixseq-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:05.916251 napari_pixseq-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:06.016304 napari_pixseq-1.0.3/src/napari_PixSeq.egg-info/
+-rw-rw-rw-   0        0        0     5275 2024-05-21 12:54:05.000000 napari_pixseq-1.0.3/src/napari_PixSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1903 2024-05-21 12:54:05.000000 napari_pixseq-1.0.3/src/napari_PixSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 12:54:05.000000 napari_pixseq-1.0.3/src/napari_PixSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-21 12:54:05.000000 napari_pixseq-1.0.3/src/napari_PixSeq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-05-21 12:54:05.000000 napari_pixseq-1.0.3/src/napari_PixSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 12:54:05.000000 napari_pixseq-1.0.3/src/napari_PixSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:05.966213 napari_pixseq-1.0.3/src/napari_pixseq/
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:05.966213 napari_pixseq-1.0.3/src/napari_pixseq/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:04:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/GUI/__init__.py
+-rw-rw-rw-   0        0        0   136428 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/GUI/pixseq_ui.py
+-rw-rw-rw-   0        0        0   136078 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/GUI/pixseq_ui.ui
+-rw-rw-rw-   0        0        0      197 2024-05-10 10:04:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:05.976254 napari_pixseq-1.0.3/src/napari_pixseq/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:04:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/_tests/__init__.py
+-rw-rw-rw-   0        0        0      667 2024-05-10 10:04:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/_tests/test_widget.py
+-rw-rw-rw-   0        0        0      427 2024-05-21 12:54:05.000000 napari_pixseq-1.0.3/src/napari_pixseq/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:05.976254 napari_pixseq-1.0.3/src/napari_pixseq/dev/
+-rw-rw-rw-   0        0        0        0 2024-05-13 10:26:25.000000 napari_pixseq-1.0.3/src/napari_pixseq/dev/__init__.py
+-rw-rw-rw-   0        0        0      438 2024-05-10 10:04:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/dev/ebfret_IO_dev.py
+-rw-rw-rw-   0        0        0     1818 2024-05-15 12:30:42.000000 napari_pixseq-1.0.3/src/napari_pixseq/dev/refactor.py
+-rw-rw-rw-   0        0        0     3226 2024-05-10 10:04:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/dev/spot_mask_dev.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:06.016304 napari_pixseq-1.0.3/src/napari_pixseq/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:04:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/__init__.py
+-rw-rw-rw-   0        0        0     9122 2024-05-15 12:25:50.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_align_utils.py
+-rw-rw-rw-   0        0        0     6790 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_cluster_utils.py
+-rw-rw-rw-   0        0        0     5949 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_colocalize_utils.py
+-rw-rw-rw-   0        0        0    32820 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_events.py
+-rw-rw-rw-   0        0        0    20369 2024-05-15 14:00:40.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_export_images_utils.py
+-rw-rw-rw-   0        0        0    35078 2024-05-21 12:46:28.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_export_traces_utils.py
+-rw-rw-rw-   0        0        0     6452 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_filter_utils.py
+-rw-rw-rw-   0        0        0    32955 2024-05-15 16:14:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_import_utils.py
+-rw-rw-rw-   0        0        0    30669 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_loc_utils.py
+-rw-rw-rw-   0        0        0    38584 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_picasso_detect.py
+-rw-rw-rw-   0        0        0    37770 2024-05-15 13:59:09.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_plot_utils.py
+-rw-rw-rw-   0        0        0     3610 2024-05-15 11:32:04.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_segmentation_events.py
+-rw-rw-rw-   0        0        0    18616 2024-05-15 10:59:04.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_segmentation_utils.py
+-rw-rw-rw-   0        0        0    13712 2024-05-10 10:04:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_simple_analysis_utils.py
+-rw-rw-rw-   0        0        0    10196 2024-05-10 10:04:52.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_temporal_filtering.py
+-rw-rw-rw-   0        0        0    49296 2024-05-15 13:53:33.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_trace_compute_utils.py
+-rw-rw-rw-   0        0        0     4191 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_tracking_utils.py
+-rw-rw-rw-   0        0        0     9379 2024-05-15 12:24:02.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_transform_utils.py
+-rw-rw-rw-   0        0        0    12199 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_undrift_utils.py
+-rw-rw-rw-   0        0        0    18425 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_utils_compute.py
+-rw-rw-rw-   0        0        0      488 2024-03-04 16:14:23.000000 napari_pixseq-1.0.3/src/napari_pixseq/napari.yaml
+-rw-rw-rw-   0        0        0    28875 2024-05-21 11:03:35.000000 napari_pixseq-1.0.3/src/napari_pixseq/pixseq_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:54:06.016304 napari_pixseq-1.0.3/src/napari_pixseq/scripts/
+-rw-rw-rw-   0        0        0      232 2024-03-04 09:54:53.000000 napari_pixseq-1.0.3/src/napari_pixseq/scripts/pypi
```

### Comparing `napari_pixseq-1.0.2/LICENSE` & `napari_pixseq-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/PKG-INFO` & `napari_pixseq-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-PixSeq
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Napari plugin for extracting time series traces from Single Molecule Localisation Microsocpy (SMLM) data.
 Home-page: https://github.com/piedrro/napari-PixSeq
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-PixSeq/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-PixSeq#README.md
```

### Comparing `napari_pixseq-1.0.2/README.md` & `napari_pixseq-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/pyproject.toml` & `napari_pixseq-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/setup.cfg` & `napari_pixseq-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/PKG-INFO` & `napari_pixseq-1.0.3/src/napari_PixSeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-PixSeq
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Napari plugin for extracting time series traces from Single Molecule Localisation Microsocpy (SMLM) data.
 Home-page: https://github.com/piedrro/napari-PixSeq
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-PixSeq/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-PixSeq#README.md
```

### Comparing `napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/SOURCES.txt` & `napari_pixseq-1.0.3/src/napari_PixSeq.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+pygpufit/Gpufit.dll
+pygpufit/__init__.py
+pygpufit/gpufit.py
+pygpufit/version.py
 src/napari_PixSeq.egg-info/PKG-INFO
 src/napari_PixSeq.egg-info/SOURCES.txt
 src/napari_PixSeq.egg-info/dependency_links.txt
 src/napari_PixSeq.egg-info/entry_points.txt
 src/napari_PixSeq.egg-info/requires.txt
 src/napari_PixSeq.egg-info/top_level.txt
 src/napari_pixseq/__init__.py
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.py` & `napari_pixseq-1.0.3/src/napari_pixseq/GUI/pixseq_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -761,14 +761,18 @@
         self.verticalLayout_23.addWidget(self.picasso_window_cropping)
         self.picasso_segmentation_filtering = QtWidgets.QCheckBox(self.tab_21)
         self.picasso_segmentation_filtering.setObjectName("picasso_segmentation_filtering")
         self.verticalLayout_23.addWidget(self.picasso_segmentation_filtering)
         self.picasso_minimise_ram = QtWidgets.QCheckBox(self.tab_21)
         self.picasso_minimise_ram.setObjectName("picasso_minimise_ram")
         self.verticalLayout_23.addWidget(self.picasso_minimise_ram)
+        self.picasso_use_gpufit = QtWidgets.QCheckBox(self.tab_21)
+        self.picasso_use_gpufit.setEnabled(False)
+        self.picasso_use_gpufit.setObjectName("picasso_use_gpufit")
+        self.verticalLayout_23.addWidget(self.picasso_use_gpufit)
         self.gridLayout_6 = QtWidgets.QGridLayout()
         self.gridLayout_6.setObjectName("gridLayout_6")
         self.picasso_fit = QtWidgets.QPushButton(self.tab_21)
         self.picasso_fit.setObjectName("picasso_fit")
         self.gridLayout_6.addWidget(self.picasso_fit, 0, 1, 1, 1)
         self.picasso_detect = QtWidgets.QPushButton(self.tab_21)
         self.picasso_detect.setObjectName("picasso_detect")
@@ -1852,14 +1856,15 @@
         self.picasso_box_size.setItemText(6, _translate("Frame", "15"))
         self.label_35.setText(_translate("Frame", "ROI Border Width (Pixels)"))
         self.picasso_roi_border_width.setText(_translate("Frame", "5"))
         self.picasso_remove_overlapping.setText(_translate("Frame", "Remove Overlapping Localisations/Bounding Boxes (determined by Picaso Box Size)"))
         self.picasso_window_cropping.setText(_translate("Frame", "Remove Localisations Outside Field Of View (FOV)"))
         self.picasso_segmentation_filtering.setText(_translate("Frame", "Remove Localisations Outside Segmentations"))
         self.picasso_minimise_ram.setText(_translate("Frame", "Minimise RAM usage"))
+        self.picasso_use_gpufit.setText(_translate("Frame", "Use Gpufit (if available)"))
         self.picasso_fit.setText(_translate("Frame", "Fit"))
         self.picasso_detect.setText(_translate("Frame", "Detect"))
         self.picasso_detectfit.setText(_translate("Frame", "Detect and Fit"))
         self.tabWidget_6.setTabText(self.tabWidget_6.indexOf(self.tab_21), _translate("Frame", "Detect"))
         self.label_92.setText(_translate("Frame", "Filter Localisations (Picasso)"))
         self.picasso_filter_dataset_label.setText(_translate("Frame", "Dataset"))
         self.label_89.setText(_translate("Frame", "Channel"))
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.ui` & `napari_pixseq-1.0.3/src/napari_pixseq/GUI/pixseq_ui.ui`

 * *Files 0% similar despite different names*

#### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.ui` & `napari_pixseq-1.0.3/src/napari_pixseq/GUI/pixseq_ui.ui`

```diff
@@ -1835,14 +1835,24 @@
                         <widget class="QCheckBox" name="picasso_minimise_ram">
                           <property name="text">
                             <string>Minimise RAM usage</string>
                           </property>
                         </widget>
                       </item>
                       <item>
+                        <widget class="QCheckBox" name="picasso_use_gpufit">
+                          <property name="enabled">
+                            <bool>false</bool>
+                          </property>
+                          <property name="text">
+                            <string>Use Gpufit (if available)</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
                         <layout class="QGridLayout" name="gridLayout_6">
                           <item row="0" column="1">
                             <widget class="QPushButton" name="picasso_fit">
                               <property name="text">
                                 <string>Fit</string>
                               </property>
                             </widget>
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/_tests/test_widget.py` & `napari_pixseq-1.0.3/src/napari_pixseq/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/dev/refactor.py` & `napari_pixseq-1.0.3/src/napari_pixseq/dev/refactor.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/dev/spot_mask_dev.py` & `napari_pixseq-1.0.3/src/napari_pixseq/dev/spot_mask_dev.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_align_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_align_utils.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_cluster_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_cluster_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,73 +94,61 @@
                 cluster_centers = self.remove_overlapping_coords(cluster_centers,
                     min_distance = box_size)
 
             if "localisations" not in mode.lower():
                 n_frames = 1
 
             clustered_locs = []
-            clustered_loc_centers = []
-            render_locs = {}
 
             for cluster_index in range(len(cluster_centers)):
                 for frame_index in range(n_frames):
                     [locX, locY] = cluster_centers[cluster_index].copy()
                     new_loc = (int(frame_index), float(locX), float(locY))
                     clustered_locs.append(new_loc)
 
-                    if frame_index not in render_locs.keys():
-                        render_locs[frame_index] = []
-
-                    render_locs[frame_index].append([locY, locX])
-                    clustered_loc_centers.append([frame_index, locY, locX])
-
             # Convert list to recarray
-            clustered_locs = np.array(clustered_locs, dtype=[('frame', '<u4'), ('x', '<f4'), ('y', '<f4')]).view(np.recarray)
+            clustered_locs = np.array(clustered_locs,
+                dtype=[('frame', '<u4'), ('x', '<f4'), ('y', '<f4')]).view(np.recarray)
 
-            result = (clustered_locs, clustered_loc_centers, render_locs)
+            result = clustered_locs
 
         except:
             print(traceback.format_exc())
             result = None
 
         return result
 
 
-    def _cluster_localisations_result(self, result):
+    def _cluster_localisations_result(self, locs):
 
         try:
 
-            if result is not None:
-
-                locs, loc_centers, render_locs = result
+            if locs is not None:
 
                 mode = self.gui.cluster_mode.currentText()
                 dataset = self.gui.cluster_dataset.currentText()
                 channel = self.gui.cluster_channel.currentText()
 
                 fiducial_dict = self.localisation_dict["localisations"][dataset][channel.lower()]
                 bbox_dict = self.localisation_dict["bounding_boxes"]
 
                 if "localisations" in mode.lower():
 
                     fiducial_dict = self.localisation_dict["localisations"][dataset][channel.lower()]
 
                     fiducial_dict["localisations"] = locs
-                    fiducial_dict["localisation_centres"] = loc_centers
-                    fiducial_dict["render_locs"] = render_locs
 
                 else:
 
                     if "box_size" in fiducial_dict.keys():
                         box_size = fiducial_dict["box_size"]
                     else:
                         box_size = int(self.gui.picasso_box_size.currentText())
 
                     bbox_dict["localisations"] = locs
-                    bbox_dict["localisation_centres"] = loc_centers
                     bbox_dict["box_size"] = box_size
 
         except:
             print(traceback.format_exc())
             pass
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_events.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,16 +457,14 @@
                 fret_modes = [self.dataset_dict[datast_name][channel]["FRET"] for channel in self.dataset_dict[datast_name].keys()]
                 channel_refs = [self.dataset_dict[datast_name][channel]["channel_ref"] for channel in self.dataset_dict[datast_name].keys()]
 
                 channel_refs = list(set(channel_refs))
                 fret_mode = list(set(fret_modes))[0]
                 import_mode = list(set(import_modes))[0]
 
-                print(datast_name, import_mode)
-
                 self.gui.pixseq_show_dd.clicked.connect(lambda: None)
                 self.gui.pixseq_show_da.clicked.connect(lambda: None)
                 self.gui.pixseq_show_aa.clicked.connect(lambda: None)
                 self.gui.pixseq_show_ad.clicked.connect(lambda: None)
 
                 if import_mode.lower() == "fret":
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_export_images_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_export_images_utils.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_export_traces_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_export_traces_utils.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_filter_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_filter_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,22 +39,15 @@
 
                         n_filtered = len(locs)
 
                         if n_filtered < n_locs:
 
                             n_removed = n_locs - n_filtered
 
-                            render_locs = {}
-
-                            for frame in np.unique(locs["frame"]):
-                                frame_locs = locs[locs["frame"] == frame].copy()
-                                render_locs[frame] = np.vstack((frame_locs.y, frame_locs.x)).T.tolist()
-
                             loc_dict["localisations"] = locs
-                            loc_dict["render_locs"] = render_locs
 
                             if localisation_type == "Localisations":
                                 self.localisation_dict["localisations"][dataset][channel.lower()] = loc_dict
                                 self.draw_localisations(update_vis=True)
                             else:
                                 self.localisation_dict["bounding_boxes"] = loc_dict
                                 self.draw_bounding_boxes(update_vis=True)
@@ -104,14 +97,16 @@
 
                 if n_locs > 0:
 
                     locs = loc_dict["localisations"].copy()
 
                     columns = list(locs.dtype.names)
 
+                    columns = [col for col in columns if col not in ["dataset","channel"]]
+
 
             selector.clear()
 
             if len(columns) > 0:
                 selector.addItems(columns)
 
         except:
@@ -140,28 +135,30 @@
 
                 columns = list(locs.dtype.names)
 
                 if criterion in columns:
 
                     values = locs[criterion]
 
-                    if plot:
-                        self.plot_filter_graph(criterion, values)
+                    if values.dtype in [np.float32, np.float64, np.int32, np.int64]:
+
+                        if plot:
+                            self.plot_filter_graph(criterion, values)
 
-                    min_value = np.min(values)
-                    max_value = np.max(values)
+                        min_value = np.min(values)
+                        max_value = np.max(values)
 
-                    self.gui.filter_min.setMinimum(min_value)
-                    self.gui.filter_min.setMaximum(max_value)
+                        self.gui.filter_min.setMinimum(min_value)
+                        self.gui.filter_min.setMaximum(max_value)
 
-                    self.gui.filter_max.setMinimum(min_value)
-                    self.gui.filter_max.setMaximum(max_value)
+                        self.gui.filter_max.setMinimum(min_value)
+                        self.gui.filter_max.setMaximum(max_value)
 
-                    self.gui.filter_min.setValue(min_value)
-                    self.gui.filter_max.setValue(max_value)
+                        self.gui.filter_min.setValue(min_value)
+                        self.gui.filter_max.setValue(max_value)
 
         except:
             print(traceback.format_exc())
 
     def plot_filter_graph(self, criterion = "", values = None):
 
         try:
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_import_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_loc_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_loc_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,37 +46,26 @@
         self.columns = self.locs.dtype.names
 
         if self.locs.dtype == self.fitted_dtype:
             self.loc_type = "fiducial"
         else:
             self.loc_type = "bbox"
 
-    def coerce_new_loc_format(self, new_loc):
-
-        if len(new_loc) != len(self.dtype):
-            difference = len(self.dtype) - len(new_loc)
-            if difference > 0:
-                new_loc = list(new_loc)
-                for i in range(difference):
-                    new_loc = new_loc + [0]
-                new_loc = tuple(new_loc)
-
-        return new_loc
 
     def remove_duplicate_locs(self, locs = None):
 
             try:
 
                 if locs is not None:
-                    self.locs = locs
-                    self.get_loc_info()
 
-                unique_records, indices = np.unique(self.locs, return_index=True)
+                    if len(locs) > 0:
 
-                self.locs = self.locs[indices]
+                        locs = pd.DataFrame(locs, columns=locs.dtype.names)
+                        locs = locs.drop_duplicates(subset=["frame", "x", "y"], keep="first")
+                        locs = locs.to_records(index=False)
 
             except:
                 print(traceback.format_exc())
                 pass
 
             return locs
 
@@ -90,19 +79,24 @@
                 self.get_loc_info()
 
             if type(new_loc) == list:
                 new_loc = tuple(new_loc)
             if type(new_loc) in [np.ndarray, np.recarray]:
                 new_loc = tuple(new_loc.tolist())
 
-            new_loc = self.coerce_new_loc_format(new_loc)
+            loc_cols = self.locs.dtype.names
+            new_loc_keys = list(new_loc.keys())
 
-            self.locs = np.array(self.locs).tolist()
-            self.locs.append(new_loc)
-            self.locs = np.rec.fromrecords(self.locs, dtype=self.dtype)
+            for key in new_loc_keys:
+                if key not in loc_cols:
+                    new_loc.pop(key)
+
+            locs = pd.DataFrame(self.locs, columns=self.locs.dtype.names)
+            locs.loc[len(locs)] = new_loc
+            self.locs = locs.to_records(index=False)
 
             self.remove_duplicate_locs()
 
         except:
             print(traceback.format_exc())
             pass
 
@@ -116,18 +110,17 @@
                 self.locs = locs
                 self.get_loc_info()
 
             if loc_index is not None:
 
                 if loc_index < len(self.locs):
 
-                    self.locs = self.locs.view(np.float32).reshape(len(self.locs), -1)
-                    self.locs = np.delete(self.locs, loc_index, axis=0)
-                    self.locs = self.locs.view(self.dtype)
-                    self.locs = np.squeeze(self.locs, axis=1)
+                    locs = pd.DataFrame(self.locs, columns=self.locs.dtype.names)
+                    locs = locs.drop(loc_index)
+                    self.locs = locs.to_records(index=False)
 
                 self.remove_duplicate_locs()
 
         except:
             print(traceback.format_exc())
             pass
 
@@ -327,44 +320,28 @@
 
                 if "Box Size" in info[1].keys():
                     box_size = info[1]["Box Size"]
 
             if type == "Localisations":
 
                 if self.verbose:
-                    print("Creating render locs")
-
-                render_locs = {}
-                for frame in np.unique(locs.frame):
-                    frame_locs = locs[locs.frame == frame].copy()
-                    render_locs[frame] = np.vstack((frame_locs.y, frame_locs.x)).T.tolist()
-
-                loc_centres = self.get_localisation_centres(locs)
-
-                if self.verbose:
                     print("Updating localisation dict")
 
                 self.localisation_dict["localisations"][dataset][channel.lower()]["localisations"] = locs.copy()
-                self.localisation_dict["localisations"][dataset][channel.lower()]["localisation_centres"] = loc_centres.copy()
-                self.localisation_dict["localisations"][dataset][channel.lower()]["render_locs"] = render_locs
                 self.localisation_dict["localisations"][dataset][channel.lower()]["fitted"] = True
                 self.localisation_dict["localisations"][dataset][channel.lower()]["box_size"] = box_size
 
             else:
                 unique_frames = np.unique(locs.frame)
                 locs = locs[locs.frame == unique_frames[0]]
 
-                loc_centres = self.get_localisation_centres(locs)
-
                 if self.verbose:
                     print("Updating localisation dict")
 
                 self.localisation_dict["bounding_boxes"]["localisations"] = locs.copy()
-                self.localisation_dict["bounding_boxes"]["localisation_centres"] = loc_centres.copy()
-                self.localisation_dict["bounding_boxes"]["render_locs"] = {}
                 self.localisation_dict["bounding_boxes"]["fitted"] = True
                 self.localisation_dict["bounding_boxes"]["box_size"] = box_size
 
         except:
             print(traceback.format_exc())
             pass
 
@@ -722,25 +699,25 @@
 
                 loc_dict, n_locs, _ = self.get_loc_dict(active_dataset, active_channel,
                     type = "localisations")
 
 
                 if n_locs > 0:
                     locs = loc_dict["localisations"].copy()
-                    render_locs = loc_dict["render_locs"].copy()
-                    loc_centers = loc_dict["localisation_centres"].copy()
                     box_size = int(loc_dict["box_size"])
-                    dtype = locs.dtype
 
                     loc_utils = picasso_loc_utils(locs)
 
                     x,y = position
 
                     frame_locs = locs[locs.frame == frame]
 
+                    new_loc = {"dataset": active_dataset, "channel": active_channel,
+                               "frame": frame, "x": x, "y": y, "net_gradient": net_gradient, }
+
                     if len(frame_locs) > 0:
 
                         loc_coords = np.vstack((frame_locs.y, frame_locs.x)).T
 
                         # Calculate Euclidean distances
                         distances = np.sqrt(np.sum((loc_coords - np.array([y,x])) ** 2, axis=1))
 
@@ -748,103 +725,63 @@
                         min_index = np.argmin(distances)
                         min_distance = distances[min_index]
 
                         if min_distance < box_size:
 
                             locs = loc_utils.remove_loc(loc_index=min_index)
 
-                            loc_centers = np.delete(loc_centers, min_index, axis=0)
-                            loc_centers = loc_centers.tolist()
-
-                            render_frame_locs = render_locs[frame].copy()
-                            render_frame_locs = np.unique(render_frame_locs, axis=0).tolist()
-                            distances = np.sqrt(np.sum((np.array(render_frame_locs) - np.array([y,x])) ** 2, axis=1))
-                            min_index = np.argmin(distances)
-                            render_frame_locs.pop(min_index)
-                            render_locs[frame] = render_frame_locs
-
                             loc_dict["localisations"] = locs
-                            loc_dict["localisation_centres"] = loc_centers
-                            loc_dict["render_locs"] = render_locs
 
                             self.update_loc_dict(active_dataset, active_channel, "localisations", loc_dict)
                             self.draw_localisations(update_vis=True)
 
                         else:
 
-                            locs = loc_utils.add_loc(new_loc = [frame, x, y, net_gradient])
-
-                            loc_centers = np.append(loc_centers, np.array([[frame,y,x]], dtype=int), axis=0)
-                            loc_centers = loc_centers.tolist()
-
-                            if len(render_locs[frame]) == 0:
-                                render_locs[frame] = [[round(y),round(x)]]
-                            else:
-                                render_locs[frame].append([round(y),round(x)])
+                            locs = loc_utils.add_loc(new_loc = new_loc)
 
                             loc_dict["localisations"] = locs
-                            loc_dict["localisation_centres"] = loc_centers
-                            loc_dict["render_locs"] = render_locs
 
                             self.update_loc_dict(active_dataset, active_channel, "localisations", loc_dict)
                             self.draw_localisations(update_vis=True)
 
                     else:
 
-                        locs = loc_utils.add_loc(new_loc=[frame, x, y, net_gradient])
-
-                        loc_centers = np.append(loc_centers, np.array([[frame, y, x]], dtype=int), axis=0)
-                        loc_centers = loc_centers.tolist()
-
-                        if frame in render_locs.keys():
-                            if len(render_locs[frame]) == 0:
-                                render_locs[frame] = [[round(y), round(x)]]
-                            else:
-                                render_locs[frame].append([round(y), round(x)])
-                        else:
-                            render_locs[frame] = [[round(y), round(x)]]
+                        locs = loc_utils.add_loc(new_loc=new_loc)
 
                         loc_dict["localisations"] = locs
-                        loc_dict["localisation_centres"] = loc_centers
-                        loc_dict["render_locs"] = render_locs
 
                         self.update_loc_dict(active_dataset, active_channel, "localisations", loc_dict)
                         self.draw_localisations(update_vis=True)
 
                 else:
                     x, y = position
 
                     box_size = int(self.gui.picasso_box_size.currentText())
 
                     new_loc = [frame, position[0], position[1], net_gradient]
 
                     loc_utils = picasso_loc_utils()
                     locs = loc_utils.create_locs(new_loc=new_loc)
 
-                    loc_centers = [[frame, y, x]]
-                    render_locs = {frame: [[y, x]]}
-
                     loc_dict["localisations"] = locs
-                    loc_dict["localisation_centres"] = loc_centers
-                    loc_dict["render_locs"] = render_locs
                     loc_dict["fitted"] = False
                     loc_dict["box_size"] = box_size
 
                     self.update_loc_dict(active_dataset, active_channel, "localisations", loc_dict)
                     self.draw_localisations(update_vis=True)
 
             elif mode == "bounding_box":
 
                 loc_dict, n_locs,_ = self.get_loc_dict(active_dataset, active_channel,
                     type = "bounding_box")
 
                 if n_locs > 0:
 
                     locs = loc_dict["localisations"].copy()
-                    loc_centers = loc_dict["localisation_centres"].copy()
+                    loc_centers = self.get_localisation_centres(locs)
                     box_size = int(loc_dict["box_size"])
                     dtype = locs.dtype
 
                     loc_utils = picasso_loc_utils(locs)
 
                     x, y = position
 
@@ -864,37 +801,23 @@
 
                     # print(f"min_distance: {min_distance}")
 
                     if min_distance < box_size:
 
                         locs = loc_utils.remove_loc(loc_index=min_index)
 
-                        loc_centers = np.delete(loc_centers, min_index, axis=0)
-                        loc_centers = loc_centers.tolist()
-
-                        # print(f"len locs: {len(locs)}, len loc_centers: {len(loc_centers)}")
-
                         loc_dict["localisations"] = locs
-                        loc_dict["localisation_centres"] = loc_centers
                         self.update_loc_dict(active_dataset, active_channel, "bounding_boxes", loc_dict)
                         self.draw_bounding_boxes()
 
                     else:
 
-                        locs = loc_utils.add_loc(new_loc = [frame, x, y, net_gradient])
-
-                        if loc_centers.shape[-1] == 3:
-                            loc_centers = np.append(loc_centers, np.array([[frame, y,x]], dtype=int), axis=0)
-                        if loc_centers.shape[-1] == 2:
-                            loc_centers = np.append(loc_centers, np.array([[y,x]], dtype=int), axis=0)
-
-                        loc_centers = loc_centers.tolist()
+                        locs = loc_utils.add_loc(new_loc = {"frame": frame, "x": x, "y": y, "net_gradient": net_gradient})
 
                         loc_dict["localisations"] = locs
-                        loc_dict["localisation_centres"] = loc_centers
 
                         self.update_loc_dict(active_dataset, active_channel, "bounding_boxes", loc_dict)
                         self.draw_bounding_boxes()
 
                 else:
 
                     x, y = position
@@ -902,28 +825,23 @@
                     box_size = int(self.gui.picasso_box_size.currentText())
 
                     new_loc = [frame, position[0], position[1], net_gradient]
 
                     loc_utils = picasso_loc_utils()
                     locs = loc_utils.create_locs(new_loc=new_loc)
 
-                    loc_centers = [[y, x]]
-
                     loc_dict["localisations"] = locs
-                    loc_dict["localisation_centres"] = loc_centers
                     loc_dict["fitted"] = False
                     loc_dict["box_size"] = box_size
 
                     self.update_loc_dict(active_dataset, active_channel, "bounding_boxes", loc_dict)
                     self.draw_bounding_boxes()
 
             elif mode == "lsp":
 
                 x, y = position
 
-                print(x,y)
-
         except:
             print(traceback.format_exc())
             pass
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_picasso_detect.py` & `napari_pixseq-1.0.3/src/napari_pixseq/pixseq_widget.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,713 +1,579 @@
+from qtpy.QtCore import QThreadPool
+from qtpy.QtWidgets import (QWidget,QVBoxLayout)
+
 import numpy as np
 import traceback
-
-import pandas as pd
-
-from napari_pixseq.funcs.pixseq_utils_compute import Worker
-import time
-import os
-from multiprocessing import shared_memory
-from picasso import localize
-from picasso.localize import get_spots, identify_frame
-from picasso.gaussmle import gaussmle
-from functools import partial
-import concurrent.futures
-import multiprocessing
-from picasso.render import render
-from shapely.geometry import Point, Polygon
 from multiprocessing import Manager
+from functools import partial
+import matplotlib.colors as mcolors
 
-def remove_overlapping_locs(locs, box_size):
-
-    try:
-
-        coordinates = np.vstack((locs.y, locs.x)).T
-
-        # Calculate all pairwise differences
-        diff = coordinates[:, np.newaxis, :] - coordinates[np.newaxis, :, :]
-
-        # Calculate squared distances
-        dist_squared = np.sum(diff ** 2, axis=-1)
-
-        # Check if the array is of integer type
-        if coordinates.dtype.kind in 'iu':
-            # Use the maximum integer value for the diagonal if the array is of integer type
-            max_int_value = np.iinfo(coordinates.dtype).max
-            np.fill_diagonal(dist_squared, max_int_value)
-        else:
-            # Use infinity for the diagonal if the array is of float type
-            np.fill_diagonal(dist_squared, np.inf)
-
-        # Identify overlapping coordinates (distance less than X)
-        overlapping = np.any(dist_squared < box_size ** 2, axis=1)
-
-        non_overlapping_locs = locs[~overlapping]
-        non_overlapping_locs = np.array(non_overlapping_locs).view(np.recarray)
-
-    except:
-        pass
+from napari_pixseq.GUI.pixseq_ui import Ui_Frame as gui
+from napari_pixseq.funcs.pixseq_utils_compute import _utils_compute
+from napari_pixseq.funcs.pixseq_undrift_utils import _undrift_utils
+from napari_pixseq.funcs.pixseq_picasso_detect import _picasso_detect_utils
+from napari_pixseq.funcs.pixseq_loc_utils import _loc_utils
+from napari_pixseq.funcs.pixseq_import_utils import _import_utils
+from napari_pixseq.funcs.pixseq_events import _events_utils
+from napari_pixseq.funcs.pixseq_export_images_utils import _export_images_utils
+from napari_pixseq.funcs.pixseq_transform_utils import _tranform_utils
+from napari_pixseq.funcs.pixseq_trace_compute_utils import _trace_compute_utils
+from napari_pixseq.funcs.pixseq_plot_utils import _plot_utils, CustomPyQTGraphWidget
+from napari_pixseq.funcs.pixseq_align_utils import _align_utils
+from napari_pixseq.funcs.pixseq_export_traces_utils import _export_traces_utils
+from napari_pixseq.funcs.pixseq_colocalize_utils import _utils_colocalize
+from napari_pixseq.funcs.pixseq_temporal_filtering import _utils_temporal_filtering
+from napari_pixseq.funcs.pixseq_cluster_utils import _cluster_utils
+from napari_pixseq.funcs.pixseq_simple_analysis_utils import _simple_analysis_utils
+from napari_pixseq.funcs.pixseq_filter_utils import _filter_utils
+from napari_pixseq.funcs.pixseq_segmentation_utils import _segmentation_utils
+from napari_pixseq.funcs.pixseq_tracking_utils import _tracking_utils
+from napari_pixseq.funcs.pixseq_segmentation_events import _segmentation_events
 
-    return non_overlapping_locs
+import napari
 
 
-def cut_spots(movie, ids_frame, ids_x, ids_y, box):
 
-    n_spots = len(ids_x)
-    r = int(box / 2)
-    spots = np.zeros((n_spots, box, box), dtype=movie.dtype)
-    for id, (frame, xc, yc) in enumerate(zip(ids_frame, ids_x, ids_y)):
-        spots[id] = movie[frame, yc - r : yc + r + 1, xc - r : xc + r + 1]
+class PixSeqWidget(QWidget, gui,
+    _undrift_utils, _picasso_detect_utils,
+    _import_utils, _events_utils, _export_images_utils,
+    _tranform_utils, _trace_compute_utils, _plot_utils,
+    _align_utils, _loc_utils, _export_traces_utils,
+    _utils_colocalize, _utils_temporal_filtering, _utils_compute,
+    _cluster_utils, _simple_analysis_utils,
+    _filter_utils, _segmentation_utils, _tracking_utils,
+    _segmentation_events):
 
-    return spots
+    # your QWidget.__init__ can optionally request the napari viewer instance
+    # use a type annotation of 'napari.viewer.Viewer' for any parameter
+    def __init__(self, viewer: "napari.viewer.Viewer"):
+        super().__init__()
 
+        self.viewer = viewer
 
-def picasso_detect(dat, progress_list):
+        #create UI
+        self.gui = gui()
+        self.gui.setupUi(self)
 
-    result = None
+        #initialise graph PyQtGraph canvases
+        self.gui.graph_container.setLayout(QVBoxLayout())
+        self.graph_canvas = CustomPyQTGraphWidget(self)
+        self.gui.graph_container.layout().addWidget(self.graph_canvas)
 
-    try:
+        self.gui.simple_graph_container.setLayout(QVBoxLayout())
+        self.simple_graph_canvas = CustomPyQTGraphWidget(self)
+        self.gui.simple_graph_container.layout().addWidget(self.simple_graph_canvas)
 
-        frame_index = dat["frame_index"]
-        min_net_gradient = dat["min_net_gradient"]
-        box_size = dat["box_size"]
-        roi = dat["roi"]
-        dataset = dat["dataset"]
-        channel = dat["channel"]
-        detect = dat["detect"]
-        fit = dat["fit"]
-        remove_overlapping = dat["remove_overlapping"]
-        stop_event = dat["stop_event"]
-        polygon_filter = dat["polygon_filter"]
-        polygons = dat["polygons"]
+        self.gui.filter_graph_container.setLayout(QVBoxLayout())
+        self.filter_graph_canvas = CustomPyQTGraphWidget(self)
+        self.gui.filter_graph_container.layout().addWidget(self.filter_graph_canvas)
 
-        if not stop_event.is_set():
+        #register events
+        self.register_events()
 
-            # Access the shared memory
-            shared_mem = shared_memory.SharedMemory(name=dat["shared_memory_name"])
-            np_array = np.ndarray(dat["shape"], dtype=dat["dtype"], buffer=shared_mem.buf)
+        #initialise variables
+        self.dataset_dict = {}
+        self.traces_dict = {}
+        self.plot_dict = {}
+        self.contrast_dict = {}
+        self.localisation_dict = {"bounding_boxes": {}, "localisations": {}}
+        self.metric_dict = {"spot_mean": "Mean", "spot_median": "Median", "spot_sum": "Sum", "spot_max": "Maximum",
+                            "spot_std": "std", "spot_photons": "Picasso Photons", }
 
-            frame = np_array.copy()
+        self.background_dict = {"None":"None",
+                                "_local_bg": "Local Background",
+                                "_masked_local_bg": "Masked Local Background",
+                                "_global_bg": "Global Background",
+                                "_masked_global_bg": "Masked Global Background",
+                                "_local_bg": "Local Background",
+                                "spot_lsp_bg": "LSP Background",
+                                }
+        self.active_dataset = None
+        self.active_channel = None
+        self.verbose = False
+        self.worker = None
+        self.multiprocessing_active = False
+        self.transform_matrix = None
 
-            if detect:
-                locs = identify_frame(frame, min_net_gradient, box_size, 0, roi=roi)
+        #create threadpool and stop event
+        self.threadpool = QThreadPool()
+        manager = Manager()
+        self.stop_event = manager.Event()
 
-                if remove_overlapping:
-                    # overlapping removed prior to fitting to increase speed
-                    locs = remove_overlapping_locs(locs, box_size)
 
-            else:
-                locs = dat["frame_locs"]
+        self.update_import_options()
+        self.update_import_append_options()
 
-            expected_loc_length = 4
+        self.check_gpufit_availibility()
 
-            if fit:
-                expected_loc_length = 12
-                try:
-                    image = np.expand_dims(frame, axis=0)
-                    camera_info = {"baseline": 100.0, "gain": 1, "sensitivity": 1.0, "qe": 0.9, }
-                    spot_data = get_spots(image, locs, box_size, camera_info)
+        self.widget_notifications = True
 
-                    theta, CRLBs, likelihoods, iterations = gaussmle(spot_data, eps=0.001, max_it=1000, method="sigma")
-                    locs = localize.locs_from_fits(locs.copy(), theta, CRLBs, likelihoods, iterations, box_size)
+    def register_events(self):
 
-                    locs.frame = frame_index
+        self.gui.pixseq_import.clicked.connect(self.pixseq_import_data)
+        self.gui.pixseq_import_mode.currentIndexChanged.connect(self.update_import_options)
+        self.gui.pixseq_update_dataset_name.clicked.connect(self.update_dataset_name)
+        self.gui.pixseq_delete_dataset.clicked.connect(self.delete_dataset)
+        self.gui.pixseq_update_labels.clicked.connect(self.update_nucleotide)
 
-                    if remove_overlapping:
-                        # sometimes locs can overlap after fitting
-                        locs = remove_overlapping_locs(locs, box_size)
+        self.gui.import_picasso.clicked.connect(self.import_picaaso_localisations)
 
-                except:
-                    # print(traceback.format_exc())
-                    pass
+        self.gui.picasso_detect.clicked.connect(partial(self.pixseq_picasso, detect = True, fit=False))
+        self.gui.picasso_fit.clicked.connect(partial(self.pixseq_picasso, detect = False, fit=True))
+        self.gui.picasso_detectfit.clicked.connect(partial(self.pixseq_picasso, detect=True, fit=True))
+        self.gui.cluster_localisations.clicked.connect(self.pixseq_cluster_localisations)
+        self.gui.dbscan_remove_overlapping = self.gui.dbscan_remove_overlapping
 
-            for loc in locs:
-                loc.frame = frame_index
+        self.gui.picasso_render.clicked.connect(self.initialise_picasso_render)
 
-            if polygon_filter:
+        self.gui.pixseq_dataset_selector.currentIndexChanged.connect(self.update_channel_select_buttons)
+        self.gui.pixseq_dataset_selector.currentIndexChanged.connect(partial(self.update_active_image,
+            dataset = self.gui.pixseq_dataset_selector.currentText()))
 
-                if len(polygons) > 0 and len(locs) > 0:
+        self.gui.picasso_undrift.clicked.connect(self.undrift_images)
 
-                    expected_loc_length += 1
+        self.gui.pixseq_align_datasets.clicked.connect(self.align_datasets)
+        self.gui.align_reference_dataset.currentIndexChanged.connect(self.update_align_reference_channel)
 
-                    loclist = pd.DataFrame(locs).to_dict(orient="records")
+        self.gui.pixseq_import_tform.clicked.connect(self.import_transform_matrix)
+        self.gui.pixseq_compute_tform.clicked.connect(self.compute_transform_matrix)
+        self.gui.pixseq_apply_tform.clicked.connect(self.apply_transform_matrix)
 
-                    filtered_locs = []
+        self.gui.picasso_detect_mode.currentIndexChanged.connect(self.update_picasso_options)
 
-                    for loc in loclist:
-                        point = Point(loc["x"], loc["y"])
+        self.gui.pixseq_export_data.clicked.connect(self.export_data)
+        self.gui.export_dataset.currentIndexChanged.connect(self.update_export_options)
 
-                        for polygon_index, polygon in enumerate(polygons):
-                            if polygon.contains(point):
-                                loc["segmentation"] = polygon_index
-                                filtered_locs.append(loc)
+        self.gui.pixseq_export_locs.clicked.connect(self.initialise_export_locs)
+        self.gui.locs_export_type.currentIndexChanged.connect(self.update_loc_export_options)
+        self.gui.locs_export_dataset.currentIndexChanged.connect(self.update_loc_export_options)
 
-                    if len(filtered_locs):
-                        locs = pd.DataFrame(filtered_locs).to_records(index=False)
-                    else:
-                        locs = []
+        self.gui.pixseq_export_traces.clicked.connect(self.export_traces)
+        self.gui.traces_export_dataset.currentIndexChanged.connect(self.populate_export_combos)
 
-                else:
-                    locs = []
+        self.viewer.dims.events.current_step.connect(partial(self.draw_localisations, update_vis = False))
 
-            render_locs = {frame_index: []}
+        self.gui.compute_traces.clicked.connect(self.pixseq_compute_traces)
+        self.gui.traces_visualise_masks.clicked.connect(self.visualise_spot_masks)
+        self.gui.traces_visualise_masks.clicked.connect(self.visualise_background_masks)
 
-            if len(locs) > 0:
-                render_locs[frame_index] = np.vstack((locs.y, locs.x)).T.tolist()
+        self.gui.plot_data.currentIndexChanged.connect(partial(self.update_plot_combos, combo="plot_data"))
+        self.gui.plot_channel.currentIndexChanged.connect(partial(self.update_plot_combos, combo="plot_channel"))
 
-                locs = [loc for loc in locs if len(loc) == expected_loc_length]
-                locs = np.array(locs).view(np.recarray)
+        self.gui.plot_data.currentIndexChanged.connect(self.initialize_plot)
+        self.gui.plot_channel.currentIndexChanged.connect(self.initialize_plot)
+        self.gui.plot_metric.currentIndexChanged.connect(self.initialize_plot)
+        self.gui.split_plots.stateChanged.connect(self.initialize_plot)
+        self.gui.normalise_plots.stateChanged.connect(self.initialize_plot)
+        self.gui.plot_background_mode.currentIndexChanged.connect(self.initialize_plot)
+        self.gui.focus_on_bbox.stateChanged.connect(self.initialize_plot)
 
-            result = {"dataset": dataset, "channel": channel, "frame_index": frame_index,
-                      "locs": locs,"render_locs": render_locs}
+        self.gui.pixseq_colocalize.clicked.connect(self.pixseq_colocalize_localisations)
 
-    except:
-        print(traceback.format_exc())
-        pass
+        self.gui.plot_localisation_number.valueChanged.connect(lambda: self.update_slider_label("plot_localisation_number"))
+        self.gui.plot_localisation_number.valueChanged.connect(partial(self.plot_traces))
 
-    progress_list.append(dat["frame_index"])
+        self.gui.filtering_start.clicked.connect(self.pixseq_temporal_filtering)
+        self.gui.filtering_datasets.currentIndexChanged.connect(self.update_filtering_channels)
 
-    return result
+        self.gui.pixseq_append.stateChanged.connect(self.update_import_append_options)
 
+        self.gui.picasso_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="picasso_dataset", channel_selector="picasso_channel"))
+        self.gui.undrift_dataset_selector.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="undrift_dataset_selector", channel_selector="undrift_channel_selector"))
+        self.gui.cluster_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="cluster_dataset", channel_selector="cluster_channel"))
+        self.gui.tform_compute_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="tform_compute_dataset", channel_selector="tform_compute_ref_channel", channel_type="donor"))
+        self.gui.tform_compute_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="tform_compute_dataset", channel_selector="tform_compute_target_channel", channel_type="acceptor"))
+        self.gui.colo_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="colo_dataset", channel_selector="colo_channel1"))
+        self.gui.colo_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="colo_dataset", channel_selector="colo_channel2"))
+        self.gui.picasso_filter_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="picasso_filter_dataset", channel_selector="picasso_filter_channel"))
+        self.gui.simple_plot_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="simple_plot_dataset", channel_selector="simple_plot_channel", efficiency=True))
+        self.gui.picasso_render_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="picasso_render_dataset", channel_selector="picasso_render_channel"))
+        self.gui.cellpose_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="cellpose_dataset", channel_selector="cellpose_channel"))
+        self.gui.tracking_dataset.currentIndexChanged.connect(partial(self.update_channel_selector, dataset_selector="tracking_dataset", channel_selector="tracking_channel"))
 
-class _picasso_detect_utils:
+        self.gui.traces_export_mode.currentIndexChanged.connect(self.populate_export_combos)
 
-    def populate_localisation_dict(self, loc_dict, render_loc_dict, detect_mode,
-            image_channel, box_size, fitted=False):
+        self.gui.picasso_filter_dataset.currentIndexChanged.connect(self.update_filter_criterion)
+        self.gui.picasso_filter_channel.currentIndexChanged.connect(self.update_filter_criterion)
+        self.gui.filter_criterion.currentIndexChanged.connect(self.update_criterion_ranges)
+        self.gui.filter_localisations.clicked.connect(self.pixseq_filter_localisations)
+        self.gui.picasso_filter_type.currentIndexChanged.connect(self.update_filter_dataset)
 
-        if self.verbose:
-            print("Populating localisation dictionary...")
+        self.viewer.bind_key('Control-D', self.dev_function)
 
-        detect_mode = detect_mode.lower()
+        self.viewer.bind_key('PageUp', self.named_partial(self.increment_active_dataset, key='Up'), overwrite=True)
+        self.viewer.bind_key('PageDown', self.named_partial(self.increment_active_dataset, key='Down'), overwrite=True)
 
-        try:
+        self.viewer.bind_key('Q', self.stop_worker, overwrite=True)
 
-            for dataset_name, locs in loc_dict.items():
+        self.viewer.layers.events.inserted.connect(self.on_add_layer)
 
-                if detect_mode == "localisations":
+        self.gui.simple_plot_mode.currentIndexChanged.connect(self.update_plot_channel)
+        self.gui.simple_plot_dataset.currentIndexChanged.connect(self.draw_line_plot)
+        self.gui.simple_plot_channel.currentIndexChanged.connect(self.draw_line_plot)
+        self.gui.simple_subtract_background.clicked.connect(self.draw_line_plot)
 
-                    if dataset_name not in self.localisation_dict["localisations"].keys():
-                        self.localisation_dict["localisations"][dataset_name] = {}
-                    if image_channel not in self.localisation_dict["localisations"][dataset_name].keys():
-                        self.localisation_dict["localisations"][dataset_name][image_channel.lower()] = {}
+        self.gui.add_line.clicked.connect(lambda: self.draw_shapes(mode="line"))
+        self.gui.add_box.clicked.connect(lambda: self.draw_shapes(mode="box"))
+        self.gui.add_background.clicked.connect(lambda: self.draw_shapes(mode="background"))
 
-                    render_locs = render_loc_dict[dataset_name]
+        self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
+        self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
+        self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
+        self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
+        self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
+        self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
+        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
+        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
 
-                    loc_centres = self.get_localisation_centres(locs)
+        self.gui.segment_active.clicked.connect(partial(self.initialise_cellpose, mode = "active"))
+        self.gui.segment_all.clicked.connect(partial(self.initialise_cellpose, mode = "all"))
+        self.gui.cellpose_load_model.clicked.connect(self.load_cellpose_model)
+        self.gui.dilate_segmentations.clicked.connect(self.dilate_segmentations)
 
-                    fiducial_dict = {"localisations": [], "localisation_centres": [], "render_locs": {}}
+        self.gui.cellpose_flowthresh.valueChanged.connect(lambda: self.update_cellpose_sliders("cellpose_flowthresh", "cellpose_flowthresh_label"))
+        self.gui.cellpose_maskthresh.valueChanged.connect(lambda: self.update_cellpose_sliders("cellpose_maskthresh", "cellpose_maskthresh_label"))
+        self.gui.cellpose_minsize.valueChanged.connect(lambda: self.update_cellpose_sliders("cellpose_minsize", "cellpose_minsize_label"))
+        self.gui.cellpose_diameter.valueChanged.connect(lambda: self.update_cellpose_sliders("cellpose_diameter", "cellpose_diameter_label"))
 
-                    fiducial_dict["localisations"] = locs.copy()
-                    fiducial_dict["localisation_centres"] = loc_centres.copy()
-                    fiducial_dict["render_locs"] = render_locs
+        self.gui.link_localisations.clicked.connect(self.initialise_tracking)
 
-                    fiducial_dict["fitted"] = fitted
-                    fiducial_dict["box_size"] = box_size
+        self.gui.dev_verbose.stateChanged.connect(self.toggle_verbose)
 
-                    self.localisation_dict["localisations"][dataset_name][image_channel.lower()] = fiducial_dict.copy()
+        self.viewer.bind_key(key="a", func=lambda event: self.segmentation_modify_mode(mode="add"), overwrite=True)
+        self.viewer.bind_key(key="e", func=lambda event: self.segmentation_modify_mode(mode="extend"), overwrite=True)
+        self.viewer.bind_key(key="j", func=lambda event: self.segmentation_modify_mode(mode="join"), overwrite=True)
+        self.viewer.bind_key(key="s", func=lambda event: self.segmentation_modify_mode(mode="split"), overwrite=True)
+        self.viewer.bind_key(key="d", func=lambda event: self.segmentation_modify_mode(mode="delete"), overwrite=True)
 
-                else:
 
-                    loc_centres = self.get_localisation_centres(locs)
+        # self.viewer.bind_key(key="e", func=self.segmentation_modify_mode(mode="extend"), overwrite=True)
+        # self.viewer.bind_key(key="j", func=self.segmentation_modify_mode(mode="join"), overwrite=True)
+        # self.viewer.bind_key(key="s", func=self.segmentation_modify_mode(mode="split"), overwrite=True)
+        # self.viewer.bind_key(key="d", func=self.segmentation_modify_mode(mode="delete"), overwrite=True)
 
-                    self.localisation_dict["bounding_boxes"]["localisations"] = locs.copy()
-                    self.localisation_dict["bounding_boxes"]["localisation_centres"] = loc_centres.copy()
-                    self.localisation_dict["bounding_boxes"]["fitted"] = fitted
-                    self.localisation_dict["bounding_boxes"]["box_size"] = box_size
 
 
-        except:
-            print(traceback.format_exc())
-            self.gui.picasso_progressbar.setValue(0)
-            self.gui.picasso_detect.setEnabled(True)
-            self.gui.picasso_fit.setEnabled(True)
-            self.gui.picasso_detectfit.setEnabled(True)
+    def check_gpufit_availibility(self):
 
-    def _picasso_wrapper_result(self, result):
+        self.gpufit_available = False
 
         try:
+            from pygpufit import gpufit as gf
+            package_installed = True
+        except:
+            package_installed = False
 
-            if self.verbose:
-                print("Picasso wrapper result received")
-
-            fitted, loc_dict, render_loc_dict, total_locs = result
-
-            detect_mode = self.gui.picasso_detect_mode.currentText()
-            image_channel = self.gui.picasso_channel.currentText()
-            box_size = int(self.gui.picasso_box_size.currentText())
+        if package_installed:
 
-            dataset_names = list(loc_dict.keys())
+            if not gf.cuda_available():
+                print("Pygpufit not available due to missing CUDA")
+            else:
+                runtime_version, driver_version = gf.get_cuda_version()
 
-            if len(dataset_names) > 0:
+                runtime_version = ".".join([str(v) for v in list(runtime_version)])
+                driver_version = ".".join([str(v) for v in list(driver_version)])
 
-                self.populate_localisation_dict(loc_dict, render_loc_dict, detect_mode,
-                    image_channel, box_size, fitted)
+                if runtime_version != driver_version:
+                    print(f"Pygpufit not available due to CUDA version mismatch. "
+                          f"Runtime: {runtime_version}, Driver: {driver_version}")
 
-                if fitted:
-                    self.pixseq_notification("Fitted {} {}".format(total_locs, detect_mode))
                 else:
-                    self.pixseq_notification("Detected {} {}".format(total_locs, detect_mode))
-
-        except:
-            print(traceback.format_exc())
-
-    def _picasso_wrapper_finished(self):
+                    self.gpufit_available = True
 
-        try:
+        else:
+            print("Pygpufit not available due to missing package")
+            print("Install pygpufit package into napari-PixSeq root directory")
 
-            image_channel = self.gui.picasso_channel.currentText()
-            dataset_name = self.gui.picasso_dataset.currentText()
+        if self.gpufit_available:
+            print("Pygpufit available")
+            self.gui.picasso_use_gpufit.setEnabled(True)
+        else:
+            self.gui.picasso_use_gpufit.setEnabled(False)
 
-            if dataset_name == "All Datasets":
-                dataset_name = self.active_dataset
 
-            self.update_active_image(channel=image_channel.lower(), dataset=dataset_name)
+    def on_add_layer(self, event):
+        if event.value.name == "Shapes":
+            layer_list = [layer.name for layer in self.viewer.layers if layer.name != "Shapes"]
 
-            self.draw_bounding_boxes()
-            self.draw_localisations()
+            self.shapes_layer = self.viewer.layers["Shapes"]
 
-            self.update_filter_criterion()
-            self.update_criterion_ranges()
+            self.shapes_layer.events.data.connect(self.shapes_layer_updated)
 
-            self.update_ui()
+            self.shapes_layer.current_edge_color = list(mcolors.to_rgb("green"))
+            self.shapes_layer.current_face_color = [0, 0, 0, 0]
+            self.shapes_layer.current_edge_width = 1
 
-        except:
-            print(traceback.format_exc())
 
+    def toggle_verbose(self):
 
+        if self.gui.dev_verbose.isChecked():
+            self.verbose = True
+        else:
+            self.verbose = False
 
+    def dev_function(self, event):
 
-    def get_frame_locs(self, dataset_name, image_channel, frame_index):
+        print("Dev function called")
 
-        try:
+        self.check_gpufit_availibility()
 
-            loc_dict, n_locs, _ = self.get_loc_dict(dataset_name,
-                image_channel.lower(), type = "localisations")
 
-            if "localisations" not in loc_dict.keys():
-                return None
-            elif len(loc_dict["localisations"]) == 0:
-                return None
-            else:
-                locs = loc_dict["localisations"]
-                locs = locs[locs.frame == frame_index]
 
-                return locs.copy()
+    def select_image_layer(self):
 
+        try:
+            if hasattr(self, "image_layer"):
+                self.viewer.layers.selection.select_only(self.image_layer)
         except:
             print(traceback.format_exc())
-            return None
+            pass
 
-    def _picasso_wrapper(self, progress_callback, detect, fit, min_net_gradient, image_channel):
+    def add_lsp_localisation(self, position = None):
 
-        loc_dict = {}
-        render_loc_dict = {}
-        total_locs = 0
         try:
+            layer_names = [layer.name for layer in self.viewer.layers]
 
-            box_size = int(self.gui.picasso_box_size.currentText())
-            dataset_name = self.gui.picasso_dataset.currentText()
-            frame_mode = self.gui.picasso_frame_mode.currentText()
-            remove_overlapping = self.gui.picasso_remove_overlapping.isChecked()
-            polygon_filter = self.gui.picasso_segmentation_filtering.isChecked()
-            roi = self.generate_roi()
-
-            if dataset_name == "All Datasets":
-                dataset_list = list(self.dataset_dict.keys())
-            else:
-                dataset_list = [dataset_name]
-
-            channel_list = [image_channel.lower()]
-
-            if frame_mode.lower() == "active":
-                frame_index = self.viewer.dims.current_step[0]
-            else:
-                frame_index = None
-
-            self.shared_frames = self.create_shared_frames(
-                dataset_list=dataset_list,
-                channel_list=channel_list,
-                frame_index=frame_index,
-            )
-
-            segmentation_polygons = self.get_segmentation_polygons()
-
-            compute_jobs = []
-
-            if self.verbose:
-                print("Creating Picasso compute jobs...")
-
-            if self.verbose:
-                print(f"Creating compute jobs for {len(self.shared_images)} datasets...")
-
-            for image_dict in self.shared_frames:
-                image_dict = image_dict.copy()
-
-                if frame_mode.lower() == "active":
-                    frame_list = [self.viewer.dims.current_step[0]]
-                else:
-                    n_frames = image_dict["shape"][0]
-                    frame_list = list(range(n_frames))
-
-                for frame_index in frame_list:
+            vis_mode = self.gui.picasso_vis_mode.currentText()
+            vis_size = float(self.gui.picasso_vis_size.currentText())
+            vis_opacity = float(self.gui.picasso_vis_opacity.currentText())
+            vis_edge_width = float(self.gui.picasso_vis_edge_width.currentText())
 
-                    polygons = []
-                    if type(segmentation_polygons) == dict:
-                        if frame_index in segmentation_polygons.keys():
-                            polygons = segmentation_polygons[frame_index]
-                    if type(segmentation_polygons) == list:
-                        polygons = segmentation_polygons
+            if vis_mode.lower() == "square":
+                symbol = "square"
+            elif vis_mode.lower() == "disk":
+                symbol = "disc"
+            elif vis_mode.lower() == "x":
+                symbol = "cross"
 
-                    frame_dict = image_dict["frame_dict"][frame_index]
+            if position is not None:
 
-                    time_start = time.time()
+                if hasattr(self, "lsp_locs"):
 
-                    if self.verbose:
-                        print(f"Creating compute job for frame {frame_index}")
+                    distances = np.sqrt(np.sum((self.lsp_locs - np.array(position)) ** 2, axis=1))
 
-                    frame_locs = self.get_frame_locs(image_dict["dataset"], image_channel, frame_index)
+                    min_index = np.argmin(distances)
+                    min_distance = distances[min_index]
 
-                    if detect == False and frame_locs is None:
-                        continue
-                    # elif polygon_filter is True and len(polygons) == 0:
-                    #     continue
+                    if min_distance < vis_size/2:
+                        self.lsp_locs.pop(min_index)
                     else:
-                        compute_job = {"dataset": frame_dict["dataset"],
-                                       "channel": frame_dict["channel"],
-                                       "frame_index": frame_index,
-                                       "shared_memory_name": frame_dict["shared_memory_name"],
-                                       "shape": frame_dict["shape"],
-                                       "dtype": frame_dict["dtype"],
-                                       "detect": detect,
-                                       "fit": fit,
-                                       "min_net_gradient": int(min_net_gradient),
-                                       "box_size": int(box_size),
-                                       "roi": roi,
-                                       "frame_locs": frame_locs,
-                                       "remove_overlapping": remove_overlapping,
-                                       "polygon_filter":polygon_filter,
-                                       "polygons": polygons,
-                                       "stop_event": self.stop_event, }
-
-                    compute_jobs.append(compute_job)
-
-                    if self.verbose:
-                        time_end = time.time()
-                        time_duration = time_end - time_start
-                        print(f"Compute job created in {time_duration} seconds")
-
-
-            if len(compute_jobs) > 0:
-                if self.verbose:
-                    print(f"Starting Picasso {len(compute_jobs)} compute jobs...")
-
-                timeout_duration = 10  # Timeout in seconds
-
-                loc_dict = {}
-                render_loc_dict = {}
-
-                if frame_mode.lower() == "active":
-                    executor_class = concurrent.futures.ThreadPoolExecutor
-                    cpu_count = 1
+                        self.lsp_locs.append(position)
                 else:
-                    executor_class = concurrent.futures.ProcessPoolExecutor
-                    cpu_count = int(multiprocessing.cpu_count() * 0.9)
-
-                with Manager() as manager:
-                    progress_list = manager.list()
-
-                    with executor_class(max_workers=cpu_count) as executor:
-                        futures = {executor.submit(picasso_detect, job, progress_list): job for job in compute_jobs}
-
-                        # Calculate and emit progress
-                        while any(not future.done() for future in futures):
-                            progress = (len(progress_list)/len(compute_jobs)) * 100
-                            if progress_callback is not None:
-                                progress_callback.emit(progress)
-
-                        for future in concurrent.futures.as_completed(futures):
-
-                            if self.stop_event.is_set():
-                                future.cancel()
-                            else:
-                                job = futures[future]
-                                try:
-                                    result = future.result(timeout=timeout_duration)  # Process result here
-
-                                    if result is not None:
-                                        dataset_name = result["dataset"]
-
-                                        if dataset_name not in loc_dict:
-                                            loc_dict[dataset_name] = []
-                                            render_loc_dict[dataset_name] = {}
-
-                                        locs = result["locs"]
-                                        render_locs = result["render_locs"]
-
-                                        if len(locs) > 0:
-                                            loc_dict[dataset_name].extend(locs)
-
-                                        render_loc_dict[dataset_name] = {**render_loc_dict[dataset_name], **render_locs, }
+                    self.lsp_locs = [position]
 
-                                except concurrent.futures.TimeoutError:
-                                    # print(f"Task {job} timed out after {timeout_duration} seconds.")
-                                    pass
-                                except Exception as e:
-                                    print(f"Error occurred in task {job}: {e}")  # Handle other exceptions
+            if hasattr(self, "lsp_locs"):
 
-                if self.verbose:
-                    print("Finished Picasso compute jobs...")
-                    print("Compiling Picasso results...")
+                lsp_locs = list(self.lsp_locs)
 
-                total_locs = 0
-                for dataset, locs in loc_dict.items():
-                    if len(locs) > 0:
-                        locs = np.hstack(locs).view(np.recarray).copy()
-                        locs.sort(kind="mergesort", order="frame")
-                        locs = np.array(locs).view(np.recarray)
-                        loc_dict[dataset] = locs
-                    total_locs += len(locs)
+                if "LSP localisations" not in layer_names:
+                    self.lsp_layer = self.viewer.add_points(lsp_locs,
+                        edge_color="green",
+                        ndim=2,
+                        face_color=[0, 0, 0,0],
+                        opacity=vis_opacity,
+                        name="LSP localisations",
+                        symbol=symbol,
+                        size=vis_size,
+                        visible=True,
+                        edge_width=vis_edge_width, )
 
+                    self.lsp_layer.mouse_drag_callbacks.append(self._mouse_event)
+                    self.lsp_layer.selected_data = []
 
-            self.restore_shared_frames()
+                else:
+                    self.lsp_layer.data = lsp_locs
+                    self.lsp_layer.selected_data = []
 
-            self.update_ui()
+                self.lsp_layer.refresh()
 
         except:
             print(traceback.format_exc())
+            pass
 
-            self.restore_shared_frames()
-
-            self.update_ui()
-
-            loc_dict = {}
-            render_loc_dict = {}
-            total_locs = 0
-
-        return fit, loc_dict, render_loc_dict, total_locs
-
-    def pixseq_picasso(self, detect = False, fit = False):
-
-        try:
-            if self.dataset_dict != {}:
-
-                min_net_gradient = self.gui.picasso_min_net_gradient.text()
-                image_channel = self.gui.picasso_channel.currentText()
-                frame_mode = self.gui.picasso_frame_mode.currentText()
-                minimise_ram = self.gui.picasso_minimise_ram.isChecked()
-
-                if min_net_gradient.isdigit() and image_channel != "":
-
-                    self.gui.picasso_progressbar.setValue(0)
-                    self.gui.picasso_detect.setEnabled(False)
-                    self.gui.picasso_fit.setEnabled(False)
-                    self.gui.picasso_detectfit.setEnabled(False)
-
-                    self.update_ui(init=True)
-
-                    if minimise_ram == True and frame_mode.lower() != "active":
-                        self.clear_live_images()
+    def draw_bounding_boxes(self, update_vis=False):
 
-                    self.worker = Worker(self._picasso_wrapper,
-                        detect=detect, fit=fit,
-                        min_net_gradient=min_net_gradient,
-                        image_channel=image_channel,)
+        if hasattr(self, "localisation_dict") and hasattr(self, "active_channel"):
 
-                    self.worker.signals.progress.connect(partial(self.pixseq_progress,
-                        progress_bar=self.gui.picasso_progressbar))
+            if hasattr(self, "bbox_layer"):
+                show_bboxes = self.bbox_layer.visible
+            else:
+                show_bboxes = True
 
-                    self.worker.signals.result.connect(self._picasso_wrapper_result)
-                    self.worker.signals.finished.connect(self._picasso_wrapper_finished)
-                    self.worker.signals.error.connect(self.update_ui)
-                    self.threadpool.start(self.worker)
+            if show_bboxes:
 
+                layer_names = [layer.name for layer in self.viewer.layers]
+                loc_dict, n_locs, fitted = self.get_loc_dict(type = "bounding_boxes")
 
-        except:
-            print(traceback.format_exc())
+                if n_locs > 0:
 
-            self.update_ui()
+                    if self.verbose:
+                        print("Drawing bounding_boxes")
 
+                    locs = loc_dict["localisations"].copy()
+                    bounding_boxes = np.vstack((locs.y, locs.x)).T.tolist()
 
-    def generate_roi(self):
+                    vis_mode = self.gui.picasso_vis_mode.currentText()
+                    vis_size = float(self.gui.picasso_vis_size.currentText())
+                    vis_opacity = float(self.gui.picasso_vis_opacity.currentText())
+                    vis_edge_width = float(self.gui.picasso_vis_edge_width.currentText())
+
+                    if vis_mode.lower() == "square":
+                        symbol = "square"
+                    elif vis_mode.lower() == "disk":
+                        symbol = "disc"
+                    elif vis_mode.lower() == "x":
+                        symbol = "cross"
+
+                    if "bounding_boxes" not in layer_names:
+                        self.bbox_layer = self.viewer.add_points(
+                            bounding_boxes,
+                            edge_color="white",
+                            ndim=2,
+                            face_color=[0,0,0,0],
+                            opacity=vis_opacity,
+                            name="bounding_boxes",
+                            symbol=symbol,
+                            size=vis_size,
+                            visible=True,
+                            edge_width=vis_edge_width,)
 
-        if self.verbose:
-            print("Generating ROI")
+                        self.bbox_layer.mouse_drag_callbacks.append(self._mouse_event)
+                        self.bbox_layer.events.visible.connect(self.draw_bounding_boxes)
 
-        border_width = self.gui.picasso_roi_border_width.text()
-        window_cropping = self.gui.picasso_window_cropping .isChecked()
+                    else:
+                        self.viewer.layers["bounding_boxes"].data = bounding_boxes
 
-        roi = None
+                    self.bbox_layer.selected_data = list(range(len(self.bbox_layer.data)))
+                    self.bbox_layer.opacity = vis_opacity
+                    self.bbox_layer.symbol = symbol
+                    self.bbox_layer.size = vis_size
+                    self.bbox_layer.edge_width = vis_edge_width
+                    self.bbox_layer.edge_color = "white"
+                    self.bbox_layer.selected_data = []
+                    self.bbox_layer.refresh()
 
-        try:
+                for layer in layer_names:
+                    self.viewer.layers[layer].refresh()
 
-            generate_roi = False
 
-            if window_cropping:
-                layers_names = [layer.name for layer in self.viewer.layers if layer.name not in ["bounding_boxes", "localisations"]]
+    def draw_localisations(self, update_vis=False):
 
-                crop = self.viewer.layers[layers_names[0]].corner_pixels[:, -2:]
-                [[y1, x1], [y2, x2]] = crop
+        remove_localisations = True
 
-                generate_roi = True
+        if hasattr(self, "localisation_dict") and hasattr(self, "active_channel"):
 
+            if hasattr(self, "fiducial_layer"):
+                show_localisations = self.fiducial_layer.visible
             else:
+                show_localisations = True
 
-                if type(border_width) == str:
-                    border_width = int(border_width)
-                    if border_width > 0:
-                        generate_roi = True
-                elif type(border_width) == int:
-                    if border_width > 0:
-                        generate_roi = True
+            if show_localisations:
 
-            if generate_roi:
+                layer_names = [layer.name for layer in self.viewer.layers]
 
-                dataset = self.gui.picasso_dataset.currentText()
-                channel = self.gui.picasso_channel.currentText()
+                active_frame = self.viewer.dims.current_step[0]
 
-                if dataset == "All Datasets":
-                    dataset = list(self.dataset_dict.keys())[0]
+                dataset_name = self.gui.pixseq_dataset_selector.currentText()
+                image_channel = self.active_channel
 
-                image_shape = self.dataset_dict[dataset][channel.lower()]["data"].shape
+                if image_channel != "" and dataset_name != "":
 
-                frame_shape = image_shape[1:]
+                    if image_channel.lower() in self.localisation_dict["localisations"][dataset_name].keys():
+                        localisation_dict = self.localisation_dict["localisations"][dataset_name][image_channel.lower()].copy()
 
-                if window_cropping:
+                        if "localisations" in localisation_dict.keys():
 
-                    border_width = int(border_width)
+                            locs = localisation_dict["localisations"]
 
-                    if x1 < border_width:
-                        x1 = border_width
-                    if y1 < border_width:
-                        y1 = border_width
-                    if x2 > frame_shape[1] - border_width:
-                        x2 = frame_shape[1] - border_width
-                    if y2 > frame_shape[0] - border_width:
-                        y2 = frame_shape[0] - border_width
+                            if active_frame in locs.frame:
 
-                    roi = [[y1, x1], [y2, x2]]
+                                frame_locs = locs[locs.frame == active_frame].copy()
+                                render_locs = np.vstack((frame_locs.y, frame_locs.x)).T.tolist()
 
-                else:
+                                vis_mode = self.gui.picasso_vis_mode.currentText()
+                                vis_size = float(self.gui.picasso_vis_size.currentText())
+                                vis_opacity = float(self.gui.picasso_vis_opacity.currentText())
+                                vis_edge_width = float(self.gui.picasso_vis_edge_width.currentText())
 
-                    roi = [[int(border_width), int(border_width)],
-                           [int(frame_shape[0] - border_width), int(frame_shape[1] - border_width)]]
+                                if vis_mode.lower() == "square":
+                                    symbol = "square"
+                                elif vis_mode.lower() == "disk":
+                                    symbol = "disc"
+                                elif vis_mode.lower() == "x":
+                                    symbol = "cross"
 
-        except:
-            print(traceback.format_exc())
-            pass
+                                remove_localisations = False
 
-        return roi
+                                if "localisations" not in layer_names:
 
-    def export_picasso_locs(self, locs):
+                                    if self.verbose:
+                                        print("Drawing localisations")
 
-        if self.verbos:
-            print("Exporting Picasso locs")
+                                    self.fiducial_layer = self.viewer.add_points(
+                                        render_locs,
+                                        ndim=2,
+                                        edge_color="red",
+                                        face_color=[0,0,0,0],
+                                        opacity=vis_opacity,
+                                        name="localisations",
+                                        symbol=symbol,
+                                        size=vis_size,
+                                        edge_width=vis_edge_width, )
 
-        try:
+                                    self.fiducial_layer.mouse_drag_callbacks.append(self._mouse_event)
+                                    self.fiducial_layer.events.visible.connect(self.draw_localisations)
 
-            dataset_name = self.gui.picasso_dataset.currentText()
-            image_channel = self.gui.picasso_channel.currentText()
-            min_net_gradient = int(self.gui.picasso_min_net_gradient.text())
-            box_size = int(self.gui.picasso_box_size.currentText())
-
-            path = self.dataset_dict[dataset_name][image_channel.lower()]["path"]
-            image_shape = self.dataset_dict[dataset_name][image_channel.lower()]["data"].shape
-
-            base, ext = os.path.splitext(path)
-            path = base + f"_{image_channel}_picasso_locs.hdf5"
-
-            info = [{"Byte Order": "<", "Data Type": "uint16", "File": path,
-                     "Frames": image_shape[0], "Height": image_shape[1],
-                     "Micro-Manager Acquisiton Comments": "", "Width": image_shape[2], },
-                    {"Box Size": box_size, "Fit method": "LQ, Gaussian",
-                     "Generated by": "Picasso Localize",
-                     "Min. Net Gradient": min_net_gradient, "Pixelsize": 130, "ROI": None, }]
+                                    update_vis = True
 
-            from picasso.io import save_locs
-            # save_locs(path, locs, info)
+                                else:
 
-        except:
-            print(traceback.format_exc())
-            pass
+                                    if self.verbose:
+                                        print("Updating fiducial data")
 
-    def render_picasso_locs(self, locs, image_shape, blur_method=None, min_blur_width=1,
-            pixel_size=1, progress_callback=None, oversampling=20, ):
-        try:
-            h, w = image_shape[-2:]
+                                    self.fiducial_layer.data = render_locs
+                                    self.fiducial_layer.selected_data = []
 
-            viewport = [(0, 0), (h, w)]
+                                if update_vis:
 
-            n_rendered_locs, image = render(locs, viewport=viewport,
-                blur_method=blur_method, min_blur_width=min_blur_width, oversampling=oversampling, )
+                                    if self.verbose:
+                                        print("Updating fiducial visualisation settings")
 
-        except:
-            image = np.zeros(image_shape[-2:], dtype=np.int8)
+                                    self.fiducial_layer.selected_data = list(range(len(self.fiducial_layer.data)))
+                                    self.fiducial_layer.opacity = vis_opacity
+                                    self.fiducial_layer.symbol = symbol
+                                    self.fiducial_layer.size = vis_size
+                                    self.fiducial_layer.edge_width = vis_edge_width
+                                    self.fiducial_layer.edge_color = "red"
+                                    self.fiducial_layer.selected_data = []
+                                    self.fiducial_layer.refresh()
 
-        return image, pixel_size, oversampling
 
-    def picasso_render_finished(self):
 
-        self.update_filter_criterion()
-        self.update_criterion_ranges()
+                if remove_localisations:
+                    if "localisations" in layer_names:
+                        self.viewer.layers["localisations"].data = []
 
-        self.update_ui(init=False)
+                for layer in layer_names:
+                    self.viewer.layers[layer].refresh()
 
 
+    def get_localisation_centres(self, locs, mode = "localisations"):
 
-    def draw_picasso_render(self, data):
+        loc_centres = []
 
         try:
-            image, pixel_size, oversampling = data
 
-            scale = [pixel_size / oversampling, pixel_size / oversampling]
-
-            layer_names = [layer.name for layer in self.viewer.layers]
-
-            if "SMLM Render" not in layer_names:
-                self.viewer.add_image(image, name="SMLM Render", colormap="viridis", scale=scale, )
-            else:
-                self.viewer.layers["SMLM Render"].data = image
-                self.viewer.layers["SMLM Render"].scale = scale
+            for loc in locs:
+                frame = int(loc.frame)
+                if mode == "localisations":
+                    loc_centres.append([frame, loc.y, loc.x])
+                else:
+                    loc_centres.append([loc.y, loc.x])
 
         except:
             print(traceback.format_exc())
 
-    def initialise_picasso_render(self):
-
-        try:
-
-            dataset_name = self.gui.picasso_render_dataset.currentText()
-            image_channel = self.gui.picasso_render_channel.currentText()
-            blur_method = self.gui.picasso_render_blur_method.currentText()
-            min_blur_width = float(self.gui.picasso_render_min_blur.text())
-
-            if (image_channel.lower() in self.localisation_dict["localisations"][dataset_name].keys()):
-                localisation_dict = self.localisation_dict["localisations"][dataset_name][image_channel.lower()].copy()
-
-                if localisation_dict["fitted"] == True:
-                    locs = localisation_dict["localisations"]
-
-                    image_shape = list(self.dataset_dict[dataset_name][image_channel.lower()]["data"].shape)
-                    pixel_size = 1
-
-                    if blur_method == "One-Pixel-Blur":
-                        blur_method = "smooth"
-                    elif blur_method == "Global Localisation Precision":
-                        blur_method = "convolve"
-                    elif (blur_method == "Individual Localisation Precision, iso"):
-                        blur_method = "gaussian_iso"
-                    elif blur_method == "Individual Localisation Precision":
-                        blur_method = "gaussian"
-                    else:
-                        blur_method = None
-
-                    self.update_ui(init=True)
+        return loc_centres
 
-                    worker = Worker(self.render_picasso_locs, locs=locs, image_shape=image_shape,
-                        blur_method=blur_method, min_blur_width=min_blur_width, pixel_size=pixel_size, )
-                    worker.signals.result.connect(self.draw_picasso_render)
-                    worker.signals.finished.connect(self.picasso_render_finished)
-                    self.threadpool.start(worker)
-
-        except:
-            print(traceback.format_exc())
-            self.update_ui()
+    def closeEvent(self):
+        print("Closing PixSeq")
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_plot_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_plot_utils.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_segmentation_events.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_segmentation_events.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_segmentation_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_simple_analysis_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_simple_analysis_utils.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_temporal_filtering.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_temporal_filtering.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_trace_compute_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_trace_compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_tracking_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_tracking_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,22 +87,16 @@
                 n_filtered = len(filtered_locs)
 
                 n_removed = n_locs - n_filtered
 
                 if n_removed > 0:
                     print(f"Removed {n_removed} unlinked localisations")
 
-                    render_locs = {}
-
-                    for frame in np.unique(filtered_locs["frame"]):
-                        frame_locs = filtered_locs[filtered_locs["frame"] == frame].copy()
-                        render_locs[frame] = np.vstack((frame_locs.y, frame_locs.x)).T.tolist()
-
                     loc_dict["localisations"] = filtered_locs
-                    loc_dict["render_locs"] = render_locs
+
 
 
         except:
             print(traceback.format_exc())
 
 
     def tracking_finished(self):
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_transform_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_transform_utils.py`

 * *Files identical despite different names*

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_undrift_utils.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_undrift_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import traceback
 import numpy as np
+import pandas as pd
+
 from napari_pixseq.funcs.pixseq_utils_compute import Worker
 import scipy.ndimage
 import multiprocessing
 from multiprocessing import shared_memory
 from functools import partial
 import concurrent.futures
 from picasso.postprocess import undrift as picasso_undrift
@@ -51,14 +53,23 @@
     try:
 
         loc_dict = dataset_dict["loc_dict"]
         undrift_locs = loc_dict["localisations"].copy()
         picasso_info = dataset_dict["picasso_info"]
         n_frames = picasso_info[0]["Frames"]
 
+        undrift_locs = pd.DataFrame(undrift_locs)
+
+        if "dataset" in undrift_locs.columns:
+            undrift_locs = undrift_locs.drop(columns=["dataset"])
+        if "channel" in undrift_locs.columns:
+            undrift_locs = undrift_locs.drop(columns=["channel"])
+
+        undrift_locs = undrift_locs.to_records(index=False)
+
         len_segments = n_frames // segmentation
         n_pairs = int(len_segments * (len_segments - 1))/2
 
         compute_progress = {"segmentation": 0,"undrift": 0}
 
         def total_progress():
             segmentation_progress = compute_progress["segmentation"]
@@ -110,31 +121,19 @@
                     fiducial_dict = self.localisation_dict["localisations"][dataset_name][channel_name.lower()].copy()
 
                     if "drift" in channel_data.keys() and "localisations" in fiducial_dict.keys():
                         locs = fiducial_dict["localisations"]
 
                         drift = channel_data["drift"]
 
-                        render_locs = {}
-
                         for loc in locs:
-                            frame = loc.frame
                             loc.x = loc.x - drift[loc.frame][0]
                             loc.y = loc.y - drift[loc.frame][1]
 
-                            if frame not in render_locs.keys():
-                                render_locs[frame] = []
-
-                            render_locs[frame].append([loc.y, loc.x])
-
-                        localisation_centres = self.get_localisation_centres(locs)
-
                         self.localisation_dict["localisations"][dataset_name][channel_name.lower()]["localisations"] = locs
-                        self.localisation_dict["localisations"][dataset_name][channel_name.lower()]["localisation_centres"] = localisation_centres
-                        self.localisation_dict["localisations"][dataset_name][channel_name.lower()]["render_locs"] = render_locs
 
         except:
             print(traceback.format_exc())
             pass
 
     def _undrift_images_finished(self):
```

### Comparing `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_utils_compute.py` & `napari_pixseq-1.0.3/src/napari_pixseq/funcs/pixseq_utils_compute.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,170 @@
 import sys
 from multiprocessing import Process, shared_memory, Pool
 import numpy as np
 import napari
 
 class _utils_compute:
 
+    def create_shared_image_chunks(self, dataset_list = None,
+            channel_list = None, chunk_size = 100, frame_index = None):
+
+        if self.verbose:
+            print("Creating shared images")
+
+        if dataset_list is None:
+            dataset_list = list(self.dataset_dict.keys())
+        else:
+            dataset_list = [dataset for dataset in dataset_list if dataset in self.dataset_dict.keys()]
+
+        self.shared_chunks = []
+
+        for dataset_name in dataset_list:
+
+            channel_names = list(self.dataset_dict[dataset_name].keys())
+
+            if channel_list is not None:
+                channel_names = [chan for chan in channel_list if chan in channel_names]
+
+            for channel_name in channel_names:
+                if channel_name in self.dataset_dict[dataset_name].keys():
+
+                    channel_dict = self.dataset_dict[dataset_name][channel_name]
+
+                    if "data" in channel_dict.keys():
+
+                        if type(frame_index) == int:
+                            n_chunks = 1
+                            image = channel_dict["data"]
+                            n_frames = 1
+                        else:
+                            image = channel_dict.pop("data")
+                            n_frames = image.shape[0]
+                            n_chunks = int(np.ceil(n_frames / chunk_size))
+
+                        for chunk_index in range(n_chunks):
+
+                            if type(frame_index) == int:
+
+                                start_index = frame_index
+                                end_index = frame_index + 1
+
+                                chunk = image[start_index].copy()
+                                chunk = np.expand_dims(chunk, axis=0)
+
+                            else:
+                                start_index = chunk_index * chunk_size
+                                end_index = (chunk_index + 1) * chunk_size
+
+                                if end_index > n_frames:
+                                    end_index = n_frames
+
+                                chunk = image[start_index:end_index]
+
+                            shared_mem = shared_memory.SharedMemory(create=True, size=chunk.nbytes)
+                            shared_memory_name = shared_mem.name
+                            shared_chunk = np.ndarray(chunk.shape, dtype=chunk.dtype, buffer=shared_mem.buf)
+                            shared_chunk[:] = chunk[:]
+
+                            self.shared_chunks.append({"dataset": dataset_name,
+                                                       "channel": channel_name,
+                                                       "gap_label": channel_dict["gap_label"],
+                                                       "sequence_label": channel_dict["sequence_label"],
+                                                       "n_frames": n_frames,
+                                                       "shape": chunk.shape,
+                                                       "dtype": chunk.dtype,
+                                                       "start_index": start_index,
+                                                       "end_index": end_index,
+                                                       "chunk_size": chunk_size,
+                                                       "shared_mem": shared_mem,
+                                                       "shared_memory_name": shared_memory_name})
+
+    def restore_shared_image_chunks(self):
+
+        if self.verbose:
+            print("Restoring shared images")
+
+        if hasattr(self, "shared_chunks"):
+
+            if type(self.shared_chunks) == list:
+
+                dataset_list = []
+                channel_list = []
+
+                for dat in self.shared_chunks:
+                    try:
+                        dataset = dat["dataset"]
+                        channel = dat["channel"]
+                        shape = dat["shape"]
+                        dtype = dat["dtype"]
+                        start_index = dat["start_index"]
+                        shared_mem = dat["shared_mem"]
+
+                        np_array = np.ndarray(shape, dtype=dtype, buffer=shared_mem.buf).copy()
+                        shared_mem.close()
+                        shared_mem.unlink()
+
+                        image_dict = self.dataset_dict[dataset][channel]
+
+                        if "data" not in image_dict.keys():
+                            image_dict["data"] = []
+                            image_dict["chunk_idices"] = []
+
+                        if type(image_dict["data"]) == list:
+
+                            image_dict["data"].append(np_array)
+                            image_dict["chunk_idices"].append(start_index)
+
+                            dataset_list.append(dataset)
+                            channel_list.append(channel)
+
+                        # else:
+                        #     print(f"Error: {dataset} {channel} data is not a list")
+
+                    except:
+                        print(traceback.format_exc())
+                        pass
+
+                dataset_list = list(set(dataset_list))
+                channel_list = list(set(channel_list))
+
+                for dataset in dataset_list:
+                    for channel in channel_list:
+
+                        try:
+
+                            image_dict = self.dataset_dict[dataset][channel]
+
+                            if "data" in image_dict.keys():
+
+                                chunk_indices = image_dict["chunk_idices"]
+                                images = image_dict["data"]
+
+                                sorted_indices = np.argsort(chunk_indices)
+
+                                # print(f"Restoring {dataset} {channel} {len(images)} chunks")
+                                # print(f"Chunk indices: {chunk_indices}")
+                                # print(f"Sorted indices: {sorted_indices}")
+
+                                sorted_images = [images[i] for i in sorted_indices]
+                                image = np.concatenate(sorted_images, axis=0)
+
+                                image_dict["data"] = image
+                                del image_dict["chunk_idices"]
+
+                        except:
+                            pass
+
+
+
+
+
+
+
+
     def create_shared_images(self, dataset_list = None, channel_list = None):
 
         if self.verbose:
             print("Creating shared images")
 
         if dataset_list is None:
             dataset_list = list(self.dataset_dict.keys())
```

