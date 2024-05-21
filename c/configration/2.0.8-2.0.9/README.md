# Comparing `tmp/configration-2.0.8.tar.gz` & `tmp/configration-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configration-2.0.8.tar", last modified: Tue Apr 16 13:29:04 2024, max compression
+gzip compressed data, was "configration-2.0.9.tar", last modified: Tue May 21 09:49:55 2024, max compression
```

## Comparing `configration-2.0.8.tar` & `configration-2.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.984440 configration-2.0.8/
--rw-r--r--   0 jeff      (1000) jeff      (1000)    33889 2018-03-05 16:24:54.000000 configration-2.0.8/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1000)     1321 2024-04-16 13:29:04.981106 configration-2.0.8/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1000)      115 2023-05-10 10:08:06.000000 configration-2.0.8/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.981106 configration-2.0.8/configration/
--rw-r--r--   0 jeff      (1000) jeff      (1000)      175 2023-05-29 08:17:28.000000 configration-2.0.8/configration/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1000)       22 2024-04-16 13:27:15.000000 configration-2.0.8/configration/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.981106 configration-2.0.8/configration/src/
--rw-r--r--   0 jeff      (1000) jeff      (1000)        0 2023-06-29 13:36:12.000000 configration-2.0.8/configration/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1000)     2791 2024-04-16 13:26:52.000000 configration-2.0.8/configration/src/config.py
--rw-r--r--   0 jeff      (1000) jeff      (1000)      397 2023-06-29 13:36:12.000000 configration-2.0.8/configration/src/constants.py
--rw-r--r--   0 jeff      (1000) jeff      (1000)     1509 2023-06-29 13:36:12.000000 configration-2.0.8/configration/src/json_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1000)     2019 2023-08-06 15:04:48.000000 configration-2.0.8/configration/src/toml_config.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.981106 configration-2.0.8/configration/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1000)        0 2023-06-29 13:36:12.000000 configration-2.0.8/configration/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1000)     2909 2023-06-29 13:36:12.000000 configration-2.0.8/configration/tests/test_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1000)     1762 2023-06-29 13:36:12.000000 configration-2.0.8/configration/tests/test_json.py
--rw-r--r--   0 jeff      (1000) jeff      (1000)     2257 2023-08-06 15:30:14.000000 configration-2.0.8/configration/tests/test_toml.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.981106 configration-2.0.8/configration.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1000)     1321 2024-04-16 13:29:04.000000 configration-2.0.8/configration.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1000)      513 2024-04-16 13:29:04.000000 configration-2.0.8/configration.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1000)        1 2024-04-16 13:29:04.000000 configration-2.0.8/configration.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1000)       13 2024-04-16 13:29:04.000000 configration-2.0.8/configration.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1000)       38 2024-04-16 13:29:04.984440 configration-2.0.8/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1000)     1158 2023-12-03 12:32:36.000000 configration-2.0.8/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-05-21 09:49:55.255818 configration-2.0.9/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    33889 2018-03-05 16:24:54.000000 configration-2.0.9/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1321 2024-05-21 09:49:55.255818 configration-2.0.9/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      115 2023-05-10 10:08:06.000000 configration-2.0.9/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-05-21 09:49:55.255818 configration-2.0.9/configration/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      175 2023-05-29 08:17:28.000000 configration-2.0.9/configration/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)       22 2024-05-21 09:46:05.000000 configration-2.0.9/configration/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-05-21 09:49:55.255818 configration-2.0.9/configration/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        0 2023-06-29 13:36:12.000000 configration-2.0.9/configration/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2886 2024-05-21 09:25:03.000000 configration-2.0.9/configration/src/config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      398 2024-05-21 09:26:38.000000 configration-2.0.9/configration/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1617 2024-05-21 09:41:49.000000 configration-2.0.9/configration/src/json_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2126 2024-05-21 09:39:26.000000 configration-2.0.9/configration/src/toml_config.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-05-21 09:49:55.255818 configration-2.0.9/configration/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        0 2023-06-29 13:36:12.000000 configration-2.0.9/configration/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2909 2023-06-29 13:36:12.000000 configration-2.0.9/configration/tests/test_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1762 2023-06-29 13:36:12.000000 configration-2.0.9/configration/tests/test_json.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2257 2023-08-06 15:30:14.000000 configration-2.0.9/configration/tests/test_toml.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-05-21 09:49:55.255818 configration-2.0.9/configration.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1321 2024-05-21 09:49:55.000000 configration-2.0.9/configration.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      513 2024-05-21 09:49:55.000000 configration-2.0.9/configration.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        1 2024-05-21 09:49:55.000000 configration-2.0.9/configration.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)       13 2024-05-21 09:49:55.000000 configration-2.0.9/configration.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)       38 2024-05-21 09:49:55.255818 configration-2.0.9/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1158 2023-12-03 12:32:36.000000 configration-2.0.9/setup.py
```

### Comparing `configration-2.0.8/LICENSE.txt` & `configration-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configration-2.0.8/PKG-INFO` & `configration-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.8
+Version: 2.0.9
 Summary: """A utility for json or toml config files."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
```

### Comparing `configration-2.0.8/configration/src/config.py` & `configration-2.0.9/configration/src/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def __init__(
             self,
             path: str,
             defaults: dict[str, str] = {},
             attrs: dict[str, list[type]] = {},
             create: bool = False
-        ):
+            ):
         self.path = path
         self.defaults = defaults
         self.attrs = attrs
         self.create = create
         self.config = self._get_config()
         for key, item in self.config.items():
             self.__dict__[key] = item
@@ -70,21 +70,25 @@
             return self.defaults
         return {}
 
     def _validate_config(self, config: dict[str, type]) -> bool:
         # Return True if structure and values in config are valid.
         for name, item_types in self.attrs.items():
             if name not in config:
-                cprint(f"{CORRUPT_FILE_MSG} {MISSING_ATTR_MSG} {name}", ERROR_COLOUR)
+                cprint(f'{CORRUPT_FILE_MSG} {MISSING_ATTR_MSG} {name}',
+                       ERROR_COLOUR)
                 return False
             if type(config[name]) not in item_types:
-                cprint(f"{CORRUPT_FILE_MSG} {name} {NOT_OF_TYPE_MSG} {item_types}", ERROR_COLOUR)
+                cprint(
+                    (f'{CORRUPT_FILE_MSG} {name} {NOT_OF_TYPE_MSG} '
+                     f'{item_types}'),
+                    ERROR_COLOUR)
                 return False
         return True
 
     def update(self, field: str, value: object, force: bool = False) -> None:
         """Update the value of an attribute in config."""
         if not force and field not in self.__dict__['config']:
-            cprint(f"{FIELD} {field} {NOT_IN_DICT}", ERROR_COLOUR)
+            cprint(f'{FIELD} {field} {NOT_IN_DICT}', ERROR_COLOUR)
             return
 
         self.__dict__['config'][field] = value
```

### Comparing `configration-2.0.8/configration/src/json_config.py` & `configration-2.0.9/configration/src/json_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Return a valid config object from a json file for the application."""
 
+from pathlib import Path
 import json
 from termcolor import cprint
 import colorama
 
 from .config import Config
 from .constants import ERROR_COLOUR, LOCATION_ERR_MSG, INVALID_JSON_MSG
 
@@ -16,14 +17,16 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _read_config(self) -> dict[str, object]:
         # Open the config file and return the contents as a dict
+        if not self.path.parent.is_dir():
+            Path.mkdir(self.path.parent)
         try:
             with open(self.path, 'r') as f_config:
                 try:
                     return json.load(f_config)
                 except json.decoder.JSONDecodeError:
                     cprint(f"{INVALID_JSON_MSG} {self.path }", ERROR_COLOUR)
         except FileNotFoundError:
```

### Comparing `configration-2.0.8/configration/src/toml_config.py` & `configration-2.0.9/configration/src/toml_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Return a valid config object from a toml file for the application."""
-
+from pathlib import Path
 import tomli
 import tomli_w
 from termcolor import cprint
 import colorama
 
 from .config import Config
 from .constants import ERROR_COLOUR, LOCATION_ERR_MSG, INVALID_TOML_MSG
@@ -20,14 +20,16 @@
     status_OK = 1
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _read_config(self) -> dict[str, object]:
         # Open the config file and return the contents as a dict
+        if not self.path.parent.is_dir():
+            Path.mkdir(self.path.parent)
         try:
             with open(self.path, 'rb') as f_config:
                 try:
                     return tomli.load(f_config)
                 except tomli.TOMLDecodeError:
                     cprint(f"{INVALID_TOML_MSG} {self.path }", ERROR_COLOUR)
         except FileNotFoundError:
```

### Comparing `configration-2.0.8/configration/tests/test_config.py` & `configration-2.0.9/configration/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.8/configration/tests/test_json.py` & `configration-2.0.9/configration/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.8/configration/tests/test_toml.py` & `configration-2.0.9/configration/tests/test_toml.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.8/configration.egg-info/PKG-INFO` & `configration-2.0.9/configration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.8
+Version: 2.0.9
 Summary: """A utility for json or toml config files."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
```

### Comparing `configration-2.0.8/configration.egg-info/SOURCES.txt` & `configration-2.0.9/configration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `configration-2.0.8/setup.py` & `configration-2.0.9/setup.py`

 * *Files identical despite different names*

