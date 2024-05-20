# Comparing `tmp/nuance-0.6.0.tar.gz` & `tmp/nuance-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuance-0.6.0.tar", max compression
+gzip compressed data, was "nuance-0.6.1.tar", max compression
```

## Comparing `nuance-0.6.0.tar` & `nuance-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1097 2024-03-18 15:32:44.931597 nuance-0.6.0/LICENSE
--rw-r--r--   0        0        0     1492 2024-03-18 15:32:44.931597 nuance-0.6.0/README.md
--rw-r--r--   0        0        0      263 2024-03-18 15:32:44.951596 nuance-0.6.0/nuance/__init__.py
--rw-r--r--   0        0        0     9245 2024-03-18 15:32:44.951596 nuance-0.6.0/nuance/combined.py
--rw-r--r--   0        0        0     1815 2024-03-18 15:32:44.951596 nuance-0.6.0/nuance/core.py
--rw-r--r--   0        0        0     1711 2024-03-18 15:32:44.951596 nuance-0.6.0/nuance/kernels.py
--rw-r--r--   0        0        0    17746 2024-03-18 15:32:44.951596 nuance-0.6.0/nuance/nuance.py
--rw-r--r--   0        0        0     4988 2024-03-18 15:32:44.951596 nuance-0.6.0/nuance/search_data.py
--rw-r--r--   0        0        0     7037 2024-03-18 15:32:44.951596 nuance-0.6.0/nuance/star.py
--rw-r--r--   0        0        0     6403 2024-03-18 15:32:44.951596 nuance-0.6.0/nuance/utils.py
--rw-r--r--   0        0        0      808 2024-03-18 15:32:44.955596 nuance-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 nuance-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-20 23:14:43.037973 nuance-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1492 2024-05-20 23:14:43.037973 nuance-0.6.1/README.md
+-rw-r--r--   0        0        0      254 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/__init__.py
+-rw-r--r--   0        0        0     9245 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/combined.py
+-rw-r--r--   0        0        0     1815 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/core.py
+-rw-r--r--   0        0        0     1811 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/kernels.py
+-rw-r--r--   0        0        0    17920 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/nuance.py
+-rw-r--r--   0        0        0     4988 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/search_data.py
+-rw-r--r--   0        0        0     7156 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/star.py
+-rw-r--r--   0        0        0     6403 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/utils.py
+-rw-r--r--   0        0        0      814 2024-05-20 23:14:43.061973 nuance-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 nuance-0.6.1/PKG-INFO
```

### Comparing `nuance-0.6.0/LICENSE` & `nuance-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nuance-0.6.0/README.md` & `nuance-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nuance-0.6.0/nuance/combined.py` & `nuance-0.6.1/nuance/combined.py`

 * *Files identical despite different names*

### Comparing `nuance-0.6.0/nuance/core.py` & `nuance-0.6.1/nuance/core.py`

 * *Files identical despite different names*

### Comparing `nuance-0.6.0/nuance/kernels.py` & `nuance-0.6.1/nuance/kernels.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from tinygp import GaussianProcess, kernels
 import jax.numpy as jnp
+from tinygp import GaussianProcess, kernels
 
 
 def Rotation(sigma, period, Q0, dQ, f):
+    """
+    A kernel for a rotating star with a single mode of oscillation.
+    """
     Q1 = 1 / 2 + Q0 + dQ
     w1 = (4 * jnp.pi * Q1) / (period * jnp.sqrt(4 * Q1**2 - 1))
     s1 = sigma**2 / ((1 + f) * w1 * Q1)
 
     Q2 = 1 / 2 + Q0
     w2 = (8 * jnp.pi * Q1) / (period * jnp.sqrt(4 * Q1**2 - 1))
     s2 = f * sigma**2 / ((1 + f) * w2 * Q2)
     kernel = kernels.quasisep.SHO(w1, Q1, s1) + kernels.quasisep.SHO(w2, Q2, s2)
     return kernel
 
 
 def rotation(period=None, error=None, long_scale=0.5):
-    params = {
+    initial_params = {
         "log_period": jnp.log(period) if period is not None else jnp.log(1.0),
         "log_Q": jnp.log(100),
         "log_sigma": jnp.log(1e-1),
         "log_dQ": jnp.log(100),
         "log_f": jnp.log(2.0),
         "log_short_scale": jnp.log(1e-2),
         "log_short_sigma": jnp.log(1e-2),
@@ -43,8 +46,8 @@
             )
             + kernels.quasisep.Exp(short_scale, short_sigma)
             + kernels.quasisep.Exp(long_scale, long_sigma)
         )
 
         return GaussianProcess(kernel, time, diag=jitter2, mean=0.0)
 
-    return build_gp, params
+    return build_gp, initial_params
```

### Comparing `nuance-0.6.0/nuance/nuance.py` & `nuance-0.6.1/nuance/nuance.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     compute : bool, optional
         Whether to pre-compute the Cholesky decomposition used by the GP, by default True.
     mean : float, optional
         Mean of the GP, by default 0.0
     search_data : SearchData, optional
         Search data instance, by default None.
     model : callable, optional
-        Model function with signature `model(time, t0, D, P=None)`, by default None.
+        Model function with signature `model(time, t0, D, P=None)`, by default None, which set the model to
+        :code:`partial(nuance.core.transit_protopapas, c=12)`
     """
 
     time: np.ndarray
     """Time"""
     flux: np.ndarray
     """Flux time series"""
     error: np.ndarray = None
@@ -63,15 +64,15 @@
     compute: bool = True
     """Whether to pre-compute the Cholesky decomposition"""
     mean: float = 0.0
     """Mean of the GP"""
     search_data: SearchData = None
     """Search data instance"""
     model: callable = None
-    """Model function with signature `model(time, t0, D, P=None)`"""
+    """Model function with signature :code:`model(time, t0, D, P=None)`"""
 
     def __post_init__(self):
         if self.model is None:
             self.model = partial(core.transit_protopapas, c=12)
 
         self.model = jax.jit(self.model)
 
@@ -133,30 +134,31 @@
 
         noise = gp_mean()
 
         return mean, signal, noise
 
     def gp_optimization(self, build_gp, mask=None):
         """
-        Optimize the Gaussian Process (GP) model using the given build_gp function.
+        Optimization functions to fit a Gaussian Process given a building function.
 
         Parameters
         ----------
         build_gp : function
-            A function that returns a GP object.
+            A function that returns a tinygp.GaussianProcess object.
         mask : array-like, optional
             A boolean array to mask the data, by default None.
 
         Returns
         -------
         tuple
             A tuple containing three functions:
-            - optimize: a function that optimizes the GP model.
-            - mu: a function that returns the mean of the GP model.
-            - nll: a function that returns the negative log-likelihood of the GP model.
+
+            - :code:`optimize`: a function that optimizes the GP model.
+            - :code:`mu`: a function that returns the mean of the GP model (jax.jit-compiled).
+            - :code:`nll`: a function that returns the negative log-likelihood of the GP model (jax.jit-compiled).
         """
         if mask is None:
             mask = np.ones_like(self.time).astype(bool)
 
         masked_x = self.time[mask]
         masked_y = self.flux[mask]
         masked_X = self.X[:, mask]
```

### Comparing `nuance-0.6.0/nuance/search_data.py` & `nuance-0.6.1/nuance/search_data.py`

 * *Files identical despite different names*

### Comparing `nuance-0.6.0/nuance/star.py` & `nuance-0.6.1/nuance/star.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass
 
-import astropy.units as u
 import numpy as np
 
 G = 2942.2062175044193
 # R_sun^3 . M_sun^-1 . day^-2
 # astropy: c.G.to(u.R_sun**3/u.M_sun/(u.day**2)).value
 
 R_EARTH = 0.009167888457668534
@@ -222,25 +221,29 @@
         return self._period(a)
 
     def period_grid(self, time_span, period_max=None, period_min=None, oversampling=1):
         """Grid of optimal periods following Ofir (2014) (in days).
 
         Parameters
         ----------
+        time_span : float
+            time span in days.
         period_max : float
             maximum period in days, by default None which
             defaults to half the time span.
         period_min : float, optional
             minimum period in days, by default None which
             defaults to the roche limit period.
+        oversampling: int, optional
+            oversampling factor, by default 1.
 
         Returns
         -------
         np.ndarray
-            period grid
+            periods in days.
         """
         if period_min is None:
             period_min = self.roche_period()
         if period_max is None:
             period_max = time_span / 2
 
         A = (
```

### Comparing `nuance-0.6.0/nuance/utils.py` & `nuance-0.6.1/nuance/utils.py`

 * *Files identical despite different names*

### Comparing `nuance-0.6.0/pyproject.toml` & `nuance-0.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "nuance"
-version = "0.6.0"
+version = "0.6.1"
 description = "Transit signals detection among correlated noises"
 authors = ["Lionel Garcia"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 tinygp = "*"
-jax = "*"
+jax = "^0.4.25"
 jaxlib = "*"
 jaxopt = "*"
 numpy = "*"
 matplotlib = "*"
 scipy = "*"
 multiprocess = "*"
 tqdm = "*"
```

### Comparing `nuance-0.6.0/PKG-INFO` & `nuance-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: nuance
-Version: 0.6.0
+Version: 0.6.1
 Summary: Transit signals detection among correlated noises
 License: MIT
 Author: Lionel Garcia
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jax
+Requires-Dist: jax (>=0.4.25,<0.5.0)
 Requires-Dist: jaxlib
 Requires-Dist: jaxopt
 Requires-Dist: matplotlib
 Requires-Dist: multiprocess
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tinygp
```

