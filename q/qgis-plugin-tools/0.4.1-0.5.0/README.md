# Comparing `tmp/qgis_plugin_tools-0.4.1.tar.gz` & `tmp/qgis_plugin_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgis_plugin_tools-0.4.1.tar", last modified: Thu Feb  1 11:11:02 2024, max compression
+gzip compressed data, was "qgis_plugin_tools-0.5.0.tar", last modified: Tue May 21 11:44:19 2024, max compression
```

## Comparing `qgis_plugin_tools-0.4.1.tar` & `qgis_plugin_tools-0.5.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:11:02.976816 qgis_plugin_tools-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-02-01 11:11:02.976816 qgis_plugin_tools-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:11:02.968816 qgis_plugin_tools-0.4.1/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/infrastructure/debugging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15403 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/infrastructure/plugin_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:11:02.976816 qgis_plugin_tools-0.4.1/qgis_plugin_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-02-01 11:11:02.000000 qgis_plugin_tools-0.4.1/qgis_plugin_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-01 11:11:02.000000 qgis_plugin_tools-0.4.1/qgis_plugin_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 11:11:02.000000 qgis_plugin_tools-0.4.1/qgis_plugin_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 11:11:02.000000 qgis_plugin_tools-0.4.1/qgis_plugin_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 11:11:02.000000 qgis_plugin_tools-0.4.1/qgis_plugin_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:11:02.968816 qgis_plugin_tools-0.4.1/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:11:02.968816 qgis_plugin_tools-0.4.1/resources/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/resources/ui/progress_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-01 11:11:02.976816 qgis_plugin_tools-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:11:02.976816 qgis_plugin_tools-0.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_decorations.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_raster_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_setings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/test/test_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:11:02.968816 qgis_plugin_tools-0.4.1/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/testing/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:11:02.972816 qgis_plugin_tools-0.4.1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/algorithm_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/custom_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/decorations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/ghost_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/logger_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11461 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/raster_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11494 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:11:02.972816 qgis_plugin_tools-0.4.1/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/widgets/grid_layout_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/widgets/json_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/widgets/list_fields_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/widgets/list_layers_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/widgets/progress_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-02-01 11:10:55.000000 qgis_plugin_tools-0.4.1/widgets/selectable_combobox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:19.075469 qgis_plugin_tools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-05-21 11:44:19.075469 qgis_plugin_tools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:19.067469 qgis_plugin_tools-0.5.0/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/infrastructure/debugging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15403 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/infrastructure/plugin_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:19.075469 qgis_plugin_tools-0.5.0/qgis_plugin_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-05-21 11:44:19.000000 qgis_plugin_tools-0.5.0/qgis_plugin_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-21 11:44:19.000000 qgis_plugin_tools-0.5.0/qgis_plugin_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:44:19.000000 qgis_plugin_tools-0.5.0/qgis_plugin_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:44:18.000000 qgis_plugin_tools-0.5.0/qgis_plugin_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 11:44:19.000000 qgis_plugin_tools-0.5.0/qgis_plugin_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:19.063469 qgis_plugin_tools-0.5.0/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:19.067469 qgis_plugin_tools-0.5.0/resources/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/resources/ui/progress_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-21 11:44:19.075469 qgis_plugin_tools-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:19.071468 qgis_plugin_tools-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_decorations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_raster_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_setings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/test/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:19.067469 qgis_plugin_tools-0.5.0/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/testing/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:19.071468 qgis_plugin_tools-0.5.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/algorithm_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/decorations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/ghost_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/logger_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11461 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/raster_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11494 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:19.071468 qgis_plugin_tools-0.5.0/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/widgets/grid_layout_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/widgets/json_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/widgets/list_fields_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/widgets/list_layers_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/widgets/progress_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-21 11:44:13.000000 qgis_plugin_tools-0.5.0/widgets/selectable_combobox.py
```

### Comparing `qgis_plugin_tools-0.4.1/LICENSE` & `qgis_plugin_tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/PKG-INFO` & `qgis_plugin_tools-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgis_plugin_tools
-Version: 0.4.1
+Version: 0.5.0
 Summary: A collection of helpful tools and widgets to aid QGIS plugin tool development
 Home-page: https://github.com/GispoCoding/qgis_plugin_tools
 Author: 3Liz, Gispo Ltd.
 Author-email: info@gispo.fi
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 License: GNU GPL v2.0
```

### Comparing `qgis_plugin_tools-0.4.1/README.md` & `qgis_plugin_tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/infrastructure/debugging.py` & `qgis_plugin_tools-0.5.0/infrastructure/debugging.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/infrastructure/plugin_maker.py` & `qgis_plugin_tools-0.5.0/infrastructure/plugin_maker.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/qgis_plugin_tools.egg-info/PKG-INFO` & `qgis_plugin_tools-0.5.0/qgis_plugin_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgis_plugin_tools
-Version: 0.4.1
+Version: 0.5.0
 Summary: A collection of helpful tools and widgets to aid QGIS plugin tool development
 Home-page: https://github.com/GispoCoding/qgis_plugin_tools
 Author: 3Liz, Gispo Ltd.
 Author-email: info@gispo.fi
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 License: GNU GPL v2.0
```

### Comparing `qgis_plugin_tools-0.4.1/qgis_plugin_tools.egg-info/SOURCES.txt` & `qgis_plugin_tools-0.5.0/qgis_plugin_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/resources/ui/progress_dialog.ui` & `qgis_plugin_tools-0.5.0/resources/ui/progress_dialog.ui`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/setup.cfg` & `qgis_plugin_tools-0.5.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [isort]
 profile = black
 multi_line_output = 3
 
 [metadata]
 name = qgis_plugin_tools
-version = 0.4.1
+version = 0.5.0
 author = 3Liz, Gispo Ltd.
 author_email = info@gispo.fi
 maintainer = Gispo Ltd.
 maintainer_email = info@gispo.fi
 description = A collection of helpful tools and widgets to aid QGIS plugin tool development
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `qgis_plugin_tools-0.4.1/setup.py` & `qgis_plugin_tools-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/test/test_decorations.py` & `qgis_plugin_tools-0.5.0/test/test_decorations.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/test/test_init.py` & `qgis_plugin_tools-0.5.0/test/test_init.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/test/test_logging.py` & `qgis_plugin_tools-0.5.0/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/test/test_network.py` & `qgis_plugin_tools-0.5.0/test/test_network.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/test/test_raster_layers.py` & `qgis_plugin_tools-0.5.0/test/test_raster_layers.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/test/test_setings.py` & `qgis_plugin_tools-0.5.0/test/test_setings.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/test/test_tasks.py` & `qgis_plugin_tools-0.5.0/test/test_tasks.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/testing/utilities.py` & `qgis_plugin_tools-0.5.0/testing/utilities.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/algorithm_processing.py` & `qgis_plugin_tools-0.5.0/tools/algorithm_processing.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/custom_logging.py` & `qgis_plugin_tools-0.5.0/tools/custom_logging.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/decorations.py` & `qgis_plugin_tools-0.5.0/tools/decorations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 __copyright__ = "Copyright 2020-2021, Gispo Ltd"
 __license__ = "GPL version 2"
 __email__ = "info@gispo.fi"
 __revision__ = "$Format:%H$"
 
-from typing import Any, Callable
+from typing import Any, Callable, Optional
 
 from .exceptions import QgsPluginException
 from .i18n import tr
-from .messages import MsgBar
+from .messages import MessageBarLogger
 from .tasks import FunctionTask
 
 
-def log_if_fails(fn: Callable) -> Callable:
+def log_if_fails(
+    fn: Optional[Callable] = None, /, *, logger_name: str = __name__
+) -> Callable:
     """
     Use this as a decorator with functions and methods that
     might throw uncaught exceptions.
     """
     from functools import wraps
 
-    @wraps(fn)
-    def wrapper(*args: Any, **kwargs: Any) -> None:  # noqa: ANN001
-        try:
-            # Qt injects False into some signals
-            if args[1:] != (False,):
-                fn(*args, **kwargs)
-            else:
-                fn(*args[:-1], **kwargs)
-        except QgsPluginException as e:
-            MsgBar.exception(e, **e.bar_msg, stack_info=True)
-        except Exception as e:
-            MsgBar.exception(tr("Unhandled exception occurred"), e, stack_info=True)
+    # caller is at depth 3 (MessageBarLogger log call, this function, actual call)
+    message_bar = MessageBarLogger(logger_name, stack_level=3)
 
-    return wrapper
+    def decorator(fn: Callable) -> Callable:
+        @wraps(fn)
+        def wrapper(*args: Any, **kwargs: Any) -> None:  # noqa: ANN001
+            try:
+                # Qt injects False into some signals
+                if args[1:] != (False,):
+                    fn(*args, **kwargs)
+                else:
+                    fn(*args[:-1], **kwargs)
+            except QgsPluginException as e:
+                message_bar.exception(e, **e.bar_msg, stack_info=True)
+            except Exception as e:
+                message_bar.exception(
+                    tr("Unhandled exception occurred"), e, stack_info=True
+                )
+
+        return wrapper
+
+    if fn is None:
+        return decorator
+
+    return decorator(fn)
 
 
 def taskify(fn: Callable) -> Callable:
     """
     Decoration used to turn any function or method into a FunctionTask task.
     """
     from functools import wraps
```

### Comparing `qgis_plugin_tools-0.4.1/tools/exceptions.py` & `qgis_plugin_tools-0.5.0/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/fields.py` & `qgis_plugin_tools-0.5.0/tools/fields.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/ghost_layers.py` & `qgis_plugin_tools-0.5.0/tools/ghost_layers.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/i18n.py` & `qgis_plugin_tools-0.5.0/tools/i18n.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/layers.py` & `qgis_plugin_tools-0.5.0/tools/layers.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/logger_processing.py` & `qgis_plugin_tools-0.5.0/tools/logger_processing.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/messages.py` & `qgis_plugin_tools-0.5.0/tools/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     """
     logging.Logger like interface to push messages to the
     message bar where necessary with info/warning/etc methods.
 
     Setup with a logger name that has a message bar set.
     """
 
-    def __init__(self, logger_name: str) -> None:
+    def __init__(self, logger_name: str, stack_level: int = 2) -> None:
         self._logger = logging.getLogger(logger_name)
         self._logger_kwargs: Dict[str, Any] = (
             {}
             if sys.version_info.major == 3 and sys.version_info.minor < 8
-            else {"stacklevel": 2}
+            else {"stacklevel": stack_level}
         )
 
     def info(
         self,
         message: Any,
         details: Any = "",
         duration: Optional[int] = None,
@@ -144,18 +144,24 @@
         :param duration: can be used to specify the message timeout in seconds. If
             ``duration`` is set to 0, then the message must be manually dismissed
             by the user.
         :param success: Whether the message is success message or not
         :param exc_info: Exception of handled exception for capturing traceback
         :param stack_info: Whether to include stack info
         """
-        self._logger.exception(
+        # for some reason using logger.exception will essentially have extra stack level
+        # even though its not visible on the printed stack (possibly due to exception
+        # being a simple helper which calls error internally). use plain error here to
+        # have same effective stacklevel on both actual log records. possibly related
+        # https://github.com/python/cpython/issues/89334 has been fixed in 3.11+
+        self._logger.error(
             str(message),
             extra=bar_msg(details, duration, success),
             stack_info=stack_info,
+            exc_info=True,
             **self._logger_kwargs,
         )
         if details != "":
             self._logger.error(
                 str(details),
                 exc_info=exc_info,
                 stack_info=stack_info,
```

### Comparing `qgis_plugin_tools-0.4.1/tools/misc_utils.py` & `qgis_plugin_tools-0.5.0/tools/misc_utils.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/network.py` & `qgis_plugin_tools-0.5.0/tools/network.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/raster_layers.py` & `qgis_plugin_tools-0.5.0/tools/raster_layers.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/resources.py` & `qgis_plugin_tools-0.5.0/tools/resources.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/settings.py` & `qgis_plugin_tools-0.5.0/tools/settings.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/tasks.py` & `qgis_plugin_tools-0.5.0/tools/tasks.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/ui.py` & `qgis_plugin_tools-0.5.0/tools/ui.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/tools/version.py` & `qgis_plugin_tools-0.5.0/tools/version.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/widgets/grid_layout_utils.py` & `qgis_plugin_tools-0.5.0/widgets/grid_layout_utils.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/widgets/list_fields_selection.py` & `qgis_plugin_tools-0.5.0/widgets/list_fields_selection.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/widgets/list_layers_selection.py` & `qgis_plugin_tools-0.5.0/widgets/list_layers_selection.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/widgets/progress_dialog.py` & `qgis_plugin_tools-0.5.0/widgets/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `qgis_plugin_tools-0.4.1/widgets/selectable_combobox.py` & `qgis_plugin_tools-0.5.0/widgets/selectable_combobox.py`

 * *Files identical despite different names*

