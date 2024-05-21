# Comparing `tmp/mg-pso-gui-0.1.85.tar.gz` & `tmp/mg-pso-gui-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mg-pso-gui-0.1.85.tar", last modified: Tue May 21 08:56:09 2024, max compression
+gzip compressed data, was "mg-pso-gui-0.1.9.tar", last modified: Wed Mar  6 06:42:33 2024, max compression
```

## Comparing `mg-pso-gui-0.1.85.tar` & `mg-pso-gui-0.1.9.tar`

### file list

```diff
@@ -1,72 +1,69 @@
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.597972 mg-pso-gui-0.1.85/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 08:56:09.597084 mg-pso-gui-0.1.85/PKG-INFO
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.596294 mg-pso-gui-0.1.85/mg_pso_gui.egg-info/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-21 08:56:09.000000 mg-pso-gui-0.1.85/mg_pso_gui.egg-info/PKG-INFO
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1871 2024-05-21 08:56:09.000000 mg-pso-gui-0.1.85/mg_pso_gui.egg-info/SOURCES.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-05-21 08:56:09.000000 mg-pso-gui-0.1.85/mg_pso_gui.egg-info/dependency_links.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-05-21 08:56:09.000000 mg-pso-gui-0.1.85/mg_pso_gui.egg-info/entry_points.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-05-21 08:56:09.000000 mg-pso-gui-0.1.85/mg_pso_gui.egg-info/requires.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-05-21 08:56:09.000000 mg-pso-gui-0.1.85/mg_pso_gui.egg-info/top_level.txt
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.566571 mg-pso-gui-0.1.85/mgpsogui/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.85/mgpsogui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.569114 mg-pso-gui-0.1.85/mgpsogui/gui/
--rwxr--r--   0 robertcordingly   (501) staff       (20)    24037 2024-05-21 08:56:02.000000 mg-pso-gui-0.1.85/mgpsogui/gui/HomePage.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12527 2024-05-21 08:47:30.000000 mg-pso-gui-0.1.85/mgpsogui/gui/OptionManager.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.570491 mg-pso-gui-0.1.85/mgpsogui/gui/PlatformTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.85/mgpsogui/gui/PlatformTab/PlatformTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.85/mgpsogui/gui/PlatformTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.571449 mg-pso-gui-0.1.85/mgpsogui/gui/RunTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1839 2024-03-20 19:57:02.000000 mg-pso-gui-0.1.85/mgpsogui/gui/RunTab/RunTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.85/mgpsogui/gui/RunTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.577388 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/BoundsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/CalibrationParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/FunctionsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/ListParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1784 2024-04-10 21:01:22.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/OptimalParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2443 2024-05-21 08:47:34.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/SetupTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/StaticParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     5955 2024-05-21 08:53:05.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/StepView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.579300 mg-pso-gui-0.1.85/mgpsogui/gui/VisualizeTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    13322 2024-05-15 21:08:56.000000 mg-pso-gui-0.1.85/mgpsogui/gui/VisualizeTab/SideBar.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3477 2024-04-10 18:55:43.000000 mg-pso-gui-0.1.85/mgpsogui/gui/VisualizeTab/VisualizeTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.85/mgpsogui/gui/VisualizeTab/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.85/mgpsogui/gui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.586328 mg-pso-gui-0.1.85/mgpsogui/gui/images/
--rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/IGOW 4 Logo.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/collapse.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/down.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/expand.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/play.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/refresh.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/refresh_hd.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/stop.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3642 2024-03-20 06:12:19.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/test.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/trash.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.85/mgpsogui/gui/images/up.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.85/mgpsogui/mgpsogui.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.85/mgpsogui/start.yaml
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.587972 mg-pso-gui-0.1.85/mgpsogui/util/
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.588973 mg-pso-gui-0.1.85/mgpsogui/util/CTkToolTip/
--rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.85/mgpsogui/util/CTkToolTip/__init__.py
--rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.85/mgpsogui/util/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    15076 2024-04-24 19:47:23.000000 mg-pso-gui-0.1.85/mgpsogui/util/GraphGenerator.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3482 2024-05-01 20:32:28.000000 mg-pso-gui-0.1.85/mgpsogui/util/PSORunner.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.85/mgpsogui/util/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.589737 mg-pso-gui-0.1.85/mgpsogui/util/recosu/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.85/mgpsogui/util/recosu/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.591546 mg-pso-gui-0.1.85/mgpsogui/util/recosu/pso/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.85/mgpsogui/util/recosu/pso/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2721 2024-03-20 06:01:30.000000 mg-pso-gui-0.1.85/mgpsogui/util/recosu/pso/csip_access.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12590 2024-05-01 20:39:10.000000 mg-pso-gui-0.1.85/mgpsogui/util/recosu/pso/pso.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.594242 mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-21 08:56:09.595504 mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/plot/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/plot/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/plot/cost_steps.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/trace_writer.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/utils.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-05-21 08:56:09.598173 mg-pso-gui-0.1.85/setup.cfg
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1526 2024-05-21 08:56:07.000000 mg-pso-gui-0.1.85/setup.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.877754 mg-pso-gui-0.1.9/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9457 2024-03-06 06:42:33.877183 mg-pso-gui-0.1.9/PKG-INFO
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.846222 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9457 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/PKG-INFO
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1759 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/entry_points.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/requires.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/top_level.txt
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.847771 mg-pso-gui-0.1.9/mgpsogui/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.9/mgpsogui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.850629 mg-pso-gui-0.1.9/mgpsogui/gui/
+-rwxr--r--   0 robertcordingly   (501) staff       (20)    25874 2024-03-06 06:33:23.000000 mg-pso-gui-0.1.9/mgpsogui/gui/HomePage.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    11712 2024-01-24 22:27:36.000000 mg-pso-gui-0.1.9/mgpsogui/gui/OptionManager.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.851516 mg-pso-gui-0.1.9/mgpsogui/gui/PlatformTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.9/mgpsogui/gui/PlatformTab/PlatformTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.9/mgpsogui/gui/PlatformTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.852229 mg-pso-gui-0.1.9/mgpsogui/gui/RunTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2850 2024-02-14 07:26:36.000000 mg-pso-gui-0.1.9/mgpsogui/gui/RunTab/RunTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.9/mgpsogui/gui/RunTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.857952 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/BoundsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/CalibrationParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/FunctionsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/ListParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1881 2024-02-14 08:15:40.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/SetupTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/StaticParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     5531 2024-02-13 06:31:26.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/StepView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.859222 mg-pso-gui-0.1.9/mgpsogui/gui/VisualizeTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3271 2024-02-28 21:07:31.000000 mg-pso-gui-0.1.9/mgpsogui/gui/VisualizeTab/VisualizeTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.9/mgpsogui/gui/VisualizeTab/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.9/mgpsogui/gui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.869677 mg-pso-gui-0.1.9/mgpsogui/gui/images/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/IGOW 4 Logo.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/collapse.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/down.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/expand.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/play.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/refresh.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/refresh_hd.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/stop.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/trash.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/up.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.9/mgpsogui/mgpsogui.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.9/mgpsogui/start.yaml
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.871312 mg-pso-gui-0.1.9/mgpsogui/util/
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.872044 mg-pso-gui-0.1.9/mgpsogui/util/CTkToolTip/
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/util/CTkToolTip/__init__.py
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/util/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     7851 2024-02-28 07:09:24.000000 mg-pso-gui-0.1.9/mgpsogui/util/GraphGenerator.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     6328 2024-03-06 06:26:18.000000 mg-pso-gui-0.1.9/mgpsogui/util/PSORunner.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.9/mgpsogui/util/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.872587 mg-pso-gui-0.1.9/mgpsogui/util/recosu/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.874160 mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2611 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/csip_access.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    13058 2024-03-06 06:42:27.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/pso.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.875592 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.876493 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/plot/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/plot/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/plot/cost_steps.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/trace_writer.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/utils.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-03-06 06:42:33.877868 mg-pso-gui-0.1.9/setup.cfg
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1525 2024-03-06 06:42:29.000000 mg-pso-gui-0.1.9/setup.py
```

### Comparing `mg-pso-gui-0.1.85/PKG-INFO` & `mg-pso-gui-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.85
+Version: 0.1.9
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.85/mg_pso_gui.egg-info/PKG-INFO` & `mg-pso-gui-0.1.9/mg_pso_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.85
+Version: 0.1.9
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.85/mg_pso_gui.egg-info/SOURCES.txt` & `mg-pso-gui-0.1.9/mg_pso_gui.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,31 +16,28 @@
 mgpsogui/gui/RunTab/RunTab.py
 mgpsogui/gui/RunTab/__init__.py
 mgpsogui/gui/SetupTab/BoundsEditorWindow.py
 mgpsogui/gui/SetupTab/BoundsList.py
 mgpsogui/gui/SetupTab/CalibrationParametersView.py
 mgpsogui/gui/SetupTab/FunctionsList.py
 mgpsogui/gui/SetupTab/ListParametersView.py
-mgpsogui/gui/SetupTab/OptimalParameterView.py
 mgpsogui/gui/SetupTab/SetupTab.py
 mgpsogui/gui/SetupTab/StaticParameterView.py
 mgpsogui/gui/SetupTab/StepView.py
 mgpsogui/gui/SetupTab/__init__.py
-mgpsogui/gui/VisualizeTab/SideBar.py
 mgpsogui/gui/VisualizeTab/VisualizeTab.py
 mgpsogui/gui/VisualizeTab/__init__.py
 mgpsogui/gui/images/IGOW 4 Logo.png
 mgpsogui/gui/images/collapse.png
 mgpsogui/gui/images/down.png
 mgpsogui/gui/images/expand.png
 mgpsogui/gui/images/play.png
 mgpsogui/gui/images/refresh.png
 mgpsogui/gui/images/refresh_hd.png
 mgpsogui/gui/images/stop.png
-mgpsogui/gui/images/test.png
 mgpsogui/gui/images/trash.png
 mgpsogui/gui/images/up.png
 mgpsogui/util/GraphGenerator.py
 mgpsogui/util/PSORunner.py
 mgpsogui/util/__init__.py
 mgpsogui/util/CTkToolTip/__init__.py
 mgpsogui/util/CTkToolTip/ctk_tooltip.py
```

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/OptionManager.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/OptionManager.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,37 +7,32 @@
 class OptionManager():
     
     def __init__(self):
         
         self.project_data = {"name": "", "path": ""}
         self.arguments = {"param": [],
                  "url": sv(),
-                 "mode": sv(),
                  "files": {},
                  "calibration_parameters": []}
         self.steps = []
         self.service_parameters = {}
             
     def clear(self):
         self.arguments['param'].clear()
         self.arguments['url'].set("")
-        self.arguments['mode'].set("PSO")
         self.arguments['files'] = {}
         self.arguments['calibration_parameters'].clear()
         self.steps = []
         self.service_parameters = {}
     
     def add_arguments(self, arguments):
         
         if ("url" in arguments):
             self.arguments["url"].set(arguments["url"])
             
-        if ("mode" in arguments):
-            self.arguments["mode"].set(arguments["mode"])
-            
         if ("files" in arguments):
             for file in arguments["files"]:
                 name = file["name"]
                 value = file["value"]
                 obj = {"name": sv(), "value": sv()}
                 obj["name"].set(name)
                 obj["value"].set(value)
@@ -66,46 +61,36 @@
             obj["message"].set("Wow")
             
             for param in step["param"]:
                 param_obj = {
                     "name": sv(), 
                     "bounds": (sv(), sv()), 
                     "default_value": sv(), 
-                    "optimal_value": sv(), 
                     "type": sv(),
                     "calibration_strategy": sv()
                 }
                 param_obj["name"].set(param["name"])
                 if "bounds" in param:
                     param_obj["bounds"][0].set(param["bounds"][0])
                     param_obj["bounds"][1].set(param["bounds"][1]) 
                 else: 
                     param_obj["bounds"][0].set(0)
                     param_obj["bounds"][1].set(1)
-                    
                 if "type" in param:
                     param_obj["type"].set(param["type"])
                 else:
                     param_obj["type"].set("float")
-                    
                 if "default_value" in param:
                     param_obj["default_value"].set(param["default_value"])
                 else:
                     param_obj["default_value"].set(1)
-                    
-                if "optimal_value" in param:
-                    param_obj["optimal_value"].set(param["optimal_value"])
-                else:
-                    param_obj["optimal_value"].set(0)
-                    
                 if "calibration_strategy" in param:
                     param_obj["calibration_strategy"].set(param["calibration_strategy"])
                 else:
                     param_obj["calibration_strategy"].set("none")
-                    
                 obj["param"].append(param_obj)
             
             for objfunc in step["objfunc"]:
                 objfunc_obj = {"name": sv(), "of": sv(), "weight": sv(), "data": (sv(), sv())}
                 objfunc_obj["name"].set(objfunc["name"])
                 objfunc_obj["of"].set(objfunc["of"])
                 
@@ -146,28 +131,25 @@
     
     def add_bound(self, step_index, 
                   name="name", 
                   min=0, 
                   max=1,
                   type="float",
                   default_value=1,
-                  optimal_value=0,
                   calibration_strategy="none"):
         obj = {
             "name": sv(), 
             "bounds": (sv(), sv()), 
             "default_value": sv(), 
-            "optimal_value": sv(),
             "type": sv(),
             "calibration_strategy": sv()
         }
         obj["name"].set(name)
         obj["type"].set(type)
         obj["default_value"].set(default_value)
-        obj["optimal_value"].set(optimal_value)
         obj["calibration_strategy"].set(calibration_strategy)
         obj["bounds"][0].set(min)
         obj["bounds"][1].set(max)
         self.steps[step_index]["param"].append(obj)
         
     def remove_bound(self, step_index, index):
         self.steps[step_index]["param"].pop(index)
@@ -241,15 +223,15 @@
     def get_metrics(self):
         result = {}
         result['arguments'] = {}
         result['calibration_parameters'] = []
         result['service_parameters'] = {}
         result['project_data'] = self.project_data
         for key, value in self.arguments.items():
-            if key == 'url' or key == 'mode':
+            if key == 'url':
                 result['arguments'][key] = value.get()
             elif key == 'files':
                 result['arguments'][key] = {}
                 #for name, obj in value.items():
                 #    result['arguments'][key].append({'name': obj['name'].get(), 'value': obj['value'].get()})
             elif key == 'param':
                 result['arguments'][key] = []
@@ -271,27 +253,25 @@
                 if param['type'].get() == 'float':
                     step_result['param'].append(
                         {
                             'name': param['name'].get(), 
                             'bounds': (float(param['bounds'][0].get()), 
                                        float(param['bounds'][1].get())),
                             'default_value': float(param['default_value'].get()),
-                            'optimal_value': float(param['optimal_value'].get()),
                             'type': 'float',
                             'calibration_strategy': param['calibration_strategy'].get()
                         }
                     )
                 elif param['type'].get() == 'list':
                     step_result['param'].append(
                         {
                             'name': param['name'].get(), 
                             'bounds': (float(param['bounds'][0].get()), 
                                        float(param['bounds'][1].get())),
                             'default_value': param['default_value'].get(),
-                            'optimal_value': param['optimal_value'].get(),
                             'type': 'list',
                             'calibration_strategy': param['calibration_strategy'].get()
                         }
                     )
                 #except ValueError:
                 #    step_result['param'].append(
                 #        {
```

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/PlatformTab/PlatformTab.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/PlatformTab/PlatformTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/RunTab/RunTab.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/RunTab/RunTab.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,29 @@
 
 def create_tab(self, tab):
     
     # URL
     tab.grid_columnconfigure(0, weight=1)
     tab.grid_rowconfigure(0, weight=1)
     tab.grid_rowconfigure(1, weight=200)
+    
+    """
+    self.url = customtkinter.CTkEntry(tab, textvariable=self.option_manager.get_arguments()['url'])
+    self.url.grid(row=0, column=0, columnspan=1, padx=(20, 20), pady=(20, 20), sticky="nsew")
 
+    self.run_button = customtkinter.CTkButton(tab, text="Run", command=self.run)
+    self.run_button.grid(row=0, column=1, padx=(20, 20), pady=(20, 20), sticky="nsew")
+    ctt(self.run_button, delay=0.5, message="Start calibration...")
+    
+        self.stop_button = customtkinter.CTkButton(tab, text="Stop", command=self.stop)
+    self.stop_button.grid(row=0, column=2, padx=(20, 20), pady=(20, 20), sticky="nsew")
+    ctt(self.stop_button, delay=0.5, message="Stop calibration...")
+    
+    """
+    
     self.progress_container = customtkinter.CTkFrame(tab)
     self.progress_container.grid_columnconfigure(0, weight=1)
     self.progress_container.grid_columnconfigure(1, weight=1)
     self.progress_container.grid_columnconfigure(2, weight=1)
     self.progress_container.grid(row=0, column=0, padx=(20, 20), pady=(20, 20), sticky="nsew")
     
     # Add progress bar to progress container
@@ -32,11 +46,16 @@
     
     self.progress_message_middle = customtkinter.CTkLabel(self.progress_container, text="Calibration not running...")
     self.progress_message_middle.grid(row=0, column=1, padx=(10, 10), pady=(10, 10), sticky="ew")
     
     self.progress_message_right = customtkinter.CTkLabel(self.progress_container, text="")
     self.progress_message_right.grid(row=0, column=2, padx=(10, 10), pady=(10, 10), sticky="e")
     
+    #self.progress_bar = customtkinter.CTkProgressBar(self.progress_container)
+    #self.progress_bar.grid(row=1, column=0, columnspan=3, padx=(10, 10), pady=(10, 10), sticky="ew")
+    #self.progress_bar.set(0)
+    #ctt(self.progress_bar, delay=0.5, message="Current calibration progress")
+    
     self.textbox = customtkinter.CTkTextbox(tab)
     self.textbox.grid(row=1, column=0, padx=(20, 20), pady=(20, 20), sticky="nsew")
-    self.textbox.insert("0.0", "Welcome to the CSIP PSO Calibration Tool!\n\nUse the Setup tab to define steps and calibration parameters. Use this tab to view logs and observe calibration progress. Once finished, use the Results tab to generate figures and graphs.")
+    self.textbox.insert("0.0", "Welcome to the CSIP PSO Calibration Tool!\n\nUse the Calibration tab to define steps and calibration parameters. Use this tab to run and observe calibration progress. Once finished, use the Visualization tab to generate figures and graphs.")
```

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/BoundsEditorWindow.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/BoundsEditorWindow.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/BoundsList.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/BoundsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/CalibrationParametersView.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/CalibrationParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/FunctionsList.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/FunctionsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/ListParametersView.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/ListParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/OptimalParameterView.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/StaticParameterView.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,45 +3,59 @@
 from customtkinter import CTkLabel
 from customtkinter import CTkButton
 from customtkinter import CTkEntry
 import tkinter as tk
 
 global option_manager
 
-class OptimalParameterView(CTkScrollableFrame):
+class StaticParameterView(CTkScrollableFrame):
     def __init__(self, *args,
                  option_manager: None,
                  **kwargs):
         super().__init__(*args, **kwargs)
         
         self.option_manager = option_manager
+        self.key_values = option_manager.get_arguments()['param']
+        self.edit_mode = False
         
         self.render()
 
     def clear(self):
         self.containerFrame.destroy()
         
+    def toggle_edit_mode(self):
+        self.clear()
+        self.edit_mode = not self.edit_mode
+        self.render()
+        
     def render(self):
         row = 0
+        index = 0
         
         self.containerFrame = CTkFrame(self)
         self.containerFrame.grid(row=0, column=0, padx=(5, 5), pady=(5, 5), sticky="nsew")
         self.containerFrame.grid_columnconfigure((0, 1), weight=1)
         
-        #CTkLabel(self.containerFrame, text="Name:").grid(row=row, column=0, columnspan=1, padx=5, pady=5, sticky="")
-        #CTkLabel(self.containerFrame, text="Value:").grid(row=row, column=1, columnspan=1, padx=5, pady=5, sticky="")
-        #row += 1
+        CTkLabel(self.containerFrame, text="Name:").grid(row=row, column=0, columnspan=1, padx=5, pady=5, sticky="")
+        CTkLabel(self.containerFrame, text="Value:").grid(row=row, column=1, columnspan=1, padx=5, pady=5, sticky="")
+        row += 1
         
-        self.steps = self.option_manager.get_steps()
-
-        for step in self.steps:
-            name = step['name'].get()
-            CTkLabel(self.containerFrame, text=name).grid(row=row, column=0, columnspan=1, padx=5, pady=5, sticky="")
-            row += 1
-            
-            for param in step['param']:
-                CTkEntry(self.containerFrame, textvariable=param['name']).grid(row=row, column=0, padx=(5, 5), pady=(5, 5), sticky="ew")
+        for key_value_pair in self.key_values:
+            CTkEntry(self.containerFrame, textvariable=self.key_values[index]["name"]).grid(row=row, column=0, padx=(5, 5), pady=(5, 5), sticky="ew")
             
+            if self.edit_mode:
+                return_func = lambda index=index: (self.clear(), self.option_manager.remove_argument(index), self.render())
+                CTkButton(self.containerFrame, text="Remove", command=return_func).grid(row=row, column=1, padx=(5, 5), pady=(5, 5), sticky="ew")
+            else:
                 bb = CTkEntry(self.containerFrame)
                 bb.grid(row=row, column=1, padx=(5, 5), pady=(5, 5), sticky="ew")
-                bb.configure(textvariable=param['optimal_value'])
-                row += 1
+                bb.configure(textvariable=self.key_values[index]["value"])
+            row += 1
+            index += 1
+            
+        if self.edit_mode:
+            CTkButton(self.containerFrame, text="Exit", command=self.toggle_edit_mode).grid(row=row, column=0, padx=(5, 5), pady=(5, 5), sticky="ew")
+        else:
+            CTkButton(self.containerFrame, text="Edit", command=self.toggle_edit_mode).grid(row=row, column=0, padx=(5, 5), pady=(5, 5), sticky="ew")
+            
+        add_key_func = lambda: (self.clear(), self.option_manager.add_argument("name", "value"), self.render())
+        CTkButton(self.containerFrame, text="Add Parameter", command=add_key_func).grid(row=row, column=1, padx=(5, 5), pady=(5, 5), sticky="ew")
```

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/SetupTab.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/SetupTab.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,43 @@
 
 
 from . import StepView as sv
 from . import StaticParameterView as spv
 from . import CalibrationParametersView as cpv
-from . import OptimalParameterView as opv
 
 import customtkinter
 
 def create_tab(self, tab):
     
     tab.grid_columnconfigure(0, weight=8)
     tab.grid_columnconfigure(1, weight=1)
     tab.grid_rowconfigure(0, weight=1)
     
     self.paramtabview = customtkinter.CTkTabview(tab, bg_color="transparent", fg_color="transparent")
     self.paramtabview.grid(row=0, column=1, padx=(0, 0), pady=(10, 10), sticky="nsew")
     
-    tab1 = "Static"
-    tab2 = "Calibration"
-    tab3 = "Optimal Parameters"
+    tab1 = "Static Parameters"
+    tab2 = "Calibration Parameters"
     self.paramtabview.add(tab1)
     self.paramtabview.add(tab2)
-    self.paramtabview.add(tab3)
     
     self.paramtabview.tab(tab1).grid_columnconfigure(0, weight=1)
     self.paramtabview.tab(tab1).grid_rowconfigure(0, weight=1)
     
     self.paramtabview.tab(tab2).grid_columnconfigure(0, weight=1)
     self.paramtabview.tab(tab2).grid_rowconfigure(0, weight=1)
     
-    self.paramtabview.tab(tab3).grid_columnconfigure(0, weight=1)
-    self.paramtabview.tab(tab3).grid_rowconfigure(0, weight=1)
-    
     self.static_param_frame = spv.StaticParameterView(self.paramtabview.tab(tab1), option_manager=self.option_manager)
     self.static_param_frame.grid(row=0, column=0, padx=(10, 10), pady=(10, 0), sticky="nsew")
     self.static_param_frame.grid_columnconfigure(0, weight=1)
     self.static_param_frame.grid_rowconfigure(0, weight=1)
     
     self.calib_param_frame = cpv.CalibrationParametersView(self.paramtabview.tab(tab2), option_manager=self.option_manager)
     self.calib_param_frame.grid(row=0, column=0, padx=(10, 10), pady=(10, 0), sticky="nsew")
     self.calib_param_frame.grid_columnconfigure(0, weight=1)
     self.calib_param_frame.grid_rowconfigure(0, weight=1)
     
-    self.optimal_param_frame = opv.OptimalParameterView(self.paramtabview.tab(tab3), option_manager=self.option_manager)
-    self.optimal_param_frame.grid(row=0, column=0, padx=(10, 10), pady=(10, 0), sticky="nsew")
-    self.optimal_param_frame.grid_columnconfigure(0, weight=1)
-    self.optimal_param_frame.grid_rowconfigure(0, weight=1)
-    
     self.steps_frame = sv.StepView(tab, label_text="Group Editor", option_manager=self.option_manager)
     self.steps_frame.grid(row=0, column=0, padx=(10, 10), pady=(10, 0), sticky="nsew")
     self.steps_frame.grid_columnconfigure(0, weight=1)
     self.steps_frame.grid_rowconfigure(0, weight=1)
```

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/SetupTab/StepView.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/StepView.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,24 +60,16 @@
 
         self.containerFrame = CTkFrame(self)
         self.containerFrame.grid(row=0, column=0, padx=(
             10, 10), pady=(10, 10), sticky="nsew")
         self.containerFrame.grid_columnconfigure((0, 1), weight=1)
 
         self.steps = self.option_manager.get_steps()
-        self.mode = self.option_manager.get_arguments()['mode'].get()
-        
-        tempSteps = self.steps
-        if self.mode == "Halton":
-            # Collapse all steps 
-            tempSteps = []
-            if len(self.steps) > 0:
-                tempSteps.append(self.steps[0])
 
-        for step in tempSteps:
+        for step in self.steps:
 
             up_image = CTkImage(Image.open(os.path.join("./images", "up.png")), size=(20, 20))
             down_image = CTkImage(Image.open(os.path.join("./images", "down.png")), size=(20, 20))
             trash_image = CTkImage(Image.open(os.path.join("./images", "trash.png")), size=(20, 20))
             expand_image = CTkImage(Image.open(os.path.join("./images", "expand.png")), size=(20, 20))
             collapse_image = CTkImage(Image.open(os.path.join("./images", "collapse.png")), size=(20, 20))
 
@@ -93,19 +85,17 @@
             button_container.grid(row=row, column=1, sticky="nse", padx=(10, 10), pady=(10, 10))
             button_container.grid_rowconfigure(0, weight=1)
             button_container.grid_columnconfigure(0, weight=1)
             
             CTkEntry(self.containerFrame, textvariable=step['name'], width=500).grid(row=row, column=0, padx=(20, 20), pady=(20, 20), sticky="nsw")
             #CTkLabel(self.containerFrame, textvariable=step['message']).grid(row=row, column=1, padx=(20, 20), pady=(20, 20), sticky="nsew")
             CTkButton(button_container, width=30, text=None, image=expand_image if not step['open'] else collapse_image, command=expand_func).grid(row=0, column=0, padx=(10, 10), pady=(10, 10), sticky="nsew")
-            
-            if (self.mode == "PSO"):
-                CTkButton(button_container, width=30, text=None, image=up_image, state="disabled" if index==0 else "normal", fg_color="gray" if index==0 else None, command=up_func).grid(row=0, column=1, padx=(10, 10), pady=(10, 10), sticky="nsew")
-                CTkButton(button_container, width=30, text=None, image=down_image, state="disabled" if index==(len(self.steps)-1) else "normal", fg_color="gray" if index==(len(self.steps)-1) else None, command=down_func).grid(row=0, column=2, padx=(10, 10), pady=(10, 10), sticky="nsew")
-                CTkButton(button_container, width=30, text=None, image=trash_image, command=remove_func).grid(row=0, column=3, padx=(10, 10), pady=(10, 10), sticky="nsew")
+            CTkButton(button_container, width=30, text=None, image=up_image, state="disabled" if index==0 else "normal", fg_color="gray" if index==0 else None, command=up_func).grid(row=0, column=1, padx=(10, 10), pady=(10, 10), sticky="nsew")
+            CTkButton(button_container, width=30, text=None, image=down_image, state="disabled" if index==(len(self.steps)-1) else "normal", fg_color="gray" if index==(len(self.steps)-1) else None, command=down_func).grid(row=0, column=2, padx=(10, 10), pady=(10, 10), sticky="nsew")
+            CTkButton(button_container, width=30, text=None, image=trash_image, command=remove_func).grid(row=0, column=3, padx=(10, 10), pady=(10, 10), sticky="nsew")
 
             row += 1
 
             if step['open']:
                 bounds = BoundsList.BoundsList(
                     self.containerFrame, option_manager=self.option_manager, step_index=index)
                 bounds.grid(row=row, column=0, padx=(10, 10),
@@ -120,11 +110,9 @@
                 funcs.grid_columnconfigure(0, weight=1)
                 funcs.grid_rowconfigure(0, weight=1)
                 
             row += 1
             index += 1
 
         # Create an "Add step button that is centered
-        
-        if (self.mode == "PSO" or len(self.steps) == 0):
-            CTkButton(self.containerFrame, text="Add Group", command=self.create_new_step).grid(
-                row=row, columnspan=2, column=0, padx=(10, 10), pady=(10, 10), sticky="ew")
+        CTkButton(self.containerFrame, text="Add Group", command=self.create_new_step).grid(
+            row=row, columnspan=2, column=0, padx=(10, 10), pady=(10, 10), sticky="ew")
```

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/VisualizeTab/VisualizeTab.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/VisualizeTab/VisualizeTab.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import customtkinter
 import tkinter as tk
 from PIL import Image, ImageTk
 import os
 import platform
 import subprocess
 
-from . import SideBar
-
 def create_tab(self, tab):
     
     def open_graph_in_browser():
         # Open the file in the default program
         info = self.option_manager.get_project_data()
         folder = os.path.join(info['path'], info['name'])
         
@@ -43,35 +41,33 @@
         self.image_height = new_height
         
         self.graph_image = customtkinter.CTkImage(self.graph_image_obj, size=(new_width, new_height))
         self.graph_label.configure(image=self.graph_image)
         self.graph_label.update_idletasks()
     
     
-    tab.grid_columnconfigure(0, weight=2)
+    tab.grid_columnconfigure(0, weight=1)
     tab.grid_columnconfigure(1, weight=8)
     tab.grid_rowconfigure(0, weight=1)
     
     self.graph_sidebar = customtkinter.CTkFrame(tab)
     self.graph_sidebar.grid(row=0, column=0, padx=(20, 20), pady=(20, 20), sticky="nsew")
     self.graph_container = customtkinter.CTkFrame(tab)
     self.graph_container.grid(row=0, column=1, padx=(20, 20), pady=(20, 20), sticky="nsew")
     
     self.graph_sidebar.grid_columnconfigure(0, weight=1)
-    self.graph_sidebar.grid_rowconfigure(1, weight=1)
+    self.graph_sidebar.grid_rowconfigure(8, weight=1)
     self.graph_container.grid_columnconfigure(0, weight=1)
     self.graph_container.grid_rowconfigure(0, weight=1)
     
-    self.graph_selector = customtkinter.CTkOptionMenu(self.graph_sidebar, values=["Best Cost Stacked", "Best Cost by Round", "Calibrated Parameters", "Iteration Table", "Custom CSV", "Compare CSV"], variable=self.graph_selector_value, command=self.update_graph)
+    self.graph_selector_value = tk.StringVar()
+    self.graph_selector_value.set("Best Cost Stacked")
+    self.graph_selector = customtkinter.CTkOptionMenu(self.graph_sidebar, values=["Best Cost Stacked", "Best Cost by Round", "Calibrated Parameters", "Iteration Table"], variable=self.graph_selector_value, command=self.update_graph)
     self.graph_selector.grid(row=0, column=0, padx=(20, 20), pady=(20, 20), sticky="nsew")
     
-    # Create SideBar
-    self.vis_sidebar = SideBar.SideBar(self.graph_sidebar, option_manager=self.option_manager, home_page=self, fg_color="transparent")
-    self.vis_sidebar.grid(row=1, column=0, rowspan=8, padx=(0, 0), pady=(0, 0), sticky="nsew")
-    
     # Add a button to call open_graph_in_browser
     self.graph_button = customtkinter.CTkButton(self.graph_sidebar, text="Open in Browser", command=open_graph_in_browser)
     self.graph_button.grid(row=9, column=0, padx=(20, 20), pady=(20, 20), sticky="nsew")
     
     self.graph_image_obj = Image.open(os.path.join("./images", "refresh_hd.png"))
     self.graph_image = customtkinter.CTkImage(self.graph_image_obj, size=(1280, 720))
     self.graph_label = customtkinter.CTkLabel(self.graph_container, text=None, image=self.graph_image)
```

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/IGOW 4 Logo.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/IGOW 4 Logo.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/collapse.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/collapse.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/down.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/down.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/expand.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/expand.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/play.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/play.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/refresh.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/refresh.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/refresh_hd.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/refresh_hd.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/stop.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/stop.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/trash.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/trash.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/gui/images/up.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/up.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/start.yaml` & `mg-pso-gui-0.1.9/mgpsogui/start.yaml`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/util/CTkToolTip/ctk_tooltip.py` & `mg-pso-gui-0.1.9/mgpsogui/util/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/util/recosu/pso/csip_access.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/csip_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 
 def csip_worker(reqq: queue.Queue, thread_no: int, stop, full_trace,
                 url, files, arg_params, conf: Dict, metainfo: Dict) -> None:
     async_call = conf.get('async_call', True)  # default is async
     save_resp = conf.get('save_response_to', None)  # save response, set it to a folder if responses should be saved.
 
     while not stop():
-        
         try:
             (rnd, step, iteration, particle, x, step_param_names, calib_params, objfunc, resq) = reqq.get(True, 0.5)
             # print(thread_no, particle)
-    
+
             c = Client(metainfo=metainfo)
 
             # static params (from args)
             for param in arg_params:
                 c.add_data(param['name'], param['value'])
 
             # particle params  (generated from steps)
@@ -45,31 +44,27 @@
                     res = c.execute(url, files=files, conf=conf)
 
                 if res.is_failed():
                     print(res)
 
                 if save_resp:
                     res.save_to(os.path.join(save_resp, 'r{}s{}i{}p{}.json'.format(rnd, step, iteration, particle)))
-                    
+
                 # print(res)
-                print('O', end='', flush=True)
-                
+                print(u'\u2714', end='', flush=True)
                 cost = utils.calc_cost(res, objfunc)
 
                 if full_trace is not None:
                     all_params = {}
                     # for i, value in enumerate(x):
                     for idx, value in enumerate(x[particle, :]):
                         all_params[step_param_names[idx]] = value
-                        
                     for name, value in calib_params.items():
                         all_params[name] = value
                     full_trace.append((all_params, cost))
 
                 resq.put((particle, cost))
-            except Exception as e:
+            except:
                 print(res)
-                print(e)
-
             reqq.task_done()
         except queue.Empty:
             continue
```

### Comparing `mg-pso-gui-0.1.85/mgpsogui/util/recosu/pso/pso.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/pso.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,14 @@
         # print("cost ", cost)
         nan_idx = np.where(np.isnan(cost))
         failed_particles = len(nan_idx[0])
 
         # leave the loop if fails acceptable
         if failed_particles <= pfail_count:
             break
-        
         print("Re-running particles, since ", failed_particles, ' out of ', particles, ' particles failed.')
         pfail_retry -= 1
 
     if pfail_retry == 0:
         print('Particle evaluation failed ', conf.get('particles_retry', 3), ' times. PSO stopped.')
         return None
 
@@ -75,18 +74,30 @@
     # assign the mean value to all failed runs.
     mean = np.nanmean(cost)
     cost[nan_idx[0]] = mean
 
     print(flush=True)
     return cost
 
+# Simulator
 def global_best(steps: Dict, rounds: Tuple, args: Dict, n_particles: int, iters: int, options: Dict,
                 oh_strategy: Dict = None, n_threads: int = 4, rtol: float = 0.001, ftol: float = -np.inf,
                 ftol_iter: int = 1, full_trace: List = None, rtol_iter: int = 1,
                 conf: Dict = None, metainfo: Dict = None, cost_target: float = -np.inf, result_queue: Queue = None) -> Tuple:
+    import time
+    while True:
+        print("WOW", flush=True)
+        if result_queue is not None:
+            result_queue.put('WOW')
+        time.sleep(1)
+
+def global_best_real(steps: Dict, rounds: Tuple, args: Dict, n_particles: int, iters: int, options: Dict,
+                oh_strategy: Dict = None, n_threads: int = 4, rtol: float = 0.001, ftol: float = -np.inf,
+                ftol_iter: int = 1, full_trace: List = None, rtol_iter: int = 1,
+                conf: Dict = None, metainfo: Dict = None, cost_target: float = -np.inf, result_queue: Queue = None) -> Tuple:
     """Performs a stepwise particle swarm optimization PSO using a global best approach.
 
         Parameters
         ----------
         steps : Dict
             step definitions
         rounds : tuple
@@ -164,23 +175,23 @@
     step_trace = {}
 
     step_trace['dir'] = os.getcwd()
     step_trace['start'] = str(datetime.datetime.now())
     step_trace['min_rounds'] = min_rounds
     step_trace['max_rounds'] = max_rounds
     step_trace['iters'] = iters
-    #step_trace['ftol'] = ftol BUG DOES NOT HANDLE -INF
+    step_trace['ftol'] = ftol
     step_trace['ftol_iter'] = ftol_iter
     step_trace['rtol'] = rtol
     step_trace['rtol_iter'] = rtol_iter
     step_trace['n_threads'] = n_threads
     step_trace['n_particles'] = n_particles
     step_trace['n_steps'] = len(steps)
     step_trace['steps'] = copy.deepcopy(steps)
-    #step_trace['args'] = args BUG MUST BE REMOVED
+    step_trace['args'] = args
 
     if step_file is not None:
         with open(step_file, "w") as fo:
             json.dump(step_trace, fo)
 
     # best round cost
     best_round_cost = np.inf
@@ -231,14 +242,15 @@
                                              bounds=bounds,
                                              ftol=step.get('ftol', ftol),
                                              ftol_iter=step.get('ftol_iter', ftol_iter),
                                              cost_target=step.get('cost_target', cost_target))
             print('\n>>>>> R{}/S{}  particle params: {}  calibrated params: {}\n'.format(r + 1, s + 1, param_names,
                                                                                          args['calib_params']))
 
+
             if result_queue is not None:
                 result_queue.put('\n>>>>> R{}/S{}  particle params: {}  calibrated params: {}\n'.format(r + 1, s + 1, param_names, args['calib_params']))
             
             args['rnd'] = r + 1
             args['step'] = s + 1
 
             # perform optimization
@@ -332,11 +344,8 @@
     step_trace['end'] = str(datetime.datetime.now())
     step_trace['time'] = elapsed
 
     if step_file is not None:
         with open(step_file, "w") as fo:
             json.dump(step_trace, fo)
 
-    result_queue.put("Step Trace")
-    result_queue.put(step_trace)
-
     return optimizer, step_trace
```

### Comparing `mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/plot/cost_steps.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/plot/cost_steps.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/trace_writer.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/trace_writer.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/mgpsogui/util/recosu/utils/utils.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.85/setup.py` & `mg-pso-gui-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.85'
+VERSION = '0.1.9'
 DESCRIPTION = 'GUI for MG-PSO'
 LONG_DESCRIPTION = open('../README.md').read()
 
 # Setting up
 setup(
     name="mg-pso-gui",
     version=VERSION,
```

