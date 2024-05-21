# Comparing `tmp/splayout-0.5.3.tar.gz` & `tmp/splayout-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splayout-0.5.3.tar", last modified: Sun May 19 11:44:50 2024, max compression
+gzip compressed data, was "splayout-0.5.4.tar", last modified: Tue May 21 09:33:03 2024, max compression
```

## Comparing `splayout-0.5.3.tar` & `splayout-0.5.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-19 11:44:46.000000 splayout-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-19 11:44:50.962710 splayout-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-19 11:44:46.000000 splayout-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/SPLayout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:44:50.962710 splayout-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-19 11:44:47.000000 splayout-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.954710 splayout-0.5.3/splayout/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.958710 splayout-0.5.3/splayout/adjointmethod/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/adjointmultitoopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/adjointshapeopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/adjointtopologyopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/scalabletoregion3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/shaperegion2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/shaperegion3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/topologyregion2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/topologyregion3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.958710 splayout-0.5.3/splayout/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/binarybatalgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/binarygeneticalgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/binaryparticleswarmalgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/directbinarysearchalgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/particleswarmalgorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/splayout/components/
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/AEMDgrating.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/bend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/doubleconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/filledpattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    48385 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/microring.py
--rw-r--r--   0 runner    (1001) docker     (127)    20977 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/pixelsregion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)    13958 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/quarbend.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/sbend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/selfdefinecomponent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27611 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/simpleasymmetricdirectionalcoupler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/slowlyvaryingtaper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/taper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/splayout/lumericalcommun/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/lumericalcommun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    85189 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/lumericalcommun/fdtdapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    43227 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/lumericalcommun/modeapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/splayout/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:03.119354 splayout-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-21 09:32:58.000000 splayout-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-21 09:33:03.119354 splayout-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-21 09:32:58.000000 splayout-0.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:03.119354 splayout-0.5.4/SPLayout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-21 09:33:03.000000 splayout-0.5.4/SPLayout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 09:33:03.000000 splayout-0.5.4/SPLayout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:33:03.000000 splayout-0.5.4/SPLayout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 09:33:03.000000 splayout-0.5.4/SPLayout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:33:03.000000 splayout-0.5.4/SPLayout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:33:03.119354 splayout-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-21 09:32:58.000000 splayout-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:03.115354 splayout-0.5.4/splayout/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:03.115354 splayout-0.5.4/splayout/adjointmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/adjointmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/adjointmethod/adjointmultitoopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/adjointmethod/adjointshapeopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/adjointmethod/adjointtopologyopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/adjointmethod/scalabletoregion3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/adjointmethod/shaperegion2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/adjointmethod/shaperegion3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/adjointmethod/topologyregion2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/adjointmethod/topologyregion3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:03.115354 splayout-0.5.4/splayout/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/algorithms/binarybatalgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/algorithms/binarygeneticalgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/algorithms/binaryparticleswarmalgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/algorithms/directbinarysearchalgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/algorithms/particleswarmalgorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:03.119354 splayout-0.5.4/splayout/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/AEMDgrating.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/bend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/doubleconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/filledpattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48385 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/microring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20977 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/pixelsregion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13958 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/quarbend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/sbend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/selfdefinecomponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27611 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/simpleasymmetricdirectionalcoupler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/slowlyvaryingtaper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/taper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/components/waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:03.119354 splayout-0.5.4/splayout/lumericalcommun/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/lumericalcommun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86013 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/lumericalcommun/fdtdapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43227 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/lumericalcommun/modeapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:03.119354 splayout-0.5.4/splayout/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15139 2024-05-21 09:32:58.000000 splayout-0.5.4/splayout/utils/utils.py
```

### Comparing `splayout-0.5.3/LICENSE` & `splayout-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/PKG-INFO` & `splayout-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.5.3
+Version: 0.5.4
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License-File: LICENSE
 Requires-Dist: gdspy
 Requires-Dist: numpy
```

### Comparing `splayout-0.5.3/README.rst` & `splayout-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/SPLayout.egg-info/PKG-INFO` & `splayout-0.5.4/SPLayout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.5.3
+Version: 0.5.4
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License-File: LICENSE
 Requires-Dist: gdspy
 Requires-Dist: numpy
```

### Comparing `splayout-0.5.3/SPLayout.egg-info/SOURCES.txt` & `splayout-0.5.4/SPLayout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/setup.py` & `splayout-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/__init__.py` & `splayout-0.5.4/splayout/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.3"
+__version__ = "0.5.4"
 
 ## Submodules
 from . import utils
 from . import components
 from . import algorithms
 from . import lumericalcommun
 from . import adjointmethod
```

### Comparing `splayout-0.5.3/splayout/adjointmethod/adjointmultitoopt.py` & `splayout-0.5.4/splayout/adjointmethod/adjointmultitoopt.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/adjointmethod/adjointshapeopt.py` & `splayout-0.5.4/splayout/adjointmethod/adjointshapeopt.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/adjointmethod/adjointtopologyopt.py` & `splayout-0.5.4/splayout/adjointmethod/adjointtopologyopt.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/adjointmethod/scalabletoregion3d.py` & `splayout-0.5.4/splayout/adjointmethod/scalabletoregion3d.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/adjointmethod/shaperegion2d.py` & `splayout-0.5.4/splayout/adjointmethod/shaperegion2d.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/adjointmethod/shaperegion3d.py` & `splayout-0.5.4/splayout/adjointmethod/shaperegion3d.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/adjointmethod/topologyregion2d.py` & `splayout-0.5.4/splayout/adjointmethod/topologyregion2d.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/adjointmethod/topologyregion3d.py` & `splayout-0.5.4/splayout/adjointmethod/topologyregion3d.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/algorithms/binarybatalgorithm.py` & `splayout-0.5.4/splayout/algorithms/binarybatalgorithm.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/algorithms/binarygeneticalgorithm.py` & `splayout-0.5.4/splayout/algorithms/binarygeneticalgorithm.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/algorithms/binaryparticleswarmalgorithm.py` & `splayout-0.5.4/splayout/algorithms/binaryparticleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/algorithms/directbinarysearchalgorithm.py` & `splayout-0.5.4/splayout/algorithms/directbinarysearchalgorithm.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/algorithms/particleswarmalgorithm.py` & `splayout-0.5.4/splayout/algorithms/particleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/AEMDgrating.py` & `splayout-0.5.4/splayout/components/AEMDgrating.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/__init__.py` & `splayout-0.5.4/splayout/components/__init__.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/bend.py` & `splayout-0.5.4/splayout/components/bend.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/doubleconnector.py` & `splayout-0.5.4/splayout/components/doubleconnector.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/filledpattern.py` & `splayout-0.5.4/splayout/components/filledpattern.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/microring.py` & `splayout-0.5.4/splayout/components/microring.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/pixelsregion.py` & `splayout-0.5.4/splayout/components/pixelsregion.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/polygon.py` & `splayout-0.5.4/splayout/components/polygon.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/quarbend.py` & `splayout-0.5.4/splayout/components/quarbend.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/sbend.py` & `splayout-0.5.4/splayout/components/sbend.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/selfdefinecomponent.py` & `splayout-0.5.4/splayout/components/selfdefinecomponent.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/simpleasymmetricdirectionalcoupler.py` & `splayout-0.5.4/splayout/components/simpleasymmetricdirectionalcoupler.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/slowlyvaryingtaper.py` & `splayout-0.5.4/splayout/components/slowlyvaryingtaper.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/taper.py` & `splayout-0.5.4/splayout/components/taper.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/text.py` & `splayout-0.5.4/splayout/components/text.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/components/waveguide.py` & `splayout-0.5.4/splayout/components/waveguide.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/lumericalcommun/fdtdapi.py` & `splayout-0.5.4/splayout/lumericalcommun/fdtdapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,43 @@
         Whether the Lumerical window is hidden (default: False).
     fdtd_path : String
         Path to the Lumerical Python API folder.
     load_file : String
         Path to the .fsp file that what want to be loaded (default: None).
 
     """
-    def __init__(self,hide=0,fdtd_path = "C:\\Program Files\\Lumerical\\v202\\api\\python\\", load_file = None):
-        sys.path.append(fdtd_path)
-        sys.path.append(os.path.dirname(__file__))
-        try:
-            os.add_dll_directory(fdtd_path)
-        except:
-            pass
-        try:
-            import lumapi
-        except:
-            raise Exception(
-                "Lumerical FDTD is not installed in the default path, please specify the python api path with fdtd_path=***.")
+    def __init__(self, hide=0, fdtd_path=None, load_file = None):
+        if not fdtd_path is None:
+            sys.path.append(fdtd_path)
+            sys.path.append(os.path.dirname(__file__))
+            try:
+                os.add_dll_directory(fdtd_path)
+            except:
+                pass
+            try:
+                import lumapi
+            except:
+                raise Exception(
+                    "Can not find Lumerical FDTD in fdtd_path.")
+        else: # auto find
+            fdtd_path = find_lumerical()
+            if not fdtd_path is None:
+                sys.path.append(fdtd_path)
+                sys.path.append(os.path.dirname(__file__))
+                try:
+                    os.add_dll_directory(fdtd_path)
+                except:
+                    pass
+                try:
+                    import lumapi
+                except:
+                    raise Exception("Import lumapi error.")
+            else: # fail to find
+                raise Exception("Can not find Lumerical FDTD automatically, please set fdtd_path=*** in FDTDSimulation.")
+
         self.lumapi = lumapi
         self.fdtd = self.lumapi.FDTD(hide=hide)
         if (type(load_file) != type(None)):
             self.fdtd.eval("load(\"" + load_file + "\");")
         self.global_monitor_set_flag = 0
         self.global_source_set_flag = 0
 
@@ -483,15 +500,15 @@
         """
         self.fdtd.eval("select(\"" + source_name + "\");")
         self.fdtd.eval("set(\"phase\"," +  "%.6f"%(phase) + ");")
 
 
     def add_fdtd_region(self,bottom_left_corner_point,top_right_corner_point,simulation_time=5000, background_material = None,
                         background_index=1.444,mesh_order =2,dimension=3,height = 1, z_min = None,
-                        z_max = None, z_symmetric = 0, y_antisymmetric = 0, y_periodic = 0, pml_layers = 8):
+                        z_max = None, z_symmetric = 0, y_antisymmetric = 0, y_periodic = 0, pml_layers = 8, use_gpu = 0):
         """
         Add simulation region in Lumerical FDTD.
 
         Parameters
         ----------
         bottom_left_corner_point : Point
             Lower left corner of the region.
@@ -515,15 +532,18 @@
             Whether set symmetric in z-axis (default: 0).
         y_antisymmetric : Bool or Int
             Whether set anti-symmetric in y-axis (default: 0).
         y_antisymmetric : Bool or Int
             Whether set anti-symmetric in y-axis (default: 0).
         y_periodic : Bool or Int
             Whether set periodic in y-axis (default: 0).
-
+        pml_layers : Int
+            Number of pml layers (default: 8).
+        use_gpu : Bool or Int
+            Whether to use gpu (default: 8).
         Notes
         -----
         If z_min and z_max are specified, the height property will be invalid.
         If background_material is specified, the background_index will be invalid.
         """
         self.fdtd.eval("addfdtd;")
         self.fdtd.eval("set(\"dimension\"," + str(dimension-1) + ");")
@@ -550,24 +570,27 @@
             else:
                 raise Exception("Wrong background_material specification!")
         else:
             self.fdtd.eval("set(\"index\"," +  str(background_index) + ");")
         self.fdtd.eval("set(\"mesh accuracy\"," + str(mesh_order) + ");")
         self.fdtd.eval("set(\"pml layers\"," +str(pml_layers) +");")
 
-        if (dimension == 3 and z_symmetric == 1):
+        if dimension == 3 and z_symmetric == 1:
             self.fdtd.eval("set(\"z min bc\", \"Symmetric\");")
 
-        if (y_antisymmetric == 1):
+        if y_antisymmetric == 1:
             self.fdtd.eval("set(\"y min bc\", \"Anti-Symmetric\");")
             self.fdtd.eval("set(\"force symmetric y mesh\", 1);")
 
-        if (y_periodic == 1):
+        if y_periodic == 1:
             self.fdtd.eval("set(\"y min bc\", \"Periodic\");")
 
+        if use_gpu == 1:
+            self.fdtd.eval("set(\"express mode\", 1);")
+
     def add_index_region(self, bottom_left_corner_point, top_right_corner_point, height = 1, z_min = None, z_max = None, index_monitor_name="index",dimension = 2):
         """
         Add index monitor (x-y plane) in Lumerical FDTD.
 
         Parameters
         ----------
         bottom_left_corner_point : Point
```

### Comparing `splayout-0.5.3/splayout/lumericalcommun/modeapi.py` & `splayout-0.5.4/splayout/lumericalcommun/modeapi.py`

 * *Files identical despite different names*

### Comparing `splayout-0.5.3/splayout/utils/utils.py` & `splayout-0.5.4/splayout/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import gdspy
 import math
+import os
 
 ## "macros"
 RIGHT = 0
 UP = 90
 LEFT = 180
 DOWN = 270
 VERTICAL = 0
@@ -401,8 +402,25 @@
         # print(polygons[(inv_source_layer.layer,inv_source_layer.datatype)])
         cover = gdspy.offset(polygons[(cover_source_layer.layer,cover_source_layer.datatype)],distance=2,join_first=True, layer=cover_target_layer.layer,datatype=cover_target_layer.datatype,tolerance=0.0001,max_points = 100000)
         top_cell.add(cover)
 
     if (filename[-4:] != ".gds"):
         filename += ".gds"
 
-    lib.write_gds(filename)
+    lib.write_gds(filename)
+
+def find_lumerical():
+    preset_disks = ["C:/", "D:/", "E:/", "F:/", "G:/", "H:/", "I:/", "J:/",
+                    "K:/", "L:/", "M:/", "N:/", "O:/", "P:/", "Q:/", "R:/",
+                    "S:/", "T:/", "U:/", "V:", "W:/", "X:/", "Y:/", "Z:/"]
+    preset_dir = ["Program Files/Lumerical/", "Lumerical/"]
+    version_numbers = [str(num) for num in range(202, 250)]
+    preset_version = [ "v" + version_number + "/api/python" for version_number in version_numbers]
+
+    lumerical_api_path = None
+    for disk in preset_disks:
+        for pdir in preset_dir:
+            for pver in preset_version:
+                if os.path.exists(disk + pdir + pver):
+                    lumerical_api_path = disk + pdir + pver
+
+    return lumerical_api_path
```

