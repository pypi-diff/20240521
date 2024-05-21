# Comparing `tmp/gokart-1.3.0.tar.gz` & `tmp/gokart-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokart-1.3.0.tar", max compression
+gzip compressed data, was "gokart-1.4.0.tar", max compression
```

## Comparing `gokart-1.3.0.tar` & `gokart-1.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1065 2024-04-23 07:31:08.592507 gokart-1.3.0/LICENSE
--rw-r--r--   0        0        0     3657 2024-04-23 07:31:08.592507 gokart-1.3.0/README.md
--rw-r--r--   0        0        0      635 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/__init__.py
--rw-r--r--   0        0        0     3590 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/build.py
--rw-r--r--   0        0        0     1534 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/config_params.py
--rw-r--r--   0        0        0     4426 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/conflict_prevention_lock/task_lock.py
--rw-r--r--   0        0        0     3962 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/conflict_prevention_lock/task_lock_wrappers.py
--rw-r--r--   0        0        0     9574 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/file_processor.py
--rw-r--r--   0        0        0     1004 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/gcs_config.py
--rw-r--r--   0        0        0     1380 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/gcs_zip_client.py
--rw-r--r--   0        0        0     1555 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/info.py
--rw-r--r--   0        0        0     2389 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/object_storage.py
--rw-r--r--   0        0        0     1754 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/pandas_type_config.py
--rw-r--r--   0        0        0     3266 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/parameter.py
--rw-r--r--   0        0        0        0 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/py.typed
--rw-r--r--   0        0        0     3899 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/run.py
--rw-r--r--   0        0        0      834 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/s3_config.py
--rw-r--r--   0        0        0     1657 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/s3_zip_client.py
--rw-r--r--   0        0        0      191 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/slack/__init__.py
--rw-r--r--   0        0        0     1693 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/slack/event_aggregator.py
--rw-r--r--   0        0        0     1819 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/slack/slack_api.py
--rw-r--r--   0        0        0      685 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/slack/slack_config.py
--rw-r--r--   0        0        0     8322 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/target.py
--rw-r--r--   0        0        0    25051 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/task.py
--rw-r--r--   0        0        0      471 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/task_complete_check.py
--rw-r--r--   0        0        0      204 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/testing/__init__.py
--rw-r--r--   0        0        0     3055 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/testing/check_if_run_with_empty_data_frame.py
--rw-r--r--   0        0        0     1289 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/testing/pandas_assert.py
--rw-r--r--   0        0        0     3918 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/tree/task_info.py
--rw-r--r--   0        0        0     4766 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/tree/task_info_formatter.py
--rw-r--r--   0        0        0     1735 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/utils.py
--rw-r--r--   0        0        0     1174 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/workspace_management.py
--rw-r--r--   0        0        0     1402 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/zip_client.py
--rw-r--r--   0        0        0      432 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/zip_client_util.py
--rw-r--r--   0        0        0     1983 2024-04-23 07:31:20.180573 gokart-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 gokart-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-21 10:43:17.179788 gokart-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3657 2024-05-21 10:43:17.183788 gokart-1.4.0/README.md
+-rw-r--r--   0        0        0      635 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/__init__.py
+-rw-r--r--   0        0        0     3590 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/build.py
+-rw-r--r--   0        0        0     1534 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/config_params.py
+-rw-r--r--   0        0        0     4426 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/conflict_prevention_lock/task_lock.py
+-rw-r--r--   0        0        0     3962 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/conflict_prevention_lock/task_lock_wrappers.py
+-rw-r--r--   0        0        0     9574 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/file_processor.py
+-rw-r--r--   0        0        0     1004 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/gcs_config.py
+-rw-r--r--   0        0        0     1380 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/gcs_zip_client.py
+-rw-r--r--   0        0        0     1555 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/info.py
+-rw-r--r--   0        0        0     2389 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/object_storage.py
+-rw-r--r--   0        0        0     1754 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/pandas_type_config.py
+-rw-r--r--   0        0        0     3266 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/parameter.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/py.typed
+-rw-r--r--   0        0        0     3899 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/run.py
+-rw-r--r--   0        0        0      834 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/s3_config.py
+-rw-r--r--   0        0        0     1657 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/s3_zip_client.py
+-rw-r--r--   0        0        0      191 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/slack/__init__.py
+-rw-r--r--   0        0        0     1693 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/slack/event_aggregator.py
+-rw-r--r--   0        0        0     1819 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/slack/slack_api.py
+-rw-r--r--   0        0        0      685 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/slack/slack_config.py
+-rw-r--r--   0        0        0     8294 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/target.py
+-rw-r--r--   0        0        0    25231 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/task.py
+-rw-r--r--   0        0        0      471 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/task_complete_check.py
+-rw-r--r--   0        0        0      204 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/testing/__init__.py
+-rw-r--r--   0        0        0     3055 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/testing/check_if_run_with_empty_data_frame.py
+-rw-r--r--   0        0        0     1289 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/testing/pandas_assert.py
+-rw-r--r--   0        0        0     3918 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/tree/task_info.py
+-rw-r--r--   0        0        0     4766 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/tree/task_info_formatter.py
+-rw-r--r--   0        0        0     1735 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/utils.py
+-rw-r--r--   0        0        0     1174 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/workspace_management.py
+-rw-r--r--   0        0        0     1402 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/zip_client.py
+-rw-r--r--   0        0        0      432 2024-05-21 10:43:17.183788 gokart-1.4.0/gokart/zip_client_util.py
+-rw-r--r--   0        0        0     1989 2024-05-21 10:43:30.179736 gokart-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4810 1970-01-01 00:00:00.000000 gokart-1.4.0/PKG-INFO
```

### Comparing `gokart-1.3.0/LICENSE` & `gokart-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/README.md` & `gokart-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/__init__.py` & `gokart-1.4.0/gokart/__init__.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/build.py` & `gokart-1.4.0/gokart/build.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/config_params.py` & `gokart-1.4.0/gokart/config_params.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/conflict_prevention_lock/task_lock.py` & `gokart-1.4.0/gokart/conflict_prevention_lock/task_lock.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/conflict_prevention_lock/task_lock_wrappers.py` & `gokart-1.4.0/gokart/conflict_prevention_lock/task_lock_wrappers.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/file_processor.py` & `gokart-1.4.0/gokart/file_processor.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/gcs_config.py` & `gokart-1.4.0/gokart/gcs_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/gcs_zip_client.py` & `gokart-1.4.0/gokart/gcs_zip_client.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/info.py` & `gokart-1.4.0/gokart/info.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/object_storage.py` & `gokart-1.4.0/gokart/object_storage.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/pandas_type_config.py` & `gokart-1.4.0/gokart/pandas_type_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/parameter.py` & `gokart-1.4.0/gokart/parameter.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/run.py` & `gokart-1.4.0/gokart/run.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/s3_config.py` & `gokart-1.4.0/gokart/s3_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/s3_zip_client.py` & `gokart-1.4.0/gokart/s3_zip_client.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/slack/event_aggregator.py` & `gokart-1.4.0/gokart/slack/event_aggregator.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/slack/slack_api.py` & `gokart-1.4.0/gokart/slack/slack_api.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/slack/slack_config.py` & `gokart-1.4.0/gokart/slack/slack_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/target.py` & `gokart-1.4.0/gokart/target.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from glob import glob
 from logging import getLogger
 from typing import Any, Optional
 
 import luigi
 import numpy as np
 import pandas as pd
-from tqdm import tqdm
 
 from gokart.conflict_prevention_lock.task_lock import TaskLockParams, make_task_lock_params
 from gokart.conflict_prevention_lock.task_lock_wrappers import wrap_dump_with_lock, wrap_load_with_lock, wrap_remove_with_lock
 from gokart.file_processor import FileProcessor, make_file_processor
 from gokart.object_storage import ObjectStorage
 from gokart.zip_client_util import make_zip_client
 
@@ -175,15 +174,15 @@
 
         if df.empty:
             df.to_pickle(os.path.join(dir_path, 'data_0.pkl'))
             return
 
         split_size = df.values.nbytes // self.max_byte + 1
         logger.info(f'saving a large pdDataFrame with split_size={split_size}')
-        for i, idx in tqdm(list(enumerate(np.array_split(range(df.shape[0]), split_size)))):
+        for i, idx in list(enumerate(np.array_split(range(df.shape[0]), split_size))):
             df.iloc[idx[0] : idx[-1] + 1].to_pickle(os.path.join(dir_path, f'data_{i}.pkl'))
 
     @staticmethod
     def load(file_path: str) -> pd.DataFrame:
         dir_path = os.path.dirname(file_path)
 
         return pd.concat([pd.read_pickle(file_path) for file_path in glob(os.path.join(dir_path, 'data_*.pkl'))])
```

### Comparing `gokart-1.3.0/gokart/task.py` & `gokart-1.4.0/gokart/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hashlib
 import inspect
 import os
+import random
 import types
 from importlib import import_module
 from logging import getLogger
 from typing import Any, Callable, Dict, List, Optional, Set, Union
 
 import luigi
 import pandas as pd
@@ -82,14 +83,18 @@
         significant=False,
     )
     complete_check_at_run: bool = ExplicitBoolParameter(
         default=True, description='Check if output file exists at run. If exists, run() will be skipped.', significant=False
     )
     should_lock_run: bool = ExplicitBoolParameter(default=False, significant=False, description='Whether to use redis lock or not at task run.')
 
+    @property
+    def priority(self):
+        return random.Random().random()  # seed is fixed, so we need to use random.Random().random() instead f random.random()
+
     def __init__(self, *args, **kwargs):
         self._add_configuration(kwargs, 'TaskOnKart')
         # 'This parameter is dumped into "workspace_directory/log/task_log/" when this task finishes with success.'
         self.task_log = dict()
         self.task_unique_id = None
         super(TaskOnKart, self).__init__(*args, **kwargs)
         self._rerun_state = self.rerun
```

### Comparing `gokart-1.3.0/gokart/testing/check_if_run_with_empty_data_frame.py` & `gokart-1.4.0/gokart/testing/check_if_run_with_empty_data_frame.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/testing/pandas_assert.py` & `gokart-1.4.0/gokart/testing/pandas_assert.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/tree/task_info.py` & `gokart-1.4.0/gokart/tree/task_info.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/tree/task_info_formatter.py` & `gokart-1.4.0/gokart/tree/task_info_formatter.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/utils.py` & `gokart-1.4.0/gokart/utils.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/workspace_management.py` & `gokart-1.4.0/gokart/workspace_management.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/gokart/zip_client.py` & `gokart-1.4.0/gokart/zip_client.py`

 * *Files identical despite different names*

### Comparing `gokart-1.3.0/pyproject.toml` & `gokart-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gokart"
-version = "1.3.0"  # using poetry-dynamic-versioning
+version = "1.4.0"  # using poetry-dynamic-versioning
 description="Gokart solves reproducibility, task dependencies, constraints of good code, and ease of use for Machine Learning Pipeline. [Documentation](https://gokart.readthedocs.io/en/latest/)"
 authors = ["M3, inc."]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/m3dev/gokart"
 repository = "https://github.com/m3dev/gokart"
 documentation = "https://gokart.readthedocs.io/en/latest/"
@@ -18,15 +18,14 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 luigi = "*"
 boto3 = "*"
 slack-sdk = "^3"
 pandas = "*"
 numpy = "*"
-tqdm = "*"
 google-auth = "*"
 pyarrow = "*"
 uritemplate = "*"
 google-api-python-client = "*"
 APScheduler = "*"
 redis = "*"
 dill = "*"
@@ -42,27 +41,28 @@
 lupa = "*"
 fakeredis = "*"
 mypy = "*"
 types-redis = "*"
 matplotlib = "*"
 
 [tool.ruff]
+line-length = 160
+exclude = ["venv/*", "tox/*"]
+
+[tool.ruff.lint]
 # All the rules are listed on https://docs.astral.sh/ruff/rules/
 extend-select = [
   "B", # bugbear
   "I" # isort
 ]
 
 # B006: Do not use mutable data structures for argument defaults. They are created during function definition time. All calls to the function reuse this one instance of that data structure, persisting changes between them.
 # B008 Do not perform function calls in argument defaults.  The call is performed only once at function definition time. All calls to your function will reuse the result of that definition-time function call.  If this is intended, assign the function call to a module-level variable and use that variable as a default value.
 ignore = ["B006", "B008"]
 
-line-length = 160
-exclude = ["venv/*", "tox/*"]
-
 [tool.ruff.format]
 quote-style = "single"
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [build-system]
```

### Comparing `gokart-1.3.0/PKG-INFO` & `gokart-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokart
-Version: 1.3.0
+Version: 1.4.0
 Summary: Gokart solves reproducibility, task dependencies, constraints of good code, and ease of use for Machine Learning Pipeline. [Documentation](https://gokart.readthedocs.io/en/latest/)
 Home-page: https://github.com/m3dev/gokart
 License: MIT
 Author: M3, inc.
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,14 @@
 Requires-Dist: google-auth
 Requires-Dist: luigi
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: redis
 Requires-Dist: slack-sdk (>=3,<4)
-Requires-Dist: tqdm
 Requires-Dist: uritemplate
 Project-URL: Documentation, https://gokart.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/m3dev/gokart
 Description-Content-Type: text/markdown
 
 # gokart
```

