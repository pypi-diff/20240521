# Comparing `tmp/neuroharmonize-2.4.4.tar.gz` & `tmp/neuroharmonize-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroharmonize-2.4.4.tar", last modified: Thu May 16 20:30:04 2024, max compression
+gzip compressed data, was "neuroharmonize-2.4.5.tar", last modified: Tue May 21 12:40:09 2024, max compression
```

## Comparing `neuroharmonize-2.4.4.tar` & `neuroharmonize-2.4.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-16 20:30:04.407502 neuroharmonize-2.4.4/
--rw-r--r--   0 pomponior   (501) staff       (20)     1069 2024-02-01 14:00:43.000000 neuroharmonize-2.4.4/LICENSE
--rw-r--r--   0 pomponior   (501) staff       (20)       18 2024-04-23 17:14:29.000000 neuroharmonize-2.4.4/MANIFEST.in
--rw-r--r--   0 pomponior   (501) staff       (20)    11042 2024-05-16 20:30:04.407272 neuroharmonize-2.4.4/PKG-INFO
--rw-r--r--   0 pomponior   (501) staff       (20)    10484 2024-05-16 20:29:41.000000 neuroharmonize-2.4.4/README.md
--rw-r--r--   0 pomponior   (501) staff       (20)      104 2024-02-01 14:00:43.000000 neuroharmonize-2.4.4/pyproject.toml
--rw-r--r--   0 pomponior   (501) staff       (20)      683 2024-05-16 20:30:04.407810 neuroharmonize-2.4.4/setup.cfg
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-16 20:30:04.404953 neuroharmonize-2.4.4/src/
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-16 20:30:04.406381 neuroharmonize-2.4.4/src/neuroHarmonize/
--rw-r--r--   0 pomponior   (501) staff       (20)      219 2024-05-16 20:29:19.000000 neuroharmonize-2.4.4/src/neuroHarmonize/__init__.py
--rwxr-xr-x   0 pomponior   (501) staff       (20)     9060 2024-05-16 20:29:19.000000 neuroharmonize-2.4.4/src/neuroHarmonize/harmonizationApply.py
--rwxr-xr-x   0 pomponior   (501) staff       (20)    18873 2024-05-16 20:29:19.000000 neuroharmonize-2.4.4/src/neuroHarmonize/harmonizationLearn.py
--rw-r--r--   0 pomponior   (501) staff       (20)     6701 2024-05-16 20:29:19.000000 neuroharmonize-2.4.4/src/neuroHarmonize/harmonizationNIFTI.py
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-16 20:30:04.407090 neuroharmonize-2.4.4/src/neuroHarmonize.egg-info/
--rw-r--r--   0 pomponior   (501) staff       (20)    11042 2024-05-16 20:30:04.000000 neuroharmonize-2.4.4/src/neuroHarmonize.egg-info/PKG-INFO
--rw-r--r--   0 pomponior   (501) staff       (20)      376 2024-05-16 20:30:04.000000 neuroharmonize-2.4.4/src/neuroHarmonize.egg-info/SOURCES.txt
--rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-05-16 20:30:04.000000 neuroharmonize-2.4.4/src/neuroHarmonize.egg-info/dependency_links.txt
--rw-r--r--   0 pomponior   (501) staff       (20)       15 2024-05-16 20:30:04.000000 neuroharmonize-2.4.4/src/neuroHarmonize.egg-info/top_level.txt
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-21 12:40:09.417959 neuroharmonize-2.4.5/
+-rw-r--r--   0 pomponior   (501) staff       (20)     1069 2024-02-01 14:00:43.000000 neuroharmonize-2.4.5/LICENSE
+-rw-r--r--   0 pomponior   (501) staff       (20)       18 2024-04-23 17:14:29.000000 neuroharmonize-2.4.5/MANIFEST.in
+-rw-r--r--   0 pomponior   (501) staff       (20)    11045 2024-05-21 12:40:09.417862 neuroharmonize-2.4.5/PKG-INFO
+-rw-r--r--   0 pomponior   (501) staff       (20)    10487 2024-05-17 16:57:02.000000 neuroharmonize-2.4.5/README.md
+-rw-r--r--   0 pomponior   (501) staff       (20)      104 2024-02-01 14:00:43.000000 neuroharmonize-2.4.5/pyproject.toml
+-rw-r--r--   0 pomponior   (501) staff       (20)      683 2024-05-21 12:40:09.418209 neuroharmonize-2.4.5/setup.cfg
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-21 12:40:09.413877 neuroharmonize-2.4.5/src/
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-21 12:40:09.416981 neuroharmonize-2.4.5/src/neuroHarmonize/
+-rw-r--r--   0 pomponior   (501) staff       (20)      219 2024-05-21 12:39:26.000000 neuroharmonize-2.4.5/src/neuroHarmonize/__init__.py
+-rwxr-xr-x   0 pomponior   (501) staff       (20)     9060 2024-05-21 12:39:26.000000 neuroharmonize-2.4.5/src/neuroHarmonize/harmonizationApply.py
+-rwxr-xr-x   0 pomponior   (501) staff       (20)    18873 2024-05-21 12:39:26.000000 neuroharmonize-2.4.5/src/neuroHarmonize/harmonizationLearn.py
+-rw-r--r--   0 pomponior   (501) staff       (20)     6701 2024-05-21 12:39:26.000000 neuroharmonize-2.4.5/src/neuroHarmonize/harmonizationNIFTI.py
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-21 12:40:09.417685 neuroharmonize-2.4.5/src/neuroHarmonize.egg-info/
+-rw-r--r--   0 pomponior   (501) staff       (20)    11045 2024-05-21 12:40:09.000000 neuroharmonize-2.4.5/src/neuroHarmonize.egg-info/PKG-INFO
+-rw-r--r--   0 pomponior   (501) staff       (20)      376 2024-05-21 12:40:09.000000 neuroharmonize-2.4.5/src/neuroHarmonize.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-05-21 12:40:09.000000 neuroharmonize-2.4.5/src/neuroHarmonize.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponior   (501) staff       (20)       15 2024-05-21 12:40:09.000000 neuroharmonize-2.4.5/src/neuroHarmonize.egg-info/top_level.txt
```

### Comparing `neuroharmonize-2.4.4/LICENSE` & `neuroharmonize-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroharmonize-2.4.4/PKG-INFO` & `neuroharmonize-2.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroHarmonize
-Version: 2.4.4
+Version: 2.4.5
 Summary: Harmonization tools for multi-center neuroimaging studies.
 Home-page: https://github.com/rpomponio/neuroHarmonize
 Author: Raymond Pomponio
 Author-email: raymond.pomponio@outlook.com
 Project-URL: Bug Tracker, https://github.com/rpomponio/neuroHarmonize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 3. Specify covariates with generic nonlinear effects. Implemented using
    Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest development version: `2.4.4` (May 2024)
+Latest development version: `2.4.5` (in dev mode)
 
 Requirements:
 
 * `git >= 2.17.2`
 * `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
```

### Comparing `neuroharmonize-2.4.4/README.md` & `neuroharmonize-2.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 3. Specify covariates with generic nonlinear effects. Implemented using
    Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest development version: `2.4.4` (May 2024)
+Latest development version: `2.4.5` (in dev mode)
 
 Requirements:
 
 * `git >= 2.17.2`
 * `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
```

### Comparing `neuroharmonize-2.4.4/setup.cfg` & `neuroharmonize-2.4.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neuroHarmonize
-version = 2.4.4
+version = 2.4.5
 author = Raymond Pomponio
 author_email = raymond.pomponio@outlook.com
 description = Harmonization tools for multi-center neuroimaging studies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rpomponio/neuroHarmonize
 project_urls =
```

### Comparing `neuroharmonize-2.4.4/src/neuroHarmonize/harmonizationApply.py` & `neuroharmonize-2.4.5/src/neuroHarmonize/harmonizationApply.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     """
     
     n_batch = info_dict['n_batch']
     n_sample = info_dict['n_sample']
     sample_per_batch = info_dict['sample_per_batch']
 
     B_hat = model['B_hat']
-    stand_mean = model['stand_mean']
+    stand_mean = model['stand_mean'][:, [0]]
     var_pooled = model['var_pooled']
     
     # new code in neuroCombat to compute model mean
     if design is not None:
         tmp = copy.deepcopy(design)
         tmp[:,range(0,n_batch)] = 0
         mod_mean = np.transpose(np.dot(tmp, B_hat))
@@ -191,24 +191,24 @@
     n_sample = 1
     sample_per_batch = 1
     D = design_i
     n_batch = len(batch_labels)
     j = batch_level_i[0]
 
     B_hat = model['B_hat']
-    stand_mean = model['stand_mean']
+    stand_mean = model['stand_mean'][:, [0]]
     var_pooled = model['var_pooled']
     
     # new code in neuroCombat to compute model mean
     if design_i is not None:
         tmp = copy.deepcopy(design_i)
         tmp[:,range(0,n_batch)] = 0
         mod_mean = np.transpose(np.dot(tmp, B_hat))
     
-    s_data = (X- stand_mean[:, [0]] - mod_mean) / np.dot(np.sqrt(var_pooled), np.ones((1, n_sample)))
+    s_data = (X- stand_mean - mod_mean) / np.dot(np.sqrt(var_pooled), np.ones((1, n_sample)))
 
     if sum(isTrainSite)==0:
         bayesdata = np.full(s_data.shape,np.nan)
     else:
         # adjust_data_final
         batch_design = D[:,:n_batch]
 
@@ -220,15 +220,15 @@
         dsq = dsq.reshape((len(dsq), 1))
         denom = np.dot(dsq, np.ones((1, sample_per_batch)))
         numer = np.array(bayesdata - np.dot(batch_design, gamma_star).T)
 
         bayesdata = numer / denom
 
         vpsq = np.sqrt(var_pooled).reshape((len(var_pooled), 1))
-        bayesdata = bayesdata * np.dot(vpsq, np.ones((1, n_sample))) + stand_mean[:, [0]]
+        bayesdata = bayesdata * np.dot(vpsq, np.ones((1, n_sample))) + stand_mean
     
 
     # return either bayesdata or both
     if return_stand_mean:
         return bayesdata.T, stand_mean.T
     else:
         return bayesdata.T
```

### Comparing `neuroharmonize-2.4.4/src/neuroHarmonize/harmonizationLearn.py` & `neuroharmonize-2.4.5/src/neuroHarmonize/harmonizationLearn.py`

 * *Files identical despite different names*

### Comparing `neuroharmonize-2.4.4/src/neuroHarmonize/harmonizationNIFTI.py` & `neuroharmonize-2.4.5/src/neuroHarmonize/harmonizationNIFTI.py`

 * *Files identical despite different names*

### Comparing `neuroharmonize-2.4.4/src/neuroHarmonize.egg-info/PKG-INFO` & `neuroharmonize-2.4.5/src/neuroHarmonize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroHarmonize
-Version: 2.4.4
+Version: 2.4.5
 Summary: Harmonization tools for multi-center neuroimaging studies.
 Home-page: https://github.com/rpomponio/neuroHarmonize
 Author: Raymond Pomponio
 Author-email: raymond.pomponio@outlook.com
 Project-URL: Bug Tracker, https://github.com/rpomponio/neuroHarmonize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 3. Specify covariates with generic nonlinear effects. Implemented using
    Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest development version: `2.4.4` (May 2024)
+Latest development version: `2.4.5` (in dev mode)
 
 Requirements:
 
 * `git >= 2.17.2`
 * `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
```

