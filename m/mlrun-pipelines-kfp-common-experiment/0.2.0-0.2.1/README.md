# Comparing `tmp/mlrun-pipelines-kfp-common-experiment-0.2.0.tar.gz` & `tmp/mlrun_pipelines_kfp_common_experiment-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlrun-pipelines-kfp-common-experiment-0.2.0.tar", last modified: Mon May 13 08:31:53 2024, max compression
+gzip compressed data, was "mlrun_pipelines_kfp_common_experiment-0.2.1.tar", last modified: Tue May 21 09:11:11 2024, max compression
```

## Comparing `mlrun-pipelines-kfp-common-experiment-0.2.0.tar` & `mlrun_pipelines_kfp_common_experiment-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-13 08:31:53.256142 mlrun-pipelines-kfp-common-experiment-0.2.0/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      323 2024-05-13 08:31:53.255701 mlrun-pipelines-kfp-common-experiment-0.2.0/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       38 2024-05-13 08:31:53.256222 mlrun-pipelines-kfp-common-experiment-0.2.0/setup.cfg
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     1283 2024-05-13 08:22:31.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/setup.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-13 08:31:53.248787 mlrun-pipelines-kfp-common-experiment-0.2.0/src/
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-13 08:31:53.248581 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-13 08:31:53.251820 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      571 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/__init__.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     4363 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/helpers.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     3523 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/models.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     1747 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/mounts.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)    22762 2024-05-13 08:22:07.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/ops.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-13 08:31:53.255360 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines_kfp_common_experiment.egg-info/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      323 2024-05-13 08:31:53.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines_kfp_common_experiment.egg-info/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      453 2024-05-13 08:31:53.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines_kfp_common_experiment.egg-info/SOURCES.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)        1 2024-05-13 08:31:53.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines_kfp_common_experiment.egg-info/dependency_links.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       16 2024-05-13 08:31:53.000000 mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines_kfp_common_experiment.egg-info/top_level.txt
+drwxr-xr-x   0 Adam_Melnick   (502) staff       (20)        0 2024-05-21 09:11:11.049668 mlrun_pipelines_kfp_common_experiment-0.2.1/
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      323 2024-05-21 09:11:11.049258 mlrun_pipelines_kfp_common_experiment-0.2.1/PKG-INFO
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)       38 2024-05-21 09:11:11.049717 mlrun_pipelines_kfp_common_experiment-0.2.1/setup.cfg
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)     1283 2024-05-21 07:57:20.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/setup.py
+drwxr-xr-x   0 Adam_Melnick   (502) staff       (20)        0 2024-05-21 09:11:11.041022 mlrun_pipelines_kfp_common_experiment-0.2.1/src/
+drwxr-xr-x   0 Adam_Melnick   (502) staff       (20)        0 2024-05-21 09:11:11.040752 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/
+drwxr-xr-x   0 Adam_Melnick   (502) staff       (20)        0 2024-05-21 09:11:11.043388 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      571 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/__init__.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)     4507 2024-05-21 07:57:20.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/helpers.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)     3523 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/models.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)     1747 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/mounts.py
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)    22762 2024-05-20 10:44:01.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/ops.py
+drwxr-xr-x   0 Adam_Melnick   (502) staff       (20)        0 2024-05-21 09:11:11.048926 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines_kfp_common_experiment.egg-info/
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      323 2024-05-21 09:11:11.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines_kfp_common_experiment.egg-info/PKG-INFO
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)      453 2024-05-21 09:11:11.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines_kfp_common_experiment.egg-info/SOURCES.txt
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)        1 2024-05-21 09:11:11.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines_kfp_common_experiment.egg-info/dependency_links.txt
+-rw-r--r--   0 Adam_Melnick   (502) staff       (20)       16 2024-05-21 09:11:11.000000 mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines_kfp_common_experiment.egg-info/top_level.txt
```

### Comparing `mlrun-pipelines-kfp-common-experiment-0.2.0/setup.py` & `mlrun_pipelines_kfp_common_experiment-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import find_namespace_packages, setup
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("mlrun-kfp-setup")
 
 setup(
     name="mlrun-pipelines-kfp-common-experiment",
-    version="0.2.0",
+    version="0.2.1",
     description="MLRun Pipelines package for providing KFP 1.8 compatibility",
     author="Yaron Haviv",
     author_email="yaronh@iguazio.com",
     license="Apache License 2.0",
     url="https://github.com/mlrun/mlrun",
     packages=find_namespace_packages(
         where="src/",
```

### Comparing `mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/__init__.py` & `mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/helpers.py` & `mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,12 +116,15 @@
 
         :return: True if the external data mapping is non-empty; False otherwise.
         """
         return bool(self._external_data)
 
     def to_dict(self) -> dict:
         """
-        Converts the mapping to a dict. This method follows the attribute rules defined on __iter__
+        Converts the mapping to a dict. The dict is the result of merging the external data dict with
+        the class attributes, where the class attributes take precedence.
 
         :returns: a dict representation of the mapping.
         """
-        return {a: getattr(self, a, None) for a in self}
+        data = self._external_data.copy()
+        data.update({a: getattr(self, a, None) for a in self})
+        return data
```

### Comparing `mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/models.py` & `mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/models.py`

 * *Files identical despite different names*

### Comparing `mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/mounts.py` & `mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/mounts.py`

 * *Files identical despite different names*

### Comparing `mlrun-pipelines-kfp-common-experiment-0.2.0/src/mlrun_pipelines/common/ops.py` & `mlrun_pipelines_kfp_common_experiment-0.2.1/src/mlrun_pipelines/common/ops.py`

 * *Files identical despite different names*

