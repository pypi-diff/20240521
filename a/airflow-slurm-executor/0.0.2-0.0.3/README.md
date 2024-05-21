# Comparing `tmp/airflow_slurm_executor-0.0.2.tar.gz` & `tmp/airflow_slurm_executor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_slurm_executor-0.0.2.tar", last modified: Tue May 21 18:09:05 2024, max compression
+gzip compressed data, was "airflow_slurm_executor-0.0.3.tar", last modified: Tue May 21 20:17:30 2024, max compression
```

## Comparing `airflow_slurm_executor-0.0.2.tar` & `airflow_slurm_executor-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 18:09:05.495353 airflow_slurm_executor-0.0.2/
--rw-r--r--   0 sunset666   (501) staff       (20)    11357 2024-05-21 16:59:13.000000 airflow_slurm_executor-0.0.2/LICENSE
--rw-r--r--   0 sunset666   (501) staff       (20)     1499 2024-05-21 18:09:05.495045 airflow_slurm_executor-0.0.2/PKG-INFO
--rw-r--r--   0 sunset666   (501) staff       (20)      976 2024-05-21 17:12:43.000000 airflow_slurm_executor-0.0.2/README.md
-drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 18:09:05.492074 airflow_slurm_executor-0.0.2/airflow_slurm_executor/
--rw-r--r--   0 sunset666   (501) staff       (20)       63 2024-05-21 18:07:29.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor/__init__.py
--rw-r--r--   0 sunset666   (501) staff       (20)     4188 2024-05-21 16:31:17.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor/slurm_control.py
--rw-r--r--   0 sunset666   (501) staff       (20)     2726 2024-05-21 18:07:29.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor/slurm_executor.py
-drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 18:09:05.494696 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/
--rw-r--r--   0 sunset666   (501) staff       (20)     1499 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/PKG-INFO
--rw-r--r--   0 sunset666   (501) staff       (20)      371 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/SOURCES.txt
--rw-r--r--   0 sunset666   (501) staff       (20)        1 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/dependency_links.txt
--rw-r--r--   0 sunset666   (501) staff       (20)       22 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/requires.txt
--rw-r--r--   0 sunset666   (501) staff       (20)       23 2024-05-21 18:09:05.000000 airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/top_level.txt
--rw-r--r--   0 sunset666   (501) staff       (20)       38 2024-05-21 18:09:05.495411 airflow_slurm_executor-0.0.2/setup.cfg
--rw-r--r--   0 sunset666   (501) staff       (20)      696 2024-05-21 18:08:21.000000 airflow_slurm_executor-0.0.2/setup.py
+drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 20:17:30.978956 airflow_slurm_executor-0.0.3/
+-rw-r--r--   0 sunset666   (501) staff       (20)    11357 2024-05-21 16:59:13.000000 airflow_slurm_executor-0.0.3/LICENSE
+-rw-r--r--   0 sunset666   (501) staff       (20)     1499 2024-05-21 20:17:30.978586 airflow_slurm_executor-0.0.3/PKG-INFO
+-rw-r--r--   0 sunset666   (501) staff       (20)      976 2024-05-21 17:12:43.000000 airflow_slurm_executor-0.0.3/README.md
+drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 20:17:30.975371 airflow_slurm_executor-0.0.3/airflow_slurm_executor/
+-rw-r--r--   0 sunset666   (501) staff       (20)       63 2024-05-21 18:07:29.000000 airflow_slurm_executor-0.0.3/airflow_slurm_executor/__init__.py
+-rw-r--r--   0 sunset666   (501) staff       (20)     4189 2024-05-21 18:57:26.000000 airflow_slurm_executor-0.0.3/airflow_slurm_executor/slurm_control.py
+-rw-r--r--   0 sunset666   (501) staff       (20)     2726 2024-05-21 18:07:29.000000 airflow_slurm_executor-0.0.3/airflow_slurm_executor/slurm_executor.py
+drwxr-xr-x   0 sunset666   (501) staff       (20)        0 2024-05-21 20:17:30.977573 airflow_slurm_executor-0.0.3/airflow_slurm_executor.egg-info/
+-rw-r--r--   0 sunset666   (501) staff       (20)     1499 2024-05-21 20:17:30.000000 airflow_slurm_executor-0.0.3/airflow_slurm_executor.egg-info/PKG-INFO
+-rw-r--r--   0 sunset666   (501) staff       (20)      371 2024-05-21 20:17:30.000000 airflow_slurm_executor-0.0.3/airflow_slurm_executor.egg-info/SOURCES.txt
+-rw-r--r--   0 sunset666   (501) staff       (20)        1 2024-05-21 20:17:30.000000 airflow_slurm_executor-0.0.3/airflow_slurm_executor.egg-info/dependency_links.txt
+-rw-r--r--   0 sunset666   (501) staff       (20)       22 2024-05-21 20:17:30.000000 airflow_slurm_executor-0.0.3/airflow_slurm_executor.egg-info/requires.txt
+-rw-r--r--   0 sunset666   (501) staff       (20)       23 2024-05-21 20:17:30.000000 airflow_slurm_executor-0.0.3/airflow_slurm_executor.egg-info/top_level.txt
+-rw-r--r--   0 sunset666   (501) staff       (20)       38 2024-05-21 20:17:30.979472 airflow_slurm_executor-0.0.3/setup.cfg
+-rw-r--r--   0 sunset666   (501) staff       (20)      696 2024-05-21 20:16:33.000000 airflow_slurm_executor-0.0.3/setup.py
```

### Comparing `airflow_slurm_executor-0.0.2/LICENSE` & `airflow_slurm_executor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_slurm_executor-0.0.2/PKG-INFO` & `airflow_slurm_executor-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_slurm_executor
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plugin for Airflow to connect to slurm clusters
 Home-page: https://github.com/sunset666/Airflow-Slurm-Executor
 Author: Sunset666
 Author-email: sunset666@sunset666.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `airflow_slurm_executor-0.0.2/README.md` & `airflow_slurm_executor-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `airflow_slurm_executor-0.0.2/airflow_slurm_executor/slurm_control.py` & `airflow_slurm_executor-0.0.3/airflow_slurm_executor/slurm_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,25 +120,25 @@
 def __compose_run_job_arguments(cmd, queue=None, executor_config=None, job_name=None):
     gpu_config = None
     output_path = None
     cpu_node = None
     account = None
     if executor_config:
         try:
-            gpu_config = executor_config.get("SlurmExecutor").get("gpu_params")
+            gpu_config = executor_config.get("SlurmExecutor").get("gpu_config")
         except:
             pass
         try:
             output_path = (
                 executor_config.get("SlurmExecutor").get("slurm_output_path") + "slurm-%j.out"
             )
         except:
             pass
         try:
-            cpu_node = executor_config.get("SlurmExecutor").get("cpu_node")
+            cpu_node = executor_config.get("SlurmExecutor").get("cpu_nodes")
         except:
             pass
         try:
             account = executor_config.get("SlurmExecutor").get("account")
         except:
             pass
```

### Comparing `airflow_slurm_executor-0.0.2/airflow_slurm_executor/slurm_executor.py` & `airflow_slurm_executor-0.0.3/airflow_slurm_executor/slurm_executor.py`

 * *Files identical despite different names*

### Comparing `airflow_slurm_executor-0.0.2/airflow_slurm_executor.egg-info/PKG-INFO` & `airflow_slurm_executor-0.0.3/airflow_slurm_executor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_slurm_executor
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plugin for Airflow to connect to slurm clusters
 Home-page: https://github.com/sunset666/Airflow-Slurm-Executor
 Author: Sunset666
 Author-email: sunset666@sunset666.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `airflow_slurm_executor-0.0.2/setup.py` & `airflow_slurm_executor-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="airflow_slurm_executor",
-    version="0.0.2",
+    version="0.0.3",
     author="Sunset666",
     author_email="sunset666@sunset666.net",
     description="Plugin for Airflow to connect to slurm clusters",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/sunset666/Airflow-Slurm-Executor",
     packages=find_packages(),
```

