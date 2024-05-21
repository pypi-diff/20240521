# Comparing `tmp/txm_sandbox-0.3.1.post2.tar.gz` & `tmp/txm_sandbox-0.3.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txm_sandbox-0.3.1.post2.tar", last modified: Sun May 19 13:51:50 2024, max compression
+gzip compressed data, was "txm_sandbox-0.3.1.post3.tar", last modified: Tue May 21 03:28:52 2024, max compression
```

## Comparing `txm_sandbox-0.3.1.post2.tar` & `txm_sandbox-0.3.1.post3.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.406340 txm_sandbox-0.3.1.post2/
--rw-rw-r--   0 xianghui   (501) staff       (20)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post2/LICENSE
--rw-rw-r--   0 xianghui   (501) staff       (20)      203 2024-05-09 00:28:45.000000 txm_sandbox-0.3.1.post2/MANIFEST.in
--rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-19 13:51:50.406156 txm_sandbox-0.3.1.post2/PKG-INFO
--rw-rw-r--   0 xianghui   (501) staff       (20)     1964 2024-05-09 00:35:34.000000 txm_sandbox-0.3.1.post2/README.md
--rwxrwxr-x   0 xianghui   (501) staff       (20)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post2/TXM_GUI2.ipynb
--rw-r--r--   0 xianghui   (501) staff       (20)       38 2024-05-19 13:51:50.406483 txm_sandbox-0.3.1.post2/setup.cfg
--rw-rw-r--   0 xianghui   (501) staff       (20)     1130 2024-05-19 13:51:00.000000 txm_sandbox-0.3.1.post2/setup.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.376176 txm_sandbox-0.3.1.post2/txm_sandbox/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/__init__.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.378336 txm_sandbox-0.3.1.post2/txm_sandbox/config/
--rw-rw-r--   0 xianghui   (501) staff       (20)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/config/XANES2D_GUI_config.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/config/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/config/analysis_tool_gui_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/config/io_tomo_h5_data_structure.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/config/io_xanes2D_h5_data_structure.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/config/io_xanes3D_h5_data_structure.json
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.379761 txm_sandbox-0.3.1.post2/txm_sandbox/dicts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/dicts/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/dicts/config_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/dicts/customized_struct_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/dicts/sklearn_opt_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/dicts/xanes_analysis_dict.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.380190 txm_sandbox-0.3.1.post2/txm_sandbox/external/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/external/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/external/user_io.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.387757 txm_sandbox-0.3.1.post2/txm_sandbox/gui/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/conv_data_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/gen_algn_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    79148 2024-05-12 04:56:04.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/gui_components.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/io_config_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/main_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/misc_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/tomo_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/xanes2D_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/xanes3D_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/xanes_analysis_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   203269 2024-05-18 14:45:10.000000 txm_sandbox-0.3.1.post2/txm_sandbox/gui/xanes_fitting_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.388867 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/__init__.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.390379 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      979 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      957 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      899 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)     2389 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)     1362 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.390851 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/dicts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/dicts/__init__.py
--rw-r--r--   0 xianghui   (501) staff       (20)     8853 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/dicts/data_struct_dict.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.394240 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/
--rw-rw-r--   0 xianghui   (501) staff       (20)      106 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16170 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/appl_mask_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     9799 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/convert_data_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)     3929 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/extra_io_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    32957 2024-05-14 07:59:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/tomo_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    24243 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    67248 2024-05-18 02:01:00.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.396605 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     4223 2024-05-14 05:10:46.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      650 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      599 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    15251 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     2441 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16610 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1197 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
--rw-r--r--   0 xianghui   (501) staff       (20)     2029 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
--rw-r--r--   0 xianghui   (501) staff       (20)     1533 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/txm_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.397718 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/utils/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/utils/__init__.py
--rw-r--r--   0 xianghui   (501) staff       (20)     5157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/utils/ext_io_lib.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1264 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/utils/io.py
--rw-r--r--   0 xianghui   (501) staff       (20)    10709 2024-05-16 05:38:21.000000 txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/utils/misc.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.398208 txm_sandbox-0.3.1.post2/txm_sandbox/tmp/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/tmp/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/tmp/readme.txt
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.405549 txm_sandbox-0.3.1.post2/txm_sandbox/utils/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/io.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/lineshapes.py
--rwxrwxr-x   0 xianghui   (501) staff       (20)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/misc.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/plotlib.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/reg_algs.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/tomo_recon_tools.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    42166 2024-05-18 14:44:34.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_analysis.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_image_utils.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    27376 2024-05-18 14:19:49.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_math.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_post_analysis.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    84137 2024-05-19 13:48:34.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_regtools.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_spectra_filters.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-19 13:51:50.405840 txm_sandbox-0.3.1.post2/txm_sandbox.egg-info/
--rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-19 13:51:50.000000 txm_sandbox-0.3.1.post2/txm_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 xianghui   (501) staff       (20)     3196 2024-05-19 13:51:50.000000 txm_sandbox-0.3.1.post2/txm_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-19 13:51:50.000000 txm_sandbox-0.3.1.post2/txm_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-19 13:51:50.000000 txm_sandbox-0.3.1.post2/txm_sandbox.egg-info/not-zip-safe
--rw-r--r--   0 xianghui   (501) staff       (20)      170 2024-05-19 13:51:50.000000 txm_sandbox-0.3.1.post2/txm_sandbox.egg-info/requires.txt
--rw-r--r--   0 xianghui   (501) staff       (20)       12 2024-05-19 13:51:50.000000 txm_sandbox-0.3.1.post2/txm_sandbox.egg-info/top_level.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.083162 txm_sandbox-0.3.1.post3/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post3/LICENSE
+-rw-rw-r--   0 xianghui   (501) staff       (20)      203 2024-05-09 00:28:45.000000 txm_sandbox-0.3.1.post3/MANIFEST.in
+-rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-21 03:28:52.082971 txm_sandbox-0.3.1.post3/PKG-INFO
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1964 2024-05-09 00:35:34.000000 txm_sandbox-0.3.1.post3/README.md
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post3/TXM_GUI2.ipynb
+-rw-r--r--   0 xianghui   (501) staff       (20)       38 2024-05-21 03:28:52.083207 txm_sandbox-0.3.1.post3/setup.cfg
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1130 2024-05-21 03:27:41.000000 txm_sandbox-0.3.1.post3/setup.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.052853 txm_sandbox-0.3.1.post3/txm_sandbox/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.055412 txm_sandbox-0.3.1.post3/txm_sandbox/config/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/config/XANES2D_GUI_config.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/config/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/config/analysis_tool_gui_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/config/io_tomo_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/config/io_xanes2D_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/config/io_xanes3D_h5_data_structure.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.057003 txm_sandbox-0.3.1.post3/txm_sandbox/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/dicts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/dicts/config_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/dicts/customized_struct_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/dicts/sklearn_opt_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/dicts/xanes_analysis_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.057513 txm_sandbox-0.3.1.post3/txm_sandbox/external/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/external/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/external/user_io.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.065475 txm_sandbox-0.3.1.post3/txm_sandbox/gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/conv_data_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/gen_algn_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    79148 2024-05-12 04:56:04.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/gui_components.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/io_config_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/main_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/misc_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/tomo_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/xanes2D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/xanes3D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/xanes_analysis_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   203269 2024-05-18 14:45:10.000000 txm_sandbox-0.3.1.post3/txm_sandbox/gui/xanes_fitting_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.067451 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.069660 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      979 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      957 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      899 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2389 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1362 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.070049 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/dicts/__init__.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     8853 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/dicts/data_struct_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.073085 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      106 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16170 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/appl_mask_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     9799 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/convert_data_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     3929 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/extra_io_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)      196 2024-05-19 15:27:59.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/lcf_cfg_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    29844 2024-05-19 22:28:29.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/tomo_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    24249 2024-05-21 03:24:11.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    67248 2024-05-18 02:01:00.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.074949 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     4223 2024-05-14 05:10:46.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      650 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      599 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15251 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2441 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16610 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1197 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     2029 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     1533 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/txm_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.076198 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/utils/__init__.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     6339 2024-05-19 22:44:39.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/utils/ext_io_lib.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1264 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/utils/io.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    10709 2024-05-16 05:38:21.000000 txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/utils/misc.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.076773 txm_sandbox-0.3.1.post3/txm_sandbox/tmp/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/tmp/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/tmp/readme.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.082422 txm_sandbox-0.3.1.post3/txm_sandbox/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/io.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/lineshapes.py
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/misc.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/plotlib.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/reg_algs.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/tomo_recon_tools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    42166 2024-05-18 14:44:34.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_image_utils.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    27376 2024-05-18 14:19:49.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_math.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_post_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    84137 2024-05-19 13:48:34.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_regtools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_spectra_filters.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 03:28:52.082725 txm_sandbox-0.3.1.post3/txm_sandbox.egg-info/
+-rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-21 03:28:52.000000 txm_sandbox-0.3.1.post3/txm_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 xianghui   (501) staff       (20)     3239 2024-05-21 03:28:52.000000 txm_sandbox-0.3.1.post3/txm_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-21 03:28:52.000000 txm_sandbox-0.3.1.post3/txm_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-21 03:28:52.000000 txm_sandbox-0.3.1.post3/txm_sandbox.egg-info/not-zip-safe
+-rw-r--r--   0 xianghui   (501) staff       (20)      170 2024-05-21 03:28:52.000000 txm_sandbox-0.3.1.post3/txm_sandbox.egg-info/requires.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)       12 2024-05-21 03:28:52.000000 txm_sandbox-0.3.1.post3/txm_sandbox.egg-info/top_level.txt
```

### Comparing `txm_sandbox-0.3.1.post2/LICENSE` & `txm_sandbox-0.3.1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/PKG-INFO` & `txm_sandbox-0.3.1.post3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.1.post2
+Version: 0.3.1.post3
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.1.post2/README.md` & `txm_sandbox-0.3.1.post3/README.md`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/TXM_GUI2.ipynb` & `txm_sandbox-0.3.1.post3/TXM_GUI2.ipynb`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/setup.py` & `txm_sandbox-0.3.1.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: xiao
 """
 
 from setuptools import setup, find_packages
 
 setup(name='txm_sandbox',
-      version='0.3.1.post2',
+      version='0.3.1.post3',
       description='Integrated Spectro-Imaging Analysis Toolbox',
       url='https://github.com/xianghuix/TXM_Sandbox',
       author='Xianghui Xiao',
       author_email='xianghuix@gmail.com',
       license='MIT',
       packages=find_packages(),
       install_requires=[
```

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/config/XANES2D_GUI_config.json` & `txm_sandbox-0.3.1.post3/txm_sandbox/config/XANES2D_GUI_config.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/config/io_xanes3D_h5_data_structure.json` & `txm_sandbox-0.3.1.post3/txm_sandbox/config/io_xanes3D_h5_data_structure.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/dicts/config_dict.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/dicts/config_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/dicts/customized_struct_dict.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/dicts/customized_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/dicts/sklearn_opt_dict.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/dicts/sklearn_opt_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/dicts/xanes_analysis_dict.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/dicts/xanes_analysis_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/conv_data_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/conv_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/gen_algn_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/gen_algn_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/gui_components.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/gui_components.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/io_config_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/io_config_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/main_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/misc_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/misc_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/tomo_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/xanes2D_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/xanes2D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/xanes3D_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/xanes3D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/xanes_analysis_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/xanes_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/gui/xanes_fitting_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/gui/xanes_fitting_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/dicts/data_struct_dict.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/dicts/data_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/appl_mask_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/appl_mask_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/convert_data_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/convert_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/extra_io_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/extra_io_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/tomo_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/tomo_gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 import glob
 import h5py
 import datetime
 from pathlib import Path
 import matplotlib.pyplot as plt
 from magicgui import widgets
 
-# from PyQt5.QtWidgets import QApplication
-# from PyQt5 import QtWidgets, QtCore
-from qtpy import QtWidgets, QtCore
-from magicgui.widgets import request_values
-from magicgui import magicgui
+from qtpy import QtCore
 
 from ...utils.io import data_reader, tomo_h5_reader
 from ...utils.tomo_recon_tools import rm_redundant
 from ...gui.gui_components import (
     check_file_availability,
 )
 from ..utils.misc import (
@@ -75,16 +71,14 @@
         self._scn_fn = None
         self._wedge_data_avg = 0
         self._trial_cen_rec_done = False
         self._multi_trial_cen_rec_done = False
         self._cen = None
         self._wedge_autodet_fig = None
         self._viewers = ["proj_prev", "data_center", "tomo_viewer"]
-        # self.extra_io_signal = QtCore.Signal()
-        # self.extra_io_signal.connect(self._show_io_win)
 
         self.label0 = widgets.Label(
             value="-------------------     Tomo Recon    --------------------",
         )
         self.label1 = widgets.Label(
             name="Step 1",
             value="--------------------     Trial Cen    --------------------",
@@ -176,58 +170,14 @@
                 self.trial_cen_done,
                 self.vol_rec,
                 self.close_file,
                 self.op_status,
             ]
         )
 
-    # def __io_win(self, dtype="APS_tomo"):
-    #     self._io_win = QtWidgets.QDialog()
-    #     self._io_win.setWindowTitle("extra data info")
-
-    #     layout = QtWidgets.QVBoxLayout()
-    #     label = QtWidgets.QLabel("This is a pop-up window")
-    #     file = QtWidgets.QFileDialog(
-    #         caption="pick a tomo file", directory=self._io_win_dir, filter="*.h5"
-    #     )
-    #     sel_file = QtWidgets.QPushButton("Click me")
-    #     # sel_file.clicked.connect()
-    #     layout.addWidget(label)
-    #     # layout.addWidget(file)
-    #     layout.addWidget(sel_file)
-    #     self._io_win.setLayout(layout)
-
-    #     # Show the pop-up window as a modal dialog
-    #     self._io_win.exec_()
-
-    # def _show_io_win(self, dtype="APS_tomo"):
-    #     # @magicgui(main_window=True,
-    #     #           )
-    #     # def create_io_win()
-    #     vals = request_values(
-    #         name={
-    #             "annotation": Path,
-    #             "label": "pick a tomo file",
-    #             "options": {"mode": "r", "filter": "tomo data file (*.h5)"},
-    #         },
-    #         title="pick a tomo file from 3D XANES data series",
-    #     )
-    #     print(repr(vals))
-
-    # def create_io_win(dtype=dtype):
-    #     win = extra_io_win(self, dtype=dtype)
-    #     # win.show()
-    #     win.show(run=True)
-
-    # create_io_win(dtype=dtype)
-
-    # app = QtWidgets.QApplication.instance() or QtWidgets.QApplication(sys.argv)
-    # QtCore.QTimer.singleShot(0, create_io_win)
-    # app.exec_()
-
     @disp_progress_info("data directory info read")
     def __check_avail_data(self):
         global _TOMO_TRL_SCN_ID_CHOICES
         ids = check_file_availability(
             str(self.top_dir.value),
             scan_id=None,
             signature=self._tomo_cfg["tomo_raw_fn_template"],
@@ -381,50 +331,23 @@
             self._tomo_cfg = FLY_CFG["io_data_structure_tomo"]
             self.top_dir.enabled = True
         elif self.file_type.value == "APS_tomo":
             _cfg = deepcopy(APS_TXM_CFG)
             name = show_io_win(dtype="APS_tomo")
             if name is not None:
                 fn_tplt = name["name"].stem.rsplit("_", maxsplit=1)[0]
-                # tem = (
-                #     _tomo_cfg["io_data_structure_tomo"]["tomo_raw_fn_template"]
-                #     .replace("{0}", fn_tplt)
-                #     .replace("{1}", "{0}")
-                # )
-                # _tomo_cfg["io_data_structure_tomo"]["tomo_raw_fn_template"] = tem
-                # _tomo_cfg["io_data_structure_xanes2D"]["xanes2D_raw_fn_template"] = tem
-                # _tomo_cfg["io_data_structure_xanes3D"]["tomo_raw_fn_template"] = tem
-                # _tomo_cfg["io_data_structure_xanes3D"]["xanes3D_recon_dir_template"] = (
-                #     "recon_" + str(Path(tem).stem)
-                # )
-                # _tomo_cfg["io_data_structure_xanes3D"]["xanes3D_recon_fn_template"] = (
-                #     "recon_" + str(Path(tem).stem) + "_{1}.tiff"
-                # )
-                # self._tomo_cfg = _tomo_cfg
                 self._tomo_cfg = mk_aps_cfg(fn_tplt, _cfg, dtype="APS 3D XANES")[
                     "io_data_structure_tomo"
                 ]
                 print(f"{self._tomo_cfg=}")
                 self.__reset_widgets()
                 self.top_dir.value = name["name"].parent
                 self._trial_cen_dir = self.top_dir.value / "data_center"
                 self.top_dir.enabled = False
 
-            # self._tomo_cfg
-            # # app = QApplication(sys.argv)
-            # win = extra_io_win(self, dtype="APS_tomo")
-
-            # app = QtWidgets.QApplication.instance()
-            # if app is None:
-            #     app = QtWidgets.QApplication(sys.argv)
-            # # win.show()
-            # QtCore.QMetaObject.invokeMethod(win, "show", QtCore.Qt.QueuedConnection)
-            # app.exec_()
-            # # win.show(run=True)
-
         self.__check_avail_data()
         self.__comp_scn_fn()
         self.__set_trial_cen_rec_widgets()
         self.__set_vol_rec_widgets()
 
     def _sel_top_dir(self):
         self.__reset_widgets()
```

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/xanes_fit_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/xanes_fit_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,15 @@
         self.sli.value = 0
         self.E.value = 0
         self.spec_in_roi.value = False
         self.roi_cen_x.value = self.roi_cen_x.min
         self.roi_cen_y.value = self.roi_cen_y.min
         self.element.value = ""
         self.analysis_type = "wl"
-        self.edge_eng = ""
+        self.edge_eng.value = ""
         self.wl_s.value = ""
         self.wl_e.value = ""
         self.edge_s.value = ""
         self.edge_e.value = ""
         self.downsample_factor.value = 1
         global _XANES_FIT_SAVE_ITEMS_CHOICES
         _XANES_FIT_SAVE_ITEMS_CHOICES = []
```

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/xanes_reg_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/xanes_reg_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/guis/xanes_vis_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/guis/xanes_vis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/txm_gui.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/txm_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/utils/ext_io_lib.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/utils/ext_io_lib.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,14 +41,57 @@
             .replace("{0}", fn_tplt)
             .replace("{1}", "{0}")
         )
         cfg["io_data_structure_xanes2D"]["xanes2D_raw_fn_template"] = tem
     return cfg
 
 
+class lcf_cfg_win:
+    def __init__(self):
+        self._ref_file_dlg = widgets.FileEdit(
+            mode="r",
+            filter="*.json",
+            name="ref file",
+        )
+        self._add_ref = widgets.PushButton(text="add", enabled=False)
+        self._eng_off
+        self.gui_layout = widgets.VBox(
+            widgets=[
+                self.label0,
+                self.label1,
+                self.file_type,
+                self.top_dir,
+                self.find_multi_cen,
+                self.scan_id,
+                self.proj_prev,
+                self.cen_sch_s,
+                self.ref_sli,
+                self.is_wedge,
+                self.wedge_thsh,
+                self.phase_retrieval,
+                self.beta_gamma_ratio,
+                self.trial_cen_rec,
+                self.label2,
+                self.cen,
+                self.pick_cen,
+                self.trial_cen_done,
+                self.vol_rec,
+                self.close_file,
+                self.op_status,
+            ]
+        )
+
+        self.gui = widgets.Dialog(
+            widgets=[
+                widgets.VBox(),
+            ]
+        )
+        self.gui.show(run=True)
+
+
 # from magicgui.widgets import request_values
 
 # vals = request_values(
 #     age=int,
 #     name={"annotation": str, "label": "Enter your name:"},
 #     title="Hi, who are you?",
 # )
```

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/utils/io.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/napari_gui/utils/misc.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/napari_gui/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/io.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/lineshapes.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/lineshapes.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/misc.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/plotlib.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/plotlib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/reg_algs.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/reg_algs.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/tomo_recon_tools.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/tomo_recon_tools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_analysis.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_image_utils.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_image_utils.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_math.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_math.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_post_analysis.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_post_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_regtools.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_regtools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox/utils/xanes_spectra_filters.py` & `txm_sandbox-0.3.1.post3/txm_sandbox/utils/xanes_spectra_filters.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox.egg-info/PKG-INFO` & `txm_sandbox-0.3.1.post3/txm_sandbox.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.1.post2
+Version: 0.3.1.post3
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.1.post2/txm_sandbox.egg-info/SOURCES.txt` & `txm_sandbox-0.3.1.post3/txm_sandbox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
 txm_sandbox/napari_gui/dicts/__init__.py
 txm_sandbox/napari_gui/dicts/data_struct_dict.py
 txm_sandbox/napari_gui/guis/__init__.py
 txm_sandbox/napari_gui/guis/appl_mask_gui.py
 txm_sandbox/napari_gui/guis/convert_data_gui.py
 txm_sandbox/napari_gui/guis/extra_io_gui.py
+txm_sandbox/napari_gui/guis/lcf_cfg_gui.py
 txm_sandbox/napari_gui/guis/tomo_gui.py
 txm_sandbox/napari_gui/guis/xanes_fit_gui.py
 txm_sandbox/napari_gui/guis/xanes_reg_gui.py
 txm_sandbox/napari_gui/guis/xanes_vis_gui.py
 txm_sandbox/napari_gui/scripts/__init__.py
 txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py
 txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
```

