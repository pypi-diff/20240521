# Comparing `tmp/covdrugsim-1.0.8.tar.gz` & `tmp/covdrugsim-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covdrugsim-1.0.8.tar", max compression
+gzip compressed data, was "covdrugsim-1.0.9.tar", max compression
```

## Comparing `covdrugsim-1.0.8.tar` & `covdrugsim-1.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1082 2024-05-07 02:34:56.851662 covdrugsim-1.0.8/LICENSE
--rw-r--r--   0        0        0     6647 2024-05-07 02:34:56.851662 covdrugsim-1.0.8/README.md
--rw-r--r--   0        0        0     1956 2024-05-07 02:35:26.791800 covdrugsim-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      733 2024-05-07 02:35:26.791800 covdrugsim-1.0.8/setup.py
--rw-r--r--   0        0        0     1337 2024-05-07 02:34:56.851662 covdrugsim-1.0.8/src/covdrugsim/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 02:34:56.851662 covdrugsim-1.0.8/src/covdrugsim/data/__init__.py
--rw-r--r--   0        0        0      170 2024-05-07 02:34:56.851662 covdrugsim-1.0.8/src/covdrugsim/data/chargesExample.txt
--rw-r--r--   0        0        0     4449 2024-05-07 02:34:56.851662 covdrugsim-1.0.8/src/covdrugsim/data/energyLevellerExample.inp
--rw-r--r--   0        0        0   592600 2024-05-07 02:34:56.855662 covdrugsim-1.0.8/src/covdrugsim/data/exampleGaussianOutputs/example1.out
--rw-r--r--   0        0        0   565812 2024-05-07 02:34:56.855662 covdrugsim-1.0.8/src/covdrugsim/data/exampleGaussianOutputs/example2.out
--rw-r--r--   0        0        0  1069703 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/data/exampleGaussianOutputs/example3.out
--rw-r--r--   0        0        0      984 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/data/exampleXYZs/example1.xyz
--rw-r--r--   0        0        0      739 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/data/exampleXYZs/example2.xyz
--rw-r--r--   0        0        0     1327 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/data/exampleXYZs/example3.xyz
--rw-r--r--   0        0        0      866 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/datasets.py
--rw-r--r--   0        0        0      241 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/main.py
--rw-r--r--   0        0        0     3839 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/mdsim/SCbondDist.py
--rw-r--r--   0        0        0        0 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/mdsim/__init__.py
--rw-r--r--   0        0        0     8141 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/mdsim/baseID.py
--rw-r--r--   0        0        0     6071 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/mdsim/bbRMSD.py
--rw-r--r--   0        0        0      331 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/mdsim/config.py
--rw-r--r--   0        0        0     3084 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/mdsim/hbondAnalysis.py
--rw-r--r--   0        0        0     3917 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/mdsim/ligDihedral.py
--rw-r--r--   0        0        0      769 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/mdsim/mdAnalyse.py
--rw-r--r--   0        0        0     5644 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/mdsim/prepMTB.py
--rw-r--r--   0        0        0        0 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/__init__.py
--rw-r--r--   0        0        0     2525 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/admin.py
--rw-r--r--   0        0        0     1313 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/constants.py
--rw-r--r--   0        0        0    10364 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/genScripts.py
--rw-r--r--   0        0        0     1605 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/gsub.sh
--rw-r--r--   0        0        0     4958 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/tabulate.py
--rw-r--r--   0        0        0     4280 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/unitConv.py
--rw-r--r--   0        0        0        0 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/visAnalysis/__init__.py
--rw-r--r--   0        0        0    17951 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
--rw-r--r--   0        0        0    11782 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
--rw-r--r--   0        0        0    13749 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
--rw-r--r--   0        0        0     3882 2024-05-07 02:34:56.863662 covdrugsim-1.0.8/tests/test_covdrugsim.py
--rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 covdrugsim-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-21 11:44:05.593944 covdrugsim-1.0.9/LICENSE
+-rw-r--r--   0        0        0     6647 2024-05-21 11:44:05.593944 covdrugsim-1.0.9/README.md
+-rw-r--r--   0        0        0     1956 2024-05-21 11:44:35.042300 covdrugsim-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      733 2024-05-21 11:44:35.038300 covdrugsim-1.0.9/setup.py
+-rw-r--r--   0        0        0     1337 2024-05-21 11:44:05.593944 covdrugsim-1.0.9/src/covdrugsim/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 11:44:05.593944 covdrugsim-1.0.9/src/covdrugsim/data/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-21 11:44:05.593944 covdrugsim-1.0.9/src/covdrugsim/data/chargesExample.txt
+-rw-r--r--   0        0        0     4449 2024-05-21 11:44:05.593944 covdrugsim-1.0.9/src/covdrugsim/data/energyLevellerExample.inp
+-rw-r--r--   0        0        0   592600 2024-05-21 11:44:05.597944 covdrugsim-1.0.9/src/covdrugsim/data/exampleGaussianOutputs/example1.out
+-rw-r--r--   0        0        0   565812 2024-05-21 11:44:05.597944 covdrugsim-1.0.9/src/covdrugsim/data/exampleGaussianOutputs/example2.out
+-rw-r--r--   0        0        0  1069703 2024-05-21 11:44:05.601944 covdrugsim-1.0.9/src/covdrugsim/data/exampleGaussianOutputs/example3.out
+-rw-r--r--   0        0        0      984 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/data/exampleXYZs/example1.xyz
+-rw-r--r--   0        0        0      739 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/data/exampleXYZs/example2.xyz
+-rw-r--r--   0        0        0     1327 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/data/exampleXYZs/example3.xyz
+-rw-r--r--   0        0        0      866 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/datasets.py
+-rw-r--r--   0        0        0      241 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/main.py
+-rw-r--r--   0        0        0     3839 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/mdsim/SCbondDist.py
+-rw-r--r--   0        0        0        0 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/mdsim/__init__.py
+-rw-r--r--   0        0        0     8141 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/mdsim/baseID.py
+-rw-r--r--   0        0        0     6071 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/mdsim/bbRMSD.py
+-rw-r--r--   0        0        0      331 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/mdsim/config.py
+-rw-r--r--   0        0        0     3084 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/mdsim/hbondAnalysis.py
+-rw-r--r--   0        0        0     3917 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/mdsim/ligDihedral.py
+-rw-r--r--   0        0        0      769 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/mdsim/mdAnalyse.py
+-rw-r--r--   0        0        0     5644 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/mdsim/prepMTB.py
+-rw-r--r--   0        0        0        0 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/__init__.py
+-rw-r--r--   0        0        0     2525 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/admin.py
+-rw-r--r--   0        0        0     1313 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/constants.py
+-rw-r--r--   0        0        0    10364 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/genScripts.py
+-rw-r--r--   0        0        0     1605 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/gsub.sh
+-rw-r--r--   0        0        0     4958 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/tabulate.py
+-rw-r--r--   0        0        0     4280 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/unitConv.py
+-rw-r--r--   0        0        0        0 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/visAnalysis/__init__.py
+-rw-r--r--   0        0        0    17951 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
+-rw-r--r--   0        0        0    11782 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
+-rw-r--r--   0        0        0    13749 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
+-rw-r--r--   0        0        0     3882 2024-05-21 11:44:05.605944 covdrugsim-1.0.9/tests/test_covdrugsim.py
+-rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 covdrugsim-1.0.9/PKG-INFO
```

### Comparing `covdrugsim-1.0.8/LICENSE` & `covdrugsim-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/README.md` & `covdrugsim-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/pyproject.toml` & `covdrugsim-1.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "covdrugsim"
-version = "1.0.8"
+version = "1.0.9"
 description = "Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/covdrugsim"
 repository = "https://github.com/Jon-Ting/covdrugsim"
 documentation = "https://covdrugsim.readthedocs.io/en/latest/"
```

### Comparing `covdrugsim-1.0.8/setup.py` & `covdrugsim-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="covdrugsim",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `covdrugsim-1.0.8/src/covdrugsim/__init__.py` & `covdrugsim-1.0.9/src/covdrugsim/__init__.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/data/energyLevellerExample.inp` & `covdrugsim-1.0.9/src/covdrugsim/data/energyLevellerExample.inp`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/data/exampleGaussianOutputs/example1.out` & `covdrugsim-1.0.9/src/covdrugsim/data/exampleGaussianOutputs/example1.out`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/data/exampleGaussianOutputs/example2.out` & `covdrugsim-1.0.9/src/covdrugsim/data/exampleGaussianOutputs/example2.out`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/data/exampleGaussianOutputs/example3.out` & `covdrugsim-1.0.9/src/covdrugsim/data/exampleGaussianOutputs/example3.out`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/data/exampleXYZs/example1.xyz` & `covdrugsim-1.0.9/src/covdrugsim/data/exampleXYZs/example1.xyz`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/data/exampleXYZs/example2.xyz` & `covdrugsim-1.0.9/src/covdrugsim/data/exampleXYZs/example2.xyz`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/data/exampleXYZs/example3.xyz` & `covdrugsim-1.0.9/src/covdrugsim/data/exampleXYZs/example3.xyz`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/datasets.py` & `covdrugsim-1.0.9/src/covdrugsim/datasets.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/mdsim/SCbondDist.py` & `covdrugsim-1.0.9/src/covdrugsim/mdsim/SCbondDist.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/mdsim/baseID.py` & `covdrugsim-1.0.9/src/covdrugsim/mdsim/baseID.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/mdsim/bbRMSD.py` & `covdrugsim-1.0.9/src/covdrugsim/mdsim/bbRMSD.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/mdsim/hbondAnalysis.py` & `covdrugsim-1.0.9/src/covdrugsim/mdsim/hbondAnalysis.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/mdsim/ligDihedral.py` & `covdrugsim-1.0.9/src/covdrugsim/mdsim/ligDihedral.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/mdsim/mdAnalyse.py` & `covdrugsim-1.0.9/src/covdrugsim/mdsim/mdAnalyse.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/mdsim/prepMTB.py` & `covdrugsim-1.0.9/src/covdrugsim/mdsim/prepMTB.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/qmcalc/admin.py` & `covdrugsim-1.0.9/src/covdrugsim/qmcalc/admin.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/qmcalc/constants.py` & `covdrugsim-1.0.9/src/covdrugsim/qmcalc/constants.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/qmcalc/genScripts.py` & `covdrugsim-1.0.9/src/covdrugsim/qmcalc/genScripts.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/qmcalc/gsub.sh` & `covdrugsim-1.0.9/src/covdrugsim/qmcalc/gsub.sh`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/qmcalc/tabulate.py` & `covdrugsim-1.0.9/src/covdrugsim/qmcalc/tabulate.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/qmcalc/unitConv.py` & `covdrugsim-1.0.9/src/covdrugsim/qmcalc/unitConv.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py` & `covdrugsim-1.0.9/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py` & `covdrugsim-1.0.9/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py` & `covdrugsim-1.0.9/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/tests/test_covdrugsim.py` & `covdrugsim-1.0.9/tests/test_covdrugsim.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-1.0.8/PKG-INFO` & `covdrugsim-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covdrugsim
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs.
 Home-page: https://github.com/Jon-Ting/covdrugsim
 License: MIT
 Keywords: covalent,drug,quantum,mechanic,molecular,dynamics,simulation
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
```

