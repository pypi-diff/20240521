# Comparing `tmp/motionsegmentation-2.9.1.tar.gz` & `tmp/motionsegmentation-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motionsegmentation-2.9.1.tar", last modified: Thu May 16 06:59:54 2024, max compression
+gzip compressed data, was "motionsegmentation-2.9.2.tar", last modified: Tue May 21 05:42:55 2024, max compression
```

## Comparing `motionsegmentation-2.9.1.tar` & `motionsegmentation-2.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 06:59:54.453796 motionsegmentation-2.9.1/
--rw-rw-rw-   0        0        0     1067 2024-05-16 06:59:00.000000 motionsegmentation-2.9.1/LICENSE
--rw-rw-rw-   0        0        0     5773 2024-05-16 06:59:54.453796 motionsegmentation-2.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     3692 2024-05-16 06:59:00.000000 motionsegmentation-2.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 06:59:54.416006 motionsegmentation-2.9.1/motionSegmentation/
--rw-rw-rw-   0        0        0   118580 2024-05-16 06:59:00.000000 motionsegmentation-2.9.1/motionSegmentation/BsplineFourier.py
--rw-rw-rw-   0        0        0    30521 2024-05-16 06:59:00.000000 motionsegmentation-2.9.1/motionSegmentation/__init__.py
--rw-rw-rw-   0        0        0    79657 2024-05-16 06:59:00.000000 motionsegmentation-2.9.1/motionSegmentation/bfSolver.py
--rw-rw-rw-   0        0        0    30300 2024-05-16 06:59:00.000000 motionsegmentation-2.9.1/motionSegmentation/motionCorrect.py
--rw-rw-rw-   0        0        0    28203 2024-05-16 06:59:00.000000 motionsegmentation-2.9.1/motionSegmentation/segment.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:59:54.453796 motionsegmentation-2.9.1/motionSegmentation.egg-info/
--rw-rw-rw-   0        0        0     5773 2024-05-16 06:59:54.000000 motionsegmentation-2.9.1/motionSegmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-05-16 06:59:54.000000 motionsegmentation-2.9.1/motionSegmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 06:59:54.000000 motionsegmentation-2.9.1/motionSegmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-16 06:59:54.000000 motionsegmentation-2.9.1/motionSegmentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-16 06:59:54.000000 motionsegmentation-2.9.1/motionSegmentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1159 2024-05-16 06:59:00.000000 motionsegmentation-2.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 06:59:54.453796 motionsegmentation-2.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 05:42:55.502811 motionsegmentation-2.9.2/
+-rw-rw-rw-   0        0        0     1067 2024-05-21 05:42:11.000000 motionsegmentation-2.9.2/LICENSE
+-rw-rw-rw-   0        0        0     5773 2024-05-21 05:42:55.502811 motionsegmentation-2.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3692 2024-05-21 05:42:11.000000 motionsegmentation-2.9.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 05:42:55.455924 motionsegmentation-2.9.2/motionSegmentation/
+-rw-rw-rw-   0        0        0   118580 2024-05-21 05:42:11.000000 motionsegmentation-2.9.2/motionSegmentation/BsplineFourier.py
+-rw-rw-rw-   0        0        0    30791 2024-05-21 05:42:11.000000 motionsegmentation-2.9.2/motionSegmentation/__init__.py
+-rw-rw-rw-   0        0        0    79821 2024-05-21 05:42:11.000000 motionsegmentation-2.9.2/motionSegmentation/bfSolver.py
+-rw-rw-rw-   0        0        0    30300 2024-05-21 05:42:11.000000 motionsegmentation-2.9.2/motionSegmentation/motionCorrect.py
+-rw-rw-rw-   0        0        0    28203 2024-05-21 05:42:11.000000 motionsegmentation-2.9.2/motionSegmentation/segment.py
+drwxrwxrwx   0        0        0        0 2024-05-21 05:42:55.502811 motionsegmentation-2.9.2/motionSegmentation.egg-info/
+-rw-rw-rw-   0        0        0     5773 2024-05-21 05:42:55.000000 motionsegmentation-2.9.2/motionSegmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-05-21 05:42:55.000000 motionsegmentation-2.9.2/motionSegmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 05:42:55.000000 motionsegmentation-2.9.2/motionSegmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-21 05:42:55.000000 motionsegmentation-2.9.2/motionSegmentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-21 05:42:55.000000 motionsegmentation-2.9.2/motionSegmentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1159 2024-05-21 05:42:11.000000 motionsegmentation-2.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 05:42:55.502811 motionsegmentation-2.9.2/setup.cfg
```

### Comparing `motionsegmentation-2.9.1/LICENSE` & `motionsegmentation-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `motionsegmentation-2.9.1/PKG-INFO` & `motionsegmentation-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionSegmentation
-Version: 2.9.1
+Version: 2.9.2
 Summary: Explicit spatio-temporal regularization of motion tracking.
 Author-email: Wei Xuan Chan <w.x.chan1986@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 W. X. Chan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `motionsegmentation-2.9.1/README.md` & `motionsegmentation-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `motionsegmentation-2.9.1/motionSegmentation/BsplineFourier.py` & `motionsegmentation-2.9.2/motionSegmentation/BsplineFourier.py`

 * *Files identical despite different names*

### Comparing `motionsegmentation-2.9.1/motionSegmentation/__init__.py` & `motionsegmentation-2.9.2/motionSegmentation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,28 +177,33 @@
                         -segment verion 2.7.19
 Author: w.x.chan@gmail.com    16May2024                - v2.9.1   
                                 -added multiresolution level for time (multiTimeRes)
                         -bfSolver version 2.8.0
                         -BsplineFourier version 2.7.14
                         -motionCorrect version 2.7.8
                         -segment verion 2.7.19
+Author: w.x.chan@gmail.com    21May2024                - v2.9.2   
+                        -bfSolver version 2.9.2
+                        -BsplineFourier version 2.7.14
+                        -motionCorrect version 2.7.8
+                        -segment verion 2.7.19
 Requirements:
     autoD
     numpy
     re
     scipy
     BsplineFourier
     pickle (optional)
     nfft
 
 Known Bug:
     HSV color format not supported
 All rights reserved.
 '''
-_version='2.9.1'
+_version='2.9.2'
 import logging
 logger = logging.getLogger('motionSegmentation v'+_version)
 logger.info('motionSegmentation version '+_version)
 
 import os
 import sys
 import numpy as np
```

### Comparing `motionsegmentation-2.9.1/motionSegmentation/bfSolver.py` & `motionsegmentation-2.9.2/motionSegmentation/bfSolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,26 +25,28 @@
                                                              -remove Bspline2D in addBsplineFile function (bug)
                                                              -debug refTimeStep option in estimateInitialwithRefTime
                                                              -auto detect timeMapList in estimateInitialwithRefTime
   Author: w.x.chan@gmail.com         08Jul2021           - v2.7.20
                                                              -added fmt for pointTrace
   Author: w.x.chan@gmail.com         15Jul2021           - v2.8.0
                                                              -added trimesh.repair.fix_normals for pointTrace 
+  Author: w.x.chan@gmail.com         21May2021           - v2.9.2
+                                                             -fixed pointbypoint_exact1 solving 
 
 Requirements:
     BsplineFourier
     numpy
     scipy
     nfft
 
 Known Bug:
     None
 All rights reserved.
 '''
-_version='2.8.0'
+_version='2.9.2'
 
 import logging
 logger = logging.getLogger(__name__)
 import numpy as np
 import autoD as ad
 import os
 import sys
@@ -347,15 +349,15 @@
         '''
         if method=='pointbypoint':
             sampleCoefList,rmsList=self.solve_pointbypoint(maxError=maxError,tRef=tRef,maxIteration=maxIteration,convergence=convergence,reportevery=reportevery,tempSave=tempSave,resume=resume)
             if type(rmsBasedWeighted)==type(None):
                 rmsweight=None
             else:
                 rmsweight=rmsBasedWeighted(rmsList)
-        elif method='pointbypoint_exact1':
+        elif method=='pointbypoint_exact1':
             sampleCoefList=self.solve_pointbypoint_exact1()
             rmsweight=None
         self.bsFourier.regrid(self.points,sampleCoefList,weight=rmsweight,linearConstrainPoints=linearConstrainPoints,linearConstrainWeight=linearConstrainWeight)
         logger.info('BsplineFourier updated')
     def solve_pointbypoint_exact1(self):
         ''' 
         Solves for the bsplineFourier with 1 cos coeficient only and bspline that goes starts from 0
```

### Comparing `motionsegmentation-2.9.1/motionSegmentation/motionCorrect.py` & `motionsegmentation-2.9.2/motionSegmentation/motionCorrect.py`

 * *Files identical despite different names*

### Comparing `motionsegmentation-2.9.1/motionSegmentation/segment.py` & `motionsegmentation-2.9.2/motionSegmentation/segment.py`

 * *Files identical despite different names*

### Comparing `motionsegmentation-2.9.1/motionSegmentation.egg-info/PKG-INFO` & `motionsegmentation-2.9.2/motionSegmentation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionSegmentation
-Version: 2.9.1
+Version: 2.9.2
 Summary: Explicit spatio-temporal regularization of motion tracking.
 Author-email: Wei Xuan Chan <w.x.chan1986@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 W. X. Chan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `motionsegmentation-2.9.1/pyproject.toml` & `motionsegmentation-2.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motionSegmentation"
-version = "2.9.1"
+version = "2.9.2"
 description = "Explicit spatio-temporal regularization of motion tracking."
 readme = "README.md"
 authors = [{ name = "Wei Xuan Chan", email = "w.x.chan1986@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

