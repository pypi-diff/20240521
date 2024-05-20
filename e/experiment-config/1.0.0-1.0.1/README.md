# Comparing `tmp/experiment-config-1.0.0.tar.gz` & `tmp/experiment-config-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-config-1.0.0.tar", last modified: Tue Mar 19 00:53:10 2024, max compression
+gzip compressed data, was "experiment-config-1.0.1.tar", last modified: Mon May 20 22:19:49 2024, max compression
```

## Comparing `experiment-config-1.0.0.tar` & `experiment-config-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,38 @@
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-03-19 00:53:10.440775 experiment-config-1.0.0/
--rw-r--r--   0 ahalev     (502) staff       (20)     1073 2023-01-29 22:38:50.000000 experiment-config-1.0.0/LICENSE.txt
--rw-r--r--   0 ahalev     (502) staff       (20)     9246 2024-03-19 00:53:10.440492 experiment-config-1.0.0/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)     8789 2023-05-31 22:41:55.000000 experiment-config-1.0.0/README.md
--rw-r--r--   0 ahalev     (502) staff       (20)       38 2024-03-19 00:53:10.440832 experiment-config-1.0.0/setup.cfg
--rw-r--r--   0 ahalev     (502) staff       (20)     1010 2024-03-19 00:50:33.000000 experiment-config-1.0.0/setup.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-03-19 00:53:10.436496 experiment-config-1.0.0/src/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-03-19 00:53:10.437860 experiment-config-1.0.0/src/experiment_config.egg-info/
--rw-r--r--   0 ahalev     (502) staff       (20)     9246 2024-03-19 00:53:10.000000 experiment-config-1.0.0/src/experiment_config.egg-info/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)      592 2024-03-19 00:53:10.000000 experiment-config-1.0.0/src/experiment_config.egg-info/SOURCES.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2024-03-19 00:53:10.000000 experiment-config-1.0.0/src/experiment_config.egg-info/dependency_links.txt
--rw-r--r--   0 ahalev     (502) staff       (20)       71 2024-03-19 00:53:10.000000 experiment-config-1.0.0/src/experiment_config.egg-info/requires.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        7 2024-03-19 00:53:10.000000 experiment-config-1.0.0/src/experiment_config.egg-info/top_level.txt
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-03-19 00:53:10.438601 experiment-config-1.0.0/src/expfig/
--rw-r--r--   0 ahalev     (502) staff       (20)      183 2023-11-21 03:55:56.000000 experiment-config-1.0.0/src/expfig/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    13149 2024-03-19 00:49:48.000000 experiment-config-1.0.0/src/expfig/fig.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-03-19 00:53:10.439178 experiment-config-1.0.0/src/expfig/functions/
--rw-r--r--   0 ahalev     (502) staff       (20)      107 2023-11-21 03:55:56.000000 experiment-config-1.0.0/src/expfig/functions/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1955 2024-03-19 00:49:48.000000 experiment-config-1.0.0/src/expfig/functions/_flatten.py
--rw-r--r--   0 ahalev     (502) staff       (20)     3250 2024-03-19 00:49:48.000000 experiment-config-1.0.0/src/expfig/functions/_parse.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-03-19 00:53:10.439741 experiment-config-1.0.0/src/expfig/logging/
--rw-r--r--   0 ahalev     (502) staff       (20)       76 2023-11-21 03:55:56.000000 experiment-config-1.0.0/src/expfig/logging/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     2225 2023-11-21 03:55:56.000000 experiment-config-1.0.0/src/expfig/logging/log_dir.py
--rw-r--r--   0 ahalev     (502) staff       (20)     2254 2023-11-21 03:55:56.000000 experiment-config-1.0.0/src/expfig/logging/logger.py
--rw-r--r--   0 ahalev     (502) staff       (20)     7248 2024-03-19 00:49:48.000000 experiment-config-1.0.0/src/expfig/namespacify.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-03-19 00:53:10.440247 experiment-config-1.0.0/src/expfig/utils/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2024-03-19 00:49:48.000000 experiment-config-1.0.0/src/expfig/utils/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1488 2024-03-19 00:49:48.000000 experiment-config-1.0.0/src/expfig/utils/api.py
--rw-r--r--   0 ahalev     (502) staff       (20)      585 2024-03-19 00:49:48.000000 experiment-config-1.0.0/src/expfig/utils/get_pandas.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-05-20 22:19:49.996184 experiment-config-1.0.1/
+-rw-r--r--   0 ahalev     (502) staff       (20)     1073 2023-01-29 22:38:50.000000 experiment-config-1.0.1/LICENSE.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)     9246 2024-05-20 22:19:49.995934 experiment-config-1.0.1/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)     8789 2023-05-31 22:41:55.000000 experiment-config-1.0.1/README.md
+-rw-r--r--   0 ahalev     (502) staff       (20)       38 2024-05-20 22:19:49.996235 experiment-config-1.0.1/setup.cfg
+-rw-r--r--   0 ahalev     (502) staff       (20)     1010 2024-05-20 22:19:21.000000 experiment-config-1.0.1/setup.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-05-20 22:19:49.989864 experiment-config-1.0.1/src/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-05-20 22:19:49.991424 experiment-config-1.0.1/src/experiment_config.egg-info/
+-rw-r--r--   0 ahalev     (502) staff       (20)     9246 2024-05-20 22:19:49.000000 experiment-config-1.0.1/src/experiment_config.egg-info/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)      786 2024-05-20 22:19:49.000000 experiment-config-1.0.1/src/experiment_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2024-05-20 22:19:49.000000 experiment-config-1.0.1/src/experiment_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)       71 2024-05-20 22:19:49.000000 experiment-config-1.0.1/src/experiment_config.egg-info/requires.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        7 2024-05-20 22:19:49.000000 experiment-config-1.0.1/src/experiment_config.egg-info/top_level.txt
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-05-20 22:19:49.992373 experiment-config-1.0.1/src/expfig/
+-rw-r--r--   0 ahalev     (502) staff       (20)      178 2024-05-20 22:18:03.000000 experiment-config-1.0.1/src/expfig/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-05-20 22:19:49.993782 experiment-config-1.0.1/src/expfig/core/
+-rw-r--r--   0 ahalev     (502) staff       (20)      162 2024-05-20 22:18:03.000000 experiment-config-1.0.1/src/expfig/core/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1992 2024-05-14 00:44:24.000000 experiment-config-1.0.1/src/expfig/core/_flatten.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     3186 2024-05-20 22:18:03.000000 experiment-config-1.0.1/src/expfig/core/_parse.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1274 2024-05-14 00:44:24.000000 experiment-config-1.0.1/src/expfig/core/_parse_yaml_obj.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      387 2024-05-20 22:18:03.000000 experiment-config-1.0.1/src/expfig/core/_str_types.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      949 2024-05-14 00:44:24.000000 experiment-config-1.0.1/src/expfig/core/similar_args.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    13255 2024-05-20 22:18:03.000000 experiment-config-1.0.1/src/expfig/fig.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-05-20 22:19:49.994083 experiment-config-1.0.1/src/expfig/functions/
+-rw-r--r--   0 ahalev     (502) staff       (20)      122 2024-05-14 00:44:24.000000 experiment-config-1.0.1/src/expfig/functions/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1327 2024-05-14 00:44:46.000000 experiment-config-1.0.1/src/expfig/functions/comparison.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-05-20 22:19:49.994696 experiment-config-1.0.1/src/expfig/logging/
+-rw-r--r--   0 ahalev     (502) staff       (20)       76 2024-05-20 22:18:03.000000 experiment-config-1.0.1/src/expfig/logging/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2225 2023-11-21 03:55:56.000000 experiment-config-1.0.1/src/expfig/logging/log_dir.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2254 2023-11-21 03:55:56.000000 experiment-config-1.0.1/src/expfig/logging/logger.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     7865 2024-05-20 22:18:03.000000 experiment-config-1.0.1/src/expfig/namespacify.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-05-20 22:19:49.995297 experiment-config-1.0.1/src/expfig/utils/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2024-03-19 00:49:48.000000 experiment-config-1.0.1/src/expfig/utils/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1488 2024-03-19 00:49:48.000000 experiment-config-1.0.1/src/expfig/utils/api.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      585 2024-03-19 00:49:48.000000 experiment-config-1.0.1/src/expfig/utils/get_pandas.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-05-20 22:19:49.995653 experiment-config-1.0.1/tests/
+-rw-r--r--   0 ahalev     (502) staff       (20)      810 2024-05-20 22:18:03.000000 experiment-config-1.0.1/tests/test_parse.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      896 2024-05-14 00:44:24.000000 experiment-config-1.0.1/tests/test_yaml_type.py
```

### Comparing `experiment-config-1.0.0/LICENSE.txt` & `experiment-config-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `experiment-config-1.0.0/PKG-INFO` & `experiment-config-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: experiment-config
-Version: 1.0.0
+Version: 1.0.1
 Summary: A yaml-based configuration for reproducible python experiments.
 Maintainer: Avishai Halev
 Maintainer-email: avishaihalev@gmail.com
 License: MIT License
-Project-URL: Source Code, https://github.com/ahalev/experiment-config/tree/v1.0.0
+Project-URL: Source Code, https://github.com/ahalev/experiment-config/tree/v1.0.1
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: pandas
 Provides-Extra: all
 License-File: LICENSE.txt
```

### Comparing `experiment-config-1.0.0/README.md` & `experiment-config-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `experiment-config-1.0.0/setup.py` & `experiment-config-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'A yaml-based configuration for reproducible python experiments.'
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 MAINTAINER = 'Avishai Halev'
 MAINTAINER_EMAIL = 'avishaihalev@gmail.com'
 LICENSE = 'MIT License'
 PROJECT_URLS = {
     'Source Code': f'https://github.com/ahalev/experiment-config/tree/v{VERSION}'
 }
```

### Comparing `experiment-config-1.0.0/src/experiment_config.egg-info/PKG-INFO` & `experiment-config-1.0.1/src/experiment_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: experiment-config
-Version: 1.0.0
+Version: 1.0.1
 Summary: A yaml-based configuration for reproducible python experiments.
 Maintainer: Avishai Halev
 Maintainer-email: avishaihalev@gmail.com
 License: MIT License
-Project-URL: Source Code, https://github.com/ahalev/experiment-config/tree/v1.0.0
+Project-URL: Source Code, https://github.com/ahalev/experiment-config/tree/v1.0.1
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: pandas
 Provides-Extra: all
 License-File: LICENSE.txt
```

### Comparing `experiment-config-1.0.0/src/expfig/fig.py` & `experiment-config-1.0.1/src/expfig/fig.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from copy import deepcopy
 
 from collections import UserDict
 from pathlib import Path
 from warnings import warn
 
 from . import Namespacify, nested_dict_update
-from .functions import unflatten
-from .functions._parse import str2bool, str2none, ListType, ListAction, parse_arg_type
+from .core import unflatten, get_similar_args_str_fmt
+from .core._parse import ListType, ListAction, parse_arg_type
 from .logging import get_logger
 from .utils import api
 
 
 DEFAULT_CONFIG_PATH = os.path.join(os.getcwd(), 'default_config.yaml')
 
 
@@ -89,33 +89,37 @@
         config_file_args, other_args = self._split_config_file_args()
         config_files = self._create_config_file_parser().parse_args(args=config_file_args)
         self.update_with_configs(config_files.config, base_config)
 
         parsed_args = self._create_parser(default=base_config).parse_known_args(args=other_args)
 
         if len(parsed_args[1]):
-            valid_args = "\n\t\t".join(sorted(parsed_args[0].__dict__.keys()))
-            warn(f'Unrecognized arguments {parsed_args[1]}.\n\tValid arguments:\n\t\t{valid_args}')
+            valid_option_keys = sorted(parsed_args[0].__dict__.keys())
+            warn_msg = get_similar_args_str_fmt(parsed_args[1], valid_option_keys)
+            warn(warn_msg)
 
-        # TODO (ahalev) deprecate, this should be handled by str2None
-        args_dict = {k: v if v != 'null' else None for k, v in parsed_args[0].__dict__.items()}
-
-        args_dict = self._extract_verbosity(args_dict)
+        args_dict = self._extract_verbosity(parsed_args[0].__dict__)
         restructured = unflatten(args_dict)
 
         self._check_restructured(restructured, self.default_config)
         return restructured
 
     def _split_config_file_args(self):
+        config_arg_loc = [x.startswith('--config') for x in sys.argv]
+
+        if sum(config_arg_loc) > 1:
+            msg = "Multiple --config arguments encountered. Pass multiple configs with a single --config prefix, e.g. " \
+                  "'python script.py --config config_1.yaml config_2.yaml'"
+            raise TypeError(msg)
+
         try:
             config_key_idx = sys.argv.index('--config')
         except ValueError:
             try:
                 # single string starting with '--config'
-                config_arg_loc = [x.startswith('--config') for x in sys.argv]
                 assert sum(config_arg_loc) == 1
             except AssertionError:
                 return [], sys.argv[1:]
             else:
                 config_arg_loc = config_arg_loc.index(True)
                 config_arg = sys.argv[config_arg_loc]
```

### Comparing `experiment-config-1.0.0/src/expfig/functions/_flatten.py` & `experiment-config-1.0.1/src/expfig/core/_flatten.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         d = args[0]
     else:
         d = kwargs
 
     for k, v in d.items():
         if isinstance(v, (dict, UserDict)):
-            if k in nested_dict:
+            if k in nested_dict and api.is_dict_like(nested_dict[k]):
                 nested_dict_update(
                     nested_dict[k], v, nest_namespacify=(nest_namespacify or isinstance(nested_dict[k], Namespacify))
                 )
             else:
                 nested_dict[k] = Namespacify(v) if nest_namespacify else v
         else:
             nested_dict[k] = v
```

### Comparing `experiment-config-1.0.0/src/expfig/functions/_parse.py` & `experiment-config-1.0.1/src/expfig/core/_parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,31 @@
 import argparse
 
 from ast import literal_eval
 from warnings import warn
 
+from expfig.core import str2bool, str2none
+from expfig.core._parse_yaml_obj import YamlType
 from expfig.utils import api
 
 
-def str2bool(v):
-    if isinstance(v, bool):
-        return v
-    if v.lower() in ('yes', 'true', 't', 'y', '1'):
-        return True
-    elif v.lower() in ('no', 'false', 'f', 'n', '0'):
-        return False
-    else:
-        raise argparse.ArgumentTypeError('Boolean value expected.')
-
-
-def str2none(v):
-    if v == 'null':
-        return None
-    return v
-
-
 def parse_arg_type(arg_name, base_default):
     additional_args = {}
 
     if api.is_list_like(base_default):
         additional_args.update(nargs='+', action=ListAction)
         _type = ListType.from_list(base_default, arg_name)
 
-    elif not base_default and not isinstance(base_default, (float, int, bool)):
-        _type = str
+    elif getattr(base_default, 'yaml_tag', None) is not None:  # is a Yaml object
+        _type = YamlType(yaml_default=True)
+    elif base_default is None or base_default == '': # allow empty strings to be yaml-objects but no failure if not
+        _type = YamlType(yaml_default=False)
     else:
         _type = type(base_default)
+
     if _type == bool:
         _type = str2bool
     elif _type == str:
         _type = str2none
 
     return _type, additional_args
 
@@ -83,15 +71,15 @@
             _value = literal_eval(value)
             return [str2none(v) for v in _value]
 
         return str2none(value)
 
     @classmethod
     def from_list(cls, list_like, arg_name=None):
-        unique_types = {type(x) for x in list_like}
+        unique_types = {type(x) for x in list_like if x is not None}
 
         if len(unique_types) == 1:
             _type = unique_types.pop()
         else:
             _type = str
 
             if len(unique_types):
```

### Comparing `experiment-config-1.0.0/src/expfig/logging/log_dir.py` & `experiment-config-1.0.1/src/expfig/logging/log_dir.py`

 * *Files identical despite different names*

### Comparing `experiment-config-1.0.0/src/expfig/logging/logger.py` & `experiment-config-1.0.1/src/expfig/logging/logger.py`

 * *Files identical despite different names*

### Comparing `experiment-config-1.0.0/src/expfig/namespacify.py` & `experiment-config-1.0.1/src/expfig/namespacify.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import yaml
 
 from contextlib import contextmanager
 from collections import UserDict
 from logging import getLogger
 
 from . import nested_dict_update
-from .functions import depth, flatten
+from .core import depth, flatten
 from .logging import make_sequential_log_dir
 
+from expfig.utils.api import is_dict_like
 from expfig.utils.get_pandas import pandas as pd
 
 
 yaml.SafeDumper.add_multi_representer(UserDict, yaml.SafeDumper.represent_dict)
 logger = getLogger(__name__)
 
 class Namespacify(UserDict):
@@ -45,15 +46,21 @@
 
     def to_dict(self):
         return {k: v.to_dict() if isinstance(v, Namespacify) else (v.copy() if hasattr(v, 'copy') else v)
                 for k, v in self.items()}
 
     def to_series(self):
         series = pd.json_normalize(self.to_dict()).squeeze()
-        series.index = pd.MultiIndex.from_tuples([x.split('.') for x in series.index])
+
+        try:
+            series.index = pd.MultiIndex.from_tuples([x.split('.') for x in series.index])
+        except TypeError:
+            if not series.empty:
+                raise
+
         return series
 
     def flatten(self, delimiter='.', levels=None):
         return flatten(self, delimiter=delimiter, levels=levels)
 
     def intersection(self, other):
         intersection = {}
@@ -90,14 +97,17 @@
         difference : :class:`.Namespacify`
             Difference between ``self`` and ``other``.
 
         """
 
         diff = {}
 
+        if type(self) != type(other):
+            return self.copy()
+
         keys = {*self.keys(), *other.keys()}
         for k in keys:
             if k not in self:
                 diff[k] = other[k]
                 continue
 
             elif k not in other:
@@ -128,15 +138,17 @@
         -------
         difference : :class:`.Namespacify`
             Difference between ``self`` and ``other``.
 
         """
         diff = {}
         for k, v in self.items():
-            if k not in other:
+            if not is_dict_like(other):
+                diff[k] = v
+            elif k not in other:
                 diff[k] = v
             elif not equal(v, other[k]):
                 if isinstance(v, Namespacify):
                     diff[k] = v.difference(other[k])
                 else:
                     diff[k] = v
 
@@ -156,14 +168,19 @@
 
         return log_dir
 
     @classmethod
     def deserialize(cls, stream):
         return cls(yaml.safe_load(stream))
 
+    @classmethod
+    def from_yaml(cls, filepath):
+        with open(filepath, 'r') as stream:
+            return cls.deserialize(stream)
+
     def __dir__(self):
         rv = set(super().__dir__())
 
         try:
             rv = rv | set(self.keys())
         except RuntimeError:
             pass
@@ -175,15 +192,18 @@
             keys = self.keys() if item[0] == slice(None) else item[0]
             return {k: self[k][item[1:]] for k in keys}
 
         elif isinstance(item, tuple):
             out = self[item[0]]
             if len(item) == 1:
                 return out
-            return out[item[1:]]
+            try:
+                return out[item[1:]]
+            except TypeError:  # out is not subscriptable, raise KeyError
+                raise KeyError(f"'{item[1:]}', item of type '{type(out).__name__}' is not subscriptable")
 
         return super().__getitem__(item)
 
     def __setitem__(self, key, value):
         if isinstance(key, tuple):
             nested_update = functools.reduce(lambda val, k: {k: val}, reversed(key), value)
             nested_dict_update(self, nested_update, nest_namespacify=True)
```

### Comparing `experiment-config-1.0.0/src/expfig/utils/api.py` & `experiment-config-1.0.1/src/expfig/utils/api.py`

 * *Files identical despite different names*

### Comparing `experiment-config-1.0.0/src/expfig/utils/get_pandas.py` & `experiment-config-1.0.1/src/expfig/utils/get_pandas.py`

 * *Files identical despite different names*

