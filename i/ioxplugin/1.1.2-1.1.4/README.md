# Comparing `tmp/ioxplugin-1.1.2.tar.gz` & `tmp/ioxplugin-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioxplugin-1.1.2.tar", last modified: Mon May 20 01:25:57 2024, max compression
+gzip compressed data, was "ioxplugin-1.1.4.tar", last modified: Tue May 21 11:10:01 2024, max compression
```

## Comparing `ioxplugin-1.1.2.tar` & `ioxplugin-1.1.4.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:25:57.889429 ioxplugin-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-20 01:25:57.889429 ioxplugin-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:25:57.889429 ioxplugin-1.1.2/ioxplugin/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50220 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/ast_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/iox_controller_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/iox_main_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/iox_node_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    10709 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/iox_node_impl_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/iox_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/iox_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/main_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/node_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/nodedef.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/oauth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/plugin_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/uom.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/ioxplugin/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:25:57.889429 ioxplugin-1.1.2/ioxplugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-20 01:25:57.000000 ioxplugin-1.1.2/ioxplugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 01:25:57.000000 ioxplugin-1.1.2/ioxplugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:25:57.000000 ioxplugin-1.1.2/ioxplugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 01:25:57.000000 ioxplugin-1.1.2/ioxplugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 01:25:57.000000 ioxplugin-1.1.2/ioxplugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:25:57.889429 ioxplugin-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:25:57.889429 ioxplugin-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/tests/test_ioxplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-20 01:25:51.000000 ioxplugin-1.1.2/tests/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:10:01.377989 ioxplugin-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-21 11:10:01.377989 ioxplugin-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:10:01.373989 ioxplugin-1.1.4/ioxplugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50220 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/ast_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/iox_controller_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/iox_main_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/iox_node_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10709 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/iox_node_impl_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/iox_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/iox_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/main_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/nodedef.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/oauth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/plugin_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/uom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/ioxplugin/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:10:01.377989 ioxplugin-1.1.4/ioxplugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-21 11:10:01.000000 ioxplugin-1.1.4/ioxplugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-21 11:10:01.000000 ioxplugin-1.1.4/ioxplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:10:01.000000 ioxplugin-1.1.4/ioxplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 11:10:01.000000 ioxplugin-1.1.4/ioxplugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 11:10:01.000000 ioxplugin-1.1.4/ioxplugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:10:01.377989 ioxplugin-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:10:01.377989 ioxplugin-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/tests/ModbusControllerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/tests/ModbusDeviceNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/tests/ModbusProtocolHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/tests/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/tests/test_ioxplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 11:09:57.000000 ioxplugin-1.1.4/tests/version.py
```

### Comparing `ioxplugin-1.1.2/PKG-INFO` & `ioxplugin-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.1.2
+Version: 1.1.4
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.1.2/ioxplugin/__init__.py` & `ioxplugin-1.1.4/ioxplugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/ast_util.py` & `ioxplugin-1.1.4/ioxplugin/ast_util.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/commands.py` & `ioxplugin-1.1.4/ioxplugin/commands.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/editor.py` & `ioxplugin-1.1.4/ioxplugin/editor.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/iox_controller_template.py` & `ioxplugin-1.1.4/ioxplugin/iox_controller_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         except Exception as ex:
             LOGGER.error(str(ex))
             return False
 
     def stop(self):
         LOGGER.info(f'Stopping ... ')
         self.protocolHandler.stop()
-        self.updateStatus(0)
+        self.updateStatus(0,True)
         return True
 
     def poll(self, polltype):
         if 'shortPoll' in polltype:
             self.protocolHandler.shortPoll()
         elif 'longPoll' in polltype:
             self.protocolHandler.longPoll()
```

### Comparing `ioxplugin-1.1.2/ioxplugin/iox_main_template.py` & `ioxplugin-1.1.4/ioxplugin/iox_main_template.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/iox_node_gen.py` & `ioxplugin-1.1.4/ioxplugin/iox_node_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/iox_node_impl_gen.py` & `ioxplugin-1.1.4/ioxplugin/iox_node_impl_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/iox_profile.py` & `ioxplugin-1.1.4/ioxplugin/iox_profile.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/iox_transport.py` & `ioxplugin-1.1.4/ioxplugin/iox_transport.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/log.py` & `ioxplugin-1.1.4/ioxplugin/log.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/main_gen.py` & `ioxplugin-1.1.4/ioxplugin/main_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/new_project.py` & `ioxplugin-1.1.4/ioxplugin/new_project.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/node_properties.py` & `ioxplugin-1.1.4/ioxplugin/node_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,14 +100,30 @@
         out = {}
         for np in self.node_properties:
             node_property:NodePropertyDetails = self.node_properties[np]
             out[node_property.id] = node_property.protocol_data
 
         return out
 
+    def getPrecisions(self):
+        precisions = {} 
+        for np in self.node_properties:
+            prop = self.node_properties[np]
+            if prop == None:
+                continue
+            editor = Editors.getEditors().editors[prop.editor.getEditorId()]
+            precision = 0
+            try:
+                precision = int(editor.precision)
+            except Exception as ex:
+                pass
+            precisions[prop.id] = precision
+        return precisions
+
+
     def getPG3Drivers(self):
         drivers = []
         for np in self.node_properties:
             prop = self.node_properties[np]
             if prop == None:
                 continue
             editor = Editors.getEditors().editors[prop.editor.getEditorId()]
```

### Comparing `ioxplugin-1.1.2/ioxplugin/nodedef.py` & `ioxplugin-1.1.4/ioxplugin/nodedef.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,17 @@
             if 'commands' in node:
                 self.commands=Commands(node['commands'])
 
         except Exception as ex:
             LOGGER.critical(str(ex))
             raise
 
+    def getPrecisions(self):
+        return self.properties.getPrecisions()
+
     def getPG3Commands(self):
         commands = []
 
         for c in self.commands.acceptCommands:
             command = self.commands.acceptCommands[c]
             commands.append(
                 {
```

### Comparing `ioxplugin-1.1.2/ioxplugin/oauth_service.py` & `ioxplugin-1.1.4/ioxplugin/oauth_service.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/plugin.py` & `ioxplugin-1.1.4/ioxplugin/plugin.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/plugin_meta.py` & `ioxplugin-1.1.4/ioxplugin/plugin_meta.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/properties.py` & `ioxplugin-1.1.4/ioxplugin/properties.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/protocol.py` & `ioxplugin-1.1.4/ioxplugin/protocol.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/uom.py` & `ioxplugin-1.1.4/ioxplugin/uom.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin/validator.py` & `ioxplugin-1.1.4/ioxplugin/validator.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.2/ioxplugin.egg-info/PKG-INFO` & `ioxplugin-1.1.4/ioxplugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.1.2
+Version: 1.1.4
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.1.2/setup.py` & `ioxplugin-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ioxplugin',
-    version='1.1.2',
+    version='1.1.4',
     packages=find_packages(),
     description='IoX Plugin Helper Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Michel Kohanim',
     author_email='support@universal-devices.com',
     url='https://github.com/universaldevices/ioxplugin.git',
```

