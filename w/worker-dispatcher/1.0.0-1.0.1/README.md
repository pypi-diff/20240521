# Comparing `tmp/worker_dispatcher-1.0.0.tar.gz` & `tmp/worker_dispatcher-1.0.1.tar.gz`

## Comparing `worker_dispatcher-1.0.0.tar` & `worker_dispatcher-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/img/introduction.planuml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/src/worker_dispatcher/__init__.py
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/src/worker_dispatcher/worker_dispatcher.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/LICENSE
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.1/img/introduction.planuml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.1/src/worker_dispatcher/__init__.py
+-rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.1/src/worker_dispatcher/worker_dispatcher.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.1/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8465 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.1/PKG-INFO
```

### Comparing `worker_dispatcher-1.0.0/.github/workflows/python-publish.yml` & `worker_dispatcher-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-1.0.0/src/worker_dispatcher/worker_dispatcher.py` & `worker_dispatcher-1.0.1/src/worker_dispatcher/worker_dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,37 +26,38 @@
         'result_callback': False
     },
     'worker': {
         'number': multiprocessing.cpu_count(),
         'per_second': 0,                # If greater than 0, the specified number of workers run at set intervals.
         'cumulative': False,            # Cumulative mode for per_second method.
         'multiprocessing': False
-    }
+    },
+    'verbose': True
 }
 
 # Global variable
 results = []
 logs = []
 result_info = {}
 
 # Start function
-def start(userConfig: dict) -> list:
+def start(user_config: dict) -> list:
 
     global results, logs, result_info
     results = []
     logs = []
 
     # Merge config with 2 level
     config = copy.deepcopy(default_config)
     for level1_key in config.keys():
-        if level1_key in userConfig:
+        if level1_key in user_config:
             if isinstance(config[level1_key], dict):
-                config[level1_key].update(userConfig[level1_key])
+                config[level1_key].update(user_config[level1_key])
             else:
-                config[level1_key] = userConfig[level1_key]
+                config[level1_key] = user_config[level1_key]
 
     # Multi-processing handler
     use_multiprocessing = config['worker']['multiprocessing']
     if use_multiprocessing:
         in_child_process = (multiprocessing.current_process().name != 'MainProcess')
         # Return False if is in worker process to let caller handle
         if in_child_process:
@@ -94,23 +95,25 @@
             task_list.append(data)
 
     # Worker dispatch
     worker_num = config['worker']['number']
     worker_num = worker_num if isinstance(worker_num, int) else 1
     worker_per_second = config['worker']['per_second'] if config['worker']['per_second'] else 0
     max_workers = len(task_list) if worker_per_second else worker_num
-    print("Worker Dispatcher Configutation:")
-    print("- Task Number: {}".format(len(task_list)))
-    print("- Worker Type:", "Processing" if use_multiprocessing else "Threading")
-    print("- Worker Number: {}".format(worker_num))
-    print("- Worker Per Second: {}".format(worker_per_second))
-    print("- Max Worker: {}".format(max_workers))
+    if config['verbose']:
+        print("Worker Dispatcher Configutation:")
+        print("- Task Number: {}".format(len(task_list)))
+        print("- Worker Type:", "Processing" if use_multiprocessing else "Threading")
+        print("- Worker Number: {}".format(worker_num))
+        print("- Worker Per Second: {}".format(worker_per_second))
+        print("- Max Worker: {}".format(max_workers))
     pool_executor_class = concurrent.futures.ProcessPoolExecutor if use_multiprocessing else concurrent.futures.ThreadPoolExecutor
     result_info['started_at'] = time.time()
-    print("\n--- Start to dispatch workers ---\n")
+    if config['verbose']:
+        print("\n--- Start to dispatch workers ---\n")
 
     # Pool Executor
     with pool_executor_class(max_workers=max_workers) as executor:
         pool_results = []
         per_second_count = worker_num
         # Task dispatch
         for task in task_list:
@@ -132,16 +135,17 @@
                 result = config['task']['result_callback'](config=config['task']['config'], id=log['task_id'], result=log['result'], log=log)
             logs.append(log)
             results.append(result)
         # results = [result.result() for result in concurrent.futures.as_completed(pool_results)]
 
     result_info['ended_at'] = time.time()
     result_info['duration'] = result_info['ended_at'] - result_info['started_at']
-    print("\n--- End of worker dispatch ---\n")
-    print("Spend Time: {:.6f} sec".format(result_info['duration']))
+    if config['verbose']:
+        print("\n--- End of worker dispatch ---\n")
+        print("Spend Time: {:.6f} sec".format(result_info['duration']))
     return results
 
 # Worker function
 def consume_task(data, config) -> dict:
     started_at = time.time()
     return_value = config['task']['callback'](config=config['task']['config'], id=data['id'], task=data['task'])
     ended_at = time.time()
```

### Comparing `worker_dispatcher-1.0.0/.gitignore` & `worker_dispatcher-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-1.0.0/LICENSE` & `worker_dispatcher-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-1.0.0/README.md` & `worker_dispatcher-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 |[task.callback](#taskcallback)             |callable |(sample)          |The callback function called by each worker runs|
 |task.config       |multitype|list         |The custom variable to be passed to the callback function|
 |[task.result_callback](#taskresultcallback) |callable |Null          |The callback function called when each task processes the result|
 |worker.number     |int      |(auto)       |The number of workers to fork. <br>(The default value is the number of local CPU cores)|
 |worker.per_second |float    |0            |If greater than 0, the specified number of workers run forcefully at set intervals.|
 |worker.cumulative |bool     |False        |Cumulative mode for per_second method.|
 |worker.multiprocessing                     |boolean  |False        |Use multi-processing instead of the default multi-threading |
+|verbose|bool      |bool     |True         |Enables or disables verbose mode for detailed output.|
 
 
 #### task.callback
 
 The callback function called by each worker runs
 
 ```python
```

### Comparing `worker_dispatcher-1.0.0/pyproject.toml` & `worker_dispatcher-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "worker_dispatcher"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Nick Tsai", email="myintaer@gmail.com" },
 ]
 description = "A flexible task dispatcher for Python with multiple threading or processing control"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `worker_dispatcher-1.0.0/PKG-INFO` & `worker_dispatcher-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: worker_dispatcher
-Version: 1.0.0
+Version: 1.0.1
 Summary: A flexible task dispatcher for Python with multiple threading or processing control
 Project-URL: Homepage, https://github.com/yidas/python-worker-dispatcher
 Project-URL: Issues, https://github.com/yidas/python-worker-dispatcher/issues
 Author-email: Nick Tsai <myintaer@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -161,14 +161,15 @@
 |[task.callback](#taskcallback)             |callable |(sample)          |The callback function called by each worker runs|
 |task.config       |multitype|list         |The custom variable to be passed to the callback function|
 |[task.result_callback](#taskresultcallback) |callable |Null          |The callback function called when each task processes the result|
 |worker.number     |int      |(auto)       |The number of workers to fork. <br>(The default value is the number of local CPU cores)|
 |worker.per_second |float    |0            |If greater than 0, the specified number of workers run forcefully at set intervals.|
 |worker.cumulative |bool     |False        |Cumulative mode for per_second method.|
 |worker.multiprocessing                     |boolean  |False        |Use multi-processing instead of the default multi-threading |
+|verbose|bool      |bool     |True         |Enables or disables verbose mode for detailed output.|
 
 
 #### task.callback
 
 The callback function called by each worker runs
 
 ```python
```

