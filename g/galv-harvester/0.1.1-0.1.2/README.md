# Comparing `tmp/galv_harvester-0.1.1.tar.gz` & `tmp/galv_harvester-0.1.2.tar.gz`

## Comparing `galv_harvester-0.1.1.tar` & `galv_harvester-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/.dockerignore
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/requirements.txt
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/.test-data/test-suite-small/headered.csv
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/.test-data/test-suite-small/headerless.csv
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/.test-data/test-suite-small/preamble.csv
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/README.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/__init__.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/api.py
--rw-r--r--   0        0        0    18017 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/harvest.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/run.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/settings.py
--rw-r--r--   0        0        0    15307 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/start.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/parse/__init__.py
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/parse/biologic_input_file.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/parse/delimited_input_file.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/parse/exceptions.py
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/parse/input_file.py
--rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/parse/ivium_input_file.py
--rw-r--r--   0        0        0    25991 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/src/galv_harvester/parse/maccor_input_file.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0    12624 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/tests/test_harvester.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/.gitignore
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/LICENSE
--rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/README.md
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10604 2020-02-02 00:00:00.000000 galv_harvester-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/requirements.txt
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/.test-data/test-suite-small/headered.csv
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/.test-data/test-suite-small/headerless.csv
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/.test-data/test-suite-small/preamble.csv
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/README.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/__init__.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/api.py
+-rw-r--r--   0        0        0    20862 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/harvest.py
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/run.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/settings.py
+-rw-r--r--   0        0        0    17425 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/start.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/parse/__init__.py
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/parse/biologic_input_file.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/parse/delimited_input_file.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/parse/exceptions.py
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/parse/input_file.py
+-rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/parse/ivium_input_file.py
+-rw-r--r--   0        0        0    25991 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/src/galv_harvester/parse/maccor_input_file.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    12624 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/tests/test_harvester.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/README.md
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 galv_harvester-0.1.2/PKG-INFO
```

### Comparing `galv_harvester-0.1.1/src/galv_harvester/README.md` & `galv_harvester-0.1.2/src/galv_harvester/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Harvester details
 
 ## Harvest process
 
-Harvesters communicate with a [Galv server](https://github.com/Battery-Intelligence-Lab/galv-backend) to upload data files.
+Harvesters communicate with a [Galv server](https://github.com/galv-team/galv-backend) to upload data files.
 The Harvester runs on a simple loop.
 **Calls to the server are in bold.** *Server responses are in italics.*:
 1. Check for settings updates, including new Monitored Paths
 2. For each Monitored Path:
    1. For each file in the Monitored Path (recursively):
       1. Attempt to open the file using the appropriate parser
       2. If the file can be opened, **report the file size to the server**
@@ -30,15 +30,15 @@
       "addition": 0.0,
       "data_type": "bool|int|float|str|datetime64[ns]"
    }
 }
 ```
 Columns will be coerced to the specified data type. 
 Coercion is done using the `pd.Series.asdtype()` function, except for datetime64[ns] columns, 
-which are coerced using `pd.to_datetime(x, format='ISO8601')`.
+which are coerced using `pd.to_datetime(x)`.
 
 Numerical (int/float) columns will be rebased and rescaled according to the `multiplier` and `addition` fields.
 New column values = (old column values + `addition`) * `multiplier`.
 
 **Columns that are not in the mapping object are converted to float.**
 This is to save space. While parquet files can handle strings fairly well, 
 they are not efficient at storing strings that are mostly numbers because
```

### Comparing `galv_harvester-0.1.1/src/galv_harvester/api.py` & `galv_harvester-0.1.2/src/galv_harvester/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             return None
         if not out.ok:
             logger.error(f"Server returned error (HTTP {out.status_code}): {out.json()}")
             return None
     except BaseException as e:
         logger.error(f"{e.__class__.__name__}: {e}")
         out = None
-    logger.info(f"API call finished in {round(time.time() - start, 2)}")
+    logger.info(f"API call finished in {round(time.time() - start, 2)}s")
     return out
 
 
 def update_config():
     logger.info("Updating configuration from API")
     try:
         url = get_setting('url')
```

### Comparing `galv_harvester-0.1.1/src/galv_harvester/harvest.py` & `galv_harvester-0.1.2/src/galv_harvester/harvest.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import dask.dataframe
 import pandas
 import fastnumbers
 import math
 import os
 import shutil
 import requests
+import holoviews as hv
+import holoviews.operation.datashader as hd
 
 from . import settings
 from .parse.exceptions import UnsupportedFileTypeError
 from .parse.ivium_input_file import IviumInputFile
 from .parse.biologic_input_file import BiologicMprInputFile
 from .parse.maccor_input_file import (
     MaccorInputFile,
@@ -195,15 +197,15 @@
             for col_name, mapping in mapping.items():
                 new_name = mapping.get('new_name')
                 if new_name in df.columns and new_name != col_name:
                     raise ValueError(f"New name '{new_name}' already exists in the dataframe")
                 if mapping['data_type'] in ["bool", "str"]:
                     df[col_name] = df[col_name].astype(mapping["data_type"])
                 elif mapping['data_type'] == 'datetime64[ns]':
-                    df[col_name] = pandas.to_datetime(df[col_name], format='ISO8601')
+                    df[col_name] = pandas.to_datetime(df[col_name])
                 else:
                     if mapping['data_type'] == 'int':
                         df[col_name] = fastnumbers.try_forceint(df[col_name], map=list, on_fail=math.nan)
                     else:
                         df[col_name] = fastnumbers.try_float(df[col_name], map=list, on_fail=math.nan)
 
                     addition = mapping.get('addition', 0)
@@ -239,27 +241,51 @@
         )
 
         data = dask.dataframe.from_map(
             pandas.DataFrame,
             partition_generator(reader, partition_line_count=partition_line_count)
         )
 
+        # Create a plot of key data columns for identification purposes
+        self._plot_png(data)
+
         # Save the data as parquet
         self.data_file_name = os.path.join(tempfile.gettempdir(), f"{os.path.basename(self.file_path)}.parquet")
         data.to_parquet(
             self.data_file_name,
             write_index=False,
             compute=True,
             custom_metadata={
                 'galv-harvester-version': VERSION
             }
         )
         self.row_count = data.shape[0].compute()
         self.partition_count = data.npartitions
 
+    def _plot_png(self, data):
+        """
+        Create a plot of key data columns for identification purposes
+        """
+        try:
+            self.png_file_name = os.path.join(tempfile.gettempdir(), f"{os.path.basename(self.file_path)}.png")
+            hd.shade.cmap = ["lightblue", "darkblue"]
+            hv.extension("matplotlib")
+            hv.output(fig='png', backend="matplotlib")
+            dataset = hv.Dataset(data, 'ElapsedTime_s', ['Voltage_V', 'Current_A'])
+            layout = (
+                    dataset.to(hv.Curve, 'ElapsedTime_s', 'Voltage_V') +
+                    dataset.to(hv.Curve, 'ElapsedTime_s', 'Current_A')
+            )
+            layout.opts(hv.opts.Curve(framewise=True, aspect=4, sublabel_format=''))
+            hv.save(layout, self.png_file_name, fmt='png')
+            self.png_ok = True
+        except Exception as e:
+            logger.warning(f"Failed to create plot: {e}")
+            self.png_ok = False
+
     def _upload_data(self):
         """
         Upload the data to the server
         """
 
         def pad0(n, width=math.floor(self.partition_count/10) + 1):
             return f"{n:0{width}d}"
@@ -272,14 +298,15 @@
             files = {'parquet_file': (filename, open(os.path.join(self.data_file_name, f"part.{i}.parquet"), 'rb'))}
             report = report_harvest_result(
                 path=self.file_path,
                 monitored_path_id=self.monitored_path.get('id'),
                 # send data in a flat format to accompany file upload protocol.
                 # Kinda hacky because it overwrites much of report_harvest_result's functionality
                 data={
+                    'format': 'flat',
                     'status': settings.HARVESTER_STATUS_SUCCESS,
                     'path': self.file_path,
                     'monitored_path_id': self.monitored_path.get('id'),
                     'task': settings.HARVESTER_TASK_IMPORT,
                     'stage': settings.HARVEST_STAGE_UPLOAD_PARQUET,
                     'total_row_count': self.row_count,
                     'partition_number': i,
@@ -316,59 +343,87 @@
                 'data': {
                     'successes': successes,
                     'errors': errors
                 }
             }
         )
 
+        if self.png_ok:
+            files = {'png_file': (os.path.basename(self.png_file_name), open(self.png_file_name, 'rb'))}
+            report = report_harvest_result(
+                path=self.file_path,
+                monitored_path_id=self.monitored_path.get('id'),
+                # send data in a flat format to accompany file upload protocol.
+                # Kinda hacky because it overwrites much of report_harvest_result's functionality
+                data={
+                    'format': 'flat',
+                    'status': settings.HARVESTER_STATUS_SUCCESS,
+                    'path': self.file_path,
+                    'monitored_path_id': self.monitored_path.get('id'),
+                    'task': settings.HARVESTER_TASK_IMPORT,
+                    'stage': settings.HARVEST_STAGE_UPLOAD_PNG,
+                    'filename': os.path.basename(self.png_file_name)
+                },
+                files=files
+            )
+            try:
+                HarvestProcessor.check_response("Upload PNG", report)
+            except BaseException as e:
+                logger.warning(f"Failed to upload PNG: {e}")
+
     def _delete_temp_files(self):
         """
         Delete temporary files created during the process
         """
-        if hasattr(self, 'data_file_name') and os.path.exists(self.data_file_name):
-            try:
-                shutil.rmtree(self.data_file_name)
-            except PermissionError:
-                logger.warning(f"Failed to delete {self.data_file_name}. This will have to be manually deleted.")
+        for attribute in ['data_file_name', 'png_file_name']:
+            if hasattr(self, attribute):
+                filename = getattr(self, attribute)
+                if os.path.exists(filename):
+                    try:
+                        if os.path.isdir(filename):
+                            shutil.rmtree(filename)
+                        else:
+                            os.remove(filename)
+                    except PermissionError:
+                        logger.warning(f"Failed to delete {filename}. This will have to be manually deleted.")
 
     def __del__(self):
         self._delete_temp_files()
 
 
 if False:
     # My debugger won't connect, so running this in the console can figure out dask issues
     import os
     import pandas
     import dask.dataframe
     import shutil
     import fastnumbers
     import math
-    from src.galv_harvester.settings import get_standard_units, get_standard_columns
+    import holoviews as hv
+    import holoviews.operation.datashader as hd
+
     from src.galv_harvester.parse.maccor_input_file import MaccorInputFile
-    os.system('cp .harvester/.harvester.json /harvester_files')
-    standard_units = get_standard_units()
-    standard_columns = get_standard_columns()
     file_path = '.test-data/test-suite-small/TPG1+-+Cell+15+-+002.txt'
-    input_file = MaccorInputFile(file_path, standard_units=standard_units, standard_columns=standard_columns)
+    input_file = MaccorInputFile(file_path)
 
     mapping = {
         "Amps": {
             "new_name": "Current_A",
             "data_type": "float",
             "multiplier": 0.001,
             "addition": 0
         },
         "Rec#": {
-            "new_name": "Sample_number",
+            "new_name": "SampleNumber",
             "data_type": "int",
             "multiplier": 1,
             "addition": 0
         },
         "Step": {
-            "new_name": "Step_number",
+            "new_name": "StepNumber",
             "data_type": "int",
             "multiplier": 1,
             "addition": 0
         },
         "State": {
             "new_name": "State",
             "data_type": "str"
@@ -392,29 +447,29 @@
         "StepTime": {
             "new_name": "Step_time_s",
             "data_type": "float",
             "multiplier": 1,
             "addition": 0
         },
         "TestTime": {
-            "new_name": "Elapsed_time_s",
+            "new_name": "ElapsedTime_s",
             "data_type": "float",
             "multiplier": 1,
             "addition": 0
         }
     }
 
     def remap(df, mapping):
         columns = list(df.columns)
         for col_name, mapping in mapping.items():
             new_name = mapping['new_name']
             if mapping['data_type'] in ["bool", "str"]:
                 df[new_name] = df[col_name].astype(mapping["data_type"])
             elif mapping['data_type'] == 'datetime64[ns]':
-                df[new_name] = pandas.to_datetime(df[col_name], format='ISO8601')
+                df[new_name] = pandas.to_datetime(df[col_name])
             else:
                 if mapping['data_type'] == 'int':
                     df[new_name] = fastnumbers.try_forceint(df[col_name], map=list, on_fail=math.nan)
                 else:
                     df[new_name] = fastnumbers.try_float(df[col_name], map=list, on_fail=math.nan)
 
                 addition = mapping.get('addition', 0)
@@ -438,24 +493,37 @@
             try:
                 for _ in range(partition_line_count):
                     rows.append(next(generator))
             except StopIteration:
                 stopping = True
             yield to_df(rows)
 
-    partition_line_count = 10_000
+    partition_line_count = 100_000
 
     reader = input_file.load_data(
         file_path,
         [c for c in input_file.column_info.keys() if input_file.column_info[c].get('has_data')]
     )
 
     data = dask.dataframe.from_map(
         pandas.DataFrame,
         partition_generator(reader, partition_line_count=partition_line_count)
     )
 
     data.compute()
     print(f"Rows: {data.shape[0].compute()}")
+
+    # Create a plot of key data columns for identification purposes
+    hd.shade.cmap = ["lightblue", "darkblue"]
+    hv.extension("matplotlib")
+    hv.output(fig='png', backend="matplotlib")
+    dataset = hv.Dataset(data, 'ElapsedTime_s', ['Voltage_V', 'Current_A'])
+    layout = (
+            dataset.to(hv.Curve, 'ElapsedTime_s', 'Voltage_V') +
+            dataset.to(hv.Curve, 'ElapsedTime_s', 'Current_A')
+    )
+    layout.opts(hv.opts.Curve(framewise=True, aspect=4, sublabel_format=''))
+    hv.save(layout, 'test.tmp.hv.png', fmt='png')
+
     # Then we would upload the data by getting presigned URLs for each partition
     shutil.rmtree("test.tmp.parquet")
     print('done')
```

### Comparing `galv_harvester-0.1.1/src/galv_harvester/run.py` & `galv_harvester-0.1.2/src/galv_harvester/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,82 +43,98 @@
 
     for path in paths:
         if path.get('active'):
             harvest_path(path)
         else:
             logger.info(f"Skipping inactive path {path.get('path')} {path.get('regex')}")
 
-def harvest_path(monitored_path: dict):
-    path = monitored_path.get('path')
-    regex_str = monitored_path.get('regex')
-    if regex_str is not None:
-        logger.info(f"Harvesting from {path} with regex {regex_str}")
+
+def harvest_file(file_path, monitored_path: dict, compiled_regex: re.Pattern = None):
+    if compiled_regex is None:
+        regex_str = monitored_path.get('regex')
+        if regex_str is not None:
+            regex = re.compile(regex_str)
+        else:
+            regex = re.compile(r".*")
     else:
-        logger.info(f"Harvesting from {path}")
+        regex = compiled_regex
+
+    path = monitored_path.get('path')
+
+    _, rel_path = split_path(path, file_path)
+    if regex is not None and not regex.search(rel_path):
+        logger.debug(f"Skipping {rel_path} as it does not match regex {regex}")
+        return
     try:
-        regex = re.compile(regex_str) if regex_str is not None else None
-        for (dir_path, dir_names, filenames) in os.walk(path):
-            for filename in filenames:
-                full_path = os.path.join(dir_path, filename)
-                core_path, file_path = split_path(path, full_path)
-                if regex is not None and not regex.search(file_path):
-                    logger.debug(f"Skipping {file_path} as it does not match regex {regex}")
-                    continue
-                try:
-                    file = HarvestProcessor(full_path, monitored_path)
-                except UnsupportedFileTypeError:
-                    logger.debug(f"Skipping unsupported file {file_path}")
-                    continue
+        file = HarvestProcessor(file_path, monitored_path)
+    except UnsupportedFileTypeError:
+        logger.debug(f"Skipping unsupported file {rel_path}")
+        return
+    try:
+        logger.info(f"Reporting stats for {rel_path}")
+        result = report_harvest_result(
+            path=file_path,
+            monitored_path_id=monitored_path.get('id'),
+            content={
+                'task': HARVESTER_TASK_FILE_SIZE,
+                'size': os.stat(file_path).st_size
+            }
+        )
+        if result is not None:
+            result = result.json()
+            status = result['state']
+            logger.info(f"Server assigned status '{status}'")
+            if status in ['STABLE', 'RETRY IMPORT', 'MAP ASSIGNED']:
+                logger.info(f"Parsing file {rel_path}")
                 try:
-                    logger.info(f"Reporting stats for {file_path}")
-                    result = report_harvest_result(
-                        path=full_path,
+                    file.harvest()
+                    report_harvest_result(
+                        path=file_path,
                         monitored_path_id=monitored_path.get('id'),
                         content={
-                            'task': HARVESTER_TASK_FILE_SIZE,
-                            'size': os.stat(full_path).st_size
+                            'task': HARVESTER_TASK_IMPORT,
+                            'stage': HARVEST_STAGE_COMPLETE
                         }
                     )
-                    if result is not None:
-                        result = result.json()
-                        status = result['state']
-                        logger.info(f"Server assigned status '{status}'")
-                        if status in ['STABLE', 'RETRY IMPORT', 'MAP ASSIGNED']:
-                            logger.info(f"Parsing file {file_path}")
-                            try:
-                                file.harvest()
-                                report_harvest_result(
-                                    path=full_path,
-                                    monitored_path_id=monitored_path.get('id'),
-                                    content={
-                                        'task': HARVESTER_TASK_IMPORT,
-                                        'stage': HARVEST_STAGE_COMPLETE
-                                    }
-                                )
-                                logger.info(f"Successfully parsed file {file_path}")
-                            except BaseException as e:
-                                logger.warning(f"FAILED parsing file {file_path}: {e.__class__.__name__}: {e}")
-                                if e.__traceback__ is not None:
-                                    logger.warning(traceback.format_exc())
-                                report_harvest_result(
-                                    path=full_path,
-                                    monitored_path_id=monitored_path.get('id'),
-                                    content={
-                                        'task': HARVESTER_TASK_IMPORT,
-                                        'stage': HARVEST_STAGE_FAILED,
-                                        'error': f"Error in Harvester. {e.__class__.__name__}: {e}. [See harvester logs for more details]"
-                                    }
-                                )
+                    logger.info(f"Successfully parsed file {rel_path}")
                 except BaseException as e:
-                    logger.error(f"{e.__class__.__name__}: {e}")
+                    logger.warning(f"FAILED parsing file {rel_path}: {e.__class__.__name__}: {e}")
+                    if e.__traceback__ is not None:
+                        logger.warning(traceback.format_exc())
                     report_harvest_result(
-                        path=full_path,
+                        path=file_path,
                         monitored_path_id=monitored_path.get('id'),
-                        error=e
+                        content={
+                            'task': HARVESTER_TASK_IMPORT,
+                            'stage': HARVEST_STAGE_FAILED,
+                            'error': f"Error in Harvester. {e.__class__.__name__}: {e}. [See harvester logs for more details]"
+                        }
                     )
+    except BaseException as e:
+        logger.error(f"{e.__class__.__name__}: {e}")
+        report_harvest_result(
+            path=file_path,
+            monitored_path_id=monitored_path.get('id'),
+            error=e
+        )
+
+
+
+def harvest_path(monitored_path: dict):
+    path = monitored_path.get('path')
+    regex_str = monitored_path.get('regex')
+    if regex_str is not None:
+        logger.info(f"Harvesting from {path} with regex {regex_str}")
+    else:
+        logger.info(f"Harvesting from {path}")
+    try:
+        regex = re.compile(regex_str) if regex_str is not None else None
+        for (dir_path, dir_names, filenames) in os.walk(path):
+            for filename in filenames:
+                harvest_file(os.path.join(dir_path, filename), monitored_path, compiled_regex=regex)
         logger.info(f"Completed directory walking of {path}")
     except BaseException as e:
         logger.error(f"{e.__class__.__name__}: {e}")
         report_harvest_result(
             monitored_path_id=monitored_path.get('id'),
             error=e,
             path=path
```

### Comparing `galv_harvester-0.1.1/src/galv_harvester/settings.py` & `galv_harvester-0.1.2/src/galv_harvester/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     format='%(asctime)s %(levelname)s %(message)s [%(name)s:%(lineno)d]',
     level=logging.INFO,
     datefmt='%Y-%m-%d %H:%M:%S'
 )
 
 
 def get_logfile() -> pathlib.Path:
-    return pathlib.Path(os.getenv('GALV_HARVESTER_LOG_FILE', "/harvester_files/harvester.log"))
+    return pathlib.Path(os.getenv('GALV_HARVESTER_LOG_FILE', "./.harvester/harvester.log"))
 
 
 def get_logger(name):
     logger = logging.getLogger(name)
     # stream_handler = logging.StreamHandler(sys.stdout)
     # stream_handler.setLevel(logging.INFO)
     # logger.addHandler(stream_handler)
@@ -33,15 +33,15 @@
     return logger
 
 
 logger = get_logger(__file__)
 
 
 def get_settings_file() -> pathlib.Path:
-    return pathlib.Path(os.getenv('GALV_HARVESTER_SETTINGS_FILE', "/harvester_files/.harvester.json"))
+    return pathlib.Path(os.getenv('GALV_HARVESTER_SETTINGS_FILE', "./.harvester/settings.json"))
 
 
 def get_settings():
     try:
         with open(get_settings_file(), 'r') as f:
             try:
                 return json.load(f)
@@ -92,9 +92,10 @@
 HARVESTER_TASK_IMPORT = 'import'
 HARVESTER_STATUS_SUCCESS = 'success'
 HARVESTER_STATUS_ERROR = 'error'
 HARVEST_STAGE_FILE_METADATA = 'file metadata'
 HARVEST_STAGE_DATA_SUMMARY = 'data summary'
 HARVEST_STAGE_UPLOAD_PARQUET = 'upload parquet partitions'
 HARVEST_STAGE_UPLOAD_COMPLETE = 'upload complete'
+HARVEST_STAGE_UPLOAD_PNG = 'upload png'
 HARVEST_STAGE_COMPLETE = 'harvest complete'
 HARVEST_STAGE_FAILED = 'harvest failed'
```

### Comparing `galv_harvester-0.1.1/src/galv_harvester/start.py` & `galv_harvester-0.1.2/src/galv_harvester/start.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import time
 
 import click
 import requests
 
 from . import run, settings
 
-
 def query(url: str, data: object = None, retries: int = 5, sleep_seconds: float = 3.0, **kwargs):
     while retries > 0:
         try:
             if data is None:
                 result = requests.get(url, **kwargs)
                 click.echo(f"GET {url} {result.status_code}")
             else:
@@ -50,21 +49,21 @@
 
 def get_url() -> str:
     click.echo("Enter the URL for the Galv server you wish to connect to.")
     url = input("API URL: ")
     return append_slash(url)
 
 def create_monitored_path(
-        api_url, api_token, harvester_uuid, specified,
+        api_url, api_token, harvester_id, specified,
         team_id, monitor_path, monitor_path_regex
 ) -> None:
     # TODO: Ensure that the team is a member of the harvester's lab
     click.echo("The harvester will monitor a path on the server for changes and upload files.")
     click.echo("You must be a Team administrator to create a monitored path. "
-                "Note that Lab administrators are not necessarily Team administrators.")
+               "Note that Lab administrators are not necessarily Team administrators.")
 
     def monitored_path_exit(error: str):
         click.echo('Harvester successfully created, but the monitored path could not be set.')
         click.echo(f"Error: {error}", err=True)
         click.echo('Please go to the frontend to set a monitored path.')
         click.echo('')
 
@@ -165,15 +164,15 @@
         click.echo(f"Setting monitor path to {monitor_path}{regex_str}")
         try:
             query(
                 f"{api_url}monitored_paths/",
                 {
                     'path': monitor_path,
                     'regex': monitor_path_regex,
-                    'harvester': harvester_uuid,
+                    'harvester': harvester_id,
                     'team': team['id'],
                     'active': True
                 },
                 headers={
                     'Authorization': f"Bearer {api_token}"
                 },
             )
@@ -296,15 +295,19 @@
 
     lab = [l for l in labs_administered if l['id'] == lab_id][0]
 
     # Check name okay
     if name is None:
         name = get_name()
     while True:
-        result = query(f"{url}harvesters/?name={name}&lab_id={lab_id}")
+        if name == "":
+            click.echo("Name cannot be blank.")
+            name = get_name()
+            continue
+        result = query(f"{url}harvesters/?name={name}&lab__id={lab_id}")
 
         if result['count'] > 0:
             click.echo(f"This Lab already has a harvester called {name}.", err=True)
             if specified:
                 exit(1)
             click.echo("Please try something else.")
             name = get_name()
@@ -328,33 +331,100 @@
         click.echo(f"Saved to {f.name}")
 
     click.echo("Success.")
     click.echo("")
 
     if monitor_path is not None or not specified:
         create_monitored_path(
-            api_url=url, api_token=api_token, harvester_uuid=result['uuid'], specified=specified,
+            api_url=url, api_token=api_token, harvester_id=result['id'], specified=specified,
             team_id=team_id, monitor_path=monitor_path, monitor_path_regex=monitor_path_regex
         )
 
     click.echo(
         f"You can configure this harvester's details by visiting the API at "
         f"{url} or going to the frontend."
     )
     click.echo("")
     click.echo("The harvester will check for updates frequently until you change its polling rate when you update it.")
     click.echo("Launching harvester...")
     if run_foreground:
         run.run_cycle()
     else:
-        subprocess.Popen(["python", "-m", "run"])
+        subprocess.Popen(["python", "-m", "galv_harvester.run"])
         click.echo(f"Complete. Harvester is running and logging to {settings.get_logfile()}")
 
 
-@click.command()
+@click.group()
+def click_wrapper():
+    pass
+
+
+@click_wrapper.command()
+@click.option('--path', type=str, help="File/Directory to harvest files from. If left blank, all Monitored Paths in the config will be harvested.")
+def harvest(path: str):
+    # Check we can access settings
+    try:
+        current_settings = settings.get_settings()
+    except FileNotFoundError:
+        click.echo("No settings file found. Please run `galv-harvester setup` wizard.")
+        exit(1)
+
+    if path:
+        path = os.path.abspath(path)
+        # Check the path is valid
+        if not os.path.exists(path):
+            click.echo(f"Path {path} does not exist on the filesystem.")
+            exit(1)
+        # Check the path is on a monitored path
+        monitored_paths = current_settings.get('monitored_paths', [])
+        monitored_path = None
+        for mp in monitored_paths:
+            # A match is where the path is a substring of the monitored path
+            if not path.lower().startswith(mp['path'].lower()):
+                continue
+            # and the regex matches (for files)
+            if os.path.isfile(path):
+                if re.match(mp['regex'], os.path.relpath(path, mp['path'])):
+                    monitored_path = mp
+                    break
+            elif os.path.isdir(path):
+                monitored_path = mp
+                break
+        if not monitored_path:
+            click.echo(f"Could not find {path} in any monitored paths.")
+            click.echo(f"Available monitored paths [path : regex] are:")
+            for mp in monitored_paths:
+                click.echo(f"{mp['path']} : {mp['regex']}")
+            exit(1)
+
+        # Harvest the path
+        if os.path.isfile(path):
+            run.harvest_file(path, monitored_path)
+        else:
+            run.harvest_path(monitored_path)
+        return
+
+    # Run the harvester for a single cycle
+    run.harvest()
+
+
+@click_wrapper.command()
+def restart():
+    click.echo("Attempting to restart harvester.")
+    # Check whether a config file already exists, if so, use it
+    if settings.get_setting('url'):
+        click.echo("Config file found, restarting harvester.")
+        run.run_cycle()
+        return
+    else:
+        click.echo("No config file found, please run `galv-harvester setup` wizard.")
+        click.echo("")
+
+
+@click_wrapper.command()
 @click.version_option()
 @click.option('--url', type=str, help="API URL to register harvester with.")
 @click.option('--name', type=str, help="Name for the harvester.")
 @click.option('--api_token', type=str, help="Your API token. You must have admin access to at least one Lab.")
 @click.option('--lab_id', type=int, help="Id of the Lab to assign the Harvester to. Only required if you administrate multiple Labs.")
 @click.option('--team_id', type=int, help="Id of the Team to create a Monitored Path for. Only required if you administrate multiple Teams and wish to create a monitored path.")
 @click.option('--monitor_path', type=str, help="Path to harvest files from.")
@@ -363,36 +433,25 @@
     '--run_foreground',
     is_flag=True,
     help=(
             "On completion, run the harvester in the foreground "
             "(will not close the thread, useful for Dockerized application)."
     )
 )
-@click.option(
-    '--restart',
-    is_flag=True,
-    help="Ignore other options and run harvester if config file already exists."
-)
-def click_wrapper(
+def setup(
         url: str, name: str, api_token: str, lab_id: int, team_id: int,
         monitor_path: str, monitor_path_regex: str,
-        run_foreground: bool, restart: bool
+        run_foreground: bool
 ):
-    restart = restart or os.getenv("GALV_HARVESTER_RESTART", False)
+    restart = os.getenv("GALV_HARVESTER_RESTART", False)
 
-    if restart:
-        click.echo("Attempting to restart harvester.")
-        # Check whether a config file already exists, if so, use it
-        if settings.get_setting('url'):
-            click.echo("Config file found, restarting harvester.")
-            run.run_cycle()
-            return
-        else:
-            click.echo("No config file found, continuing to setup.")
-            click.echo("")
+    if restart and not any([url, name, api_token, lab_id, team_id, monitor_path, monitor_path_regex]):
+        click.echo("Restarting harvester because GALV_HARVESTER_RESTART envvar is set.")
+        run.run_cycle()
+        return
 
     click.echo("Welcome to Harvester setup.")
     register(
         url=url, name=name, api_token=api_token, lab_id=lab_id, team_id=team_id,
         monitor_path=monitor_path, monitor_path_regex=monitor_path_regex,
         run_foreground=run_foreground
     )
```

### Comparing `galv_harvester-0.1.1/src/galv_harvester/parse/biologic_input_file.py` & `galv_harvester-0.1.2/src/galv_harvester/parse/biologic_input_file.py`

 * *Files identical despite different names*

### Comparing `galv_harvester-0.1.1/src/galv_harvester/parse/delimited_input_file.py` & `galv_harvester-0.1.2/src/galv_harvester/parse/delimited_input_file.py`

 * *Files identical despite different names*

### Comparing `galv_harvester-0.1.1/src/galv_harvester/parse/exceptions.py` & `galv_harvester-0.1.2/src/galv_harvester/parse/exceptions.py`

 * *Files identical despite different names*

### Comparing `galv_harvester-0.1.1/src/galv_harvester/parse/input_file.py` & `galv_harvester-0.1.2/src/galv_harvester/parse/input_file.py`

 * *Files identical despite different names*

### Comparing `galv_harvester-0.1.1/src/galv_harvester/parse/ivium_input_file.py` & `galv_harvester-0.1.2/src/galv_harvester/parse/ivium_input_file.py`

 * *Files identical despite different names*

### Comparing `galv_harvester-0.1.1/src/galv_harvester/parse/maccor_input_file.py` & `galv_harvester-0.1.2/src/galv_harvester/parse/maccor_input_file.py`

 * *Files identical despite different names*

### Comparing `galv_harvester-0.1.1/tests/test_harvester.py` & `galv_harvester-0.1.2/tests/test_harvester.py`

 * *Files identical despite different names*

### Comparing `galv_harvester-0.1.1/LICENSE` & `galv_harvester-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galv_harvester-0.1.1/README.md` & `galv_harvester-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Galv Harvester (Python program)
 > A metadata secretary for battery science
 
+[![PyPI - Version](https://img.shields.io/pypi/v/galv-harvester)](https://pypi.org/project/galv-harvester/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/galv-harvester)](https://pypi.org/project/galv-harvester/)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
-[![Test, Build, and Publish](https://github.com/Battery-Intelligence-Lab/galv-harvester/actions/workflows/publish.yml/badge.svg)](https://github.com/Battery-Intelligence-Lab/galv-harvester/actions/workflows/publish.yml)
+[![Test, Build, and Publish](https://github.com/galv-team/galv-harvester/actions/workflows/publish.yml/badge.svg)](https://github.com/galv-team/galv-harvester/actions/workflows/publish.yml)
 
 ## Galv Project
-- [Specification](https://github.com/Battery-Intelligence-Lab/galv-spec)
-- [Backend](https://github.com/Battery-Intelligence-Lab/galv-backend)
-- [Frontend](https://github.com/Battery-Intelligence-Lab/galv-frontend)
-- [**Harvester**](https://github.com/Battery-Intelligence-Lab/galv-harvester)
+- [Backend](https://github.com/galv-team/galv-backend)
+- [Frontend](https://github.com/galv-team/galv-frontend)
+- [**Harvester**](https://github.com/galv-team/galv-harvester)
 
 ## Installation
 
 The Galv Harvester can be installed from the [Python Package Index](https://pypi.org/project/galv-harvester/).
 
 ```bash
 pip install galv-harvester
@@ -41,15 +42,15 @@
 or by specifying [environment variables](#using-environment-variables).
 You can use a combination of both methods, specifying some settings in the environment and others in the wizard.
 
 If you launch the program using the commands above, you will be prompted to enter the necessary settings by the wizard.
 
 ### Using the setup wizard
 
-First, you'll be asked for the [Galv server](https://github.com/Battery-Intelligence-Lab/galv-backend) URL.
+First, you'll be asked for the [Galv server](https://github.com/galv-team/galv-backend) URL.
 This should be the URL of the Galv server you have set up.
 Providing a frontend URL will not work, as the harvester needs to communicate with the backend.
 
 Next, you'll be asked for your API token. 
 This can be generated in either the Galv frontend or backend.
 The token should be for a User who administers the Lab the Harvester will belong to.
 
@@ -152,11 +153,11 @@
 Monitored Paths can only be created and edited by Team administrators, as a security measure.
 
 ## Restarting the harvester
 
 If you need to restart the harvester, you can do so by running the following command:
 
 ```bash
-galv-harvester --restart
+galv-harvester restart
 ```
 
 This will restart the harvester using the previously-configured settings.
```

### Comparing `galv_harvester-0.1.1/pyproject.toml` & `galv_harvester-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     "pandas~=2.2.1",
     "dask[complete] > 2023.5.0",
     "fastnumbers~=5.1.0",
     "galvani ~= 0.4.1",
     "maya~=0.6.1",
     "xlrd~=2.0.1",
     "psutil~=5.9.4",
+    "holoviews~=1.18.3",
+    "datashader~=0.16.1",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/galv-harvester#readme"
 Issues = "https://github.com/unknown/galv-harvester/issues"
 Source = "https://github.com/unknown/galv-harvester"
```

### Comparing `galv_harvester-0.1.1/PKG-INFO` & `galv_harvester-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: galv-harvester
-Version: 0.1.1
+Version: 0.1.2
 Project-URL: Documentation, https://github.com/unknown/galv-harvester#readme
 Project-URL: Issues, https://github.com/unknown/galv-harvester/issues
 Project-URL: Source, https://github.com/unknown/galv-harvester
 Author-email: Matt Jaquiery <matt.jaquiery@dtc.ox.ac.uk>
 License: Copyright  (c) 2020-2023, The Chancellor, Masters and Scholars of the University
         of Oxford, and the 'Galv' Developers. All rights reserved.
         
@@ -27,34 +27,37 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: click~=8.1.3
 Requires-Dist: dask[complete]>2023.5.0
+Requires-Dist: datashader~=0.16.1
 Requires-Dist: fastnumbers~=5.1.0
 Requires-Dist: galvani~=0.4.1
+Requires-Dist: holoviews~=1.18.3
 Requires-Dist: maya~=0.6.1
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: psutil~=5.9.4
 Requires-Dist: requests~=2.28.1
 Requires-Dist: xlrd~=2.0.1
 Description-Content-Type: text/markdown
 
 # Galv Harvester (Python program)
 > A metadata secretary for battery science
 
+[![PyPI - Version](https://img.shields.io/pypi/v/galv-harvester)](https://pypi.org/project/galv-harvester/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/galv-harvester)](https://pypi.org/project/galv-harvester/)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
-[![Test, Build, and Publish](https://github.com/Battery-Intelligence-Lab/galv-harvester/actions/workflows/publish.yml/badge.svg)](https://github.com/Battery-Intelligence-Lab/galv-harvester/actions/workflows/publish.yml)
+[![Test, Build, and Publish](https://github.com/galv-team/galv-harvester/actions/workflows/publish.yml/badge.svg)](https://github.com/galv-team/galv-harvester/actions/workflows/publish.yml)
 
 ## Galv Project
-- [Specification](https://github.com/Battery-Intelligence-Lab/galv-spec)
-- [Backend](https://github.com/Battery-Intelligence-Lab/galv-backend)
-- [Frontend](https://github.com/Battery-Intelligence-Lab/galv-frontend)
-- [**Harvester**](https://github.com/Battery-Intelligence-Lab/galv-harvester)
+- [Backend](https://github.com/galv-team/galv-backend)
+- [Frontend](https://github.com/galv-team/galv-frontend)
+- [**Harvester**](https://github.com/galv-team/galv-harvester)
 
 ## Installation
 
 The Galv Harvester can be installed from the [Python Package Index](https://pypi.org/project/galv-harvester/).
 
 ```bash
 pip install galv-harvester
@@ -83,15 +86,15 @@
 or by specifying [environment variables](#using-environment-variables).
 You can use a combination of both methods, specifying some settings in the environment and others in the wizard.
 
 If you launch the program using the commands above, you will be prompted to enter the necessary settings by the wizard.
 
 ### Using the setup wizard
 
-First, you'll be asked for the [Galv server](https://github.com/Battery-Intelligence-Lab/galv-backend) URL.
+First, you'll be asked for the [Galv server](https://github.com/galv-team/galv-backend) URL.
 This should be the URL of the Galv server you have set up.
 Providing a frontend URL will not work, as the harvester needs to communicate with the backend.
 
 Next, you'll be asked for your API token. 
 This can be generated in either the Galv frontend or backend.
 The token should be for a User who administers the Lab the Harvester will belong to.
 
@@ -194,11 +197,11 @@
 Monitored Paths can only be created and edited by Team administrators, as a security measure.
 
 ## Restarting the harvester
 
 If you need to restart the harvester, you can do so by running the following command:
 
 ```bash
-galv-harvester --restart
+galv-harvester restart
 ```
 
 This will restart the harvester using the previously-configured settings.
```

