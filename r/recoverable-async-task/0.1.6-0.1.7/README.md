# Comparing `tmp/recoverable_async_task-0.1.6.tar.gz` & `tmp/recoverable_async_task-0.1.7.tar.gz`

## Comparing `recoverable_async_task-0.1.6.tar` & `recoverable_async_task-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11368 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.6/recoverable_async_task.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.6/.gitignore
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.6/README.md
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/recoverable_async_task.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/.gitignore
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/README.md
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/PKG-INFO
```

### Comparing `recoverable_async_task-0.1.6/recoverable_async_task.py` & `recoverable_async_task-0.1.7/recoverable_async_task.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import asyncio
 import functools
 import json
+import sys
 import traceback
 from pathlib import Path
 from typing import (
     AsyncIterator,
     Callable,
     Coroutine,
     Generic,
     Iterator,
-    TypedDict,
     TypeVar,
     Union,
 )
 
 from loguru import logger
 from tqdm import tqdm
 
+if sys.version_info >= (3, 11):
+    from typing import TypedDict
+else:
+    from typing_extensions import TypedDict
+
+
 JSON_ITEM = TypeVar("JSON_ITEM", bound=Union[str, int, float, bool, None])
 
 JSON = Union[JSON_ITEM, dict[str, "JSON"], list["JSON"]]
 
 T = TypeVar("T", bound=JSON)
```

### Comparing `recoverable_async_task-0.1.6/README.md` & `recoverable_async_task-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `recoverable_async_task-0.1.6/pyproject.toml` & `recoverable_async_task-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 description = "`recoverable-async-task` is a Python library that streamlines the handling of asynchronous tasks through its `RecoverableAsyncTask` class, with the added benefit of **supporting task checkpointing and resumption**. This feature ensures that tasks can pick up from where they left off in the event of unexpected failures."
 authors = [
     { name = "Haskely", email = "Haskely@live.com" }
 ]
 dependencies = [
     "tqdm>=4.66.2",
     "loguru>=0.7.2",
+    "typing-extensions>=4.11.0",
 ]
 readme = "README.md"
-requires-python = ">= 3.8"
+requires-python = ">= 3.10"
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/Haskely/recoverable-async-task"
 "Bug Reports" = "https://github.com/Haskely/recoverable-async-task/issues"
 "Source" = "https://github.com/Haskely/recoverable-async-task"
 
@@ -29,10 +30,9 @@
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.sdist]
 only-include = ["recoverable_async_task.py"]
 
-
 [tool.hatch.version]
 source = "vcs"
```

### Comparing `recoverable_async_task-0.1.6/PKG-INFO` & `recoverable_async_task-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: recoverable-async-task
-Version: 0.1.6
+Version: 0.1.7
 Summary: `recoverable-async-task` is a Python library that streamlines the handling of asynchronous tasks through its `RecoverableAsyncTask` class, with the added benefit of **supporting task checkpointing and resumption**. This feature ensures that tasks can pick up from where they left off in the event of unexpected failures.
 Project-URL: Homepage, https://github.com/Haskely/recoverable-async-task
 Project-URL: Bug Reports, https://github.com/Haskely/recoverable-async-task/issues
 Project-URL: Source, https://github.com/Haskely/recoverable-async-task
 Author-email: Haskely <Haskely@live.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: tqdm>=4.66.2
+Requires-Dist: typing-extensions>=4.11.0
 Description-Content-Type: text/markdown
 
 # recoverable-async-task: An Asynchronous Task Processing Library
 
 [中文文档](README_ZH.md) | [English](README.md)
 
 `recoverable-async-task` is a Python library that streamlines the handling of asynchronous tasks through its `RecoverableAsyncTask` class, with the added benefit of **supporting task checkpointing and resumption**. This feature ensures that tasks can pick up from where they left off in the event of unexpected failures.
```

