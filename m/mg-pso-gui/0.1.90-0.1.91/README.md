# Comparing `tmp/mg-pso-gui-0.1.90.tar.gz` & `tmp/mg-pso-gui-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mg-pso-gui-0.1.90.tar", last modified: Tue May 21 09:07:42 2024, max compression
+gzip compressed data, was "mg-pso-gui-0.1.91.tar", last modified: Tue May 21 09:10:14 2024, max compression
```

## Comparing `mg-pso-gui-0.1.90.tar` & `mg-pso-gui-0.1.91.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.710602 mg-pso-gui-0.1.90/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 09:07:42.710014 mg-pso-gui-0.1.90/PKG-INFO
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.709398 mg-pso-gui-0.1.90/mg_pso_gui.egg-info/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 09:07:42.000000 mg-pso-gui-0.1.90/mg_pso_gui.egg-info/PKG-INFO
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1871 2024-05-21 09:07:42.000000 mg-pso-gui-0.1.90/mg_pso_gui.egg-info/SOURCES.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-05-21 09:07:42.000000 mg-pso-gui-0.1.90/mg_pso_gui.egg-info/dependency_links.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-05-21 09:07:42.000000 mg-pso-gui-0.1.90/mg_pso_gui.egg-info/entry_points.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-05-21 09:07:42.000000 mg-pso-gui-0.1.90/mg_pso_gui.egg-info/requires.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-05-21 09:07:42.000000 mg-pso-gui-0.1.90/mg_pso_gui.egg-info/top_level.txt
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.686394 mg-pso-gui-0.1.90/mgpsogui/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.90/mgpsogui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.688395 mg-pso-gui-0.1.90/mgpsogui/gui/
--rwxr--r--   0 robertcordingly   (501) staff       (20)    24070 2024-05-21 09:07:37.000000 mg-pso-gui-0.1.90/mgpsogui/gui/HomePage.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12527 2024-05-21 08:47:30.000000 mg-pso-gui-0.1.90/mgpsogui/gui/OptionManager.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.689294 mg-pso-gui-0.1.90/mgpsogui/gui/PlatformTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.90/mgpsogui/gui/PlatformTab/PlatformTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.90/mgpsogui/gui/PlatformTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.690225 mg-pso-gui-0.1.90/mgpsogui/gui/RunTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1839 2024-03-20 19:57:02.000000 mg-pso-gui-0.1.90/mgpsogui/gui/RunTab/RunTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.90/mgpsogui/gui/RunTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.694750 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/BoundsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/CalibrationParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/FunctionsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/ListParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1784 2024-04-10 21:01:22.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/OptimalParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2443 2024-05-21 09:01:39.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/SetupTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/StaticParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     5892 2024-05-21 09:06:58.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/StepView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.695949 mg-pso-gui-0.1.90/mgpsogui/gui/VisualizeTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    13322 2024-05-15 21:08:56.000000 mg-pso-gui-0.1.90/mgpsogui/gui/VisualizeTab/SideBar.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3477 2024-04-10 18:55:43.000000 mg-pso-gui-0.1.90/mgpsogui/gui/VisualizeTab/VisualizeTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.90/mgpsogui/gui/VisualizeTab/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.90/mgpsogui/gui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.701792 mg-pso-gui-0.1.90/mgpsogui/gui/images/
--rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/IGOW 4 Logo.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/collapse.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/down.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/expand.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/play.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/refresh.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/refresh_hd.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/stop.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3642 2024-03-20 06:12:19.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/test.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/trash.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.90/mgpsogui/gui/images/up.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.90/mgpsogui/mgpsogui.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.90/mgpsogui/start.yaml
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.703394 mg-pso-gui-0.1.90/mgpsogui/util/
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.704029 mg-pso-gui-0.1.90/mgpsogui/util/CTkToolTip/
--rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.90/mgpsogui/util/CTkToolTip/__init__.py
--rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.90/mgpsogui/util/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    15076 2024-04-24 19:47:23.000000 mg-pso-gui-0.1.90/mgpsogui/util/GraphGenerator.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3482 2024-05-01 20:32:28.000000 mg-pso-gui-0.1.90/mgpsogui/util/PSORunner.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.90/mgpsogui/util/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.704539 mg-pso-gui-0.1.90/mgpsogui/util/recosu/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.90/mgpsogui/util/recosu/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.706416 mg-pso-gui-0.1.90/mgpsogui/util/recosu/pso/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.90/mgpsogui/util/recosu/pso/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2721 2024-03-20 06:01:30.000000 mg-pso-gui-0.1.90/mgpsogui/util/recosu/pso/csip_access.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12590 2024-05-01 20:39:10.000000 mg-pso-gui-0.1.90/mgpsogui/util/recosu/pso/pso.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.707812 mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:07:42.708913 mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/plot/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/plot/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/plot/cost_steps.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/trace_writer.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/utils.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-05-21 09:07:42.710716 mg-pso-gui-0.1.90/setup.cfg
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1526 2024-05-21 09:07:39.000000 mg-pso-gui-0.1.90/setup.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.589532 mg-pso-gui-0.1.91/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 09:10:14.588742 mg-pso-gui-0.1.91/PKG-INFO
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.587813 mg-pso-gui-0.1.91/mg_pso_gui.egg-info/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 09:10:14.000000 mg-pso-gui-0.1.91/mg_pso_gui.egg-info/PKG-INFO
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1871 2024-05-21 09:10:14.000000 mg-pso-gui-0.1.91/mg_pso_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-05-21 09:10:14.000000 mg-pso-gui-0.1.91/mg_pso_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-05-21 09:10:14.000000 mg-pso-gui-0.1.91/mg_pso_gui.egg-info/entry_points.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-05-21 09:10:14.000000 mg-pso-gui-0.1.91/mg_pso_gui.egg-info/requires.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-05-21 09:10:14.000000 mg-pso-gui-0.1.91/mg_pso_gui.egg-info/top_level.txt
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.560575 mg-pso-gui-0.1.91/mgpsogui/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.91/mgpsogui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.561997 mg-pso-gui-0.1.91/mgpsogui/gui/
+-rwxr--r--   0 robertcordingly   (501) staff       (20)    24166 2024-05-21 09:09:47.000000 mg-pso-gui-0.1.91/mgpsogui/gui/HomePage.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12527 2024-05-21 08:47:30.000000 mg-pso-gui-0.1.91/mgpsogui/gui/OptionManager.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.562572 mg-pso-gui-0.1.91/mgpsogui/gui/PlatformTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.91/mgpsogui/gui/PlatformTab/PlatformTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.91/mgpsogui/gui/PlatformTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.563077 mg-pso-gui-0.1.91/mgpsogui/gui/RunTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1839 2024-03-20 19:57:02.000000 mg-pso-gui-0.1.91/mgpsogui/gui/RunTab/RunTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.91/mgpsogui/gui/RunTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.566762 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/BoundsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/CalibrationParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/FunctionsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/ListParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1784 2024-04-10 21:01:22.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/OptimalParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2443 2024-05-21 09:01:39.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/SetupTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/StaticParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     5892 2024-05-21 09:06:58.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/StepView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.567800 mg-pso-gui-0.1.91/mgpsogui/gui/VisualizeTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    13322 2024-05-15 21:08:56.000000 mg-pso-gui-0.1.91/mgpsogui/gui/VisualizeTab/SideBar.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3477 2024-04-10 18:55:43.000000 mg-pso-gui-0.1.91/mgpsogui/gui/VisualizeTab/VisualizeTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.91/mgpsogui/gui/VisualizeTab/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.91/mgpsogui/gui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.576687 mg-pso-gui-0.1.91/mgpsogui/gui/images/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/IGOW 4 Logo.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/collapse.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/down.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/expand.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/play.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/refresh.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/refresh_hd.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/stop.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3642 2024-03-20 06:12:19.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/test.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/trash.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.91/mgpsogui/gui/images/up.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.91/mgpsogui/mgpsogui.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.91/mgpsogui/start.yaml
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.578965 mg-pso-gui-0.1.91/mgpsogui/util/
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.579802 mg-pso-gui-0.1.91/mgpsogui/util/CTkToolTip/
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.91/mgpsogui/util/CTkToolTip/__init__.py
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.91/mgpsogui/util/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    15076 2024-04-24 19:47:23.000000 mg-pso-gui-0.1.91/mgpsogui/util/GraphGenerator.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3482 2024-05-01 20:32:28.000000 mg-pso-gui-0.1.91/mgpsogui/util/PSORunner.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.91/mgpsogui/util/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.580408 mg-pso-gui-0.1.91/mgpsogui/util/recosu/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.91/mgpsogui/util/recosu/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.582783 mg-pso-gui-0.1.91/mgpsogui/util/recosu/pso/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.91/mgpsogui/util/recosu/pso/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2721 2024-03-20 06:01:30.000000 mg-pso-gui-0.1.91/mgpsogui/util/recosu/pso/csip_access.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12590 2024-05-01 20:39:10.000000 mg-pso-gui-0.1.91/mgpsogui/util/recosu/pso/pso.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.585356 mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 09:10:14.586923 mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/plot/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/plot/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/plot/cost_steps.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/trace_writer.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/utils.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-05-21 09:10:14.589661 mg-pso-gui-0.1.91/setup.cfg
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1526 2024-05-21 09:10:12.000000 mg-pso-gui-0.1.91/setup.py
```

### Comparing `mg-pso-gui-0.1.90/PKG-INFO` & `mg-pso-gui-0.1.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.90
+Version: 0.1.91
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.90/mg_pso_gui.egg-info/PKG-INFO` & `mg-pso-gui-0.1.91/mg_pso_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.90
+Version: 0.1.91
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.90/mg_pso_gui.egg-info/SOURCES.txt` & `mg-pso-gui-0.1.91/mg_pso_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/HomePage.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/HomePage.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 		self.scaling_label.grid(row=0, column=6, padx=header_padding_x, pady=header_padding_y)
 		self.scaling_optionemenu = customtkinter.CTkOptionMenu(self.sidebar_frame, values=["50%", "75%", "100%", "125%", "150%", "175%", "200%"], width=60,
 															   command=self.change_scaling_event)
 		self.scaling_optionemenu.grid(row=0, column=7, padx=header_padding_x, pady=header_padding_y)
 		self.scaling_optionemenu.set("100%")
 		
 		expand_image = customtkinter.CTkImage(Image.open(os.path.join("./images", "expand.png")), size=(20, 20))
-		self.new_window = customtkinter.CTkButton(self.sidebar_frame, text=None, width=30, image=expand_image, command=self.new_window)
+		self.new_window = customtkinter.CTkButton(self.sidebar_frame, text=None, width=30, image=expand_image, command=self.open_new_window)
 		ctt(self.new_window, delay=0.1, alpha=0.95, message="Open New Window")
 		self.new_window.grid(row=0, column=8, padx=(5, 20), pady=header_padding_y)
 		
 		self.tabview = customtkinter.CTkTabview(self, bg_color="transparent", fg_color="transparent")
 		self.tabview.grid(row=1, column=0, padx=(0, 0), pady=(10, 10), sticky="nsew")
 		tab1 = "Platform"
 		tab2 = "Setup"
@@ -170,15 +170,15 @@
 		self.footer_progress_label = customtkinter.CTkLabel(self.footer_frame, text="Stopped", width=150, font=customtkinter.CTkFont(size=16, weight="bold"), anchor="w")
 		self.footer_progress_label.grid(row=0, column=0, padx=(20, 5), pady=header_padding_y)
 
 		self.footer_progress_bar = customtkinter.CTkProgressBar(self.footer_frame)
 		self.footer_progress_bar.grid(row=0, column=4, padx=(50, 100), pady=header_padding_y, sticky="ew")
 		self.footer_progress_bar.set(0)
 		
-		self.algorithm_optionmenu = customtkinter.CTkOptionMenu(self.footer_frame, variable=self.option_manager.get_arguments()['mode'], values=["PSO", "Halton"], width=50, command=self.step_frame.refresh)
+		self.algorithm_optionmenu = customtkinter.CTkOptionMenu(self.footer_frame, variable=self.option_manager.get_arguments()['mode'], values=["PSO", "Halton"], width=50, command=self.refresh_step_view)
 		self.algorithm_optionmenu.grid(row=0, column=6, padx=header_padding_x, pady=header_padding_y)
 		self.algorithm_optionmenu.set("PSO")
 
 		play_image = customtkinter.CTkImage(Image.open(os.path.join("./images", "play.png")), size=(20, 20))
 		self.run_button = customtkinter.CTkButton(self.footer_frame, text=None, width=30, image=play_image, command=self.run)
 		ctt(self.run_button, delay=0.1, alpha=0.95, message="Start Calibration")
 		self.run_button.grid(row=0, column=7, padx=(20, 5), pady=header_padding_y)
@@ -270,15 +270,19 @@
 			self.save_button.configure(text="Saved!")
 			self.after(3000, lambda: self.save_button.configure(text="Save"))
 		except Exception as e:
 			self.save_button.configure(text="Error!")
 			print(e)
 			self.after(3000, lambda: self.save_button.configure(text="Save"))
 	
-	def new_window(self):
+	def refresh_step_view(self):
+		self.steps_frame.clear()
+		self.steps_frame.render()
+ 
+	def open_new_window(self):
 		# Shell out and run ./main.py
 		subprocess.Popen(["python3", "../mgpsogui.py"])
 	
 	def load_project(self):
 		
 		filename = askopenfilename(filetypes=[("JSON", "*.json")], title="Open Project", multiple=False)
 		print(filename)
```

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/OptionManager.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/OptionManager.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/PlatformTab/PlatformTab.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/PlatformTab/PlatformTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/RunTab/RunTab.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/RunTab/RunTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/BoundsEditorWindow.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/BoundsEditorWindow.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/BoundsList.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/BoundsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/CalibrationParametersView.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/CalibrationParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/FunctionsList.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/FunctionsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/ListParametersView.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/ListParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/OptimalParameterView.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/OptimalParameterView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/SetupTab.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/SetupTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/StaticParameterView.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/StaticParameterView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/SetupTab/StepView.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/SetupTab/StepView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/VisualizeTab/SideBar.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/VisualizeTab/SideBar.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/VisualizeTab/VisualizeTab.py` & `mg-pso-gui-0.1.91/mgpsogui/gui/VisualizeTab/VisualizeTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/IGOW 4 Logo.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/IGOW 4 Logo.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/collapse.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/collapse.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/down.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/down.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/expand.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/expand.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/play.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/play.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/refresh.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/refresh.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/refresh_hd.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/refresh_hd.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/stop.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/stop.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/test.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/test.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/trash.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/trash.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/gui/images/up.png` & `mg-pso-gui-0.1.91/mgpsogui/gui/images/up.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/start.yaml` & `mg-pso-gui-0.1.91/mgpsogui/start.yaml`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/util/CTkToolTip/ctk_tooltip.py` & `mg-pso-gui-0.1.91/mgpsogui/util/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/util/GraphGenerator.py` & `mg-pso-gui-0.1.91/mgpsogui/util/GraphGenerator.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/util/PSORunner.py` & `mg-pso-gui-0.1.91/mgpsogui/util/PSORunner.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/util/recosu/pso/csip_access.py` & `mg-pso-gui-0.1.91/mgpsogui/util/recosu/pso/csip_access.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/util/recosu/pso/pso.py` & `mg-pso-gui-0.1.91/mgpsogui/util/recosu/pso/pso.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/plot/cost_steps.py` & `mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/plot/cost_steps.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/trace_writer.py` & `mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/trace_writer.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/mgpsogui/util/recosu/utils/utils.py` & `mg-pso-gui-0.1.91/mgpsogui/util/recosu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.90/setup.py` & `mg-pso-gui-0.1.91/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.90'
+VERSION = '0.1.91'
 DESCRIPTION = 'GUI for MG-PSO'
 LONG_DESCRIPTION = open('../README.md').read()
 
 # Setting up
 setup(
     name="mg-pso-gui",
     version=VERSION,
```

