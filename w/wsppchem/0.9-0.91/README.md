# Comparing `tmp/wsppchem-0.9.tar.gz` & `tmp/wsppchem-0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsppchem-0.9.tar", last modified: Tue May 21 09:26:42 2024, max compression
+gzip compressed data, was "wsppchem-0.91.tar", last modified: Tue May 21 09:37:34 2024, max compression
```

## Comparing `wsppchem-0.9.tar` & `wsppchem-0.91.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.561012 wsppchem-0.9/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-21 09:26:16.000000 wsppchem-0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3878 2024-05-21 09:26:42.561012 wsppchem-0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3391 2024-05-21 09:26:16.000000 wsppchem-0.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 09:26:42.561012 wsppchem-0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      962 2024-05-21 09:26:16.000000 wsppchem-0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.547011 wsppchem-0.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.552011 wsppchem-0.9/src/wsppchem/
--rw-r--r--   0 root         (0) root         (0)     3701 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/Template.csv
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.560012 wsppchem-0.9/src/wsppchem/model_and_scaler/
--rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/model_and_scaler/LGBM_model.pkl
--rw-r--r--   0 root         (0) root         (0)    10174 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
--rw-r--r--   0 root         (0) root         (0)     9616 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/wspp_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.554011 wsppchem-0.9/src/wsppchem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3878 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.561012 wsppchem-0.9/tests/
--rw-r--r--   0 root         (0) root         (0)     1427 2024-05-21 09:26:16.000000 wsppchem-0.9/tests/test_wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:37:34.184865 wsppchem-0.91/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-21 09:37:02.000000 wsppchem-0.91/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3879 2024-05-21 09:37:34.184865 wsppchem-0.91/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-05-21 09:37:02.000000 wsppchem-0.91/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 09:37:34.184865 wsppchem-0.91/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      963 2024-05-21 09:37:02.000000 wsppchem-0.91/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:37:34.176864 wsppchem-0.91/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:37:34.177864 wsppchem-0.91/src/wsppchem/
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-21 09:37:02.000000 wsppchem-0.91/src/wsppchem/Template.csv
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-21 09:37:02.000000 wsppchem-0.91/src/wsppchem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:37:34.183865 wsppchem-0.91/src/wsppchem/model_and_scaler/
+-rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-21 09:37:02.000000 wsppchem-0.91/src/wsppchem/model_and_scaler/LGBM_model.pkl
+-rw-r--r--   0 root         (0) root         (0)    10174 2024-05-21 09:37:02.000000 wsppchem-0.91/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
+-rw-r--r--   0 root         (0) root         (0)     9676 2024-05-21 09:37:02.000000 wsppchem-0.91/src/wsppchem/wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:37:34.179865 wsppchem-0.91/src/wsppchem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3879 2024-05-21 09:37:34.000000 wsppchem-0.91/src/wsppchem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-21 09:37:34.000000 wsppchem-0.91/src/wsppchem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:37:34.000000 wsppchem-0.91/src/wsppchem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-21 09:37:34.000000 wsppchem-0.91/src/wsppchem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 09:37:34.000000 wsppchem-0.91/src/wsppchem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:37:34.184865 wsppchem-0.91/tests/
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-21 09:37:02.000000 wsppchem-0.91/tests/test_wspp_functions.py
```

### Comparing `wsppchem-0.9/LICENSE` & `wsppchem-0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `wsppchem-0.9/PKG-INFO` & `wsppchem-0.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.9
+Version: 0.91
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsppchem-0.9/README.md` & `wsppchem-0.91/README.md`

 * *Files identical despite different names*

### Comparing `wsppchem-0.9/setup.py` & `wsppchem-0.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name="wsppchem",
-    version="0.9",
+    version="0.91",
     author="Cossard Lucas and Enzo Venancio",
     author_email="lucas.cossard@epfl.ch and enzo.venancio@epfl.ch",
     description="Water Solubility Prediction Project",
     long_description=open('README.md').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url="https://github.com/Nohalyan/WSPP_Projectppchem",
     packages=find_packages(where='src'),
```

### Comparing `wsppchem-0.9/src/wsppchem/Template.csv` & `wsppchem-0.91/src/wsppchem/Template.csv`

 * *Files identical despite different names*

### Comparing `wsppchem-0.9/src/wsppchem/model_and_scaler/LGBM_model.pkl` & `wsppchem-0.91/src/wsppchem/model_and_scaler/LGBM_model.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.9/src/wsppchem/model_and_scaler/LGBM_scaler.pkl` & `wsppchem-0.91/src/wsppchem/model_and_scaler/LGBM_scaler.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.9/src/wsppchem/wspp_functions.py` & `wsppchem-0.91/src/wsppchem/wspp_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,16 @@
     """
     
     canonical_smiles = canonical_SMILES([smiles])
     descriptors, _ = RDkit_descriptors(canonical_smiles)
 
     model, scaler = load_model_and_scalers()
     scaled_descriptors = scaler.transform(descriptors)
-
+    
+    logS_prediction = model.predict(scaled_descriptors)
     rounded_logS_prediction = round(logS_prediction[0], 2)
     return rounded_logS_prediction
 
 #==========================================================================================================================================
 
 # Prediction functions
```

### Comparing `wsppchem-0.9/src/wsppchem.egg-info/PKG-INFO` & `wsppchem-0.91/src/wsppchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.9
+Version: 0.91
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsppchem-0.9/tests/test_wspp_functions.py` & `wsppchem-0.91/tests/test_wspp_functions.py`

 * *Files identical despite different names*

