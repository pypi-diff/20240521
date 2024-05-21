# Comparing `tmp/pandorasim-1.0.3.tar.gz` & `tmp/pandorasim-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorasim-1.0.3.tar", max compression
+gzip compressed data, was "pandorasim-1.0.4.tar", max compression
```

## Comparing `pandorasim-1.0.3.tar` & `pandorasim-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.3/LICENSE
--rw-r--r--   0        0        0      229 2024-05-21 03:54:38.629003 pandorasim-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      419 2024-05-21 03:54:47.765205 pandorasim-1.0.3/src/pandorasim/__init__.py
--rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.3/src/pandorasim/docstrings.py
--rw-r--r--   0        0        0    14831 2024-05-21 02:31:51.097349 pandorasim-1.0.3/src/pandorasim/nirsim.py
--rw-r--r--   0        0        0     6351 2024-05-21 02:31:51.097525 pandorasim-1.0.3/src/pandorasim/sim.py
--rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.3/src/pandorasim/utils.py
--rw-r--r--   0        0        0    19887 2024-05-21 02:31:51.097951 pandorasim-1.0.3/src/pandorasim/visiblesim.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 pandorasim-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.4/LICENSE
+-rw-r--r--   0        0        0      229 2024-05-21 17:26:54.940213 pandorasim-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      419 2024-05-21 17:27:00.156611 pandorasim-1.0.4/src/pandorasim/__init__.py
+-rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.4/src/pandorasim/docstrings.py
+-rw-r--r--   0        0        0    14831 2024-05-21 17:26:05.474937 pandorasim-1.0.4/src/pandorasim/nirsim.py
+-rw-r--r--   0        0        0     6368 2024-05-21 17:25:58.109880 pandorasim-1.0.4/src/pandorasim/sim.py
+-rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.4/src/pandorasim/utils.py
+-rw-r--r--   0        0        0    20033 2024-05-21 17:26:34.804258 pandorasim-1.0.4/src/pandorasim/visiblesim.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 pandorasim-1.0.4/PKG-INFO
```

### Comparing `pandorasim-1.0.3/LICENSE` & `pandorasim-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.3/src/pandorasim/docstrings.py` & `pandorasim-1.0.4/src/pandorasim/docstrings.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.3/src/pandorasim/nirsim.py` & `pandorasim-1.0.4/src/pandorasim/nirsim.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.3/src/pandorasim/sim.py` & `pandorasim-1.0.4/src/pandorasim/sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.psf = pp.PSF.from_name(self.detector.name)
         logger.stop_spinner()
 
     @add_docstring("ra", "dec", "theta")
     @abstractmethod
     def point(self, ra: u.Quantity, dec: u.Quantity, roll: u.Quantity):
         self.ra, self.dec, self.roll = ra, dec, roll
-        self.wcs = self.detector.get_wcs(self.ra, self.dec)
+        self.wcs = self.detector.get_wcs(self.ra, self.dec, theta=self.roll)
 
         logger.start_spinner("Finding nearby sources...")
         self.source_catalog = self._get_source_catalog()
         self.locations = np.asarray(
             [self.source_catalog.row, self.source_catalog.column]
         ).T
         logger.stop_spinner()
```

### Comparing `pandorasim-1.0.3/src/pandorasim/utils.py` & `pandorasim-1.0.4/src/pandorasim/utils.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.3/src/pandorasim/visiblesim.py` & `pandorasim-1.0.4/src/pandorasim/visiblesim.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,18 +136,19 @@
         source_catalog["flux"] = vis_flux
         return source_catalog
 
     @property
     def background_rate(self):
         return 4 * u.electron / u.second
 
-    @add_docstring("nreads")
+    @add_docstring("nreads", "noise")
     def get_FFI(
         self,
         nreads: int = 50,
+        noise=True,
     ):
         """Get a single frame of data as an FFI
 
         Returns:
         --------
         data : np.ndarray
             Returns a single FFI as a numpy array with dtype uint32.
@@ -158,43 +159,43 @@
         ).value.astype(int)
 
         # FFI has shape (nrows, ncolumns), in units of electrons.
         ffi = self.scene.model(source_flux)
 
         # Apply poisson (shot) noise, ffi now has shape  (nrows, ncolumns), units of electrons
         ffi = np.random.poisson(self.scene.model(source_flux)[0])
-
-        # Apply background to every read, units of electrons
-        ffi += np.random.poisson(
-            (self.background_rate * int_time).value, size=ffi.shape
-        ).astype(int)
-
-        # # Apply a bias to every read which is a Gaussian with mean = bias * nreads value and std = (nreads * (read noise)**2)**0.5
-        # We actually do this as a sum because otherwise the integer math doesn't work out...!?
-
-        test_distribution = (
-            np.random.normal(
-                loc=self.detector.bias.value,
-                scale=self.detector.read_noise.value,
-                size=(nreads, 10000),
+        if noise:
+            # Apply background to every read, units of electrons
+            ffi += np.random.poisson(
+                (self.background_rate * int_time).value, size=ffi.shape
+            ).astype(int)
+
+            # # Apply a bias to every read which is a Gaussian with mean = bias * nreads value and std = (nreads * (read noise)**2)**0.5
+            # We actually do this as a sum because otherwise the integer math doesn't work out...!?
+
+            test_distribution = (
+                np.random.normal(
+                    loc=self.detector.bias.value,
+                    scale=self.detector.read_noise.value,
+                    size=(nreads, 10000),
+                )
+                .astype(int)
+                .sum(axis=0)
             )
-            .astype(int)
-            .sum(axis=0)
-        )
-        ffi += np.random.normal(
-            loc=test_distribution.mean(),
-            scale=self.detector.read_noise.value * np.sqrt(nreads),
-            size=(ffi.shape),
-        ).astype(int)
-
-        # Add poisson noise for the dark current to every frame, units of electrons
-        ffi += np.random.poisson(
-            lam=(self.detector.dark * int_time).value,
-            size=ffi.shape,
-        ).astype(int)
+            ffi += np.random.normal(
+                loc=test_distribution.mean(),
+                scale=self.detector.read_noise.value * np.sqrt(nreads),
+                size=(ffi.shape),
+            ).astype(int)
+
+            # Add poisson noise for the dark current to every frame, units of electrons
+            ffi += np.random.poisson(
+                lam=(self.detector.dark * int_time).value,
+                size=ffi.shape,
+            ).astype(int)
 
         # Apply gain
         #        ffi = self.detector.apply_gain(u.Quantity(ffi.ravel(), unit='electron')).value.reshape(ffi.shape)
         # Crap gain for now because gain calculations are wicked broken
         ffi *= 2
 
         # This is a bit hacky, but for FFIs we'll be ok. We do this because working with individual reads for FFI data is slow.
```

