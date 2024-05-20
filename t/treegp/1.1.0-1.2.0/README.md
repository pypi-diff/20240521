# Comparing `tmp/treegp-1.1.0.tar.gz` & `tmp/treegp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treegp-1.1.0.tar", last modified: Wed May 15 20:12:11 2024, max compression
+gzip compressed data, was "treegp-1.2.0.tar", last modified: Mon May 20 22:52:08 2024, max compression
```

## Comparing `treegp-1.1.0.tar` & `treegp-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 leget      (501) staff       (20)        0 2024-05-15 20:12:11.378097 treegp-1.1.0/
--rw-r--r--   0 leget      (501) staff       (20)     1528 2024-05-15 20:10:01.000000 treegp-1.1.0/LICENCE
--rw-r--r--   0 leget      (501) staff       (20)       29 2024-05-15 20:10:01.000000 treegp-1.1.0/MANIFEST.in
--rw-r--r--   0 leget      (501) staff       (20)     2769 2024-05-15 20:12:11.377891 treegp-1.1.0/PKG-INFO
--rw-r--r--   0 leget      (501) staff       (20)     2259 2024-05-15 20:10:01.000000 treegp-1.1.0/README.rst
--rw-r--r--   0 leget      (501) staff       (20)       38 2024-05-15 20:12:11.378136 treegp-1.1.0/setup.cfg
--rw-r--r--   0 leget      (501) staff       (20)     1961 2024-05-15 20:10:01.000000 treegp-1.1.0/setup.py
-drwxr-xr-x   0 leget      (501) staff       (20)        0 2024-05-15 20:12:11.376001 treegp-1.1.0/tests/
--rw-r--r--   0 leget      (501) staff       (20)     8052 2024-05-15 20:10:01.000000 treegp-1.1.0/tests/test_gp_interp.py
--rw-r--r--   0 leget      (501) staff       (20)     7419 2024-05-15 20:10:01.000000 treegp-1.1.0/tests/test_hyp_search.py
--rw-r--r--   0 leget      (501) staff       (20)     8075 2024-05-15 20:10:01.000000 treegp-1.1.0/tests/test_kernels.py
--rw-r--r--   0 leget      (501) staff       (20)     4290 2024-05-15 20:10:01.000000 treegp-1.1.0/tests/test_meanify.py
-drwxr-xr-x   0 leget      (501) staff       (20)        0 2024-05-15 20:12:11.377058 treegp-1.1.0/treegp/
--rw-r--r--   0 leget      (501) staff       (20)      771 2024-05-15 20:10:01.000000 treegp-1.1.0/treegp/__init__.py
--rw-r--r--   0 leget      (501) staff       (20)       81 2024-05-15 20:11:13.000000 treegp-1.1.0/treegp/_version.py
--rw-r--r--   0 leget      (501) staff       (20)    14064 2024-05-15 20:10:01.000000 treegp-1.1.0/treegp/gp_interp.py
--rw-r--r--   0 leget      (501) staff       (20)    17933 2024-05-15 20:10:01.000000 treegp-1.1.0/treegp/kernels.py
--rw-r--r--   0 leget      (501) staff       (20)     2005 2024-05-15 20:10:01.000000 treegp-1.1.0/treegp/log_likelihood.py
--rw-r--r--   0 leget      (501) staff       (20)     5580 2024-05-15 20:10:01.000000 treegp-1.1.0/treegp/meanify.py
--rw-r--r--   0 leget      (501) staff       (20)    16567 2024-05-15 20:10:01.000000 treegp-1.1.0/treegp/two_pcf.py
--rw-r--r--   0 leget      (501) staff       (20)     3565 2024-05-15 20:10:01.000000 treegp-1.1.0/treegp/utils.py
-drwxr-xr-x   0 leget      (501) staff       (20)        0 2024-05-15 20:12:11.377658 treegp-1.1.0/treegp.egg-info/
--rw-r--r--   0 leget      (501) staff       (20)     2769 2024-05-15 20:12:11.000000 treegp-1.1.0/treegp.egg-info/PKG-INFO
--rw-r--r--   0 leget      (501) staff       (20)      434 2024-05-15 20:12:11.000000 treegp-1.1.0/treegp.egg-info/SOURCES.txt
--rw-r--r--   0 leget      (501) staff       (20)        1 2024-05-15 20:12:11.000000 treegp-1.1.0/treegp.egg-info/dependency_links.txt
--rw-r--r--   0 leget      (501) staff       (20)       70 2024-05-15 20:12:11.000000 treegp-1.1.0/treegp.egg-info/requires.txt
--rw-r--r--   0 leget      (501) staff       (20)        7 2024-05-15 20:12:11.000000 treegp-1.1.0/treegp.egg-info/top_level.txt
+drwxr-xr-x   0 leget      (501) staff       (20)        0 2024-05-20 22:52:08.473055 treegp-1.2.0/
+-rw-r--r--   0 leget      (501) staff       (20)     1528 2024-05-15 20:10:01.000000 treegp-1.2.0/LICENCE
+-rw-r--r--   0 leget      (501) staff       (20)       29 2024-05-15 20:10:01.000000 treegp-1.2.0/MANIFEST.in
+-rw-r--r--   0 leget      (501) staff       (20)     2769 2024-05-20 22:52:08.472856 treegp-1.2.0/PKG-INFO
+-rw-r--r--   0 leget      (501) staff       (20)     2259 2024-05-15 20:10:01.000000 treegp-1.2.0/README.rst
+-rw-r--r--   0 leget      (501) staff       (20)       38 2024-05-20 22:52:08.473095 treegp-1.2.0/setup.cfg
+-rw-r--r--   0 leget      (501) staff       (20)     1961 2024-05-15 20:10:01.000000 treegp-1.2.0/setup.py
+drwxr-xr-x   0 leget      (501) staff       (20)        0 2024-05-20 22:52:08.471070 treegp-1.2.0/tests/
+-rw-r--r--   0 leget      (501) staff       (20)     8052 2024-05-20 22:24:15.000000 treegp-1.2.0/tests/test_gp_interp.py
+-rw-r--r--   0 leget      (501) staff       (20)     7419 2024-05-15 20:10:01.000000 treegp-1.2.0/tests/test_hyp_search.py
+-rw-r--r--   0 leget      (501) staff       (20)     8075 2024-05-15 20:10:01.000000 treegp-1.2.0/tests/test_kernels.py
+-rw-r--r--   0 leget      (501) staff       (20)     4290 2024-05-15 20:10:01.000000 treegp-1.2.0/tests/test_meanify.py
+drwxr-xr-x   0 leget      (501) staff       (20)        0 2024-05-20 22:52:08.472095 treegp-1.2.0/treegp/
+-rw-r--r--   0 leget      (501) staff       (20)      771 2024-05-15 20:10:01.000000 treegp-1.2.0/treegp/__init__.py
+-rw-r--r--   0 leget      (501) staff       (20)       81 2024-05-20 22:50:46.000000 treegp-1.2.0/treegp/_version.py
+-rw-r--r--   0 leget      (501) staff       (20)    14425 2024-05-20 22:50:05.000000 treegp-1.2.0/treegp/gp_interp.py
+-rw-r--r--   0 leget      (501) staff       (20)    17933 2024-05-15 20:10:01.000000 treegp-1.2.0/treegp/kernels.py
+-rw-r--r--   0 leget      (501) staff       (20)     2005 2024-05-15 20:10:01.000000 treegp-1.2.0/treegp/log_likelihood.py
+-rw-r--r--   0 leget      (501) staff       (20)     5580 2024-05-15 20:10:01.000000 treegp-1.2.0/treegp/meanify.py
+-rw-r--r--   0 leget      (501) staff       (20)    16567 2024-05-18 01:00:05.000000 treegp-1.2.0/treegp/two_pcf.py
+-rw-r--r--   0 leget      (501) staff       (20)     3565 2024-05-15 20:10:01.000000 treegp-1.2.0/treegp/utils.py
+drwxr-xr-x   0 leget      (501) staff       (20)        0 2024-05-20 22:52:08.472643 treegp-1.2.0/treegp.egg-info/
+-rw-r--r--   0 leget      (501) staff       (20)     2769 2024-05-20 22:52:08.000000 treegp-1.2.0/treegp.egg-info/PKG-INFO
+-rw-r--r--   0 leget      (501) staff       (20)      434 2024-05-20 22:52:08.000000 treegp-1.2.0/treegp.egg-info/SOURCES.txt
+-rw-r--r--   0 leget      (501) staff       (20)        1 2024-05-20 22:52:08.000000 treegp-1.2.0/treegp.egg-info/dependency_links.txt
+-rw-r--r--   0 leget      (501) staff       (20)       70 2024-05-20 22:52:08.000000 treegp-1.2.0/treegp.egg-info/requires.txt
+-rw-r--r--   0 leget      (501) staff       (20)        7 2024-05-20 22:52:08.000000 treegp-1.2.0/treegp.egg-info/top_level.txt
```

### Comparing `treegp-1.1.0/LICENCE` & `treegp-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/PKG-INFO` & `treegp-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: treegp
-Version: 1.1.0
+Version: 1.2.0
 Summary: treegp
 Home-page: https://github.com/PFLeget/treegp
-Download-URL: https://github.com/PFLeget/treegp/releases/tag/v1.1.0.zip
+Download-URL: https://github.com/PFLeget/treegp/releases/tag/v1.2.0.zip
 Author: PFLeget
 License: BSD License
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
 License-File: LICENCE
 Requires-Dist: numpy
 Requires-Dist: scipy
```

### Comparing `treegp-1.1.0/README.rst` & `treegp-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/setup.py` & `treegp-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/tests/test_gp_interp.py` & `treegp-1.2.0/tests/test_gp_interp.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/tests/test_hyp_search.py` & `treegp-1.2.0/tests/test_hyp_search.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/tests/test_kernels.py` & `treegp-1.2.0/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/tests/test_meanify.py` & `treegp-1.2.0/tests/test_meanify.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/treegp/__init__.py` & `treegp-1.2.0/treegp/__init__.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/treegp/gp_interp.py` & `treegp-1.2.0/treegp/gp_interp.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,22 +102,25 @@
             y0 = average["PARAMS0"][0]
         else:
             X0 = None
             y0 = None
         self._X0 = X0
         self._y0 = y0
 
+        self._alpha = None
+
     def _fit(self, kernel, X, y, y_err):
         """Update the Kernel with data.
 
         :param kernel: sklearn.gaussian_process kernel.
         :param X:  Coordinates of the field.  (n_samples, 1 or 2)
         :param y:  Values of the field.  (n_samples)
         :param y_err: Error of y. (n_samples)
         """
+        self._alpha = None
         if self.optimizer != "none":
             # Hyperparameters estimation using 2-point correlation
             # function information.
             if self.optimizer in ["two-pcf", "anisotropic"]:
                 anisotropic = self.optimizer == "anisotropic"
                 self._optimizer = treegp.two_pcf(
                     X,
@@ -168,19 +171,23 @@
         :param y:      Values of the field.  (n_samples)
         :param X1:     The coodinates of the field.  (n_samples, 1 or 2)
         :param X2:     The coordinates at which to interpolate.  (n_samples, 1 or 2)
         :param kernel: sklearn.gaussian_process kernel.
         :param y_err:  Error of y. (n_samples)
         """
         HT = kernel.__call__(X2, Y=X1)
-        K = kernel.__call__(X1) + np.eye(len(y)) * y_err**2
-        factor = (cholesky(K, overwrite_a=True, lower=False), False)
-        alpha = cho_solve(factor, y, overwrite_b=False)
-        y_predict = np.dot(HT, alpha.reshape((len(alpha), 1))).T[0]
+        K = None
+        if self._alpha is None:
+            K = kernel.__call__(X1) + np.eye(len(y)) * y_err**2
+            factor = (cholesky(K, overwrite_a=True, lower=False), False)
+            self._alpha = cho_solve(factor, y, overwrite_b=False)
+        y_predict = np.dot(HT, self._alpha.reshape((len(self._alpha), 1))).T[0]
         if return_cov:
+            if K is None:
+                K = kernel.__call__(X1) + np.eye(len(y)) * y_err**2
             fact = cholesky(
                 K, lower=True
             )  # I am computing maybe twice the same things...
             v = cho_solve((fact, True), HT.T)
             y_cov = kernel.__call__(X2) - HT.dot(v)
             return y_predict, y_cov
         else:
@@ -211,14 +218,17 @@
             y_err = np.sqrt(copy.deepcopy(self._y_err) ** 2 + self.white_noise**2)
         self._y_err = y_err
 
         if self.normalize:
             self._mean = np.mean(y - self._spatial_average)
         else:
             self._mean = 0.0
+        # Initialize alpha to None so that we know to recompute it if we change the
+        # input data.
+        self._alpha = None
 
     def _build_average_meanify(self, X):
         """Compute spatial average from meanify output for a given coordinate using KN interpolation.
         If no average_fits was given, return array of 0.
 
         :param X: Coordinates of training coordinates where to interpolate. (n_samples, 1 or 2)
         """
```

### Comparing `treegp-1.1.0/treegp/kernels.py` & `treegp-1.2.0/treegp/kernels.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/treegp/log_likelihood.py` & `treegp-1.2.0/treegp/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/treegp/meanify.py` & `treegp-1.2.0/treegp/meanify.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/treegp/two_pcf.py` & `treegp-1.2.0/treegp/two_pcf.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/treegp/utils.py` & `treegp-1.2.0/treegp/utils.py`

 * *Files identical despite different names*

### Comparing `treegp-1.1.0/treegp.egg-info/PKG-INFO` & `treegp-1.2.0/treegp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: treegp
-Version: 1.1.0
+Version: 1.2.0
 Summary: treegp
 Home-page: https://github.com/PFLeget/treegp
-Download-URL: https://github.com/PFLeget/treegp/releases/tag/v1.1.0.zip
+Download-URL: https://github.com/PFLeget/treegp/releases/tag/v1.2.0.zip
 Author: PFLeget
 License: BSD License
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
 License-File: LICENCE
 Requires-Dist: numpy
 Requires-Dist: scipy
```

