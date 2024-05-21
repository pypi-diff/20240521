# Comparing `tmp/vegspec-1.0.2.tar.gz` & `tmp/vegspec-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegspec-1.0.2.tar", last modified: Tue Apr  2 13:11:18 2024, max compression
+gzip compressed data, was "vegspec-1.0.3.tar", last modified: Tue May 21 21:06:47 2024, max compression
```

## Comparing `vegspec-1.0.2.tar` & `vegspec-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-04-02 13:11:18.578197 vegspec-1.0.2/
--rwx------   0 kthorp    (1000) kthorp    (1000)     1378 2022-01-25 01:01:56.000000 vegspec-1.0.2/LICENSE.md
--rw-r--r--   0 kthorp    (1000) kthorp    (1000)     5077 2024-04-02 13:11:18.578197 vegspec-1.0.2/PKG-INFO
--rwx------   0 kthorp    (1000) kthorp    (1000)     4467 2024-01-25 17:43:44.000000 vegspec-1.0.2/README.md
--rwx------   0 kthorp    (1000) kthorp    (1000)      104 2021-12-03 23:38:41.000000 vegspec-1.0.2/pyproject.toml
--rwx------   0 kthorp    (1000) kthorp    (1000)      725 2024-04-02 13:11:18.578197 vegspec-1.0.2/setup.cfg
-drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-04-02 13:11:18.574197 vegspec-1.0.2/src/
-drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-04-02 13:11:18.578197 vegspec-1.0.2/src/vegspec/
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)      608 2024-01-24 13:59:01.000000 vegspec-1.0.2/src/vegspec/__init__.py
--rwx------   0 kthorp    (1000) kthorp    (1000)    65864 2024-03-29 14:25:19.000000 vegspec-1.0.2/src/vegspec/vegspec.py
-drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-04-02 13:11:18.578197 vegspec-1.0.2/src/vegspec.egg-info/
--rw-r--r--   0 kthorp    (1000) kthorp    (1000)     5077 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/PKG-INFO
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)      266 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/SOURCES.txt
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)        1 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/dependency_links.txt
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)       12 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/requires.txt
--rw-rw-r--   0 kthorp    (1000) kthorp    (1000)        8 2024-04-02 13:11:18.000000 vegspec-1.0.2/src/vegspec.egg-info/top_level.txt
+drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-05-21 21:06:47.142224 vegspec-1.0.3/
+-rwx------   0 kthorp    (1000) kthorp    (1000)     1378 2022-01-25 01:01:56.000000 vegspec-1.0.3/LICENSE.md
+-rw-r--r--   0 kthorp    (1000) kthorp    (1000)     7284 2024-05-21 21:06:47.142224 vegspec-1.0.3/PKG-INFO
+-rwx------   0 kthorp    (1000) kthorp    (1000)     6626 2024-05-21 21:01:41.000000 vegspec-1.0.3/README.md
+-rwx------   0 kthorp    (1000) kthorp    (1000)      104 2021-12-03 23:38:41.000000 vegspec-1.0.3/pyproject.toml
+-rwx------   0 kthorp    (1000) kthorp    (1000)      745 2024-05-21 21:06:47.142224 vegspec-1.0.3/setup.cfg
+drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-05-21 21:06:47.138224 vegspec-1.0.3/src/
+drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-05-21 21:06:47.138224 vegspec-1.0.3/src/vegspec/
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)      608 2024-01-24 13:59:01.000000 vegspec-1.0.3/src/vegspec/__init__.py
+-rwx------   0 kthorp    (1000) kthorp    (1000)    66341 2024-05-09 17:49:44.000000 vegspec-1.0.3/src/vegspec/vegspec.py
+drwxrwxr-x   0 kthorp    (1000) kthorp    (1000)        0 2024-05-21 21:06:47.142224 vegspec-1.0.3/src/vegspec.egg-info/
+-rw-r--r--   0 kthorp    (1000) kthorp    (1000)     7284 2024-05-21 21:06:47.000000 vegspec-1.0.3/src/vegspec.egg-info/PKG-INFO
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)      266 2024-05-21 21:06:47.000000 vegspec-1.0.3/src/vegspec.egg-info/SOURCES.txt
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)        1 2024-05-21 21:06:47.000000 vegspec-1.0.3/src/vegspec.egg-info/dependency_links.txt
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)       30 2024-05-21 21:06:47.000000 vegspec-1.0.3/src/vegspec.egg-info/requires.txt
+-rw-rw-r--   0 kthorp    (1000) kthorp    (1000)        8 2024-05-21 21:06:47.000000 vegspec-1.0.3/src/vegspec.egg-info/top_level.txt
```

### Comparing `vegspec-1.0.2/LICENSE.md` & `vegspec-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vegspec-1.0.2/setup.cfg` & `vegspec-1.0.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vegspec
-version = 1.0.2
+version = 1.0.3
 author = Dr. Kelly R. Thorp
 author_email = kelly.thorp@usda.gov
 description = A compilation of vegetative spectral indices and transformations in Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://github.com/kthorp/vegspec
 project_urls = 
@@ -17,15 +17,17 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
 install_requires = 
+	matplotlib
 	numpy
+	pandas
 	scipy
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `vegspec-1.0.2/src/vegspec/__init__.py` & `vegspec-1.0.3/src/vegspec/__init__.py`

 * *Files identical despite different names*

### Comparing `vegspec-1.0.2/src/vegspec/vegspec.py` & `vegspec-1.0.3/src/vegspec/vegspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 functions for analysis of one vegetative reflectance spectrum, including
 calculations of spectral derivatives, log inverse reflectance, continuum
 removal, and more than 145 published spectral vegetation indices.
 
 04/06/2022 Initial Python functions developed by Kelly Thorp
 12/02/2022 Finalized code for release in the vegspec Python package
 01/23/2023 Added more spectral vegetation indices
+05/09/2024 Finalized code for first SoftwareX published release
 ########################################################################
 """
 
 import numpy as np
-#import matplotlib.pyplot as plt
+import matplotlib.pyplot as plt
 from scipy.signal import savgol_filter
 from scipy.spatial import ConvexHull
 from scipy.optimize import curve_fit
 import math
 
 class VegSpec:
     """A class for analyzing vegetative spectral reflectance data.
@@ -282,15 +283,14 @@
         self.indices.update({'WUTOR':  self._WUTOR()  })
         self.indices.update({'WUMOR':  self._WUMOR()  })
         self.indices.update({'DCNI':   self._DCNI()   })
         self.indices.update({'TGI':    self._TGI()    })
         self.indices.update({'WDRVI2': self._WDRVI2() })
         self.indices.update({'AIVI':   self._AIVI()   })
         self.indices.update({'DND':    self._DND()    })
-        self.indices.update({'GRSUM':  self._GRSUM()  })
 
     #Spectral transformations
     def _derivative1(self,fs1,po1):
         """Compute first derivative using a Savitsky-Golay filter"""
         return savgol_filter(self.rf,fs1,po1,1)
 
     def _derivative2(self,fs2,po2):
@@ -365,14 +365,15 @@
         b = self.solicpt
         return (Rnir-a*Rred-b)/math.sqrt(1.+a*a)
 
     def _WLREIP(self):
         """Identify the wavelength (nm) of the red edge inflection point
         (Collins, 1978; Horler et al., 1983)"""
         widx = np.where(np.logical_and(self.wl>=680.,self.wl<=750.))
+        if len(widx[0])==0: return self.NaN
         return self.wl[widx][np.argmax(self.rfd1[widx])]
 
     def _DVI(self):
         """Compute the Difference Vegetation Index (DVI)
         (Tucker, 1979)"""
         Rred = np.interp(self.wlred,self.wl,self.rf,self.NaN,self.NaN)
         Rnir = np.interp(self.wlnir,self.wl,self.rf,self.NaN,self.NaN)
@@ -433,14 +434,15 @@
         return np.interp(703.,self.wl,self.rfd1,self.NaN,self.NaN)
 
     def _BDR(self):
         """Compute the Boochs derivative ratio (BDR)
         (Boochs et al., 1990)"""
         D703 = np.interp(703.,self.wl,self.rfd1,self.NaN,self.NaN)
         widx = np.where(np.logical_and(self.wl>=680.,self.wl<=750.))
+        if len(widx[0])==0: return self.NaN
         Dmax = np.amax(self.rfd1[widx])
         return D703/Dmax
 
     def _SAVI2(self):
         """Compute the Soil-Adjusted Vegetation Index 2 (SAVI2)
         Original SAVI2 publication (Major et al., 1990)
         Soil line parameters (Huete et al., 1984)"""
@@ -589,20 +591,22 @@
         R900 = np.interp(900.,self.wl,self.rf,self.NaN,self.NaN)
         return R970/R900
 
     def _PD(self):
         """Compute the Penuelas derivative (PD)
         (Penuelas et al., 1993)"""
         widx = np.where(np.logical_and(self.wl>=900.,self.wl<=970.))
+        if len(widx[0])==0: return self.NaN
         return np.amin(self.rfd1[widx])
 
     def _WLPD(self):
         """Identify the wavelength (nm) of the minimum first derivative
         in the near infrared region (WLPD) (Penuelas et al., 1993)"""
         widx = np.where(np.logical_and(self.wl>=900.,self.wl<=970.))
+        if len(widx[0])==0: return self.NaN
         return self.wl[widx][np.argmin(self.rfd1[widx])]
 
     def _VSR(self):
         """Compute the Vogelmann simple ratio (VSR)
         (Vogelmann et al., 1993)"""
         R720 = np.interp(720.,self.wl,self.rf,self.NaN,self.NaN)
         R740 = np.interp(740.,self.wl,self.rf,self.NaN,self.NaN)
@@ -646,21 +650,23 @@
         return R695/R670
 
     def _FSUM(self):
         """Compute the area of the first derivative red edge peak from
         680 nm to 780 nm (FSUM) (Filella & Penuelas, 1994;
         Fillela et al., 1995)"""
         widx = np.where(np.logical_and(self.wl>=680.,self.wl<=780.))
+        if len(widx[0])==0: return self.NaN
         return np.sum(self.rfd1[widx]*self.bndwdth[widx])
 
     def _DREIP(self):
         """Identify the amplitude of the first derivative at the red
         edge inflection point (DREIP) (Filella & Penuelas, 1994;
         Fillela et al., 1995)"""
         widx = np.where(np.logical_and(self.wl>=680.,self.wl<=780.))
+        if len(widx[0])==0: return self.NaN
         return np.amax(self.rfd1[widx])
 
     def _NDVI3(self):
         """Compute the Normalized Difference Vegetation Index 3 (NDVI3)
         (Gitelson & Merzlyak, 1994)"""
         R705 = np.interp(705.,self.wl,self.rf,self.NaN,self.NaN)
         R750 = np.interp(750.,self.wl,self.rf,self.NaN,self.NaN)
@@ -668,22 +674,24 @@
 
     def _GSUM1(self):
         """Compute the sum of reflectance from 705 nm to 750 nm,
         normalized by reflectance at 705 nm (GSUM1)
         (Gitelson & Merzlyak, 1994)"""
         R705 = np.interp(705.,self.wl,self.rf,self.NaN,self.NaN)
         widx = np.where(np.logical_and(self.wl>=705.,self.wl<=750.))
+        if len(widx[0])==0: return self.NaN
         return np.sum((self.rf[widx]/R705-1.)*self.bndwdth[widx])
 
     def _GSUM2(self):
         """Compute the sum of reflectance from 705 nm to 750 nm,
         normalized by reflectance at 555 nm (GSUM2)
         (Gitelson & Merzlyak, 1994)"""
         R555 = np.interp(555.,self.wl,self.rf,self.NaN,self.NaN)
         widx = np.where(np.logical_and(self.wl>=705.,self.wl<=750.))
+        if len(widx[0])==0: return self.NaN
         return np.sum((self.rf[widx]/R555-1.)*self.bndwdth[widx])
 
     def _NLI(self):
         """Compute the Nonlinear Index (NLI) (Goel & Qin, 1994)"""
         Rred = np.interp(self.wlred,self.wl,self.rf,self.NaN,self.NaN)
         Rnir = np.interp(self.wlnir,self.wl,self.rf,self.NaN,self.NaN)
         return (Rnir*Rnir-Rred)/(Rnir*Rnir+Rred)
@@ -716,16 +724,18 @@
         R680 = np.interp(680.,self.wl,self.rf,self.NaN,self.NaN)
         return (R680-R430)/(R680+R430)
 
     def _EGFN(self):
         """Compute the Edge-Green First-derivative Normalized Difference
         Index (EGFN) (Penuelas et al., 1994)"""
         widx = np.where(np.logical_and(self.wl>=500.,self.wl<=600.))
+        if len(widx[0])==0: return self.NaN
         dG = np.amax(self.rfd1[widx])
         widx = np.where(np.logical_and(self.wl>=680.,self.wl<=750.))
+        if len(widx[0])==0: return self.NaN
         dRE = np.amax(self.rfd1[widx])
         return (dRE-dG)/(dRE+dG)
 
     def _MSAVI1(self):
         """Compute the Modified Soil Adjusted Vegetation Index 1 (MSAVI1)
         MSAVI formualtion (Qi et al., 1994)
         Soil line slope (Heute et al., 1984)"""
@@ -745,20 +755,22 @@
         sqrterm = math.pow(2.*Rnir+1.,2.)
         return 0.5*(2.*Rnir+1.-math.sqrt(sqrterm-8.*(Rnir-Rred)))
 
     def _ESUM1(self):
         """Compute the area of the first derivative red edge peak from
         626 nm to 795 nm (ESUM1) (Elvidge & Chen, 1995)"""
         widx = np.where(np.logical_and(self.wl>=626.,self.wl<=795.))
+        if len(widx[0])==0: return self.NaN
         return np.sum(np.absolute(self.rfd1[widx])*self.bndwdth[widx])
 
     def _ESUM2(self):
         """Compute the area of the second derivative red edge peaks from
         626 nm to 795 nm (ESUM2) (Elvidge & Chen, 1995)"""
         widx = np.where(np.logical_and(self.wl>=626.,self.wl<=795.))
+        if len(widx[0])==0: return self.NaN
         return np.sum(np.absolute(self.rfd2[widx])*self.bndwdth[widx])
 
     def _NDPI(self):
         """Compute the Normalized Difference Pigment Index (NDPI)
         (Penuelas et al., 1995a) Photosynthetica"""
         R420 = np.interp(420.,self.wl,self.rf,self.NaN,self.NaN)
         R670 = np.interp(670.,self.wl,self.rf,self.NaN,self.NaN)
@@ -1022,52 +1034,57 @@
 
     def _MND2(self):
         """Compute the Maccioni normalize difference 2 (MND2)
         (Maccioni et al., 2001)"""
         R542 = np.interp(542.,self.wl,self.rf,self.NaN,self.NaN)
         R750 = np.interp(750.,self.wl,self.rf,self.NaN,self.NaN)
         widx = np.where(np.logical_and(self.wl>=660.,self.wl<=680.))
+        if len(widx[0])==0: return self.NaN
         Rredmin = np.amin(self.rf[widx])
         return (R542-Rredmin)/(R750-Rredmin)
 
     def _MND3(self):
         """Compute the Maccioni normalize difference 3 (MND3)
         (Maccioni et al., 2001)"""
         R706 = np.interp(706.,self.wl,self.rf,self.NaN,self.NaN)
         R750 = np.interp(750.,self.wl,self.rf,self.NaN,self.NaN)
         widx = np.where(np.logical_and(self.wl>=660.,self.wl<=680.))
+        if len(widx[0])==0: return self.NaN
         Rredmin = np.amin(self.rf[widx])
         return (R706-Rredmin)/(R750-Rredmin)
 
     def _MND4(self):
         """Compute the Maccioni normalize difference 4 (MND4)
         (Maccioni et al., 2001)"""
         R556 = np.interp(556.,self.wl,self.rf,self.NaN,self.NaN)
         R750 = np.interp(750.,self.wl,self.rf,self.NaN,self.NaN)
         widx = np.where(np.logical_and(self.wl>=660.,self.wl<=680.))
+        if len(widx[0])==0: return self.NaN
         Rredmin = np.amin(self.rf[widx])
         return (R556-Rredmin)/(R750-Rredmin)
 
     def _CAINT(self):
         """Compute the Chlorophyll Absorption Integral (CAINT)
         (Oppelt & Mauser, 2001)"""
         widx = np.where(np.logical_and(self.wl>=600.,self.wl<=735.))
+        if len(widx[0])==0: return self.NaN
         R600 = np.interp(600.,self.wl,self.rf,self.NaN,self.NaN)*100.
         R735 = np.interp(735.,self.wl,self.rf,self.NaN,self.NaN)*100.
         x = [600.,735.]
         y = [R600,R735]
         coef = np.polyfit(x,y,1)
         re = coef[0]*self.wl+coef[1]
         req = self.rf[widx]/re[widx]*self.bndwdth[widx]
         return np.sum(req)
 
     def _ZTSUM(self):
         """Compute the area of the first derivative peak from 680 nm to
         760 nm (ZTSUM) (Zarco-Tejada et al., 2001b)"""
         widx = np.where(np.logical_and(self.wl>=680.,self.wl<=760.))
+        if len(widx[0])==0: return self.NaN
         return np.sum(self.rfd1[widx]*self.bndwdth[widx])
 
     def _PRI3(self):
         """Compute the Photochemical Reflectance Index 3 (PRI3)
         (Zarco-Tejada et al., 2001b)"""
         R531 = np.interp(531.,self.wl,self.rf,self.NaN,self.NaN)
         R570 = np.interp(570.,self.wl,self.rf,self.NaN,self.NaN)
@@ -1500,13 +1517,7 @@
 
     def _DND(self):
         """Compute the Derivative Normalized Difference (DND)
         (Sonobe & Wang, 2017)"""
         D522 = np.interp(522.,self.wl,self.rfd1,self.NaN,self.NaN)
         D728 = np.interp(728.,self.wl,self.rfd1,self.NaN,self.NaN)
         return (D522-D728)/(D522+D728)
-
-    def _GRSUM(self):
-        """Compute the area of the green reflectance peak from 500 nm
-        to 600 nm (GRSUM) (Thorp and Thompson, in prep)"""
-        widx = np.where(np.logical_and(self.wl>=500.,self.wl<=600.))
-        return np.sum(self.rf[widx]*self.bndwdth[widx])
```

