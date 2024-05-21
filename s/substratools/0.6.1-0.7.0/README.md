# Comparing `tmp/substratools-0.6.1.tar.gz` & `tmp/substratools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/substratools-0.6.1.tar", last modified: Fri Jul 24 14:46:05 2020, max compression
+gzip compressed data, was "dist/substratools-0.7.0.tar", last modified: Tue Nov 17 07:54:45 2020, max compression
```

## Comparing `substratools-0.6.1.tar` & `substratools-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-24 14:46:05.000000 substratools-0.6.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2394 2020-07-24 14:46:05.000000 substratools-0.6.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1318 2020-07-24 14:45:26.000000 substratools-0.6.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2020-07-24 14:46:05.000000 substratools-0.6.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1166 2020-07-24 14:45:26.000000 substratools-0.6.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-24 14:46:05.000000 substratools-0.6.1/substratools/
--rw-rw-r--   0 travis    (2000) travis    (2000)      256 2020-07-24 14:45:26.000000 substratools-0.6.1/substratools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-07-24 14:45:26.000000 substratools-0.6.1/substratools/__version__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35458 2020-07-24 14:45:26.000000 substratools-0.6.1/substratools/algo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      186 2020-07-24 14:45:26.000000 substratools-0.6.1/substratools/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6799 2020-07-24 14:45:26.000000 substratools-0.6.1/substratools/metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6466 2020-07-24 14:45:26.000000 substratools-0.6.1/substratools/opener.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3226 2020-07-24 14:45:26.000000 substratools-0.6.1/substratools/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7208 2020-07-24 14:45:26.000000 substratools-0.6.1/substratools/workspace.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-24 14:46:05.000000 substratools-0.6.1/substratools.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2394 2020-07-24 14:46:04.000000 substratools-0.6.1/substratools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-07-24 14:46:04.000000 substratools-0.6.1/substratools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-24 14:46:04.000000 substratools-0.6.1/substratools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-24 14:46:04.000000 substratools-0.6.1/substratools.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-07-24 14:46:04.000000 substratools-0.6.1/substratools.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-17 07:54:45.000000 substratools-0.7.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2394 2020-11-17 07:54:45.000000 substratools-0.7.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1318 2020-11-17 07:54:09.000000 substratools-0.7.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2020-11-17 07:54:45.000000 substratools-0.7.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1166 2020-11-17 07:54:09.000000 substratools-0.7.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-17 07:54:45.000000 substratools-0.7.0/substratools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      256 2020-11-17 07:54:09.000000 substratools-0.7.0/substratools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-11-17 07:54:09.000000 substratools-0.7.0/substratools/__version__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35504 2020-11-17 07:54:09.000000 substratools-0.7.0/substratools/algo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      186 2020-11-17 07:54:09.000000 substratools-0.7.0/substratools/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6818 2020-11-17 07:54:09.000000 substratools-0.7.0/substratools/metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6243 2020-11-17 07:54:09.000000 substratools-0.7.0/substratools/opener.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3226 2020-11-17 07:54:09.000000 substratools-0.7.0/substratools/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7582 2020-11-17 07:54:09.000000 substratools-0.7.0/substratools/workspace.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-17 07:54:45.000000 substratools-0.7.0/substratools.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2394 2020-11-17 07:54:45.000000 substratools-0.7.0/substratools.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-11-17 07:54:45.000000 substratools-0.7.0/substratools.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-17 07:54:45.000000 substratools-0.7.0/substratools.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-17 07:54:45.000000 substratools-0.7.0/substratools.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-11-17 07:54:45.000000 substratools-0.7.0/substratools.egg-info/top_level.txt
```

### Comparing `substratools-0.6.1/PKG-INFO` & `substratools-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substratools
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python tools to submit algo on the Substra platform
 Home-page: https://github.com/SubstraFoundation/substra-tools
 Author: Owkin
 Author-email: fldev@owkin.com
 License: Apache 2.0
 Description: # Substra-tools
```

### Comparing `substratools-0.6.1/README.md` & `substratools-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `substratools-0.6.1/setup.py` & `substratools-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `substratools-0.6.1/substratools/algo.py` & `substratools-0.7.0/substratools/algo.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 
 
 def _generate_algo_cli(interface):
     """Helper to generate a command line interface client."""
 
     def _algo_from_args(args):
         workspace = AlgoWorkspace(
-            input_data_folder_path=args.data_samples_path,
+            input_data_folder_paths=args.data_sample_paths,
             input_models_folder_path=args.models_path,
             log_path=args.log_path,
             output_model_path=args.output_model_path,
             output_predictions_path=args.output_predictions_path,
         )
         utils.configure_logging(workspace.log_path, debug_mode=args.debug)
         opener_wrapper = opener.load_from_module(
@@ -307,16 +307,17 @@
             help="Enable fake data mode",
         )
         _parser.add_argument(
             '--n-fake-samples', default=None, type=int,
             help="Number of fake samples if fake data is used.",
         )
         _parser.add_argument(
-            '--data-samples-path', default=None,
-            help="Define train/test data samples folder path",
+            '--data-sample-paths', default=[],
+            nargs='*',
+            help="Define train/test data samples folder paths",
         )
         _parser.add_argument(
             '--models-path', default=None,
             help="Define models folder path",
         )
         _parser.add_argument(
             '--output-model-path', default=None,
@@ -684,15 +685,15 @@
 
 
 def _generate_composite_algo_cli(interface):
     """Helper to generate a command line interface client."""
 
     def _algo_from_args(args):
         workspace = CompositeAlgoWorkspace(
-            input_data_folder_path=args.data_samples_path,
+            input_data_folder_paths=args.data_sample_paths,
             input_models_folder_path=args.input_models_path,
             output_models_folder_path=args.output_models_path,
             output_head_model_filename=args.output_head_model_filename,
             output_trunk_model_filename=args.output_trunk_model_filename,
             log_path=args.log_path,
             output_predictions_path=args.output_predictions_path,
         )
@@ -713,16 +714,17 @@
             help="Enable fake data mode",
         )
         _parser.add_argument(
             '--n-fake-samples', default=None, type=int,
             help="Number of fake samples if fake data is used.",
         )
         _parser.add_argument(
-            '--data-samples-path', default=None,
-            help="Define train/test data samples folder path",
+            '--data-sample-paths', default=[],
+            nargs='*',
+            help="Define train/test data samples folder paths",
         )
         _parser.add_argument(
             '--input-models-path', default=None,
             help="Define input models folder path",
         )
         _parser.add_argument(
             '--output-predictions-path', default=None,
```

### Comparing `substratools-0.6.1/substratools/metrics.py` & `substratools-0.7.0/substratools/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,16 +166,17 @@
         help="Set fake data mode",
     )
     parser.add_argument(
         '--n-fake-samples', type=int, default=None,
         help="Number of fake samples if fake data is used.",
     )
     parser.add_argument(
-        '--data-samples-path', default=None,
-        help="Define train/test data samples folder path",
+        '--data-sample-paths', default=[],
+        nargs='*',
+        help="Define train/test data samples folder paths",
     )
     parser.add_argument(
         '--input-predictions-path', default=None,
         help="Define input predictions file path",
     )
     parser.add_argument(
         '--output-perf-path', default=None,
@@ -205,15 +206,15 @@
             interface_signature=REQUIRED_FUNCTIONS)
 
     cli = _generate_cli()
     sysargs = sysargs if sysargs is not None else sys.argv[1:]
     args = cli.parse_args(sysargs)
 
     workspace = MetricsWorkspace(
-        input_data_folder_path=args.data_samples_path,
+        input_data_folder_paths=args.data_sample_paths,
         input_predictions_path=args.input_predictions_path,
         log_path=args.log_path,
         output_perf_path=args.output_perf_path,
     )
     opener_wrapper = opener.load_from_module(
         path=args.opener_path,
         workspace=workspace,
```

### Comparing `substratools-0.6.1/substratools/opener.py` & `substratools-0.7.0/substratools/opener.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,19 +178,15 @@
             isinstance(interface, types.ModuleType)
 
         self._workspace = workspace or OpenerWorkspace()
         self._interface = interface
 
     @property
     def data_folder_paths(self):
-        rootpath = self._workspace.input_data_folder_path
-        folders = [os.path.join(rootpath, subfolder_name)
-                   for subfolder_name in os.listdir(rootpath)
-                   if os.path.isdir(os.path.join(rootpath, subfolder_name))]
-        return folders
+        return self._workspace.input_data_folder_paths
 
     def get_X(self, fake_data=False, n_fake_samples=None):
         if fake_data:
             logger.info("loading X from fake data")
             return self._interface.fake_X(n_samples=n_fake_samples)
         else:
             logger.info("loading X from '{}'".format(self.data_folder_paths))
```

### Comparing `substratools-0.6.1/substratools/utils.py` & `substratools-0.7.0/substratools/utils.py`

 * *Files identical despite different names*

### Comparing `substratools-0.6.1/substratools/workspace.py` & `substratools-0.7.0/substratools/workspace.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,37 +30,46 @@
 
     def __init__(self, dirpath=None):
         self._workdir = dirpath if dirpath else os.getcwd()
 
     def _get_default_path(self, path):
         return os.path.join(self._workdir, path)
 
+    def _get_default_subpaths(self, path):
+        rootpath = os.path.join(self._workdir, path)
+        if os.path.isdir(rootpath):
+            return [
+                os.path.join(rootpath, subfolder)
+                for subfolder in os.listdir(rootpath)
+                if os.path.isdir(os.path.join(rootpath, subfolder))
+            ]
+        return []
+
 
 class OpenerWorkspace(Workspace):
     """Filesystem workspace required by the opener."""
 
     def __init__(self,
                  dirpath=None,
-                 input_data_folder_path=None,
+                 input_data_folder_paths=None,
                  input_predictions_path=None,
                  output_predictions_path=None, ):
         super().__init__(dirpath=dirpath)
 
-        self.input_data_folder_path = input_data_folder_path or \
-            self._get_default_path(DEFAULT_INPUT_DATA_FOLDER_PATH)
+        self.input_data_folder_paths = input_data_folder_paths or \
+            self._get_default_subpaths(DEFAULT_INPUT_DATA_FOLDER_PATH)
 
         self.input_predictions_path = input_predictions_path or \
             self._get_default_path(DEFAULT_INPUT_PREDICTIONS_PATH)
 
         self.output_predictions_path = output_predictions_path or \
             self._get_default_path(DEFAULT_OUTPUT_PREDICTIONS_PATH)
 
-        dirs = [
-            self.input_data_folder_path,
-        ]
+        dirs = []
+        dirs.extend(self.input_data_folder_paths)
         paths = [
             self.input_predictions_path,
             self.output_predictions_path,
         ]
         dirs.extend([os.path.dirname(p) for p in paths])
         for d in dirs:
             if d:
@@ -68,20 +77,20 @@
 
 
 class MetricsWorkspace(OpenerWorkspace):
     """Filesystem workspace for metrics execution."""
 
     def __init__(self,
                  dirpath=None,
-                 input_data_folder_path=None,
+                 input_data_folder_paths=None,
                  input_predictions_path=None,
                  output_perf_path=None,
                  log_path=None, ):
         super().__init__(dirpath=dirpath,
-                         input_data_folder_path=input_data_folder_path,
+                         input_data_folder_paths=input_data_folder_paths,
                          input_predictions_path=input_predictions_path, )
 
         self.output_perf_path = output_perf_path or \
             self._get_default_path(DEFAULT_OUTPUT_PERF_PATH)
 
         self.log_path = log_path or \
             self._get_default_path(DEFAULT_LOG_PATH)
@@ -98,22 +107,22 @@
 
 
 class AlgoWorkspace(OpenerWorkspace):
     """Filesystem workspace for algo execution."""
 
     def __init__(self,
                  dirpath=None,
-                 input_data_folder_path=None,
+                 input_data_folder_paths=None,
                  input_models_folder_path=None,
                  input_predictions_path=None,
                  output_model_path=None,
                  output_predictions_path=None,
                  log_path=None, ):
         super().__init__(dirpath=dirpath,
-                         input_data_folder_path=input_data_folder_path,
+                         input_data_folder_paths=input_data_folder_paths,
                          input_predictions_path=input_predictions_path,
                          output_predictions_path=output_predictions_path, )
 
         self.input_models_folder_path = input_models_folder_path or \
             self._get_default_path(DEFAULT_INPUT_MODELS_FOLDER_PATH)
 
         self.output_model_path = output_model_path or \
@@ -134,24 +143,24 @@
             if d:
                 makedir_safe(d)
 
 
 class CompositeAlgoWorkspace(OpenerWorkspace):
     def __init__(self,
                  dirpath=None,
-                 input_data_folder_path=None,
+                 input_data_folder_paths=None,
                  input_models_folder_path=None,
                  input_predictions_path=None,
                  output_models_folder_path=None,
                  output_head_model_filename=None,
                  output_trunk_model_filename=None,
                  output_predictions_path=None,
                  log_path=None, ):
         super().__init__(dirpath=dirpath,
-                         input_data_folder_path=input_data_folder_path,
+                         input_data_folder_paths=input_data_folder_paths,
                          input_predictions_path=input_predictions_path,
                          output_predictions_path=output_predictions_path, )
 
         self.input_models_folder_path = input_models_folder_path or \
             self._get_default_path(DEFAULT_SRC_MODELS_FOLDER_PATH)
 
         self.output_models_folder_path = output_models_folder_path or \
```

### Comparing `substratools-0.6.1/substratools.egg-info/PKG-INFO` & `substratools-0.7.0/substratools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substratools
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python tools to submit algo on the Substra platform
 Home-page: https://github.com/SubstraFoundation/substra-tools
 Author: Owkin
 Author-email: fldev@owkin.com
 License: Apache 2.0
 Description: # Substra-tools
```

