# Comparing `tmp/libreflow_extensions_anpo_scene_builder-1.0.0.tar.gz` & `tmp/libreflow_extensions_anpo_scene_builder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_extensions_anpo_scene_builder-1.0.0.tar", last modified: Wed May 15 22:41:43 2024, max compression
+gzip compressed data, was "libreflow_extensions_anpo_scene_builder-1.0.2.tar", last modified: Tue May 21 10:28:45 2024, max compression
```

## Comparing `libreflow_extensions_anpo_scene_builder-1.0.0.tar` & `libreflow_extensions_anpo_scene_builder-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:41:43.284791 libreflow_extensions_anpo_scene_builder-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1219 2024-05-15 22:41:43.284791 libreflow_extensions_anpo_scene_builder-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-15 22:41:43.284791 libreflow_extensions_anpo_scene_builder-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:41:43.279791 libreflow_extensions_anpo_scene_builder-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:41:43.281791 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:41:43.282791 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/extensions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:41:43.282791 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/extensions/anpo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/extensions/anpo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:41:43.283791 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/extensions/anpo/scene_builder/
--rw-rw-rw-   0 root         (0) root         (0)    19182 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/extensions/anpo/scene_builder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-15 22:41:43.284791 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/extensions/anpo/scene_builder/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/extensions/anpo/scene_builder/build_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:41:43.283791 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow.extensions.anpo.scene_builder.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1219 2024-05-15 22:41:43.000000 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow.extensions.anpo.scene_builder.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      611 2024-05-15 22:41:43.000000 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow.extensions.anpo.scene_builder.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 22:41:43.000000 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow.extensions.anpo.scene_builder.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-15 22:41:43.000000 libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow.extensions.anpo.scene_builder.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-15 22:41:33.000000 libreflow_extensions_anpo_scene_builder-1.0.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.428262 libreflow_extensions_anpo_scene_builder-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1561 2024-05-21 10:28:45.428262 libreflow_extensions_anpo_scene_builder-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-21 10:28:45.429262 libreflow_extensions_anpo_scene_builder-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.423262 libreflow_extensions_anpo_scene_builder-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.426262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.427262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.427262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.428262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/
+-rw-rw-rw-   0 root         (0) root         (0)    19915 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-21 10:28:45.429262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/build_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.428262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1561 2024-05-21 10:28:45.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-21 10:28:45.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:28:45.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-21 10:28:45.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/versioneer.py
```

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.0/CHANGELOG.md` & `libreflow_extensions_anpo_scene_builder-1.0.2/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,12 +15,24 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.2] - 2024-05-21
+
+### Added
+
+* An option to refresh dependencies (which might be updated in Kitsu before the cache invalidates).
+
+## [1.0.1] - 2024-05-16
+
+### Changed
+
+* A layout scene is now built with the video of the animatic (in addition to its audio track), using the updated LFS Playblast `scene_builder_add_animatic` operator.
+
 ## [1.0.0] - 2024-05-16
 
 ### Added
 
 * initial release
```

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.0/PKG-INFO` & `libreflow_extensions_anpo_scene_builder-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.scene-builder
-Version: 1.0.0
+Version: 1.0.2
 Home-page: https://gitlab.com/lfs.coop/libreflow/extensions/anpo/scene_builder
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -34,12 +34,24 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.2] - 2024-05-21
+
+### Added
+
+* An option to refresh dependencies (which might be updated in Kitsu before the cache invalidates).
+
+## [1.0.1] - 2024-05-16
+
+### Changed
+
+* A layout scene is now built with the video of the animatic (in addition to its audio track), using the updated LFS Playblast `scene_builder_add_animatic` operator.
+
 ## [1.0.0] - 2024-05-16
 
 ### Added
 
 * initial release
```

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.0/setup.py` & `libreflow_extensions_anpo_scene_builder-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow/extensions/anpo/scene_builder/__init__.py` & `libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 import glob
 import time
 from kabaret import flow
 from kabaret.app import resources
 from libreflow.baseflow.file import GenericRunAction
 from libreflow.baseflow.task import Task
+from libreflow.resources.icons import gui as _
 from .build_utils import wrap_python_expr
 
 from . import _version
 __version__ = _version.get_versions()['version']
 
 
 class AssetStatus(flow.values.ChoiceValue):
@@ -110,15 +111,28 @@
                 child_value.set("Available")
             elif self.asset_file_oid.get():
                 child_value.set("Downloadable")
             else:
                 child_value.set("NotAvailable")
 
 
+class RefreshDependencies(flow.Action):
+    ICON = ('icons.gui', 'refresh')
+    _map = flow.Parent()
+
+    def needs_dialog(self):
+        return False
+
+    def run(self, button):
+        self._map.refresh()
+
+
 class LayoutDependencies(flow.DynamicMap):
+    refresh_action = flow.Child(RefreshDependencies).ui(
+        label="Refresh")
     _task = flow.Parent(2)
     _shot = flow.Parent(4)
     _sequence = flow.Parent(6)
     _updated = flow.BoolParam(False)
 
     def __init__(self, parent, name):
         super(LayoutDependencies, self).__init__(parent, name)
@@ -181,14 +195,18 @@
             return asset.tasks['design'].files
         elif asset_type == 'animatic':
             return self._task.files
         elif asset.tasks.has_mapped_name('rigging'):
             return asset.tasks['rigging'].files
         else:
             return None
+
+    def refresh(self):
+        self._assets_data = None
+        self.touch()
     
     def _fill_row_cells(self, row, item):
         row["Name"] = item.name()
         row["Type"] = item.asset_type.get()
         row["Family"] = item.asset_family.get()
         
         rev_oid = item.asset_revision_oid.get()
@@ -296,36 +314,43 @@
 
         return revision.get_path()
 
     def _blender_cmd(self, operator, **kwargs):
         '''
         Returns Blender scene builder operator command as a string.
 
-        Operator must be one of the following: `setup`, `setup_anim`,
-                                               `add_asset`, `add_set`, `add_audio`, `add_board`,
-                                               `update_audio", "update_storyboard`,
-                                               `export_ae`,
-                                               `cleanup`, `save`.
+        Operator must be one of the following:
+        `setup`, `setup_anim`,
+        `add_asset`, `add_set`,
+        `add_animatic`, `update_animatic`,
+        `add_audio`, `add_board`, (deprecated, use add_animatic instead)
+        `update_audio`, `update_board`, (deprecated, use update_animatic instead without args)
+        `export_ae`, `setup_render`,
+        `cleanup`, `save`.
         '''
 
         blender_operators = {
             "setup": {'operator_command': "bpy.ops.pipeline.scene_builder_setup",
                       'args': "frame_start={frame_start}, frame_end={frame_end}, resolution_x={resolution_x}, resolution_y={resolution_y}, fps={fps}, create_camera=False"},
             "setup_anim": {'operator_command': "bpy.ops.pipeline.scene_builder_setup_animation",
                            'args': 'alembic_filepath="{alembic_filepath}", assets={assets}, do_automate={do_automate}'},
 
             "add_asset": {'operator_command': 'bpy.ops.pipeline.scene_builder_import_asset',
                           'args': 'filepath="{filepath}", asset_name="{asset_name}", target_collection="{asset_type}"'},
+            "add_animatic": {'operator_command': 'bpy.ops.pipeline.scene_builder_add_animatic',
+                             'args': 'filepath="{filepath}"'},
             "add_set": {'operator_command': 'bpy.ops.pipeline.scene_builder_import_set',
                         'args': 'directory="{set_dir}", files={set_dicts}'},
             "add_audio": {'operator_command': 'bpy.ops.pipeline.scene_builder_import_audio',
                           'args': 'filepath="{filepath}"'},
             "add_board": {'operator_command': 'bpy.ops.pipeline.scene_builder_import_storyboard',
                           'args': 'filepath="{filepath}", use_corner={use_corner}'},
 
+            "update_animatic": {'operator_command': 'bpy.ops.pipeline.scene_builder_update_animatic',
+                                'args': ''},
             "update_audio": {'operator_command': 'bpy.ops.pipeline.scene_builder_update_audio',
                              'args' :''},
             "update_board": {'operator_command': 'bpy.ops.pipeline.scene_builder_update_storyboard',
                              'args' :'filepath="{filepath}"'},
 
             "export_ae": {'operator_command': 'bpy.ops.pipeline.scene_builder_export_ae',
                           'args' :'filepath="{filepath}"'},
@@ -372,15 +397,15 @@
         
         for name, path, asset_type, asset_number in assets:
             for i in range(asset_number):
                 python_expr += self._blender_cmd("add_asset", filepath=path, asset_name=name, asset_type=asset_type)
         for set_dir, set_dicts in sets:
             python_expr += self._blender_cmd("add_set", set_dir=set_dir, set_dicts=set_dicts)
         if animatic_path:
-            python_expr += self._blender_cmd("add_audio", filepath=animatic_path)
+            python_expr += self._blender_cmd("add_animatic", filepath=animatic_path)
 
         # python_expr += self._blender_cmd("cleanup")
         python_expr += self._blender_cmd("save", filepath=layout_path)
 
         return [
             "-b", template_path,
             "--addons", "io_import_images_as_planes,camera_plane,lfs_scene_builder,add_camera_rigs",
```

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow.extensions.anpo.scene_builder.egg-info/PKG-INFO` & `libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.scene-builder
-Version: 1.0.0
+Version: 1.0.2
 Home-page: https://gitlab.com/lfs.coop/libreflow/extensions/anpo/scene_builder
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -34,12 +34,24 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.2] - 2024-05-21
+
+### Added
+
+* An option to refresh dependencies (which might be updated in Kitsu before the cache invalidates).
+
+## [1.0.1] - 2024-05-16
+
+### Changed
+
+* A layout scene is now built with the video of the animatic (in addition to its audio track), using the updated LFS Playblast `scene_builder_add_animatic` operator.
+
 ## [1.0.0] - 2024-05-16
 
 ### Added
 
 * initial release
```

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.0/src/libreflow.extensions.anpo.scene_builder.egg-info/SOURCES.txt` & `libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.0/versioneer.py` & `libreflow_extensions_anpo_scene_builder-1.0.2/versioneer.py`

 * *Files identical despite different names*

