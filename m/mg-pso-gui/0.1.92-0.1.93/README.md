# Comparing `tmp/mg-pso-gui-0.1.92.tar.gz` & `tmp/mg-pso-gui-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mg-pso-gui-0.1.92.tar", last modified: Tue May 21 09:11:18 2024, max compression
+gzip compressed data, was "mg-pso-gui-0.1.93.tar", last modified: Tue May 21 09:12:57 2024, max compression
```

## Comparing `mg-pso-gui-0.1.92.tar` & `mg-pso-gui-0.1.93.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.457692 mg-pso-gui-0.1.92/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 09:11:18.456720 mg-pso-gui-0.1.92/PKG-INFO
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.456185 mg-pso-gui-0.1.92/mg_pso_gui.egg-info/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 09:11:18.000000 mg-pso-gui-0.1.92/mg_pso_gui.egg-info/PKG-INFO
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1871 2024-05-21 09:11:18.000000 mg-pso-gui-0.1.92/mg_pso_gui.egg-info/SOURCES.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-05-21 09:11:18.000000 mg-pso-gui-0.1.92/mg_pso_gui.egg-info/dependency_links.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-05-21 09:11:18.000000 mg-pso-gui-0.1.92/mg_pso_gui.egg-info/entry_points.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-05-21 09:11:18.000000 mg-pso-gui-0.1.92/mg_pso_gui.egg-info/requires.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-05-21 09:11:18.000000 mg-pso-gui-0.1.92/mg_pso_gui.egg-info/top_level.txt
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.430585 mg-pso-gui-0.1.92/mgpsogui/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.92/mgpsogui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.432251 mg-pso-gui-0.1.92/mgpsogui/gui/
--rwxr--r--   0 robertcordingly   (501) staff       (20)    24173 2024-05-21 09:11:11.000000 mg-pso-gui-0.1.92/mgpsogui/gui/HomePage.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12527 2024-05-21 08:47:30.000000 mg-pso-gui-0.1.92/mgpsogui/gui/OptionManager.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.433222 mg-pso-gui-0.1.92/mgpsogui/gui/PlatformTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.92/mgpsogui/gui/PlatformTab/PlatformTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.92/mgpsogui/gui/PlatformTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.434011 mg-pso-gui-0.1.92/mgpsogui/gui/RunTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1839 2024-03-20 19:57:02.000000 mg-pso-gui-0.1.92/mgpsogui/gui/RunTab/RunTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.92/mgpsogui/gui/RunTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.439184 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/BoundsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/CalibrationParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/FunctionsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/ListParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1784 2024-04-10 21:01:22.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/OptimalParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2443 2024-05-21 09:01:39.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/SetupTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/StaticParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     5892 2024-05-21 09:06:58.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/StepView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.440751 mg-pso-gui-0.1.92/mgpsogui/gui/VisualizeTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    13322 2024-05-15 21:08:56.000000 mg-pso-gui-0.1.92/mgpsogui/gui/VisualizeTab/SideBar.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3477 2024-04-10 18:55:43.000000 mg-pso-gui-0.1.92/mgpsogui/gui/VisualizeTab/VisualizeTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.92/mgpsogui/gui/VisualizeTab/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.92/mgpsogui/gui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.447693 mg-pso-gui-0.1.92/mgpsogui/gui/images/
--rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/IGOW 4 Logo.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/collapse.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/down.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/expand.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/play.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/refresh.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/refresh_hd.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/stop.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3642 2024-03-20 06:12:19.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/test.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/trash.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.92/mgpsogui/gui/images/up.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.92/mgpsogui/mgpsogui.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.92/mgpsogui/start.yaml
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.449631 mg-pso-gui-0.1.92/mgpsogui/util/
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.450552 mg-pso-gui-0.1.92/mgpsogui/util/CTkToolTip/
--rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.92/mgpsogui/util/CTkToolTip/__init__.py
--rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.92/mgpsogui/util/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    15076 2024-04-24 19:47:23.000000 mg-pso-gui-0.1.92/mgpsogui/util/GraphGenerator.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3482 2024-05-01 20:32:28.000000 mg-pso-gui-0.1.92/mgpsogui/util/PSORunner.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.92/mgpsogui/util/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.451458 mg-pso-gui-0.1.92/mgpsogui/util/recosu/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.92/mgpsogui/util/recosu/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.452872 mg-pso-gui-0.1.92/mgpsogui/util/recosu/pso/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.92/mgpsogui/util/recosu/pso/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2721 2024-03-20 06:01:30.000000 mg-pso-gui-0.1.92/mgpsogui/util/recosu/pso/csip_access.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12590 2024-05-01 20:39:10.000000 mg-pso-gui-0.1.92/mgpsogui/util/recosu/pso/pso.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.454778 mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:11:18.455755 mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/plot/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/plot/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/plot/cost_steps.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/trace_writer.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/utils.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-05-21 09:11:18.457854 mg-pso-gui-0.1.92/setup.cfg
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1526 2024-05-21 09:11:16.000000 mg-pso-gui-0.1.92/setup.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.357364 mg-pso-gui-0.1.93/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 09:12:57.356458 mg-pso-gui-0.1.93/PKG-INFO
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.355757 mg-pso-gui-0.1.93/mg_pso_gui.egg-info/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 09:12:57.000000 mg-pso-gui-0.1.93/mg_pso_gui.egg-info/PKG-INFO
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1871 2024-05-21 09:12:57.000000 mg-pso-gui-0.1.93/mg_pso_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-05-21 09:12:57.000000 mg-pso-gui-0.1.93/mg_pso_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-05-21 09:12:57.000000 mg-pso-gui-0.1.93/mg_pso_gui.egg-info/entry_points.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-05-21 09:12:57.000000 mg-pso-gui-0.1.93/mg_pso_gui.egg-info/requires.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-05-21 09:12:57.000000 mg-pso-gui-0.1.93/mg_pso_gui.egg-info/top_level.txt
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.329524 mg-pso-gui-0.1.93/mgpsogui/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.93/mgpsogui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.331021 mg-pso-gui-0.1.93/mgpsogui/gui/
+-rwxr--r--   0 robertcordingly   (501) staff       (20)    24173 2024-05-21 09:11:11.000000 mg-pso-gui-0.1.93/mgpsogui/gui/HomePage.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12527 2024-05-21 08:47:30.000000 mg-pso-gui-0.1.93/mgpsogui/gui/OptionManager.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.331610 mg-pso-gui-0.1.93/mgpsogui/gui/PlatformTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.93/mgpsogui/gui/PlatformTab/PlatformTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.93/mgpsogui/gui/PlatformTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.332332 mg-pso-gui-0.1.93/mgpsogui/gui/RunTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1839 2024-03-20 19:57:02.000000 mg-pso-gui-0.1.93/mgpsogui/gui/RunTab/RunTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.93/mgpsogui/gui/RunTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.337130 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/BoundsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/CalibrationParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/FunctionsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/ListParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1784 2024-04-10 21:01:22.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/OptimalParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2443 2024-05-21 09:01:39.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/SetupTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/StaticParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     5937 2024-05-21 09:12:51.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/StepView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.338506 mg-pso-gui-0.1.93/mgpsogui/gui/VisualizeTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    13322 2024-05-15 21:08:56.000000 mg-pso-gui-0.1.93/mgpsogui/gui/VisualizeTab/SideBar.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3477 2024-04-10 18:55:43.000000 mg-pso-gui-0.1.93/mgpsogui/gui/VisualizeTab/VisualizeTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.93/mgpsogui/gui/VisualizeTab/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.93/mgpsogui/gui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.346719 mg-pso-gui-0.1.93/mgpsogui/gui/images/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/IGOW 4 Logo.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/collapse.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/down.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/expand.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/play.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/refresh.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/refresh_hd.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/stop.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3642 2024-03-20 06:12:19.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/test.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/trash.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.93/mgpsogui/gui/images/up.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.93/mgpsogui/mgpsogui.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.93/mgpsogui/start.yaml
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.348373 mg-pso-gui-0.1.93/mgpsogui/util/
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.349321 mg-pso-gui-0.1.93/mgpsogui/util/CTkToolTip/
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.93/mgpsogui/util/CTkToolTip/__init__.py
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.93/mgpsogui/util/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    15076 2024-04-24 19:47:23.000000 mg-pso-gui-0.1.93/mgpsogui/util/GraphGenerator.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3482 2024-05-01 20:32:28.000000 mg-pso-gui-0.1.93/mgpsogui/util/PSORunner.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.93/mgpsogui/util/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.349969 mg-pso-gui-0.1.93/mgpsogui/util/recosu/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.93/mgpsogui/util/recosu/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.352071 mg-pso-gui-0.1.93/mgpsogui/util/recosu/pso/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.93/mgpsogui/util/recosu/pso/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2721 2024-03-20 06:01:30.000000 mg-pso-gui-0.1.93/mgpsogui/util/recosu/pso/csip_access.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12590 2024-05-01 20:39:10.000000 mg-pso-gui-0.1.93/mgpsogui/util/recosu/pso/pso.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.354021 mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:12:57.355195 mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/plot/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/plot/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/plot/cost_steps.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/trace_writer.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/utils.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-05-21 09:12:57.357532 mg-pso-gui-0.1.93/setup.cfg
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1526 2024-05-21 09:12:54.000000 mg-pso-gui-0.1.93/setup.py
```

### Comparing `mg-pso-gui-0.1.92/PKG-INFO` & `mg-pso-gui-0.1.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.92
+Version: 0.1.93
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.92/mg_pso_gui.egg-info/PKG-INFO` & `mg-pso-gui-0.1.93/mg_pso_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.92
+Version: 0.1.93
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.92/mg_pso_gui.egg-info/SOURCES.txt` & `mg-pso-gui-0.1.93/mg_pso_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/HomePage.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/HomePage.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/OptionManager.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/OptionManager.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/PlatformTab/PlatformTab.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/PlatformTab/PlatformTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/RunTab/RunTab.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/RunTab/RunTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/BoundsEditorWindow.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/BoundsEditorWindow.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/BoundsList.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/BoundsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/CalibrationParametersView.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/CalibrationParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/FunctionsList.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/FunctionsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/ListParametersView.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/ListParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/OptimalParameterView.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/OptimalParameterView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/SetupTab.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/SetupTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/StaticParameterView.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/StaticParameterView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/SetupTab/StepView.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/SetupTab/StepView.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,28 +82,29 @@
             expand_func = lambda index=index: (self.clear(), self.option_manager.toggle_step_open(index), self.render())
             up_func = lambda index=index: (self.clear(), self.option_manager.move_step_up(index), self.render())
             down_func = lambda index=index: (self.clear(), self.option_manager.move_step_down(index), self.render())
             remove_func = lambda index=index: (self.clear(), self.option_manager.remove_step(index), self.render())
             
             #CTkLabel(self.containerFrame, text="Step:").grid(row=row, column=0, padx=10, pady=5, sticky="nsew")
             
-            button_container = CTkFrame(self.containerFrame, width=200)
-            button_container.grid(row=row, column=1, sticky="nse", padx=(10, 10), pady=(10, 10))
-            button_container.grid_rowconfigure(0, weight=1)
-            button_container.grid_columnconfigure(0, weight=1)
-            
-            CTkEntry(self.containerFrame, textvariable=step['name'], width=500).grid(row=row, column=0, padx=(20, 20), pady=(20, 20), sticky="nsw")
-            #CTkLabel(self.containerFrame, textvariable=step['message']).grid(row=row, column=1, padx=(20, 20), pady=(20, 20), sticky="nsew")
             if (self.mode == "PSO"):
+                button_container = CTkFrame(self.containerFrame, width=200)
+                button_container.grid(row=row, column=1, sticky="nse", padx=(10, 10), pady=(10, 10))
+                button_container.grid_rowconfigure(0, weight=1)
+                button_container.grid_columnconfigure(0, weight=1)
+                
+                CTkEntry(self.containerFrame, textvariable=step['name'], width=500).grid(row=row, column=0, padx=(20, 20), pady=(20, 20), sticky="nsw")
+                #CTkLabel(self.containerFrame, textvariable=step['message']).grid(row=row, column=1, padx=(20, 20), pady=(20, 20), sticky="nsew")
+            
                 CTkButton(button_container, width=30, text=None, image=expand_image if not step['open'] else collapse_image, command=expand_func).grid(row=0, column=0, padx=(10, 10), pady=(10, 10), sticky="nsew")
                 CTkButton(button_container, width=30, text=None, image=up_image, state="disabled" if index==0 else "normal", fg_color="gray" if index==0 else None, command=up_func).grid(row=0, column=1, padx=(10, 10), pady=(10, 10), sticky="nsew")
                 CTkButton(button_container, width=30, text=None, image=down_image, state="disabled" if index==(len(self.steps)-1) else "normal", fg_color="gray" if index==(len(self.steps)-1) else None, command=down_func).grid(row=0, column=2, padx=(10, 10), pady=(10, 10), sticky="nsew")
                 CTkButton(button_container, width=30, text=None, image=trash_image, command=remove_func).grid(row=0, column=3, padx=(10, 10), pady=(10, 10), sticky="nsew")
 
-            row += 1
+                row += 1
 
             if step['open'] or self.mode == "Halton":
                 bounds = BoundsList.BoundsList(
                     self.containerFrame, option_manager=self.option_manager, step_index=index)
                 bounds.grid(row=row, column=0, padx=(10, 10),
                             pady=(10, 10), sticky="nsew")
                 bounds.grid_columnconfigure(0, weight=1)
```

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/VisualizeTab/SideBar.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/VisualizeTab/SideBar.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/VisualizeTab/VisualizeTab.py` & `mg-pso-gui-0.1.93/mgpsogui/gui/VisualizeTab/VisualizeTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/IGOW 4 Logo.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/IGOW 4 Logo.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/collapse.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/collapse.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/down.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/down.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/expand.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/expand.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/play.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/play.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/refresh.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/refresh.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/refresh_hd.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/refresh_hd.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/stop.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/stop.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/test.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/test.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/trash.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/trash.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/gui/images/up.png` & `mg-pso-gui-0.1.93/mgpsogui/gui/images/up.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/start.yaml` & `mg-pso-gui-0.1.93/mgpsogui/start.yaml`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/util/CTkToolTip/ctk_tooltip.py` & `mg-pso-gui-0.1.93/mgpsogui/util/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/util/GraphGenerator.py` & `mg-pso-gui-0.1.93/mgpsogui/util/GraphGenerator.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/util/PSORunner.py` & `mg-pso-gui-0.1.93/mgpsogui/util/PSORunner.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/util/recosu/pso/csip_access.py` & `mg-pso-gui-0.1.93/mgpsogui/util/recosu/pso/csip_access.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/util/recosu/pso/pso.py` & `mg-pso-gui-0.1.93/mgpsogui/util/recosu/pso/pso.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/plot/cost_steps.py` & `mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/plot/cost_steps.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/trace_writer.py` & `mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/trace_writer.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/mgpsogui/util/recosu/utils/utils.py` & `mg-pso-gui-0.1.93/mgpsogui/util/recosu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.92/setup.py` & `mg-pso-gui-0.1.93/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.92'
+VERSION = '0.1.93'
 DESCRIPTION = 'GUI for MG-PSO'
 LONG_DESCRIPTION = open('../README.md').read()
 
 # Setting up
 setup(
     name="mg-pso-gui",
     version=VERSION,
```

