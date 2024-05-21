# Comparing `tmp/fairbalance-0.0.3.tar.gz` & `tmp/fairbalance-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairbalance-0.0.3.tar", last modified: Fri May 17 14:03:07 2024, max compression
+gzip compressed data, was "fairbalance-0.0.4.tar", last modified: Tue May 21 07:26:34 2024, max compression
```

## Comparing `fairbalance-0.0.3.tar` & `fairbalance-0.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:07.030307 fairbalance-0.0.3/
--rw-rw-rw-   0        0        0      285 2024-05-17 10:03:47.000000 fairbalance-0.0.3/.gitignore
--rw-rw-rw-   0        0        0      602 2024-05-17 14:03:06.999938 fairbalance-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:06.184390 fairbalance-0.0.3/fairbalance/
--rw-rw-rw-   0        0        0       54 2024-05-15 13:38:01.000000 fairbalance-0.0.3/fairbalance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:06.397862 fairbalance-0.0.3/fairbalance/datasets/
--rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.0.3/fairbalance/datasets/__init__.py
--rw-rw-rw-   0        0        0    11236 2024-05-17 08:03:24.000000 fairbalance-0.0.3/fairbalance/datasets/_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:06.429869 fairbalance-0.0.3/fairbalance/datasets/tests/
--rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.0.3/fairbalance/datasets/tests/test_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:06.538318 fairbalance-0.0.3/fairbalance/metrics/
--rw-rw-rw-   0        0        0      263 2024-05-15 13:29:26.000000 fairbalance-0.0.3/fairbalance/metrics/__init__.py
--rw-rw-rw-   0        0        0     7673 2024-05-15 09:52:05.000000 fairbalance-0.0.3/fairbalance/metrics/_dataset_metrics.py
--rw-rw-rw-   0        0        0     2849 2024-05-15 09:30:16.000000 fairbalance-0.0.3/fairbalance/metrics/_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:06.643421 fairbalance-0.0.3/fairbalance/metrics/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.0.3/fairbalance/metrics/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:46.000000 fairbalance-0.0.3/fairbalance/metrics/tests/test_dataset_metrics.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.0.3/fairbalance/metrics/tests/test_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:06.862736 fairbalance-0.0.3/fairbalance/tools/
--rw-rw-rw-   0        0        0      305 2024-05-15 13:32:38.000000 fairbalance-0.0.3/fairbalance/tools/__init__.py
--rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.0.3/fairbalance/tools/_fairness_analysis.py
--rw-rw-rw-   0        0        0    21172 2024-05-17 09:17:53.000000 fairbalance-0.0.3/fairbalance/tools/_mitigator.py
--rw-rw-rw-   0        0        0     5271 2024-05-17 14:01:21.000000 fairbalance-0.0.3/fairbalance/tools/_processor.py
--rw-rw-rw-   0        0        0     2115 2024-05-17 08:30:33.000000 fairbalance-0.0.3/fairbalance/tools/_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:06.983984 fairbalance-0.0.3/fairbalance/tools/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.0.3/fairbalance/tools/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:25.000000 fairbalance-0.0.3/fairbalance/tools/tests/test_fairness_analysis.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.0.3/fairbalance/tools/tests/test_mitigator.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:44.000000 fairbalance-0.0.3/fairbalance/tools/tests/test_processor.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.0.3/fairbalance/tools/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:06.330531 fairbalance-0.0.3/fairbalance.egg-info/
--rw-rw-rw-   0        0        0      602 2024-05-17 14:03:03.000000 fairbalance-0.0.3/fairbalance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-17 14:03:05.000000 fairbalance-0.0.3/fairbalance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 14:03:03.000000 fairbalance-0.0.3/fairbalance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-05-17 14:03:03.000000 fairbalance-0.0.3/fairbalance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 14:03:03.000000 fairbalance-0.0.3/fairbalance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 14:03:07.033307 fairbalance-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-05-17 14:02:37.000000 fairbalance-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.768938 fairbalance-0.0.4/
+-rw-rw-rw-   0        0        0      285 2024-05-17 10:03:47.000000 fairbalance-0.0.4/.gitignore
+-rw-rw-rw-   0        0        0      602 2024-05-21 07:26:34.759725 fairbalance-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.444362 fairbalance-0.0.4/fairbalance/
+-rw-rw-rw-   0        0        0       54 2024-05-15 13:38:01.000000 fairbalance-0.0.4/fairbalance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.535697 fairbalance-0.0.4/fairbalance/datasets/
+-rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.0.4/fairbalance/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11236 2024-05-17 08:03:24.000000 fairbalance-0.0.4/fairbalance/datasets/_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.556830 fairbalance-0.0.4/fairbalance/datasets/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.0.4/fairbalance/datasets/tests/test_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.594830 fairbalance-0.0.4/fairbalance/metrics/
+-rw-rw-rw-   0        0        0      263 2024-05-15 13:29:26.000000 fairbalance-0.0.4/fairbalance/metrics/__init__.py
+-rw-rw-rw-   0        0        0     7673 2024-05-15 09:52:05.000000 fairbalance-0.0.4/fairbalance/metrics/_dataset_metrics.py
+-rw-rw-rw-   0        0        0     2849 2024-05-15 09:30:16.000000 fairbalance-0.0.4/fairbalance/metrics/_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.628465 fairbalance-0.0.4/fairbalance/metrics/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.0.4/fairbalance/metrics/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:46.000000 fairbalance-0.0.4/fairbalance/metrics/tests/test_dataset_metrics.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.0.4/fairbalance/metrics/tests/test_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.697057 fairbalance-0.0.4/fairbalance/tools/
+-rw-rw-rw-   0        0        0      305 2024-05-15 13:32:38.000000 fairbalance-0.0.4/fairbalance/tools/__init__.py
+-rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.0.4/fairbalance/tools/_fairness_analysis.py
+-rw-rw-rw-   0        0        0    21172 2024-05-17 09:17:53.000000 fairbalance-0.0.4/fairbalance/tools/_mitigator.py
+-rw-rw-rw-   0        0        0     5271 2024-05-17 14:01:21.000000 fairbalance-0.0.4/fairbalance/tools/_processor.py
+-rw-rw-rw-   0        0        0     2115 2024-05-17 08:30:33.000000 fairbalance-0.0.4/fairbalance/tools/_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.748744 fairbalance-0.0.4/fairbalance/tools/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.0.4/fairbalance/tools/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:25.000000 fairbalance-0.0.4/fairbalance/tools/tests/test_fairness_analysis.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.0.4/fairbalance/tools/tests/test_mitigator.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:44.000000 fairbalance-0.0.4/fairbalance/tools/tests/test_processor.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.0.4/fairbalance/tools/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.511926 fairbalance-0.0.4/fairbalance.egg-info/
+-rw-rw-rw-   0        0        0      602 2024-05-21 07:26:30.000000 fairbalance-0.0.4/fairbalance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-21 07:26:33.000000 fairbalance-0.0.4/fairbalance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 07:26:31.000000 fairbalance-0.0.4/fairbalance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-05-21 07:26:31.000000 fairbalance-0.0.4/fairbalance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 07:26:31.000000 fairbalance-0.0.4/fairbalance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 07:26:34.776901 fairbalance-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-05-21 07:26:22.000000 fairbalance-0.0.4/setup.py
```

### Comparing `fairbalance-0.0.3/PKG-INFO` & `fairbalance-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.0.3
+Version: 0.0.4
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
-Requires-Dist: folktables==0.0.12
+Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
-Requires-Dist: numpy==1.24.3
+Requires-Dist: numpy>=1.24.3
 Requires-Dist: pandas==2.0.3
 Requires-Dist: scikit_learn==1.3.2
 Requires-Dist: ucimlrepo==0.0.3
 
 bias mitigation by balancing target and/or protected attributes using resampling techniques
```

### Comparing `fairbalance-0.0.3/fairbalance/datasets/_datasets_loader.py` & `fairbalance-0.0.4/fairbalance/datasets/_datasets_loader.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.3/fairbalance/metrics/_dataset_metrics.py` & `fairbalance-0.0.4/fairbalance/metrics/_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.3/fairbalance/metrics/_model_metrics.py` & `fairbalance-0.0.4/fairbalance/metrics/_model_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.3/fairbalance/tools/_fairness_analysis.py` & `fairbalance-0.0.4/fairbalance/tools/_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.3/fairbalance/tools/_mitigator.py` & `fairbalance-0.0.4/fairbalance/tools/_mitigator.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.3/fairbalance/tools/_processor.py` & `fairbalance-0.0.4/fairbalance/tools/_processor.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.3/fairbalance/tools/_utils.py` & `fairbalance-0.0.4/fairbalance/tools/_utils.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.3/fairbalance.egg-info/PKG-INFO` & `fairbalance-0.0.4/fairbalance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.0.3
+Version: 0.0.4
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
-Requires-Dist: folktables==0.0.12
+Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
-Requires-Dist: numpy==1.24.3
+Requires-Dist: numpy>=1.24.3
 Requires-Dist: pandas==2.0.3
 Requires-Dist: scikit_learn==1.3.2
 Requires-Dist: ucimlrepo==0.0.3
 
 bias mitigation by balancing target and/or protected attributes using resampling techniques
```

### Comparing `fairbalance-0.0.3/fairbalance.egg-info/SOURCES.txt` & `fairbalance-0.0.4/fairbalance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.3/setup.py` & `fairbalance-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "fairbalance",
-    version = "0.0.3",
+    version = "0.0.4",
     author = "Pierre-Antoine Lequeu @ Fujitsu Luxembourg",
     author_email = "pierre-antoine.lequeu@fujitsu.com",
     description = "bias mitigation by balancing target and/or protected attributes using resampling techniques",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     install_requires=[
-        'folktables==0.0.12',
+        'folktables>=0.0.12',
         'imbalanced_learn==0.9.1',
-        'numpy==1.24.3',
+        'numpy>=1.24.3',
         'pandas==2.0.3',
         'scikit_learn==1.3.2',
         'ucimlrepo==0.0.3'
     ]
 )
```

