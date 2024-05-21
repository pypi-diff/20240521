# Comparing `tmp/handshakes-0.3.7.tar.gz` & `tmp/handshakes-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handshakes-0.3.7.tar", max compression
+gzip compressed data, was "handshakes-0.3.8.tar", max compression
```

## Comparing `handshakes-0.3.7.tar` & `handshakes-0.3.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      749 2024-05-20 21:26:47.809582 handshakes-0.3.7/README.md
--rw-r--r--   0        0        0      448 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/.version
--rw-r--r--   0        0        0       22 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/CommandLine/__init__.py
--rw-r--r--   0        0        0     8485 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/CommandLine/_init.py
--rw-r--r--   0        0        0     4326 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/CommandLine/center.py
--rw-r--r--   0        0        0       15 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/__init__.py
--rw-r--r--   0        0        0     3107 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/lifecycle.py
--rw-r--r--   0        0        0     4234 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/migrator.py
--rw-r--r--   0        0        0      570 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/models/__init__.py
--rw-r--r--   0        0        0      939 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/models/attachmentBase.py
--rw-r--r--   0        0        0     2034 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/models/config_base.py
--rw-r--r--   0        0        0     1618 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/models/dynamic_base.py
--rw-r--r--   0        0        0     1010 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/models/enums.py
--rw-r--r--   0        0        0     5833 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/models/result_base.py
--rw-r--r--   0        0        0     1167 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/models/static_base.py
--rw-r--r--   0        0        0     2102 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/models/types.py
--rw-r--r--   0        0        0       50 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/sanic_free_shared.py
--rw-r--r--   0        0        0      221 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/scripts/bump-v5.sql
--rw-r--r--   0        0        0      369 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/scripts/bump-v6.sql
--rw-r--r--   0        0        0      407 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/scripts/revert-v4.sql
--rw-r--r--   0        0        0       99 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/scripts/revert-v6.sql
--rw-r--r--   0        0        0      452 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/scripts/revert-v7.sql
--rw-r--r--   0        0        0      753 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/DBService/shared.py
--rw-r--r--   0        0        0        0 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/blueprints/__init__.py
--rw-r--r--   0        0        0     7967 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/blueprints/coreEndpoints.py
--rw-r--r--   0        0        0     1434 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/blueprints/utils.py
--rw-r--r--   0        0        0     1956 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/blueprints/writeServices.py
--rw-r--r--   0        0        0      431 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/center.py
--rw-r--r--   0        0        0     1055 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/core.py
--rw-r--r--   0        0        0      278 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/errorHandling.py
--rw-r--r--   0        0        0      954 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/internalEndpoints.py
--rw-r--r--   0        0        0      128 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/Endpoints/static_server.py
--rw-r--r--   0        0        0     2587 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/README.md
--rw-r--r--   0        0        0        0 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/__init__.py
--rw-r--r--   0        0        0     9654 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/completeTestRun.py
--rw-r--r--   0        0        0      875 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/constants.py
--rw-r--r--   0        0        0     4562 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/handlePending.py
--rw-r--r--   0        0        0     1635 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/handleTestResults.py
--rw-r--r--   0        0        0     8216 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/modifySuites.py
--rw-r--r--   0        0        0     1867 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/pruneTasks.py
--rw-r--r--   0        0        0      666 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/refer_types.py
--rw-r--r--   0        0        0     1653 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/register.py
--rw-r--r--   0        0        0    19394 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/SchedularService/start.py
--rw-r--r--   0        0        0        0 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/__init__.py
--rw-r--r--   0        0        0      193 2024-05-20 21:26:47.825582 handshakes-0.3.7/handshake/services/starter.py
--rw-r--r--   0        0        0     1576 2024-05-20 21:26:47.825582 handshakes-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 handshakes-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      749 2024-05-21 06:44:30.233990 handshakes-0.3.8/README.md
+-rw-r--r--   0        0        0      448 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/.version
+-rw-r--r--   0        0        0       22 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/CommandLine/__init__.py
+-rw-r--r--   0        0        0     8485 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/CommandLine/_init.py
+-rw-r--r--   0        0        0     4326 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/CommandLine/center.py
+-rw-r--r--   0        0        0       15 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/__init__.py
+-rw-r--r--   0        0        0     3107 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/lifecycle.py
+-rw-r--r--   0        0        0     4234 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/migrator.py
+-rw-r--r--   0        0        0      570 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/__init__.py
+-rw-r--r--   0        0        0      939 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/attachmentBase.py
+-rw-r--r--   0        0        0     2034 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/config_base.py
+-rw-r--r--   0        0        0     1618 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/dynamic_base.py
+-rw-r--r--   0        0        0     1010 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/enums.py
+-rw-r--r--   0        0        0     5833 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/result_base.py
+-rw-r--r--   0        0        0     1167 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/static_base.py
+-rw-r--r--   0        0        0     2102 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/types.py
+-rw-r--r--   0        0        0       50 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/sanic_free_shared.py
+-rw-r--r--   0        0        0      221 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/bump-v5.sql
+-rw-r--r--   0        0        0      369 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/bump-v6.sql
+-rw-r--r--   0        0        0      407 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/revert-v4.sql
+-rw-r--r--   0        0        0       99 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/revert-v6.sql
+-rw-r--r--   0        0        0      452 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/revert-v7.sql
+-rw-r--r--   0        0        0      753 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/shared.py
+-rw-r--r--   0        0        0        0 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/blueprints/__init__.py
+-rw-r--r--   0        0        0     7967 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/blueprints/coreEndpoints.py
+-rw-r--r--   0        0        0     1434 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/blueprints/utils.py
+-rw-r--r--   0        0        0     1956 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/blueprints/writeServices.py
+-rw-r--r--   0        0        0      431 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/center.py
+-rw-r--r--   0        0        0     1055 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/core.py
+-rw-r--r--   0        0        0      278 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/Endpoints/errorHandling.py
+-rw-r--r--   0        0        0      954 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/Endpoints/internalEndpoints.py
+-rw-r--r--   0        0        0      128 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/Endpoints/static_server.py
+-rw-r--r--   0        0        0     2587 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/__init__.py
+-rw-r--r--   0        0        0     9654 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/completeTestRun.py
+-rw-r--r--   0        0        0      875 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/constants.py
+-rw-r--r--   0        0        0     4562 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/handlePending.py
+-rw-r--r--   0        0        0     1635 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/handleTestResults.py
+-rw-r--r--   0        0        0     8216 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/modifySuites.py
+-rw-r--r--   0        0        0     1867 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/pruneTasks.py
+-rw-r--r--   0        0        0      666 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/refer_types.py
+-rw-r--r--   0        0        0     1653 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/register.py
+-rw-r--r--   0        0        0    19555 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/start.py
+-rw-r--r--   0        0        0        0 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/starter.py
+-rw-r--r--   0        0        0     1576 2024-05-21 06:44:30.253990 handshakes-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 handshakes-0.3.8/PKG-INFO
```

### Comparing `handshakes-0.3.7/README.md` & `handshakes-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/CommandLine/_init.py` & `handshakes-0.3.8/handshake/services/CommandLine/_init.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/CommandLine/center.py` & `handshakes-0.3.8/handshake/services/CommandLine/center.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/lifecycle.py` & `handshakes-0.3.8/handshake/services/DBService/lifecycle.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/migrator.py` & `handshakes-0.3.8/handshake/services/DBService/migrator.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/models/__init__.py` & `handshakes-0.3.8/handshake/services/DBService/models/__init__.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/models/attachmentBase.py` & `handshakes-0.3.8/handshake/services/DBService/models/attachmentBase.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/models/config_base.py` & `handshakes-0.3.8/handshake/services/DBService/models/config_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/models/dynamic_base.py` & `handshakes-0.3.8/handshake/services/DBService/models/dynamic_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/models/enums.py` & `handshakes-0.3.8/handshake/services/DBService/models/enums.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/models/result_base.py` & `handshakes-0.3.8/handshake/services/DBService/models/result_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/models/static_base.py` & `handshakes-0.3.8/handshake/services/DBService/models/static_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/models/types.py` & `handshakes-0.3.8/handshake/services/DBService/models/types.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/DBService/shared.py` & `handshakes-0.3.8/handshake/services/DBService/shared.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/Endpoints/blueprints/coreEndpoints.py` & `handshakes-0.3.8/handshake/services/Endpoints/blueprints/coreEndpoints.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/Endpoints/blueprints/utils.py` & `handshakes-0.3.8/handshake/services/Endpoints/blueprints/utils.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/Endpoints/blueprints/writeServices.py` & `handshakes-0.3.8/handshake/services/Endpoints/blueprints/writeServices.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/Endpoints/core.py` & `handshakes-0.3.8/handshake/services/Endpoints/core.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/Endpoints/internalEndpoints.py` & `handshakes-0.3.8/handshake/services/Endpoints/internalEndpoints.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/README.md` & `handshakes-0.3.8/handshake/services/SchedularService/README.md`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/completeTestRun.py` & `handshakes-0.3.8/handshake/services/SchedularService/completeTestRun.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/constants.py` & `handshakes-0.3.8/handshake/services/SchedularService/constants.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/handlePending.py` & `handshakes-0.3.8/handshake/services/SchedularService/handlePending.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/handleTestResults.py` & `handshakes-0.3.8/handshake/services/SchedularService/handleTestResults.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/modifySuites.py` & `handshakes-0.3.8/handshake/services/SchedularService/modifySuites.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/pruneTasks.py` & `handshakes-0.3.8/handshake/services/SchedularService/pruneTasks.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/refer_types.py` & `handshakes-0.3.8/handshake/services/SchedularService/refer_types.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/register.py` & `handshakes-0.3.8/handshake/services/SchedularService/register.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.7/handshake/services/SchedularService/start.py` & `handshakes-0.3.8/handshake/services/SchedularService/start.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from asyncio import gather, to_thread, TaskGroup
 from handshake.services.DBService.lifecycle import (
     init_tortoise_orm,
     db_path,
     close_connection,
 )
-from shutil import rmtree
+from shutil import rmtree, copytree
 from tarfile import open
 from pathlib import Path
 from typing import Optional
 from loguru import logger
 from tortoise.expressions import Q, RawSQL
 from handshake.services.DBService.models.result_base import (
     RunBase,
@@ -523,14 +523,19 @@
             rmtree(self.export_dir)
 
         self.export_dir.mkdir(exist_ok=False)
 
         with open(self.dashboard_build, "r:bz2") as tar_file:
             tar_file.extractall(self.export_dir)
 
+        copytree(
+            self.db_path.parent / writtenAttachmentFolderName,
+            self.export_dir / writtenAttachmentFolderName,
+        )
+
     def save_runs_query(self, feed: str, projectsFeed: str):
         (self.import_dir / EXPORT_RUNS_PAGE_FILE_NAME).write_text(feed)
         (self.import_dir / EXPORT_PROJECTS_FILE_NAME).write_text(projectsFeed)
 
     def save_test_run_level_files(self, file_name: str, testID: str, feed: str):
         (self.import_dir / testID / file_name).write_text(feed)
```

### Comparing `handshakes-0.3.7/pyproject.toml` & `handshakes-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "handshakes"
-version = "0.3.7"
+version = "0.3.8"
 description = "A service that's keen to process your test results"
 authors = ["Rahul <saihanumarahul66@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "handshake"}]
 maintainers = [
     "Rahul <saihanumarahul66@gmail.com>"
```

### Comparing `handshakes-0.3.7/PKG-INFO` & `handshakes-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handshakes
-Version: 0.3.7
+Version: 0.3.8
 Summary: A service that's keen to process your test results
 License: MIT
 Author: Rahul
 Author-email: saihanumarahul66@gmail.com
 Maintainer: Rahul
 Maintainer-email: saihanumarahul66@gmail.com
 Requires-Python: >=3.11,<3.13
```

