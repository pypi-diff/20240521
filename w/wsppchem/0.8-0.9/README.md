# Comparing `tmp/wsppchem-0.8.tar.gz` & `tmp/wsppchem-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsppchem-0.8.tar", last modified: Fri May 17 19:54:33 2024, max compression
+gzip compressed data, was "wsppchem-0.9.tar", last modified: Tue May 21 09:26:42 2024, max compression
```

## Comparing `wsppchem-0.8.tar` & `wsppchem-0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:54:33.825933 wsppchem-0.8/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 19:54:18.000000 wsppchem-0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3875 2024-05-17 19:54:33.825933 wsppchem-0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3388 2024-05-17 19:54:18.000000 wsppchem-0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 19:54:33.825933 wsppchem-0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 19:54:18.000000 wsppchem-0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:54:33.818932 wsppchem-0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:54:33.820932 wsppchem-0.8/src/wsppchem/
--rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 19:54:18.000000 wsppchem-0.8/src/wsppchem/Template.csv
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 19:54:18.000000 wsppchem-0.8/src/wsppchem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:54:33.824933 wsppchem-0.8/src/wsppchem/model_and_scaler/
--rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 19:54:18.000000 wsppchem-0.8/src/wsppchem/model_and_scaler/LGBM_model.pkl
--rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 19:54:18.000000 wsppchem-0.8/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
--rw-r--r--   0 root         (0) root         (0)     9591 2024-05-17 19:54:18.000000 wsppchem-0.8/src/wsppchem/wspp_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:54:33.820932 wsppchem-0.8/src/wsppchem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3875 2024-05-17 19:54:33.000000 wsppchem-0.8/src/wsppchem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-17 19:54:33.000000 wsppchem-0.8/src/wsppchem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 19:54:33.000000 wsppchem-0.8/src/wsppchem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 19:54:33.000000 wsppchem-0.8/src/wsppchem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 19:54:33.000000 wsppchem-0.8/src/wsppchem.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:54:33.824933 wsppchem-0.8/tests/
--rw-r--r--   0 root         (0) root         (0)     1432 2024-05-17 19:54:18.000000 wsppchem-0.8/tests/test_wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.561012 wsppchem-0.9/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-21 09:26:16.000000 wsppchem-0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3878 2024-05-21 09:26:42.561012 wsppchem-0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-05-21 09:26:16.000000 wsppchem-0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 09:26:42.561012 wsppchem-0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      962 2024-05-21 09:26:16.000000 wsppchem-0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.547011 wsppchem-0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.552011 wsppchem-0.9/src/wsppchem/
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/Template.csv
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.560012 wsppchem-0.9/src/wsppchem/model_and_scaler/
+-rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/model_and_scaler/LGBM_model.pkl
+-rw-r--r--   0 root         (0) root         (0)    10174 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
+-rw-r--r--   0 root         (0) root         (0)     9616 2024-05-21 09:26:16.000000 wsppchem-0.9/src/wsppchem/wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.554011 wsppchem-0.9/src/wsppchem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3878 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 09:26:42.000000 wsppchem-0.9/src/wsppchem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:26:42.561012 wsppchem-0.9/tests/
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-21 09:26:16.000000 wsppchem-0.9/tests/test_wspp_functions.py
```

### Comparing `wsppchem-0.8/LICENSE` & `wsppchem-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wsppchem-0.8/PKG-INFO` & `wsppchem-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.8
+Version: 0.9
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -81,15 +81,15 @@
 ```
 
 ```
 predict_logS_csv(csv_file_path)
 ```
 
 The first function `predict_logS_smiles(*smiles_codes)` can be used to predict the LogS value for one or more SMILES at the same time.
-The second fucntion `predict_logS_csv(csv_file_path)` can be used to predicts LogS values for SMILES codes stored in a CSV file.
+The second fucntion `predict_logS_csv(csv_file_path)` can be used to predicts LogS values for SMILES codes stored in a `.csv` file.
 And if you need any help, you can use the function `wspphelp()` which will give you more precise information on the functions as well as an example of how to use them. 
 
 ## 📗 License 📕
 This project is licensed under the MIT License.
 
 ## 📜 References 📜
 This project is based on the code of this Github Jupyter notebook: https://github.com/gashawmg, as well as data from https://github.com/PatWalters.
```

### Comparing `wsppchem-0.8/README.md` & `wsppchem-0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ```
 
 ```
 predict_logS_csv(csv_file_path)
 ```
 
 The first function `predict_logS_smiles(*smiles_codes)` can be used to predict the LogS value for one or more SMILES at the same time.
-The second fucntion `predict_logS_csv(csv_file_path)` can be used to predicts LogS values for SMILES codes stored in a CSV file.
+The second fucntion `predict_logS_csv(csv_file_path)` can be used to predicts LogS values for SMILES codes stored in a `.csv` file.
 And if you need any help, you can use the function `wspphelp()` which will give you more precise information on the functions as well as an example of how to use them. 
 
 ## 📗 License 📕
 This project is licensed under the MIT License.
 
 ## 📜 References 📜
 This project is based on the code of this Github Jupyter notebook: https://github.com/gashawmg, as well as data from https://github.com/PatWalters.
```

### Comparing `wsppchem-0.8/setup.py` & `wsppchem-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name="wsppchem",
-    version="0.8",
+    version="0.9",
     author="Cossard Lucas and Enzo Venancio",
     author_email="lucas.cossard@epfl.ch and enzo.venancio@epfl.ch",
     description="Water Solubility Prediction Project",
     long_description=open('README.md').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url="https://github.com/Nohalyan/WSPP_Projectppchem",
     packages=find_packages(where='src'),
```

### Comparing `wsppchem-0.8/src/wsppchem/Template.csv` & `wsppchem-0.9/src/wsppchem/Template.csv`

 * *Files identical despite different names*

### Comparing `wsppchem-0.8/src/wsppchem/model_and_scaler/LGBM_model.pkl` & `wsppchem-0.9/src/wsppchem/model_and_scaler/LGBM_model.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.8/src/wsppchem/model_and_scaler/LGBM_scaler.pkl` & `wsppchem-0.9/src/wsppchem/model_and_scaler/LGBM_scaler.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.8/src/wsppchem/wspp_functions.py` & `wsppchem-0.9/src/wsppchem/wspp_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,25 +154,25 @@
     """
     Predicts LogS values for a given SMILES code using a trained model.
 
     Parameters:
     smiles (str): A valid SMILES code for a chemical compound.
 
     Returns:
-    Predicted LogS value for the input SMILES code.
+    Predicted LogS value for the input SMILES code, rounded to 0.01.
     """
     
     canonical_smiles = canonical_SMILES([smiles])
     descriptors, _ = RDkit_descriptors(canonical_smiles)
 
     model, scaler = load_model_and_scalers()
     scaled_descriptors = scaler.transform(descriptors)
 
-    logS_prediction = model.predict(scaled_descriptors)
-    return logS_prediction[0]
+    rounded_logS_prediction = round(logS_prediction[0], 2)
+    return rounded_logS_prediction
 
 #==========================================================================================================================================
 
 # Prediction functions
 
 def predict_logS_smiles(*smiles_codes):
     """
```

### Comparing `wsppchem-0.8/src/wsppchem.egg-info/PKG-INFO` & `wsppchem-0.9/src/wsppchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.8
+Version: 0.9
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -81,15 +81,15 @@
 ```
 
 ```
 predict_logS_csv(csv_file_path)
 ```
 
 The first function `predict_logS_smiles(*smiles_codes)` can be used to predict the LogS value for one or more SMILES at the same time.
-The second fucntion `predict_logS_csv(csv_file_path)` can be used to predicts LogS values for SMILES codes stored in a CSV file.
+The second fucntion `predict_logS_csv(csv_file_path)` can be used to predicts LogS values for SMILES codes stored in a `.csv` file.
 And if you need any help, you can use the function `wspphelp()` which will give you more precise information on the functions as well as an example of how to use them. 
 
 ## 📗 License 📕
 This project is licensed under the MIT License.
 
 ## 📜 References 📜
 This project is based on the code of this Github Jupyter notebook: https://github.com/gashawmg, as well as data from https://github.com/PatWalters.
```

### Comparing `wsppchem-0.8/tests/test_wspp_functions.py` & `wsppchem-0.9/tests/test_wspp_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     predict_LogS,
     predict_logS_smiles,
     predict_logS_csv,
 )
 
 def test_canonical_SMILES():
     smiles = ["CC(=O)NC1=CC=C(C=C1)O", "CN1C=NC2=C1C(=O)N(C(=O)N2C)C"]
-    expected = ["CC(=O)NC1=CC=C(C=C1)O", "CN1C=NC2=C1C(=O)N(C(=O)N2C)C"]
+    expected = ["CC(=O)Nc1ccc(O)cc1", "Cn1c(=O)c2c(ncn2C)n(C)c1=O"]
     assert canonical_SMILES(smiles) == expected
 
 def test_RDkit_descriptors():
     smiles = ["CC(=O)NC1=CC=C(C=C1)O", "CN1C=NC2=C1C(=O)N(C(=O)N2C)C"]
     descriptors, desc_names = RDkit_descriptors(smiles)
     assert len(descriptors) == 2
     assert len(desc_names) > 0
```

