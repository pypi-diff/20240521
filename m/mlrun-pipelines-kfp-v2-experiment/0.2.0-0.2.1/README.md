# Comparing `tmp/mlrun-pipelines-kfp-v2-experiment-0.2.0.tar.gz` & `tmp/mlrun_pipelines_kfp_v2_experiment-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlrun-pipelines-kfp-v2-experiment-0.2.0.tar", last modified: Mon May 13 08:31:54 2024, max compression
+gzip compressed data, was "mlrun_pipelines_kfp_v2_experiment-0.2.1.tar", last modified: Tue May 21 09:10:54 2024, max compression
```

## Comparing `mlrun-pipelines-kfp-v2-experiment-0.2.0.tar` & `mlrun_pipelines_kfp_v2_experiment-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-13 08:31:54.048988 mlrun-pipelines-kfp-v2-experiment-0.2.0/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      357 2024-05-13 08:31:54.048581 mlrun-pipelines-kfp-v2-experiment-0.2.0/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       38 2024-05-13 08:31:54.049053 mlrun-pipelines-kfp-v2-experiment-0.2.0/setup.cfg
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     1336 2024-05-13 08:22:42.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/setup.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-13 08:31:54.038642 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-13 08:31:54.042563 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      871 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/helpers.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     3104 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/mixins.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     3193 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/models.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)    10470 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/mounts.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)    12573 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/ops.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      571 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/patcher.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      829 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/utils.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-13 08:31:54.048221 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines_kfp_v2_experiment.egg-info/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      357 2024-05-13 08:31:53.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines_kfp_v2_experiment.egg-info/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      520 2024-05-13 08:31:54.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines_kfp_v2_experiment.egg-info/SOURCES.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)        1 2024-05-13 08:31:53.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines_kfp_v2_experiment.egg-info/dependency_links.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       23 2024-05-13 08:31:53.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines_kfp_v2_experiment.egg-info/requires.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       16 2024-05-13 08:31:53.000000 mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines_kfp_v2_experiment.egg-info/top_level.txt
+drwxr-xr-x   0 Adam_Melnick   (502) staff       (20)        0 2024-05-21 09:10:54.152521 mlrun_pipelines_kfp_v2_experiment-0.2.1/
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      357 2024-05-21 09:10:54.152027 mlrun_pipelines_kfp_v2_experiment-0.2.1/PKG-INFO
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)       38 2024-05-21 09:10:54.152580 mlrun_pipelines_kfp_v2_experiment-0.2.1/setup.cfg
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)     1336 2024-05-21 07:57:20.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/setup.py
+drwxr-xr-x   0 Adam_Melnick   (502) staff       (20)        0 2024-05-21 09:10:54.144042 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/
+drwxr-xr-x   0 Adam_Melnick   (502) staff       (20)        0 2024-05-21 09:10:54.146927 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      871 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/helpers.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)     3104 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/mixins.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)     3875 2024-05-21 07:57:20.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/models.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)    10470 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/mounts.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)    12573 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/ops.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      571 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/patcher.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      829 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/utils.py
+drwxr-xr-x   0 Adam_Melnick   (502) staff       (20)        0 2024-05-21 09:10:54.151497 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines_kfp_v2_experiment.egg-info/
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      357 2024-05-21 09:10:54.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines_kfp_v2_experiment.egg-info/PKG-INFO
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      520 2024-05-21 09:10:54.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines_kfp_v2_experiment.egg-info/SOURCES.txt
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)        1 2024-05-21 09:10:54.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines_kfp_v2_experiment.egg-info/dependency_links.txt
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)       23 2024-05-21 09:10:54.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines_kfp_v2_experiment.egg-info/requires.txt
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)       16 2024-05-21 09:10:54.000000 mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines_kfp_v2_experiment.egg-info/top_level.txt
```

### Comparing `mlrun-pipelines-kfp-v2-experiment-0.2.0/setup.py` & `mlrun_pipelines_kfp_v2_experiment-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import find_namespace_packages, setup
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("mlrun-kfp-setup")
 
 setup(
     name="mlrun-pipelines-kfp-v2-experiment",
-    version="0.2.0",
+    version="0.2.1",
     description="MLRun Pipelines package for providing KFP 2.* compatibility",
     author="Yaron Haviv",
     author_email="yaronh@iguazio.com",
     license="Apache License 2.0",
     url="https://github.com/mlrun/mlrun",
     packages=find_namespace_packages(
         where="src/",
```

### Comparing `mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/helpers.py` & `mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/helpers.py`

 * *Files identical despite different names*

### Comparing `mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/mixins.py` & `mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/mixins.py`

 * *Files identical despite different names*

### Comparing `mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/mounts.py` & `mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/mounts.py`

 * *Files identical despite different names*

### Comparing `mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/ops.py` & `mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/ops.py`

 * *Files identical despite different names*

### Comparing `mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/patcher.py` & `mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/patcher.py`

 * *Files identical despite different names*

### Comparing `mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines/utils.py` & `mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `mlrun-pipelines-kfp-v2-experiment-0.2.0/src/mlrun_pipelines_kfp_v2_experiment.egg-info/SOURCES.txt` & `mlrun_pipelines_kfp_v2_experiment-0.2.1/src/mlrun_pipelines_kfp_v2_experiment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

