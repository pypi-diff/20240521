# Comparing `tmp/riogisoffline-0.0.25.tar.gz` & `tmp/riogisoffline-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riogisoffline-0.0.25.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riogisoffline-0.0.26.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riogisoffline-0.0.25.tar` & `riogisoffline-0.0.26.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      717 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/pyproject.toml
--rw-r--r--   0        0        0     1071 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/LICENSE
--rw-r--r--   0        0        0     7264 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/Makefile
--rw-r--r--   0        0        0      261 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/README.md
--rw-r--r--   0        0        0     2217 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/__init__.py
--rw-r--r--   0        0        0      158 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/compile.bat
--rw-r--r--   0        0        0     2810 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/dialog/riogis_dialog_settings.ui
--rw-r--r--   0        0        0     6345 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/dialog/riogis_dockwidget.ui
--rw-r--r--   0        0        0    30219 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/icon.png
--rw-r--r--   0        0        0     1505 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/metadata.txt
--rw-r--r--   0        0        0     1723 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/pb_tool.cfg
--rw-r--r--   0        0        0        2 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/__init__.py
--rw-r--r--   0        0        0     1283 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/azure_blob_storage_connection.py
--rw-r--r--   0        0        0      424 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/dependency_installer.py
--rw-r--r--   0        0        0    17046 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/refresh_map.py
--rw-r--r--   0        0        0   126345 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/resources.py
--rw-r--r--   0        0        0    14047 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/riogis.py
--rw-r--r--   0        0        0     1313 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/riogis_dockedwidget.py
--rw-r--r--   0        0        0     1310 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/settings_dialog.py
--rw-r--r--   0        0        0     7700 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/syncronizer.py
--rw-r--r--   0        0        0     2436 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/user_settings_generator.py
--rw-r--r--   0        0        0     2402 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/utils.py
--rw-r--r--   0        0        0      947 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin/worker.py
--rw-r--r--   0        0        0     3559 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/plugin_upload.py
--rw-r--r--   0        0        0     8798 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/pylintrc
--rw-r--r--   0        0        0       18 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/requirements.txt
--rw-r--r--   0        0        0      102 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/resources.qrc
--rw-r--r--   0        0        0     2740 2024-05-14 13:51:16.502658 riogisoffline-0.0.25/riogisoffline/settings.json
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 riogisoffline-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0      717 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/pyproject.toml
+-rw-r--r--   0        0        0     1071 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/LICENSE
+-rw-r--r--   0        0        0     7264 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/Makefile
+-rw-r--r--   0        0        0      261 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/README.md
+-rw-r--r--   0        0        0     2239 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/compile.bat
+-rw-r--r--   0        0        0     2810 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/dialog/riogis_dialog_settings.ui
+-rw-r--r--   0        0        0     6345 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/dialog/riogis_dockwidget.ui
+-rw-r--r--   0        0        0    30219 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/icon.png
+-rw-r--r--   0        0        0     1505 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/metadata.txt
+-rw-r--r--   0        0        0     1723 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/pb_tool.cfg
+-rw-r--r--   0        0        0      195 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/__init__.py
+-rw-r--r--   0        0        0     1283 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/azure_blob_storage_connection.py
+-rw-r--r--   0        0        0      424 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/dependency_installer.py
+-rw-r--r--   0        0        0    17046 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/refresh_map.py
+-rw-r--r--   0        0        0   126345 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/resources.py
+-rw-r--r--   0        0        0    14047 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/riogis.py
+-rw-r--r--   0        0        0     1313 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/riogis_dockedwidget.py
+-rw-r--r--   0        0        0     1310 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/settings_dialog.py
+-rw-r--r--   0        0        0     7700 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/syncronizer.py
+-rw-r--r--   0        0        0     2436 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/user_settings_generator.py
+-rw-r--r--   0        0        0     2402 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/utils.py
+-rw-r--r--   0        0        0      947 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/worker.py
+-rw-r--r--   0        0        0     3559 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin_upload.py
+-rw-r--r--   0        0        0     8798 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/pylintrc
+-rw-r--r--   0        0        0       18 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/requirements.txt
+-rw-r--r--   0        0        0      102 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/resources.qrc
+-rw-r--r--   0        0        0     2740 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/settings.json
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 riogisoffline-0.0.26/PKG-INFO
```

### Comparing `riogisoffline-0.0.25/pyproject.toml` & `riogisoffline-0.0.26/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "riogisoffline"
-version = "0.0.25"
+version = "0.0.26"
 description = "This Exports attributes of a given feature to a Wincan consumable text file."
 authors = [
   { name = "Vann- og avløpsetaten Oslo kommune", email = "gis@vav.oslo.kommune.no" },
 ]
 license = { file = "riogisoffline/LICENSE" }
 readme = "riogisoffline/README.md"
 classifiers = [
```

### Comparing `riogisoffline-0.0.25/riogisoffline/LICENSE` & `riogisoffline-0.0.26/riogisoffline/LICENSE`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/Makefile` & `riogisoffline-0.0.26/riogisoffline/Makefile`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/__init__.py` & `riogisoffline-0.0.26/riogisoffline/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,16 @@
  *                                                                         *
  *                                                                         *
  *                                                                         *
  *                                                                         *
  ***************************************************************************/
 """
 
+__all__ = ["plugin"]
+
 # noinspection PyPep8Naming
 def classFactory(iface):  # pylint: disable=invalid-name
     """
     Handle directory path environment variable and depencdecies, then load RioGIS from file riogis.
 
     :param iface: A QGIS interface instance.
     :type iface: QgsInterface
```

### Comparing `riogisoffline-0.0.25/riogisoffline/dialog/riogis_dialog_settings.ui` & `riogisoffline-0.0.26/riogisoffline/dialog/riogis_dialog_settings.ui`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/dialog/riogis_dockwidget.ui` & `riogisoffline-0.0.26/riogisoffline/dialog/riogis_dockwidget.ui`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/icon.png` & `riogisoffline-0.0.26/riogisoffline/icon.png`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/metadata.txt` & `riogisoffline-0.0.26/riogisoffline/metadata.txt`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/pb_tool.cfg` & `riogisoffline-0.0.26/riogisoffline/pb_tool.cfg`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/azure_blob_storage_connection.py` & `riogisoffline-0.0.26/riogisoffline/plugin/azure_blob_storage_connection.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/refresh_map.py` & `riogisoffline-0.0.26/riogisoffline/plugin/refresh_map.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/resources.py` & `riogisoffline-0.0.26/riogisoffline/plugin/resources.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/riogis.py` & `riogisoffline-0.0.26/riogisoffline/plugin/riogis.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/riogis_dockedwidget.py` & `riogisoffline-0.0.26/riogisoffline/plugin/riogis_dockedwidget.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/settings_dialog.py` & `riogisoffline-0.0.26/riogisoffline/plugin/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/syncronizer.py` & `riogisoffline-0.0.26/riogisoffline/plugin/syncronizer.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/user_settings_generator.py` & `riogisoffline-0.0.26/riogisoffline/plugin/user_settings_generator.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/utils.py` & `riogisoffline-0.0.26/riogisoffline/plugin/utils.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin/worker.py` & `riogisoffline-0.0.26/riogisoffline/plugin/worker.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/plugin_upload.py` & `riogisoffline-0.0.26/riogisoffline/plugin_upload.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/pylintrc` & `riogisoffline-0.0.26/riogisoffline/pylintrc`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/riogisoffline/settings.json` & `riogisoffline-0.0.26/riogisoffline/settings.json`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.25/PKG-INFO` & `riogisoffline-0.0.26/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riogisoffline
-Version: 0.0.25
+Version: 0.0.26
 Summary: This Exports attributes of a given feature to a Wincan consumable text file.
 Author-email: Vann- og avløpsetaten Oslo kommune <gis@vav.oslo.kommune.no>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

