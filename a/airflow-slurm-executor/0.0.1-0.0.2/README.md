# Comparing `tmp/airflow_slurm_executor-0.0.1.tar.gz` & `tmp/airflow_slurm_executor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_slurm_executor-0.0.1.tar", last modified: Tue May 21 17:26:11 2024, max compression
+gzip compressed data, was "airflow_slurm_executor-0.0.2.tar", last modified: Tue May 21 18:09:05 2024, max compression
```

## Comparing `airflow_slurm_executor-0.0.1.tar` & `airflow_slurm_executor-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 17:26:11.311132 airflow_slurm_executor-0.0.1/
--rw-r--r--   0 sunset666   (501) staff       (20)    11357 2024-05-21 16:59:13.000000 airflow_slurm_executor-0.0.1/LICENSE
--rw-r--r--   0 sunset666   (501) staff       (20)     1517 2024-05-21 17:26:11.310791 airflow_slurm_executor-0.0.1/PKG-INFO
--rw-r--r--   0 sunset666   (501) staff       (20)      976 2024-05-21 17:12:43.000000 airflow_slurm_executor-0.0.1/README.md
-drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 17:26:11.308399 airflow_slurm_executor-0.0.1/airflow_slurm_executor/
--rw-r--r--   0 sunset666   (501) staff       (20)        0 2024-05-21 16:35:00.000000 airflow_slurm_executor-0.0.1/airflow_slurm_executor/__init__.py
--rw-r--r--   0 sunset666   (501) staff       (20)     4188 2024-05-21 16:31:17.000000 airflow_slurm_executor-0.0.1/airflow_slurm_executor/slurm_control.py
--rw-r--r--   0 sunset666   (501) staff       (20)     2703 2024-05-21 16:39:04.000000 airflow_slurm_executor-0.0.1/airflow_slurm_executor/slurm_executor.py
--rw-r--r--   0 sunset666   (501) staff       (20)      202 2024-05-21 16:39:04.000000 airflow_slurm_executor-0.0.1/airflow_slurm_executor/slurm_executor_plugin.py
-drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 17:26:11.310415 airflow_slurm_executor-0.0.1/airflow_slurm_executor.egg-info/
--rw-r--r--   0 sunset666   (501) staff       (20)     1517 2024-05-21 17:26:11.000000 airflow_slurm_executor-0.0.1/airflow_slurm_executor.egg-info/PKG-INFO
--rw-r--r--   0 sunset666   (501) staff       (20)      419 2024-05-21 17:26:11.000000 airflow_slurm_executor-0.0.1/airflow_slurm_executor.egg-info/SOURCES.txt
--rw-r--r--   0 sunset666   (501) staff       (20)        1 2024-05-21 17:26:11.000000 airflow_slurm_executor-0.0.1/airflow_slurm_executor.egg-info/dependency_links.txt
--rw-r--r--   0 sunset666   (501) staff       (20)       22 2024-05-21 17:26:11.000000 airflow_slurm_executor-0.0.1/airflow_slurm_executor.egg-info/requires.txt
--rw-r--r--   0 sunset666   (501) staff       (20)       23 2024-05-21 17:26:11.000000 airflow_slurm_executor-0.0.1/airflow_slurm_executor.egg-info/top_level.txt
--rw-r--r--   0 sunset666   (501) staff       (20)       38 2024-05-21 17:26:11.311205 airflow_slurm_executor-0.0.1/setup.cfg
--rw-r--r--   0 sunset666   (501) staff       (20)      714 2024-05-21 17:25:24.000000 airflow_slurm_executor-0.0.1/setup.py
+drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 18:09:05.495353 airflow_slurm_executor-0.0.2/
+-rw-r--r--   0 sunset666   (501) staff       (20)    11357 2024-05-21 16:59:13.000000 airflow_slurm_executor-0.0.2/LICENSE
+-rw-r--r--   0 sunset666   (501) staff       (20)     1499 2024-05-21 18:09:05.495045 airflow_slurm_executor-0.0.2/PKG-INFO
+-rw-r--r--   0 sunset666   (501) staff       (20)      976 2024-05-21 17:12:43.000000 airflow_slurm_executor-0.0.2/README.md
+drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 18:09:05.492074 airflow_slurm_executor-0.0.2/airflow_slurm_executor/
+-rw-r--r--   0 sunset666   (501) staff       (20)       63 2024-05-21 18:07:29.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor/__init__.py
+-rw-r--r--   0 sunset666   (501) staff       (20)     4188 2024-05-21 16:31:17.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor/slurm_control.py
+-rw-r--r--   0 sunset666   (501) staff       (20)     2726 2024-05-21 18:07:29.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor/slurm_executor.py
+drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 18:09:05.494696 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/
+-rw-r--r--   0 sunset666   (501) staff       (20)     1499 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/PKG-INFO
+-rw-r--r--   0 sunset666   (501) staff       (20)      371 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/SOURCES.txt
+-rw-r--r--   0 sunset666   (501) staff       (20)        1 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/dependency_links.txt
+-rw-r--r--   0 sunset666   (501) staff       (20)       22 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/requires.txt
+-rw-r--r--   0 sunset666   (501) staff       (20)       23 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/top_level.txt
+-rw-r--r--   0 sunset666   (501) staff       (20)       38 2024-05-21 18:09:05.495411 airflow_slurm_executor-0.0.2/setup.cfg
+-rw-r--r--   0 sunset666   (501) staff       (20)      696 2024-05-21 18:08:21.000000 airflow_slurm_executor-0.0.2/setup.py
```

### Comparing `airflow_slurm_executor-0.0.1/LICENSE` & `airflow_slurm_executor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_slurm_executor-0.0.1/PKG-INFO` & `airflow_slurm_executor-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: airflow_slurm_executor
-Version: 0.0.1
-Summary: Pluging for Airflow to connect to slurm clusters
+Version: 0.0.2
+Summary: Plugin for Airflow to connect to slurm clusters
 Home-page: https://github.com/sunset666/Airflow-Slurm-Executor
-Author: Sunset666 (David Betancur)
+Author: Sunset666
 Author-email: sunset666@sunset666.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `airflow_slurm_executor-0.0.1/README.md` & `airflow_slurm_executor-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `airflow_slurm_executor-0.0.1/airflow_slurm_executor/slurm_control.py` & `airflow_slurm_executor-0.0.2/airflow_slurm_executor/slurm_control.py`

 * *Files identical despite different names*

### Comparing `airflow_slurm_executor-0.0.1/airflow_slurm_executor/slurm_executor.py` & `airflow_slurm_executor-0.0.2/airflow_slurm_executor/slurm_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from airflow.plugins_manager import AirflowPlugin
 from airflow.executors.base_executor import BaseExecutor
 from airflow.utils.state import State
-from slurm_control import get_jobs_status, run_job
+from airflow_slurm_executor.slurm_control import get_jobs_status, run_job
 import logging
 import uuid
 import sys
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `airflow_slurm_executor-0.0.1/airflow_slurm_executor.egg-info/PKG-INFO` & `airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: airflow_slurm_executor
-Version: 0.0.1
-Summary: Pluging for Airflow to connect to slurm clusters
+Version: 0.0.2
+Summary: Plugin for Airflow to connect to slurm clusters
 Home-page: https://github.com/sunset666/Airflow-Slurm-Executor
-Author: Sunset666 (David Betancur)
+Author: Sunset666
 Author-email: sunset666@sunset666.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `airflow_slurm_executor-0.0.1/setup.py` & `airflow_slurm_executor-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="airflow_slurm_executor",
-    version="0.0.1",
-    author="Sunset666 (David Betancur)",
+    version="0.0.2",
+    author="Sunset666",
     author_email="sunset666@sunset666.net",
-    description="Pluging for Airflow to connect to slurm clusters",
+    description="Plugin for Airflow to connect to slurm clusters",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/sunset666/Airflow-Slurm-Executor",
     packages=find_packages(),
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: Apache Software License",
                  "Operating System :: OS Independent"],
```

