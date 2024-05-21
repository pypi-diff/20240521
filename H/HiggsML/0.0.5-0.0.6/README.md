# Comparing `tmp/higgsml-0.0.5.tar.gz` & `tmp/higgsml-0.0.6.tar.gz`

## Comparing `higgsml-0.0.5.tar` & `higgsml-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.5/HiggsML/__init__.py
--rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 higgsml-0.0.5/HiggsML/datasets.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 higgsml-0.0.5/HiggsML/ingestion.py
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 higgsml-0.0.5/HiggsML/score.py
--rw-r--r--   0        0        0    20062 2020-02-02 00:00:00.000000 higgsml-0.0.5/HiggsML/systematics.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 higgsml-0.0.5/HiggsML/visualization.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.5/LICENSE
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 higgsml-0.0.5/README.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 higgsml-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 higgsml-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/__init__.py
+-rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/datasets.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/ingestion.py
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/score.py
+-rw-r--r--   0        0        0    20064 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/systematics.py
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/visualization.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.6/LICENSE
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 higgsml-0.0.6/README.md
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 higgsml-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 higgsml-0.0.6/PKG-INFO
```

### Comparing `higgsml-0.0.5/HiggsML/datasets.py` & `higgsml-0.0.6/HiggsML/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from frozendict import frozendict
 import numpy as np
 import pandas as pd
 import json
 import os
 import subprocess
 import wget
 
@@ -54,33 +53,31 @@
             train_weights = np.array(f.read().splitlines(), dtype=float)
 
         # read train process flags
         with open(train_detailed_labels_file) as f:
             train_detailed_labels = f.read().splitlines()
 
         if self.data_format == "parquet":
-            self.__train_set = frozendict(
-                {
+            self.__train_set = {
                     "data": pd.read_parquet(train_data_file, engine="pyarrow"),
                     "labels": train_labels,
                     "settings": train_settings,
                     "weights": train_weights,
                     "detailed_labels": train_detailed_labels,
                 }
-            )
+            
         else:
-            self.__train_set = frozendict(
-                {
+            self.__train_set = {
                     "data": pd.read_csv(train_data_file),
                     "labels": train_labels,
                     "settings": train_settings,
                     "weights": train_weights,
                     "detailed_labels": train_detailed_labels,
                 }
-            )
+            
 
         del train_labels, train_settings, train_weights, train_detailed_labels
 
         print(self.__train_set["data"].info(verbose=False, memory_usage="deep"))
 
         test_settings_file = os.path.join(
             self.input_dir, "test", "settings", "data.json"
@@ -171,15 +168,15 @@
     file_read_loc = os.path.join(current_path, "public_data")
     if not os.path.isdir(file_read_loc):
         os.mkdir(file_read_loc)
 
     file = "public_data.zip"
     if file not in os.listdir(file_read_loc):
         wget.download(
-            "https://www.codabench.org/datasets/download/c3b5c664-2f7e-4e81-8975-7926dae44703/",
+            "https://www.codabench.org/datasets/download/8fa63d64-8110-4ee5-9722-9d5ec8e3c3d8/",
             out=os.path.join(file_read_loc, "public_data.zip"),
         )
 
     if "input_data" not in os.listdir(file_read_loc):
         subprocess.run(
             ["unzip", os.path.join(file_read_loc, file), "-d", file_read_loc]
         )
```

### Comparing `higgsml-0.0.5/HiggsML/ingestion.py` & `higgsml-0.0.6/HiggsML/ingestion.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,46 +126,41 @@
                 bkg_scale=bkg_scale,
                 seed=42,
             )
 
             predicted_dict = self.model.predict(test_set)
             predicted_dict["test_set_index"] = test_set_index
 
-            print(
-                f"[*] - mu_hat: {predicted_dict['mu_hat']} - del_mu_tot: {predicted_dict['del_mu_tot']} - del_mu_stat: {predicted_dict['del_mu_stat']} - del_mu_sys: {predicted_dict['del_mu_sys']}"
-            )
 
             if set_index not in self.results_dict:
                 self.results_dict[set_index] = []
             self.results_dict[set_index].append(predicted_dict)
 
     def compute_result(self):
         print("[*] Saving ingestion result")
 
-        # loop over sets
         for key in self.results_dict.keys():
             set_result = self.results_dict[key]
             set_result.sort(key=lambda x: x["test_set_index"])
-            mu_hats, del_mu_tots, del_mu_stats, del_mu_syss = [], [], [], []
+            mu_hats, delta_mu_hats, p16, p84 = [], [], [], []
             for test_set_dict in set_result:
                 mu_hats.append(test_set_dict["mu_hat"])
-                del_mu_tots.append(test_set_dict["del_mu_tot"])
-                del_mu_stats.append(test_set_dict["del_mu_stat"])
-                del_mu_syss.append(test_set_dict["del_mu_sys"])
-
-
+                delta_mu_hats.append(test_set_dict["delta_mu_hat"])
+                p16.append(test_set_dict["p16"])
+                p84.append(test_set_dict["p84"])
 
             ingestion_result_dict = {
                 "mu_hats": mu_hats,
-                "del_mu_stats": del_mu_stats,
-                "del_mu_syss": del_mu_syss,
-                "del_mu_tots": del_mu_tots,
+                "delta_mu_hats": delta_mu_hats,
+                "p16": p16,
+                "p84": p84,
             }
             self.results_dict[key] = ingestion_result_dict
 
+
     def save_result(self, output_dir=None):
         for key in self.results_dict.keys():
             result_file = os.path.join(output_dir, "result_" + str(key) + ".json")
             with open(result_file, "w") as f:
                 f.write(json.dumps(self.results_dict[key], indent=4))
```

### Comparing `higgsml-0.0.5/HiggsML/systematics.py` & `higgsml-0.0.6/HiggsML/systematics.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,19 +569,19 @@
             data_syst_set[key] = data_syst.pop(key)
     data_syst_set["data"] = data_syst
 
     return data_syst_set
 
 
 LHC_NUMBERS = {
-    "ztautau": 7306660,
-    "wjets": 3812700,
-    "diboson": 2398564,
-    "ttbar": 616017,
-    "htautau": 285
+    "ztautau": 6177943,
+    "wjets": 2704182,
+    "diboson": 2192528,
+    "ttbar": 617402,
+    "htautau": 14139
 }
 
 def get_bootstraped_dataset(
     test_set,
     mu=1.0,
     seed=31415,
     w_scale=1.0,
```

### Comparing `higgsml-0.0.5/HiggsML/visualization.py` & `higgsml-0.0.6/HiggsML/visualization.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.5/.gitignore` & `higgsml-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.5/LICENSE` & `higgsml-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.5/pyproject.toml` & `higgsml-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HiggsML"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Ragansu Chakkappai", email="ragansu.chakkappai@universite-paris-saclay.fr"},
   { name="David Rousseau", email="david.rousseau@uijclab.in2p3.fr" },
   { name="V. Estrade", email="v.estrade@centralesupelec.fr" },
   { name="Ihsan Ullah", email="ihsan.ullah@universite-paris-saclay.fr"}
 ]
 description = "A Black Swan test package"
@@ -17,32 +17,30 @@
 ]
 dependencies = [
     "numpy",
     "pandas",
     "scikit-learn",
     "matplotlib",
     "seaborn",
-    "frozendict",
     "pyarrow",
     "wget",
     "setuptools"
 ]
 install_requires=["numpy>=1.26.4",
                   "sklearn>=1.4.2",
                   "pandas>=2.2.2",
                   "matplotlib>=3.8.0",
                   "seaborn>=0.13.1",
-                  "frozendict>=2.4.4",
                   "pyarrow>=15.0.0",
                   "wget>=3.2",
                   "setuptools>=58.2.0"
                   ]
 
 
 
 [build-system]
-requires = ["hatchling", "numpy", "pandas", "scikit-learn", "matplotlib", "seaborn", "frozendict", "pyarrow","wget", "setuptools"]
+requires = ["hatchling", "numpy", "pandas", "scikit-learn", "matplotlib", "seaborn", "pyarrow","wget", "setuptools"]
 build-backend = "hatchling.build"
 
 [project.urls]
 Homepage = "https://github.com/blackSwanCS/black_swan_pkg"
 Issues = "https://github.com/blackSwanCS/black_swan_pkg/issues"
```

