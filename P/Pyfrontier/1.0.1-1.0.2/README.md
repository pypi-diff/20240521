# Comparing `tmp/Pyfrontier-1.0.1.tar.gz` & `tmp/pyfrontier-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyfrontier-1.0.1.tar", last modified: Mon Mar 25 14:43:02 2024, max compression
+gzip compressed data, was "pyfrontier-1.0.2.tar", last modified: Tue May 21 09:55:59 2024, max compression
```

## Comparing `Pyfrontier-1.0.1.tar` & `pyfrontier-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-03-25 14:43:02.586199 Pyfrontier-1.0.1/
--rw-r--r--   0 morinibu   (501) staff       (20)     1065 2022-07-03 08:51:57.000000 Pyfrontier-1.0.1/LICENSE
--rw-r--r--   0 morinibu   (501) staff       (20)     2739 2024-03-25 14:43:02.585961 Pyfrontier-1.0.1/PKG-INFO
--rwxr-xr-x   0 morinibu   (501) staff       (20)     1732 2024-03-25 14:41:24.000000 Pyfrontier-1.0.1/README.md
--rw-r--r--   0 morinibu   (501) staff       (20)      101 2022-09-03 03:56:55.000000 Pyfrontier-1.0.1/pyproject.toml
--rwxrwxrwx   0 morinibu   (501) staff       (20)       73 2024-03-25 14:43:02.587065 Pyfrontier-1.0.1/setup.cfg
--rwxr-xr-x   0 morinibu   (501) staff       (20)     1830 2024-03-25 14:41:24.000000 Pyfrontier-1.0.1/setup.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-03-25 14:43:02.568608 Pyfrontier-1.0.1/src/
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-03-25 14:43:02.572143 Pyfrontier-1.0.1/src/Pyfrontier/
--rwxrwxrwx   0 morinibu   (501) staff       (20)       22 2022-09-10 11:40:40.000000 Pyfrontier-1.0.1/src/Pyfrontier/__init__.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-03-25 14:43:02.579425 Pyfrontier-1.0.1/src/Pyfrontier/domain/
--rw-r--r--   0 morinibu   (501) staff       (20)      538 2024-03-25 14:38:39.000000 Pyfrontier-1.0.1/src/Pyfrontier/domain/__init__.py
--rw-r--r--   0 morinibu   (501) staff       (20)      300 2022-08-07 01:54:52.000000 Pyfrontier-1.0.1/src/Pyfrontier/domain/assurance_region.py
--rw-r--r--   0 morinibu   (501) staff       (20)     1030 2024-03-25 14:39:17.000000 Pyfrontier-1.0.1/src/Pyfrontier/domain/dmu.py
--rw-r--r--   0 morinibu   (501) staff       (20)        0 2022-07-30 13:18:39.000000 Pyfrontier-1.0.1/src/Pyfrontier/domain/metrics.py
--rw-r--r--   0 morinibu   (501) staff       (20)     1162 2024-03-25 13:01:55.000000 Pyfrontier-1.0.1/src/Pyfrontier/domain/parallel.py
--rw-r--r--   0 morinibu   (501) staff       (20)     1749 2022-09-10 07:49:12.000000 Pyfrontier-1.0.1/src/Pyfrontier/domain/result.py
--rw-r--r--   0 morinibu   (501) staff       (20)      973 2024-03-25 13:01:55.000000 Pyfrontier-1.0.1/src/Pyfrontier/domain/slack_weight.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-03-25 14:43:02.582133 Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/
--rw-r--r--   0 morinibu   (501) staff       (20)      274 2022-08-11 05:33:06.000000 Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/__init__.py
--rw-r--r--   0 morinibu   (501) staff       (20)     1946 2024-03-25 13:01:55.000000 Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/_additive_dea.py
--rw-r--r--   0 morinibu   (501) staff       (20)      684 2022-08-07 04:47:01.000000 Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/_base.py
--rw-r--r--   0 morinibu   (501) staff       (20)     6580 2024-03-25 14:40:36.000000 Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/_dea.py
--rw-r--r--   0 morinibu   (501) staff       (20)      733 2022-08-07 05:04:34.000000 Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/_hierarchical_dea.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-03-25 14:43:02.584443 Pyfrontier-1.0.1/src/Pyfrontier/solver/
--rw-r--r--   0 morinibu   (501) staff       (20)      252 2022-08-11 05:33:06.000000 Pyfrontier-1.0.1/src/Pyfrontier/solver/__init__.py
--rw-r--r--   0 morinibu   (501) staff       (20)     2734 2024-03-25 13:01:55.000000 Pyfrontier-1.0.1/src/Pyfrontier/solver/_additive_solver.py
--rw-r--r--   0 morinibu   (501) staff       (20)      789 2022-08-06 02:21:59.000000 Pyfrontier-1.0.1/src/Pyfrontier/solver/_base.py
--rw-r--r--   0 morinibu   (501) staff       (20)     7832 2024-03-25 13:01:55.000000 Pyfrontier-1.0.1/src/Pyfrontier/solver/_envelope_solver.py
--rw-r--r--   0 morinibu   (501) staff       (20)     4607 2024-03-25 13:01:55.000000 Pyfrontier-1.0.1/src/Pyfrontier/solver/_multiple_solver.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-03-25 14:43:02.585156 Pyfrontier-1.0.1/src/Pyfrontier.egg-info/
--rw-r--r--   0 morinibu   (501) staff       (20)     2739 2024-03-25 14:43:02.000000 Pyfrontier-1.0.1/src/Pyfrontier.egg-info/PKG-INFO
--rw-r--r--   0 morinibu   (501) staff       (20)      954 2024-03-25 14:43:02.000000 Pyfrontier-1.0.1/src/Pyfrontier.egg-info/SOURCES.txt
--rw-r--r--   0 morinibu   (501) staff       (20)        1 2024-03-25 14:43:02.000000 Pyfrontier-1.0.1/src/Pyfrontier.egg-info/dependency_links.txt
--rw-r--r--   0 morinibu   (501) staff       (20)        0 2022-08-01 11:27:37.000000 Pyfrontier-1.0.1/src/Pyfrontier.egg-info/not-zip-safe
--rw-r--r--   0 morinibu   (501) staff       (20)       24 2024-03-25 14:43:02.000000 Pyfrontier-1.0.1/src/Pyfrontier.egg-info/requires.txt
--rw-r--r--   0 morinibu   (501) staff       (20)       11 2024-03-25 14:43:02.000000 Pyfrontier-1.0.1/src/Pyfrontier.egg-info/top_level.txt
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-05-21 09:55:59.093530 pyfrontier-1.0.2/
+-rw-r--r--   0 morinibu   (501) staff       (20)     1065 2022-07-03 08:51:57.000000 pyfrontier-1.0.2/LICENSE
+-rw-r--r--   0 morinibu   (501) staff       (20)     2669 2024-05-21 09:55:59.093268 pyfrontier-1.0.2/PKG-INFO
+-rwxr-xr-x   0 morinibu   (501) staff       (20)     1662 2024-05-21 08:58:26.000000 pyfrontier-1.0.2/README.md
+-rw-r--r--   0 morinibu   (501) staff       (20)      101 2022-09-03 03:56:55.000000 pyfrontier-1.0.2/pyproject.toml
+-rwxrwxrwx   0 morinibu   (501) staff       (20)       73 2024-05-21 09:55:59.094925 pyfrontier-1.0.2/setup.cfg
+-rwxr-xr-x   0 morinibu   (501) staff       (20)     1830 2024-05-21 08:58:03.000000 pyfrontier-1.0.2/setup.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-05-21 09:55:59.058646 pyfrontier-1.0.2/src/
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-05-21 09:55:59.062921 pyfrontier-1.0.2/src/Pyfrontier/
+-rwxrwxrwx   0 morinibu   (501) staff       (20)       22 2024-05-21 08:58:53.000000 pyfrontier-1.0.2/src/Pyfrontier/__init__.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-05-21 09:55:59.077502 pyfrontier-1.0.2/src/Pyfrontier/domain/
+-rw-r--r--   0 morinibu   (501) staff       (20)      538 2024-05-21 00:22:37.000000 pyfrontier-1.0.2/src/Pyfrontier/domain/__init__.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      300 2022-08-07 01:54:52.000000 pyfrontier-1.0.2/src/Pyfrontier/domain/assurance_region.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     1030 2024-05-21 00:22:37.000000 pyfrontier-1.0.2/src/Pyfrontier/domain/dmu.py
+-rw-r--r--   0 morinibu   (501) staff       (20)        0 2022-07-30 13:18:39.000000 pyfrontier-1.0.2/src/Pyfrontier/domain/metrics.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     1162 2024-03-25 13:01:55.000000 pyfrontier-1.0.2/src/Pyfrontier/domain/parallel.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     1797 2024-05-21 04:57:05.000000 pyfrontier-1.0.2/src/Pyfrontier/domain/result.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      973 2024-03-25 13:01:55.000000 pyfrontier-1.0.2/src/Pyfrontier/domain/slack_weight.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-05-21 09:55:59.083447 pyfrontier-1.0.2/src/Pyfrontier/frontier_model/
+-rw-r--r--   0 morinibu   (501) staff       (20)      274 2022-08-11 05:33:06.000000 pyfrontier-1.0.2/src/Pyfrontier/frontier_model/__init__.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     2044 2024-05-21 04:37:47.000000 pyfrontier-1.0.2/src/Pyfrontier/frontier_model/_additive_dea.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      684 2022-08-07 04:47:01.000000 pyfrontier-1.0.2/src/Pyfrontier/frontier_model/_base.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     6768 2024-05-21 04:37:29.000000 pyfrontier-1.0.2/src/Pyfrontier/frontier_model/_dea.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      733 2022-08-07 05:04:34.000000 pyfrontier-1.0.2/src/Pyfrontier/frontier_model/_hierarchical_dea.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-05-21 09:55:59.091128 pyfrontier-1.0.2/src/Pyfrontier/solver/
+-rw-r--r--   0 morinibu   (501) staff       (20)      252 2022-08-11 05:33:06.000000 pyfrontier-1.0.2/src/Pyfrontier/solver/__init__.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     2968 2024-05-21 03:39:32.000000 pyfrontier-1.0.2/src/Pyfrontier/solver/_additive_solver.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      789 2022-08-06 02:21:59.000000 pyfrontier-1.0.2/src/Pyfrontier/solver/_base.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     7458 2024-05-21 03:39:46.000000 pyfrontier-1.0.2/src/Pyfrontier/solver/_envelope_solver.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      807 2024-05-21 01:22:49.000000 pyfrontier-1.0.2/src/Pyfrontier/solver/_models.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     4554 2024-05-21 01:16:27.000000 pyfrontier-1.0.2/src/Pyfrontier/solver/_multiple_solver.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2024-05-21 09:55:59.092311 pyfrontier-1.0.2/src/Pyfrontier.egg-info/
+-rw-r--r--   0 morinibu   (501) staff       (20)     2669 2024-05-21 09:55:58.000000 pyfrontier-1.0.2/src/Pyfrontier.egg-info/PKG-INFO
+-rw-r--r--   0 morinibu   (501) staff       (20)      987 2024-05-21 09:55:58.000000 pyfrontier-1.0.2/src/Pyfrontier.egg-info/SOURCES.txt
+-rw-r--r--   0 morinibu   (501) staff       (20)        1 2024-05-21 09:55:58.000000 pyfrontier-1.0.2/src/Pyfrontier.egg-info/dependency_links.txt
+-rw-r--r--   0 morinibu   (501) staff       (20)        0 2022-08-01 11:27:37.000000 pyfrontier-1.0.2/src/Pyfrontier.egg-info/not-zip-safe
+-rw-r--r--   0 morinibu   (501) staff       (20)       24 2024-05-21 09:55:58.000000 pyfrontier-1.0.2/src/Pyfrontier.egg-info/requires.txt
+-rw-r--r--   0 morinibu   (501) staff       (20)       11 2024-05-21 09:55:58.000000 pyfrontier-1.0.2/src/Pyfrontier.egg-info/top_level.txt
```

### Comparing `Pyfrontier-1.0.1/LICENSE` & `pyfrontier-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Pyfrontier-1.0.1/PKG-INFO` & `pyfrontier-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyfrontier
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pyfrontier is a data envelopment analysis for Python user.
 Home-page: https://nibutake.github.io/PyDEA/index.html?
 Download-URL: https://github.com/NibuTake/PyDEA
 Author: Takeshi Morinibu
 Author-email: takeshi715tech@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
@@ -29,15 +29,15 @@
 
 <div align="center"><img src="./images/logo.png" height="200"/></div>
 
 [![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%20%7C3.11%20-blue)](https://codecov.io/gh/NibuTake/PyDEA)
 [![License](https://img.shields.io/github/license/NibuTake/PyDEA?color=blue)](LICENSE)
 [![codecov](https://codecov.io/gh/NibuTake/PyDEA/branch/main/graph/badge.svg?token=EL44JBAYOT)](https://codecov.io/gh/NibuTake/PyDEA)
 
-[Install](#installation) | [Tutorial](https://nibutake.github.io/PyDEA/tutorials/index.html#) | [Docs](https://nibutake.github.io/PyDEA/index.html) | [Contribution](./CONTRIBUTING.md)
+[Install](#installation)| [Docs](https://nibutake.github.io/PyDEA/index.html) | [Contribution](./CONTRIBUTING.md)
 
 Pyfrontier is a data envelopment analysis for Python user. Our main motivation is to encourage more people to use DEA effectively and contribute to the development of DEA field.
 
 ## Installation
 
 This module is provided by [PyPI](https://pypi.org/project/Pyfrontier/).
```

### Comparing `Pyfrontier-1.0.1/README.md` & `pyfrontier-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center"><img src="./images/logo.png" height="200"/></div>
 
 [![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%20%7C3.11%20-blue)](https://codecov.io/gh/NibuTake/PyDEA)
 [![License](https://img.shields.io/github/license/NibuTake/PyDEA?color=blue)](LICENSE)
 [![codecov](https://codecov.io/gh/NibuTake/PyDEA/branch/main/graph/badge.svg?token=EL44JBAYOT)](https://codecov.io/gh/NibuTake/PyDEA)
 
-[Install](#installation) | [Tutorial](https://nibutake.github.io/PyDEA/tutorials/index.html#) | [Docs](https://nibutake.github.io/PyDEA/index.html) | [Contribution](./CONTRIBUTING.md)
+[Install](#installation)| [Docs](https://nibutake.github.io/PyDEA/index.html) | [Contribution](./CONTRIBUTING.md)
 
 Pyfrontier is a data envelopment analysis for Python user. Our main motivation is to encourage more people to use DEA effectively and contribute to the development of DEA field.
 
 ## Installation
 
 This module is provided by [PyPI](https://pypi.org/project/Pyfrontier/).
```

### Comparing `Pyfrontier-1.0.1/setup.py` & `pyfrontier-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "Topic :: Software Development :: Libraries",
 ]
 
 
 setup(
     name="Pyfrontier",
     # version=Pyfrontier.__version__,
-    version="1.0.1",
+    version="1.0.2",
     license="MIT",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Takeshi Morinibu",
     author_email="takeshi715tech@gmail.com",
     url=URL,
```

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/domain/__init__.py` & `pyfrontier-1.0.2/src/Pyfrontier/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/domain/dmu.py` & `pyfrontier-1.0.2/src/Pyfrontier/domain/dmu.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/domain/parallel.py` & `pyfrontier-1.0.2/src/Pyfrontier/domain/parallel.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/domain/result.py` & `pyfrontier-1.0.2/src/Pyfrontier/domain/result.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     - x_slack:
     - y_slack:
     """
 
     score: float
     id: int
     dmu: DMU
-    weight: List[float]
+    weights: List[float]
     x_slack: List[float]
     y_slack: List[float]
 
     def __post_init__(self):
         pass
 
     @property
@@ -83,21 +83,23 @@
 class AdditiveResult(BaseResult):
     """
     - score: efficiency
     - id:
     - dmu:
     - x_slack:
     - y_slack:
+    - weights: lambda
     """
 
     score: float
     id: int
     dmu: DMU
     x_slack: List[float]
     y_slack: List[float]
+    weights: List[float]
 
     @property
     def is_efficient(self) -> bool:
         if np.sum(self.x_slack) + np.sum(self.y_slack) > 0:
             return False
         else:
             return True
```

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/domain/slack_weight.py` & `pyfrontier-1.0.2/src/Pyfrontier/domain/slack_weight.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/_additive_dea.py` & `pyfrontier-1.0.2/src/Pyfrontier/frontier_model/_additive_dea.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 from Pyfrontier.solver import AdditiveSolver
 
 
 class AdditiveDEA(BaseDataEnvelopmentAnalysis):
     """This is a envelop dea model.
 
     Args:
-        frontier (Literal["CRS", "VRS"]): CRS means constant returns to scale.
-        VRS means variable returns to scale.
+        frontier (Literal["CRS", "VRS", "IRS", "DRS"]): CRS means constant returns to scale. VRS means variable returns to scale. IRS means increasing returns to scale. DRS means decreasing returns to scale.
         n_jobs (int, optional): The number of parallel jobs to solve DMU programming.
     """
 
-    def __init__(self, frontier: Literal["CRS", "VRS"], n_jobs: int = 1):
+    def __init__(self, frontier: Literal["CRS", "VRS", "IRS", "DRS"], n_jobs: int = 1):
         self.frontier = frontier
         self.DMUs: Optional[DMUSet] = None
         self._result: List[AdditiveResult] = []
         self.n_jobs = NumberOfJobs(n_jobs).value
 
     def fit(
         self,
```

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/_base.py` & `pyfrontier-1.0.2/src/Pyfrontier/frontier_model/_base.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/_dea.py` & `pyfrontier-1.0.2/src/Pyfrontier/frontier_model/_dea.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from typing import List, Literal
 
 import numpy as np
 
-import multiprocessing
-
 from Pyfrontier.domain import AssuranceRegion, DMUSet, EnvelopResult, MultipleResult
 from Pyfrontier.domain.dmu import BooleanInput
 from Pyfrontier.domain.parallel import NumberOfJobs
 from Pyfrontier.frontier_model._base import BaseDataEnvelopmentAnalysis
 from Pyfrontier.solver import EnvelopeSolver, MultipleSolver
 
 
 class EnvelopDEA(BaseDataEnvelopmentAnalysis):
     """This is a envelop dea model.
 
     Args:
-        frontier (Literal["CRS", "VRS"]): CRS means constant returns to scale. VRS means variable returns to scale.
+        frontier (Literal["CRS", "VRS", "IRS", "DRS"]): CRS means constant returns to scale. VRS means variable returns to scale. IRS means increasing returns to scale. DRS means decreasing returns to scale.
         orient (Literal["in", "out"]): Input or output oriented model.
         super_efficiency (bool, optional): Whether to use super-efficiency. Defaults to False.
         n_jobs (int, optional): The number of parallel jobs to solve DMU programming.
     """
 
     def __init__(
         self,
-        frontier: Literal["CRS", "VRS"],
+        frontier: Literal["CRS", "VRS", "IRS", "DRS"],
         orient: Literal["in", "out"],
         super_efficiency: bool = False,
         n_jobs: int = 1,
     ):
         self.frontier = frontier
         self.orient = orient
         self.super_efficiency = BooleanInput(super_efficiency).value
@@ -75,22 +73,22 @@
         return self.result
 
 
 class MultipleDEA(BaseDataEnvelopmentAnalysis):
     """This is a multiplier dea model.
 
     Args:
-        frontier (Literal["CRS", "VRS"]): CRS means constant returns to scale. VRS means variable returns to scale.
+        frontier (Literal["CRS", "VRS", "IRS", "DRS"]): CRS means constant returns to scale. VRS means variable returns to scale. IRS means increasing returns to scale. DRS means decreasing returns to scale.
         orient (Literal["in", "out"]): Input or output oriented model.
         n_jobs (int, optional): The number of parallel jobs to solve DMU programming.
     """
 
     def __init__(
         self,
-        frontier: Literal["CRS", "VRS"],
+        frontier: Literal["CRS", "VRS", "IRS", "DRS"],
         orient: Literal["in", "out"],
         n_jobs: int = 1,
     ):
         self.frontier = frontier
         self.orient = orient
         self.DMUs = None
         self.result: List[MultipleResult] = []
```

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/frontier_model/_hierarchical_dea.py` & `pyfrontier-1.0.2/src/Pyfrontier/frontier_model/_hierarchical_dea.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/solver/_additive_solver.py` & `pyfrontier-1.0.2/src/Pyfrontier/solver/_additive_solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from Pyfrontier.domain import MultiProcessor
 from Pyfrontier.solver._base import BaseSolver
 
 
 class AdditiveSolver(BaseSolver):
     def __init__(
         self,
-        frontier: Optional[Literal["CRS", "VRS"]],
+        frontier: Literal["CRS", "VRS", "IRS", "DRS"],
         DMUs: DMUSet,
         x_weight: np.ndarray,
         y_weight: np.ndarray,
         n_jobs: int = 1,
     ) -> None:
         self.x_weight = x_weight
         self.y_weight = y_weight
@@ -50,14 +50,18 @@
             problem += (
                 pulp.lpDot(lambda_N, self.DMUs.outputs[:, r]) - sy[r]
                 >= self.DMUs.outputs[o, r]
             )
 
         if self.frontier == "VRS":
             problem += np.sum(lambda_N) == 1
+        elif self.frontier == "IRS":
+            problem += np.sum(lambda_N) >= 1
+        elif self.frontier == "DRS":
+            problem += np.sum(lambda_N) <= 1
 
         return problem
 
     def _solve_problem(self, o: int) -> AdditiveResult:
         # Define variables.
         sx = self._dict_to_list(
             pulp.LpVariable.dicts(
@@ -79,8 +83,9 @@
 
         return AdditiveResult(
             score=np.nan,
             id=o,
             dmu=DMU(self.DMUs.inputs[o], self.DMUs.outputs[o], self.DMUs.get_id(o)),
             x_slack=[self._rounder(i.value()) for i in sx],
             y_slack=[self._rounder(r.value()) for r in sy],
+            weights=[self._rounder(n.value()) for n in lambda_N],
         )
```

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/solver/_base.py` & `pyfrontier-1.0.2/src/Pyfrontier/solver/_base.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/solver/_envelope_solver.py` & `pyfrontier-1.0.2/src/Pyfrontier/solver/_envelope_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import List, Tuple, Union
+from typing import List, Literal, Tuple, Union
 
 import numpy as np
 import pulp
 
-import multiprocessing
 
 from Pyfrontier.domain import DMU, DMUSet, EnvelopResult
 from Pyfrontier.domain import MultiProcessor
 from Pyfrontier.solver._base import BaseSolver
 
 
 class EnvelopeSolver(BaseSolver):
@@ -17,16 +16,16 @@
         orient (str): [description]
         frontier (str): [description]
         DMUs ([type]): [description]
     """
 
     def __init__(
         self,
-        orient: str,
-        frontier: str,
+        orient: Literal["in", "out"],
+        frontier: Literal["CRS", "VRS", "IRS", "DRS"],
         DMUs: DMUSet,
         uncontrollable_index: List[int] = [],
         is_super_efficiency: bool = False,
         n_jobs: int = 1,
     ):
         self.orient = orient
         self.DMUs = DMUs
@@ -35,31 +34,14 @@
         self._is_super_efficiency = is_super_efficiency
         self.n_jobs = n_jobs
 
     def apply(self) -> List[EnvelopResult]:
         processor = MultiProcessor(self._solve_problem, self.DMUs.N)
         return processor.solve(self.n_jobs)
 
-        if self.n_jobs <= 1:
-            return [self._solve_problem(j) for j in range(self.DMUs.N)]
-        else:
-            # faster than problem.solve(pulp.PULP_CBC_CMD(threads=self.n_jobs))
-            pool = multiprocessing.Pool(self.n_jobs)
-
-            problem_processes = []
-            for j in range(self.DMUs.N):
-                problem_processes.append(
-                    pool.apply_async(self._solve_problem, args=(j,))
-                )
-
-            pool.close()
-            pool.join()
-
-            return [problem.get() for problem in problem_processes]
-
     def _redefine_theta_i(
         self, i: int, theta: pulp.LpVariable
     ) -> Union[int, pulp.LpVariable]:
         if i in self._uncontrollable_index:
             return 1
         else:
             return theta
@@ -132,23 +114,27 @@
         if self.orient == "in":
             problem = self._define_input_orient_problem(o, lambda_N, theta)
         else:
             problem = self._define_output_orient_problem(o, lambda_N, theta)
 
         if self.frontier == "VRS":
             problem += np.sum(lambda_N) == 1
+        elif self.frontier == "IRS":
+            problem += np.sum(lambda_N) >= 1
+        elif self.frontier == "DRS":
+            problem += np.sum(lambda_N) <= 1
 
         problem.solve()
 
         score = self._rounder(problem.objective.value())
         sx, sy = self._optimize_slack(score, o)
 
         return EnvelopResult(
             score=self._rounder(problem.objective.value()),
-            weight=[self._rounder(n.value()) for n in lambda_N],
+            weights=[self._rounder(n.value()) for n in lambda_N],
             id=o,
             x_slack=sx,
             y_slack=sy,
             dmu=DMU(self.DMUs.inputs[o], self.DMUs.outputs[o], self.DMUs.get_id(o)),
         )
 
     def _optimize_slack(self, theta: float, o: int) -> Tuple[list, list]:
```

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier/solver/_multiple_solver.py` & `pyfrontier-1.0.2/src/Pyfrontier/solver/_multiple_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from typing import List, Union
+from typing import List, Literal, Union
 
 import pulp
 
 from Pyfrontier.domain import AssuranceRegion, DMUSet, MultipleResult
 from Pyfrontier.domain.dmu import DMU
 from Pyfrontier.domain import MultiProcessor
 from Pyfrontier.solver._base import BaseSolver
+from Pyfrontier.solver._models import Bias
 
 
 class MultipleSolver(BaseSolver):
     """AI is creating summary for __init__
 
     Args:
         orient (str): [description]
         frontier (str): [description]
         DMUs ([type]): [description]
     """
 
     def __init__(
         self,
-        orient: str,
-        frontier: str,
+        orient: Literal["in", "out"],
+        frontier: Literal["CRS", "VRS", "IRS", "DRS"],
         DMUs: DMUSet,
         assurance_region: List[AssuranceRegion],
         bound: float = 0.0,
         n_jobs: int = 1,
     ):
         self.orient = orient
         self.DMUs = DMUs
@@ -33,20 +34,14 @@
         self.bound = bound
         self.n_jobs = n_jobs
 
     def apply(self) -> List[MultipleResult]:
         processor = MultiProcessor(self._solve_problem, self.DMUs.N)
         return processor.solve(self.n_jobs)
 
-    def _define_bias(self) -> Union[pulp.LpVariable, int]:
-        if self.frontier == "VRS":
-            return pulp.LpVariable("bias")
-        else:
-            return 0
-
     def _define_input_oriented_problem(
         self, bias: Union[pulp.LpVariable, int], mu: list, nu: list, o: int
     ) -> pulp.LpProblem:
         problem = pulp.LpProblem(
             self.orient + str(o), pulp.LpMaximize
         )  # avoid repeated name
         problem += pulp.lpDot(mu, self.DMUs.outputs[o, :]) + bias
@@ -82,15 +77,15 @@
         # Define variables.
         mu = self._dict_to_list(
             pulp.LpVariable.dicts("Mu", range(self.DMUs.s), lowBound=self.bound)
         )
         nu = self._dict_to_list(
             pulp.LpVariable.dicts("Nu", range(self.DMUs.m), lowBound=self.bound)
         )
-        bias = self._define_bias()
+        bias = Bias(self.frontier, self.orient).value
 
         # Problem.
         if self.orient == "in":
             problem = self._define_input_oriented_problem(bias, mu, nu, o)
         else:
             problem = self._define_output_oriented_problem(bias, mu, nu, o)
```

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier.egg-info/PKG-INFO` & `pyfrontier-1.0.2/src/Pyfrontier.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyfrontier
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pyfrontier is a data envelopment analysis for Python user.
 Home-page: https://nibutake.github.io/PyDEA/index.html?
 Download-URL: https://github.com/NibuTake/PyDEA
 Author: Takeshi Morinibu
 Author-email: takeshi715tech@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
@@ -29,15 +29,15 @@
 
 <div align="center"><img src="./images/logo.png" height="200"/></div>
 
 [![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%20%7C3.11%20-blue)](https://codecov.io/gh/NibuTake/PyDEA)
 [![License](https://img.shields.io/github/license/NibuTake/PyDEA?color=blue)](LICENSE)
 [![codecov](https://codecov.io/gh/NibuTake/PyDEA/branch/main/graph/badge.svg?token=EL44JBAYOT)](https://codecov.io/gh/NibuTake/PyDEA)
 
-[Install](#installation) | [Tutorial](https://nibutake.github.io/PyDEA/tutorials/index.html#) | [Docs](https://nibutake.github.io/PyDEA/index.html) | [Contribution](./CONTRIBUTING.md)
+[Install](#installation)| [Docs](https://nibutake.github.io/PyDEA/index.html) | [Contribution](./CONTRIBUTING.md)
 
 Pyfrontier is a data envelopment analysis for Python user. Our main motivation is to encourage more people to use DEA effectively and contribute to the development of DEA field.
 
 ## Installation
 
 This module is provided by [PyPI](https://pypi.org/project/Pyfrontier/).
```

### Comparing `Pyfrontier-1.0.1/src/Pyfrontier.egg-info/SOURCES.txt` & `pyfrontier-1.0.2/src/Pyfrontier.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 src/Pyfrontier/frontier_model/_base.py
 src/Pyfrontier/frontier_model/_dea.py
 src/Pyfrontier/frontier_model/_hierarchical_dea.py
 src/Pyfrontier/solver/__init__.py
 src/Pyfrontier/solver/_additive_solver.py
 src/Pyfrontier/solver/_base.py
 src/Pyfrontier/solver/_envelope_solver.py
+src/Pyfrontier/solver/_models.py
 src/Pyfrontier/solver/_multiple_solver.py
```

