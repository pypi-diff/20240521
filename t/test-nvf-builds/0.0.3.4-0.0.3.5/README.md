# Comparing `tmp/test_nvf_builds-0.0.3.4.tar.gz` & `tmp/test_nvf_builds-0.0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_nvf_builds-0.0.3.4.tar", last modified: Tue May  7 08:34:39 2024, max compression
+gzip compressed data, was "test_nvf_builds-0.0.3.5.tar", last modified: Tue May 21 07:43:47 2024, max compression
```

## Comparing `test_nvf_builds-0.0.3.4.tar` & `test_nvf_builds-0.0.3.5.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.423136 test_nvf_builds-0.0.3.4/
--rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-07 07:57:47.000000 test_nvf_builds-0.0.3.4/LICENSE
--rw-r--r--   0 mostafa    (501) staff       (20)      459 2024-05-07 08:34:39.423068 test_nvf_builds-0.0.3.4/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3.4/README.md
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.419585 test_nvf_builds-0.0.3.4/oasysnow/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3.4/oasysnow/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.419706 test_nvf_builds-0.0.3.4/oasysnow/federated/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.419829 test_nvf_builds-0.0.3.4/oasysnow/federated/client/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/client/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.420226 test_nvf_builds-0.0.3.4/oasysnow/federated/client/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/client/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3468 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/client/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/client/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.420468 test_nvf_builds-0.0.3.4/oasysnow/federated/client/trainer/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/client/trainer/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5234 2024-05-06 15:59:26.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/client/trainer/trainer.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.420858 test_nvf_builds-0.0.3.4/oasysnow/federated/model/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/model/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2460 2024-05-02 13:22:42.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/model/gennet_model.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1930 2024-05-06 15:58:12.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/model/global_model.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.420986 test_nvf_builds-0.0.3.4/oasysnow/federated/server/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/server/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.421336 test_nvf_builds-0.0.3.4/oasysnow/federated/server/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/server/filters/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.421688 test_nvf_builds-0.0.3.4/oasysnow/federated/server/filters/attestation_service/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/server/filters/attestation_service/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:46:21.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/server/filters/attestation_service/server.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:28.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/server/filters/attestation_service/verification.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4442 2024-05-06 15:57:39.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/server/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/server/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.421921 test_nvf_builds-0.0.3.4/oasysnow/federated/server/model_runner/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/server/model_runner/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5424 2024-05-06 15:59:11.000000 test_nvf_builds-0.0.3.4/oasysnow/federated/server/model_runner/model_runner.py
--rw-r--r--   0 mostafa    (501) staff       (20)       22 2024-05-07 08:34:21.000000 test_nvf_builds-0.0.3.4/requirements.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      479 2024-05-07 08:34:39.423394 test_nvf_builds-0.0.3.4/setup.cfg
--rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3.4/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:34:39.422820 test_nvf_builds-0.0.3.4/test_nvf_builds.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)      459 2024-05-07 08:34:39.000000 test_nvf_builds-0.0.3.4/test_nvf_builds.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)     1185 2024-05-07 08:34:39.000000 test_nvf_builds-0.0.3.4/test_nvf_builds.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-07 08:34:39.000000 test_nvf_builds-0.0.3.4/test_nvf_builds.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       22 2024-05-07 08:34:39.000000 test_nvf_builds-0.0.3.4/test_nvf_builds.egg-info/requires.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-07 08:34:39.000000 test_nvf_builds-0.0.3.4/test_nvf_builds.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.995382 test_nvf_builds-0.0.3.5/
+-rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-07 07:57:47.000000 test_nvf_builds-0.0.3.5/LICENSE
+-rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-21 07:43:47.995312 test_nvf_builds-0.0.3.5/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3.5/README.md
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.991580 test_nvf_builds-0.0.3.5/oasysnow/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3.5/oasysnow/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.991707 test_nvf_builds-0.0.3.5/oasysnow/federated/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.991837 test_nvf_builds-0.0.3.5/oasysnow/federated/client/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.992218 test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2484 2024-05-16 12:49:15.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.992461 test_nvf_builds-0.0.3.5/oasysnow/federated/client/trainer/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/trainer/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4653 2024-05-15 14:56:42.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/trainer/trainer.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.992593 test_nvf_builds-0.0.3.5/oasysnow/federated/common/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-15 14:50:33.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.992941 test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1596 2024-05-15 14:50:41.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/server.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1324 2024-05-15 14:50:41.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/verification.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.993304 test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1803 2024-05-15 14:55:57.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/gennet_model.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1288 2024-05-15 14:55:47.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/global_model.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.993440 test_nvf_builds-0.0.3.5/oasysnow/federated/server/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.993799 test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2501 2024-05-15 14:51:04.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.994127 test_nvf_builds-0.0.3.5/oasysnow/federated/server/model_runner/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/model_runner/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4843 2024-05-15 14:56:24.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/model_runner/model_runner.py
+-rw-r--r--   0 mostafa    (501) staff       (20)       29 2024-05-15 14:24:19.000000 test_nvf_builds-0.0.3.5/requirements.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      479 2024-05-21 07:43:47.995637 test_nvf_builds-0.0.3.5/setup.cfg
+-rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3.5/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.995066 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)     1220 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       28 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/requires.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/top_level.txt
```

### Comparing `test_nvf_builds-0.0.3.4/LICENSE` & `test_nvf_builds-0.0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.4/oasysnow/federated/client/filters/filter_results.py` & `test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.4/oasysnow/federated/client/trainer/trainer.py` & `test_nvf_builds-0.0.3.5/oasysnow/federated/client/trainer/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,10 @@
-# Copyright (c) 2021, NVIDIA CORPORATION.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 import os
+
+from oasysnow.federated.common.model.global_model import GlobalModel
 os.environ["CUDA_DEVICE_ORDER"]="PCI_BUS_ID"   # see issue #152
 os.environ["CUDA_VISIBLE_DEVICES"]=""
 import tensorflow as tf
 import numpy as np
 import os
 import pickle
 from nvflare.apis.dxo import DXO, DataKind, from_shareable
@@ -25,15 +13,14 @@
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.fl_constant import FLContextKey, ReturnCode
 from nvflare.app_common.app_constant import AppConstants
 from nvflare.apis.shareable import Shareable, make_reply
 from nvflare.apis.signal import Signal
 from gennet.utils.Dataloader import *
 from gennet.utils.Utility_functions import *
-from oasysnow.federated.model.global_model import GlobalModel
 
 import random
 
 
 class Trainer(Executor):
     def __init__(self, epochs_per_round):
         super().__init__()
```

### Comparing `test_nvf_builds-0.0.3.4/oasysnow/federated/server/filters/filter_results.py` & `test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.4/oasysnow/federated/server/model_runner/model_runner.py` & `test_nvf_builds-0.0.3.5/oasysnow/federated/server/model_runner/model_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright (c) 2021, NVIDIA CORPORATION.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 import json
 import os
 import pickle
 import pathlib
 import tensorflow as tf
 
 from nvflare.apis.event_type import EventType
@@ -23,15 +9,16 @@
 from nvflare.apis.fl_context import FLContext
 from nvflare.app_common.abstract.model import ModelLearnable
 from nvflare.app_common.abstract.model import make_model_learnable
 from nvflare.app_common.abstract.model_persistor import ModelPersistor
 from nvflare.app_common.app_constant import AppConstants
 import nvflare.app_common.shareablegenerators.full_model_shareable_generator as SG
 import numpy as np
-from oasysnow.federated.model.global_model import GlobalModel
+
+from oasysnow.federated.common.model.global_model import GlobalModel
 
 
 class ModelRunner(ModelPersistor):
     def __init__(self, save_name="tf2_model.pkl"):
         super().__init__()
         self.save_name = save_name
         self.inputsize = 100
```

