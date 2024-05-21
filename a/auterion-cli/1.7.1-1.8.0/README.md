# Comparing `tmp/auterion-cli-1.7.1.tar.gz` & `tmp/auterion-cli-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.7.1.tar", last modified: Mon May 13 12:55:41 2024, max compression
+gzip compressed data, was "auterion-cli-1.8.0.tar", last modified: Tue May 21 15:09:13 2024, max compression
```

## Comparing `auterion-cli-1.7.1.tar` & `auterion-cli-1.8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 12:55:40.000000 auterion-cli-1.7.1/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.562714 auterion-cli-1.7.1/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.562714 auterion-cli-1.7.1/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.562714 auterion-cli-1.7.1/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_inspect_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11456 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4407 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:09:13.636628 auterion-cli-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-21 15:09:13.636628 auterion-cli-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 15:09:12.000000 auterion-cli-1.8.0/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:09:13.632628 auterion-cli-1.8.0/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-21 15:09:13.000000 auterion-cli-1.8.0/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-21 15:09:13.000000 auterion-cli-1.8.0/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:09:13.000000 auterion-cli-1.8.0/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 15:09:13.000000 auterion-cli-1.8.0/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:09:13.000000 auterion-cli-1.8.0/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-21 15:09:13.000000 auterion-cli-1.8.0/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 15:09:13.000000 auterion-cli-1.8.0/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:09:13.632628 auterion-cli-1.8.0/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:09:13.632628 auterion-cli-1.8.0/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:09:13.632628 auterion-cli-1.8.0/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:09:13.636628 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/api-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/api-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app_inspect_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11456 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4407 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:09:13.636628 auterion-cli-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-21 15:09:05.000000 auterion-cli-1.8.0/setup.py
```

### Comparing `auterion-cli-1.7.1/README.md` & `auterion-cli-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.8.0/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_command.py` & `auterion-cli-1.8.0/auterioncli/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-1.json` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/api-1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'definitions'": "{'AuterionAppYmlTargetPlatform': {delete: ['pattern']}}"}*

```diff
@@ -89,12 +89,11 @@
                     "$ref": "#/definitions/AuterionAppYmlService"
                 }
             },
             "title": "AuterionAppYmlServices",
             "type": "object"
         },
         "AuterionAppYmlTargetPlatform": {
-            "pattern": "^skynode|ainode|jetson|rb5|simulation$",
             "type": "string"
         }
     }
 }
```

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-2.json` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/api-2.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962121212121212%*

 * *Differences: {"'definitions'": "{'AuterionAppYmlTargetPlatform': {delete: ['pattern']}}"}*

```diff
@@ -217,12 +217,11 @@
                     "$ref": "#/definitions/AuterionAppYmlService"
                 }
             },
             "title": "AuterionAppYmlServices",
             "type": "object"
         },
         "AuterionAppYmlTargetPlatform": {
-            "pattern": "^skynode|ainode|jetson|rb5|simulation$",
             "type": "string"
         }
     }
 }
```

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777777%*

 * *Differences: {"'definitions'": "{'AuterionAppYmlTargetPlatform': {delete: ['pattern']}}"}*

```diff
@@ -327,12 +327,11 @@
                     "$ref": "#/definitions/AuterionAppYmlService"
                 }
             },
             "title": "AuterionAppYmlServices",
             "type": "object"
         },
         "AuterionAppYmlTargetPlatform": {
-            "pattern": "^skynode|ainode|jetson|rb5|simulation$",
             "type": "string"
         }
     }
 }
```

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 DEVICE_ALIAS = {
     'ainode': 'jetson'
 }
 
 PLATFORM_ALIAS = {
     'skynode': 'linux/arm64',
+    'skynode-s': 'linux/arm64',
     'jetson': 'linux/arm64',
     'rb5': 'linux/arm64',
     'simulation': 'linux/amd64'
 }
 
 
 def deep_dict_update(d, u):
@@ -144,14 +145,17 @@
                   f' entity that authored the app, e.g. `com.auterion`')
         return meta
 
     def _extract_target_devices(self, meta):
         target_devices = [meta['target-platform']] \
             if isinstance(meta['target-platform'], str) else meta['target-platform']
         target_devices = [DEVICE_ALIAS.get(d, d) for d in target_devices]
+        for d in target_devices:
+            if d not in PLATFORM_ALIAS:
+                error(f'Target platform "{d}" is not supported. Must be one of: {", ".join(PLATFORM_ALIAS.keys())}. Aborting.')
         return target_devices
 
     def _extract_target_platform(self, meta):
         target_devices = self._extract_target_devices(meta)
         target_platforms = [PLATFORM_ALIAS.get(d, d) for d in target_devices]
         if len(set(target_platforms)) > 1:
             error('Targets have multiple architectures. Aborting.')
@@ -329,18 +333,24 @@
             target_devices_args += ['-t', d]
 
         if 'simulation' in target_devices:
             out_file = os.path.join(args.project_dir, 'build', slug + '-simulation.auterionos')
         else:
             out_file = os.path.join(args.project_dir, 'build', slug + '.auterionos')
 
-        # re-write auterion-app.yml to temp dir, as it may have changed
+        content_for_packaged_meta_file = copy.deepcopy(meta)
+        if meta['auterion-api-version'] <= 4:
+            # legacy AuterionOS do strictly check for the target platform in schema check. Fake the target platform
+            # in the bundled auterion-app.yml file, so that the schema check passes
+            content_for_packaged_meta_file['target-platform'] = ['skynode']
+
+        # write meta content to a new auterion-app.yml file to be bundled in the app
         meta_file = os.path.join(self._temp_dir, 'auterion-app.yml')
         with open(meta_file, 'w') as f:
-            yaml.dump(meta, f)
+            yaml.dump(content_for_packaged_meta_file, f)
 
         version_file = os.path.join(self._temp_dir, 'version')
         with open(version_file, 'w') as f:
             f.write(version)
 
         settings_file = os.path.join(args.project_dir, 'settings.default.env')
```

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_inspect_command.py` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/app_inspect_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/slimify.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.8.0/auterioncli/commands/app_sdk/update.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/container_command.py` & `auterion-cli-1.8.0/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/device_command.py` & `auterion-cli-1.8.0/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/info_command.py` & `auterion-cli-1.8.0/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/report_command.py` & `auterion-cli-1.8.0/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/commands/utils.py` & `auterion-cli-1.8.0/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/main.py` & `auterion-cli-1.8.0/auterioncli/main.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.1/auterioncli/meta_util.py` & `auterion-cli-1.8.0/auterioncli/meta_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if persist_hash == self._load_hash:
             return
 
         with open(self._config_path, 'w') as f:
             f.write(contents)
 
 
-AUTERION_DEVICES = ['skynode', 'jetson', 'simulation']
+AUTERION_DEVICES = ['skynode', 'skynode-s', 'jetson', 'simulation']
 
 
 def get_host_device_type():
     device_type_file = '/persistent/mender/device_type'
     if os.path.exists(device_type_file):
         with open(device_type_file, 'r') as f:
             for l in f.readlines():
```

### Comparing `auterion-cli-1.7.1/setup.py` & `auterion-cli-1.8.0/setup.py`

 * *Files identical despite different names*

