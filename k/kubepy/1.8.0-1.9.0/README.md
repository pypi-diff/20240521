# Comparing `tmp/kubepy-1.8.0.tar.gz` & `tmp/kubepy-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kubepy-1.8.0.tar", last modified: Tue Jun 27 10:16:35 2017, max compression
+gzip compressed data, was "dist/kubepy-1.9.0.tar", last modified: Thu Nov 23 11:42:15 2017, max compression
```

## Comparing `kubepy-1.8.0.tar` & `kubepy-1.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 kubag     (1016) developers  (1100)        0 2017-06-27 10:16:35.000000 kubepy-1.8.0/
-drwxr-xr-x   0 kubag     (1016) developers  (1100)        0 2017-06-27 10:16:35.000000 kubepy-1.8.0/kubepy/
--rw-r--r--   0 kubag     (1016) developers  (1100)     1701 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/definition_manager.py
-drwxr-xr-x   0 kubag     (1016) developers  (1100)        0 2017-06-27 10:16:35.000000 kubepy-1.8.0/kubepy/commands/
--rwxr-xr-x   0 kubag     (1016) developers  (1100)     1117 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/commands/apply_all.py
--rw-r--r--   0 kubag     (1016) developers  (1100)        0 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/commands/__init__.py
--rwxr-xr-x   0 kubag     (1016) developers  (1100)     1656 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/commands/apply_one.py
--rw-r--r--   0 kubag     (1016) developers  (1100)     1152 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/definition_merger.py
--rw-r--r--   0 kubag     (1016) developers  (1100)     1902 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/api.py
--rw-r--r--   0 kubag     (1016) developers  (1100)        0 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/__init__.py
--rw-r--r--   0 kubag     (1016) developers  (1100)      576 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/base_commands.py
--rw-r--r--   0 kubag     (1016) developers  (1100)     2319 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/definition_transformers.py
--rw-r--r--   0 kubag     (1016) developers  (1100)     8008 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/appliers.py
--rw-r--r--   0 kubag     (1016) developers  (1100)     2235 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy/appliers_options.py
--rw-r--r--   0 kubag     (1016) developers  (1100)      640 2017-06-27 10:16:35.000000 kubepy-1.8.0/PKG-INFO
--rw-r--r--   0 kubag     (1016) developers  (1100)     1080 2017-06-27 10:16:34.000000 kubepy-1.8.0/setup.py
-drwxr-xr-x   0 kubag     (1016) developers  (1100)        0 2017-06-27 10:16:35.000000 kubepy-1.8.0/kubepy.egg-info/
--rw-r--r--   0 kubag     (1016) developers  (1100)        7 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy.egg-info/top_level.txt
--rw-r--r--   0 kubag     (1016) developers  (1100)        1 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy.egg-info/dependency_links.txt
--rw-r--r--   0 kubag     (1016) developers  (1100)      640 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy.egg-info/PKG-INFO
--rw-r--r--   0 kubag     (1016) developers  (1100)       32 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy.egg-info/requires.txt
--rw-r--r--   0 kubag     (1016) developers  (1100)      545 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy.egg-info/SOURCES.txt
--rw-r--r--   0 kubag     (1016) developers  (1100)      117 2017-06-27 10:16:34.000000 kubepy-1.8.0/kubepy.egg-info/entry_points.txt
--rw-r--r--   0 kubag     (1016) developers  (1100)       32 2017-06-27 10:16:34.000000 kubepy-1.8.0/base_requirements.txt
--rw-r--r--   0 kubag     (1016) developers  (1100)       85 2017-06-27 10:16:34.000000 kubepy-1.8.0/MANIFEST.in
--rw-r--r--   0 kubag     (1016) developers  (1100)     1516 2017-06-27 10:16:34.000000 kubepy-1.8.0/LICENSE
--rw-r--r--   0 kubag     (1016) developers  (1100)      107 2017-06-27 10:16:35.000000 kubepy-1.8.0/setup.cfg
--rw-r--r--   0 kubag     (1016) developers  (1100)     1202 2017-06-27 10:16:34.000000 kubepy-1.8.0/CHANGELOG.md
--rw-r--r--   0 kubag     (1016) developers  (1100)     2533 2017-06-27 10:16:34.000000 kubepy-1.8.0/README.md
+drwxr-xr-x   0 kubag     (1016) developers  (1100)        0 2017-11-23 11:42:15.000000 kubepy-1.9.0/
+drwxr-xr-x   0 kubag     (1016) developers  (1100)        0 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/
+-rw-r--r--   0 kubag     (1016) developers  (1100)     1701 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/definition_manager.py
+drwxr-xr-x   0 kubag     (1016) developers  (1100)        0 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/commands/
+-rwxr-xr-x   0 kubag     (1016) developers  (1100)     1117 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/commands/apply_all.py
+-rw-r--r--   0 kubag     (1016) developers  (1100)        0 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/commands/__init__.py
+-rwxr-xr-x   0 kubag     (1016) developers  (1100)     1656 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/commands/apply_one.py
+-rw-r--r--   0 kubag     (1016) developers  (1100)     1152 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/definition_merger.py
+-rw-r--r--   0 kubag     (1016) developers  (1100)     1902 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/api.py
+-rw-r--r--   0 kubag     (1016) developers  (1100)        0 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/__init__.py
+-rw-r--r--   0 kubag     (1016) developers  (1100)      576 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/base_commands.py
+-rw-r--r--   0 kubag     (1016) developers  (1100)     2319 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/definition_transformers.py
+-rw-r--r--   0 kubag     (1016) developers  (1100)     8031 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/appliers.py
+-rw-r--r--   0 kubag     (1016) developers  (1100)     2235 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy/appliers_options.py
+-rw-r--r--   0 kubag     (1016) developers  (1100)      640 2017-11-23 11:42:15.000000 kubepy-1.9.0/PKG-INFO
+-rw-r--r--   0 kubag     (1016) developers  (1100)     1080 2017-11-23 11:42:15.000000 kubepy-1.9.0/setup.py
+drwxr-xr-x   0 kubag     (1016) developers  (1100)        0 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy.egg-info/
+-rw-r--r--   0 kubag     (1016) developers  (1100)        7 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy.egg-info/top_level.txt
+-rw-r--r--   0 kubag     (1016) developers  (1100)        1 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy.egg-info/dependency_links.txt
+-rw-r--r--   0 kubag     (1016) developers  (1100)      640 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy.egg-info/PKG-INFO
+-rw-r--r--   0 kubag     (1016) developers  (1100)       32 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy.egg-info/requires.txt
+-rw-r--r--   0 kubag     (1016) developers  (1100)      545 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy.egg-info/SOURCES.txt
+-rw-r--r--   0 kubag     (1016) developers  (1100)      117 2017-11-23 11:42:15.000000 kubepy-1.9.0/kubepy.egg-info/entry_points.txt
+-rw-r--r--   0 kubag     (1016) developers  (1100)       32 2017-11-23 11:42:15.000000 kubepy-1.9.0/base_requirements.txt
+-rw-r--r--   0 kubag     (1016) developers  (1100)       85 2017-11-23 11:42:15.000000 kubepy-1.9.0/MANIFEST.in
+-rw-r--r--   0 kubag     (1016) developers  (1100)     1516 2017-11-23 11:42:15.000000 kubepy-1.9.0/LICENSE
+-rw-r--r--   0 kubag     (1016) developers  (1100)      107 2017-11-23 11:42:15.000000 kubepy-1.9.0/setup.cfg
+-rw-r--r--   0 kubag     (1016) developers  (1100)     1283 2017-11-23 11:42:15.000000 kubepy-1.9.0/CHANGELOG.md
+-rw-r--r--   0 kubag     (1016) developers  (1100)     2621 2017-11-23 11:42:15.000000 kubepy-1.9.0/README.md
```

### Comparing `kubepy-1.8.0/kubepy/definition_manager.py` & `kubepy-1.9.0/kubepy/definition_manager.py`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/kubepy/commands/apply_all.py` & `kubepy-1.9.0/kubepy/commands/apply_all.py`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/kubepy/commands/apply_one.py` & `kubepy-1.9.0/kubepy/commands/apply_one.py`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/kubepy/definition_merger.py` & `kubepy-1.9.0/kubepy/definition_merger.py`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/kubepy/api.py` & `kubepy-1.9.0/kubepy/api.py`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/kubepy/base_commands.py` & `kubepy-1.9.0/kubepy/base_commands.py`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/kubepy/definition_transformers.py` & `kubepy-1.9.0/kubepy/definition_transformers.py`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/kubepy/appliers.py` & `kubepy-1.9.0/kubepy/appliers.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     @property
     def new_definition(self):
         raise NotImplementedError
 
 
 class ResourceApplier(BaseDefinitionApplier):
     usable_with = ['Service', 'Secret', 'StorageClass', 'PersistentVolume',
-                   'PersistentVolumeClaim', 'Ingress']
+                   'PersistentVolumeClaim', 'Ingress', 'PodDisruptionBudget']
 
     def apply(self):
         api.apply(self.definition)
 
 
 class ReplicatedTemplateResourceApplier(BaseDefinitionApplier):
     usable_with = ['Deployment', 'StatefulSet']
```

### Comparing `kubepy-1.8.0/kubepy/appliers_options.py` & `kubepy-1.9.0/kubepy/appliers_options.py`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/PKG-INFO` & `kubepy-1.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kubepy
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python wrapper on kubectl that makes deploying easy.
 Home-page: https://github.com/socialwifi/kubepy
 Author: Jakub Skiepko
 Author-email: it@socialwifi.com
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kubepy-1.8.0/setup.py` & `kubepy-1.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pip.req import parse_requirements
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name='kubepy',
-    version='1.8.0',
+    version='1.9.0',
     description='Python wrapper on kubectl that makes deploying easy.',
     author='Jakub Skiepko',
     author_email='it@socialwifi.com',
     url='https://github.com/socialwifi/kubepy',
     packages=find_packages(),
     install_requires=[str(ir.req) for ir in parse_requirements('base_requirements.txt', session=False)],
     entry_points={
```

### Comparing `kubepy-1.8.0/kubepy.egg-info/PKG-INFO` & `kubepy-1.9.0/kubepy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kubepy
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python wrapper on kubectl that makes deploying easy.
 Home-page: https://github.com/socialwifi/kubepy
 Author: Jakub Skiepko
 Author-email: it@socialwifi.com
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kubepy-1.8.0/kubepy.egg-info/SOURCES.txt` & `kubepy-1.9.0/kubepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/LICENSE` & `kubepy-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubepy-1.8.0/CHANGELOG.md` & `kubepy-1.9.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog for kubepy
 =================
 
+1.9.0 (2017-11-23)
+------------------
+
+- Support PodDisruptionBudget resource.
+
+
 1.8.0 (2017-06-27)
 ------------------
 
 - Support ingress resource.
 
 
 1.7.1 (2017-03-24)
```

### Comparing `kubepy-1.8.0/README.md` & `kubepy-1.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 # kubepy
 
 [![Latest Version](https://img.shields.io/pypi/v/kubepy.svg)](https://github.com/socialwifi/kubepy/blob/master/CHANGELOG.md)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/kubepy.svg)](https://pypi.python.org/pypi/kubepy/)
 [![Wheel Status](https://img.shields.io/pypi/wheel/kubepy.svg)](https://pypi.python.org/pypi/kubepy/)
 [![License](https://img.shields.io/pypi/l/kubepy.svg)](https://github.com/socialwifi/kubepy/blob/master/LICENSE)
 
-Python wrapper on kubectl that makes deploying easy.
+Python wrapper on `kubectl` that makes deploying easy.
 
 ## Installation
-Requires python 3.5 and configured kubectl. To install run:
+Requires python 3.5 and configured `kubectl`. To install run:
 `pip3 install kubepy`
 
 ## Usage
 You can use this package to install all yml definitions from given directory.
-Supported kinds are deployment, service, secret, job, storage class, persistent volume,
-persistent volume claim, stateful set and ingress.
-Just run `kubepy-apply-all` from a directory where all of you kubernetes definition yml files are.
+Just run `kubepy-apply-all` from a directory where all of you Kubernetes definition yml files are.
+
+Supported Kubernetes resources:
+* Deployment
+* StatefulSet
+* Job
+* Pod (used to run a one-off command)
+* Service
+* Ingress
+* Secret
+* StorageClass
+* PersistentVolume
+* PersistentVolumeClaim
+* PodDisruptionBudget
 
 Options:
 * `--directory <path>` - uses path instead of local directory.
-  Can be used multiple times to add new and partialy override existing definitions.
+  Can be used multiple times to add new and partially override existing definitions.
 * `--build-tag <tag>` - sets tag to all images without specified tag in your definition files
 * `--replace` - if present, replaces deployments instead of updating them. Default: false.
 * `--host-volume <name>=<path>` Adds host volume to each pod definition. Can be used multiple times.
-* `--env <VAR>=value` Sets environment vatiable on every container.
+* `--env <VAR>=value` Sets environment variable on every container.
 * `--max-job-retries <n>` While waiting for job to finish if it fails n times than delete job and fail.
   Job sometimes can still be executed more than n times.
 
 There is also `kubepy-apply-one` command which is called as `kubepy-apply-one name1 [name2 ...]`
 It applies only files selected files. Names should be without ".yml".
-It accepts all options from `kubepy-apply-all`. Additionaly you can pass option:
+It accepts all options from `kubepy-apply-all`. Additionally you can pass option:
 * `--show-definition` - shows definition instead of applying them.
 
 ## Applying jobs.
-Applying usualy means that underlying `kubectl apply` or `kubectl replace` is called. However applying job is treated differently.
-To ensure that job finished and succeeded kubectl waits for job to finish and fails if job failed.
+Applying usualy means that underlying `kubectl apply` or `kubectl replace` is called. However applying job is treated 
+differently.
+To ensure that job finished and succeeded `kubectl` waits for job to finish and fails if job failed.
 
 ## Applying pods.
-Usualy you don't need to aply pods manualy, but if you want to run some kind of check and you need to know if it succeeded without retries then you can use pod with `restartPolicy: Never`. Only pods with this policy are currently supported. They are treated as jobs, so applying waits for them to finish and fails if they fail.
+Usually you don't need to apply pods manually, but if you want to run some kind of check and you need to know if it 
+succeeded without retries then you can use pod with `restartPolicy: Never`. Only pods with this policy are currently 
+supported. They are treated as jobs, so applying waits for them to finish and fails if they fail.
```

