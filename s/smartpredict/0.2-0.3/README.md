# Comparing `tmp/smartpredict-0.2.tar.gz` & `tmp/smartpredict-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartpredict-0.2.tar", last modified: Tue May 21 08:59:49 2024, max compression
+gzip compressed data, was "smartpredict-0.3.tar", last modified: Tue May 21 09:05:17 2024, max compression
```

## Comparing `smartpredict-0.2.tar` & `smartpredict-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 subashanannair   (501) staff       (20)        0 2024-05-21 08:59:49.476721 smartpredict-0.2/
--rw-r--r--   0 subashanannair   (501) staff       (20)      454 2024-05-21 08:59:49.476483 smartpredict-0.2/PKG-INFO
--rw-r--r--   0 subashanannair   (501) staff       (20)       38 2024-05-21 08:59:49.476770 smartpredict-0.2/setup.cfg
--rw-r--r--   0 subashanannair   (501) staff       (20)      804 2024-05-21 08:59:29.000000 smartpredict-0.2/setup.py
-drwxr-xr-x   0 subashanannair   (501) staff       (20)        0 2024-05-21 08:59:49.475142 smartpredict-0.2/smartpredict/
--rw-r--r--   0 subashanannair   (501) staff       (20)      188 2024-05-21 08:10:34.000000 smartpredict-0.2/smartpredict/__init__.py
--rw-r--r--   0 subashanannair   (501) staff       (20)     1068 2024-05-21 08:10:56.000000 smartpredict-0.2/smartpredict/base.py
--rw-r--r--   0 subashanannair   (501) staff       (20)      634 2024-05-21 08:15:33.000000 smartpredict-0.2/smartpredict/ensemble_methods.py
--rw-r--r--   0 subashanannair   (501) staff       (20)      554 2024-05-21 08:15:17.000000 smartpredict-0.2/smartpredict/explainability.py
--rw-r--r--   0 subashanannair   (501) staff       (20)      606 2024-05-21 08:15:06.000000 smartpredict-0.2/smartpredict/feature_engineering.py
--rw-r--r--   0 subashanannair   (501) staff       (20)      800 2024-05-21 08:14:00.000000 smartpredict-0.2/smartpredict/hyperparameter_tuning.py
--rw-r--r--   0 subashanannair   (501) staff       (20)     2564 2024-05-21 08:34:53.000000 smartpredict-0.2/smartpredict/model_selection.py
--rw-r--r--   0 subashanannair   (501) staff       (20)     3256 2024-05-21 08:12:55.000000 smartpredict-0.2/smartpredict/supervised.py
--rw-r--r--   0 subashanannair   (501) staff       (20)        0 2024-05-21 07:58:09.000000 smartpredict-0.2/smartpredict/utils.py
-drwxr-xr-x   0 subashanannair   (501) staff       (20)        0 2024-05-21 08:59:49.476225 smartpredict-0.2/smartpredict.egg-info/
--rw-r--r--   0 subashanannair   (501) staff       (20)      454 2024-05-21 08:59:49.000000 smartpredict-0.2/smartpredict.egg-info/PKG-INFO
--rw-r--r--   0 subashanannair   (501) staff       (20)      479 2024-05-21 08:59:49.000000 smartpredict-0.2/smartpredict.egg-info/SOURCES.txt
--rw-r--r--   0 subashanannair   (501) staff       (20)        1 2024-05-21 08:59:49.000000 smartpredict-0.2/smartpredict.egg-info/dependency_links.txt
--rw-r--r--   0 subashanannair   (501) staff       (20)       81 2024-05-21 08:59:49.000000 smartpredict-0.2/smartpredict.egg-info/requires.txt
--rw-r--r--   0 subashanannair   (501) staff       (20)       13 2024-05-21 08:59:49.000000 smartpredict-0.2/smartpredict.egg-info/top_level.txt
-drwxr-xr-x   0 subashanannair   (501) staff       (20)        0 2024-05-21 08:59:49.476070 smartpredict-0.2/tests/
--rw-r--r--   0 subashanannair   (501) staff       (20)        0 2024-05-21 07:59:33.000000 smartpredict-0.2/tests/test_smartpredict.py
+drwxr-xr-x   0 subashanannair   (501) staff       (20)        0 2024-05-21 09:05:17.532570 smartpredict-0.3/
+-rw-r--r--   0 subashanannair   (501) staff       (20)     4506 2024-05-21 09:05:17.532320 smartpredict-0.3/PKG-INFO
+-rw-r--r--   0 subashanannair   (501) staff       (20)       38 2024-05-21 09:05:17.532631 smartpredict-0.3/setup.cfg
+-rw-r--r--   0 subashanannair   (501) staff       (20)     1993 2024-05-21 09:05:10.000000 smartpredict-0.3/setup.py
+drwxr-xr-x   0 subashanannair   (501) staff       (20)        0 2024-05-21 09:05:17.530982 smartpredict-0.3/smartpredict/
+-rw-r--r--   0 subashanannair   (501) staff       (20)      188 2024-05-21 08:10:34.000000 smartpredict-0.3/smartpredict/__init__.py
+-rw-r--r--   0 subashanannair   (501) staff       (20)     1068 2024-05-21 08:10:56.000000 smartpredict-0.3/smartpredict/base.py
+-rw-r--r--   0 subashanannair   (501) staff       (20)      634 2024-05-21 08:15:33.000000 smartpredict-0.3/smartpredict/ensemble_methods.py
+-rw-r--r--   0 subashanannair   (501) staff       (20)      554 2024-05-21 08:15:17.000000 smartpredict-0.3/smartpredict/explainability.py
+-rw-r--r--   0 subashanannair   (501) staff       (20)      606 2024-05-21 08:15:06.000000 smartpredict-0.3/smartpredict/feature_engineering.py
+-rw-r--r--   0 subashanannair   (501) staff       (20)      800 2024-05-21 08:14:00.000000 smartpredict-0.3/smartpredict/hyperparameter_tuning.py
+-rw-r--r--   0 subashanannair   (501) staff       (20)     2564 2024-05-21 08:34:53.000000 smartpredict-0.3/smartpredict/model_selection.py
+-rw-r--r--   0 subashanannair   (501) staff       (20)     3256 2024-05-21 08:12:55.000000 smartpredict-0.3/smartpredict/supervised.py
+-rw-r--r--   0 subashanannair   (501) staff       (20)        0 2024-05-21 07:58:09.000000 smartpredict-0.3/smartpredict/utils.py
+drwxr-xr-x   0 subashanannair   (501) staff       (20)        0 2024-05-21 09:05:17.532009 smartpredict-0.3/smartpredict.egg-info/
+-rw-r--r--   0 subashanannair   (501) staff       (20)     4506 2024-05-21 09:05:17.000000 smartpredict-0.3/smartpredict.egg-info/PKG-INFO
+-rw-r--r--   0 subashanannair   (501) staff       (20)      479 2024-05-21 09:05:17.000000 smartpredict-0.3/smartpredict.egg-info/SOURCES.txt
+-rw-r--r--   0 subashanannair   (501) staff       (20)        1 2024-05-21 09:05:17.000000 smartpredict-0.3/smartpredict.egg-info/dependency_links.txt
+-rw-r--r--   0 subashanannair   (501) staff       (20)       81 2024-05-21 09:05:17.000000 smartpredict-0.3/smartpredict.egg-info/requires.txt
+-rw-r--r--   0 subashanannair   (501) staff       (20)       13 2024-05-21 09:05:17.000000 smartpredict-0.3/smartpredict.egg-info/top_level.txt
+drwxr-xr-x   0 subashanannair   (501) staff       (20)        0 2024-05-21 09:05:17.531837 smartpredict-0.3/tests/
+-rw-r--r--   0 subashanannair   (501) staff       (20)        0 2024-05-21 07:59:33.000000 smartpredict-0.3/tests/test_smartpredict.py
```

### Comparing `smartpredict-0.2/smartpredict/base.py` & `smartpredict-0.3/smartpredict/base.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.2/smartpredict/ensemble_methods.py` & `smartpredict-0.3/smartpredict/ensemble_methods.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.2/smartpredict/explainability.py` & `smartpredict-0.3/smartpredict/explainability.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.2/smartpredict/feature_engineering.py` & `smartpredict-0.3/smartpredict/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.2/smartpredict/hyperparameter_tuning.py` & `smartpredict-0.3/smartpredict/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.2/smartpredict/model_selection.py` & `smartpredict-0.3/smartpredict/model_selection.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.2/smartpredict/supervised.py` & `smartpredict-0.3/smartpredict/supervised.py`

 * *Files identical despite different names*

