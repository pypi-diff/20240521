# Comparing `tmp/pyquickbench-0.2.1.tar.gz` & `tmp/pyquickbench-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquickbench-0.2.1.tar", last modified: Wed Apr 10 21:01:32 2024, max compression
+gzip compressed data, was "pyquickbench-0.2.2.tar", last modified: Tue May 21 16:20:14 2024, max compression
```

## Comparing `pyquickbench-0.2.1.tar` & `pyquickbench-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-04-10 21:01:32.699876 pyquickbench-0.2.1/
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     1326 2023-02-10 09:29:15.000000 pyquickbench-0.2.1/LICENSE
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     6278 2024-04-10 21:01:32.694675 pyquickbench-0.2.1/PKG-INFO
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     2785 2024-02-08 13:53:18.000000 pyquickbench-0.2.1/README.md
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     1860 2024-04-10 20:39:14.000000 pyquickbench-0.2.1/pyproject.toml
-drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-04-10 21:01:32.590066 pyquickbench-0.2.1/pyquickbench/
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3866 2024-04-10 20:59:03.000000 pyquickbench-0.2.1/pyquickbench/__init__.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)    50575 2024-04-10 20:45:31.000000 pyquickbench-0.2.1/pyquickbench/_benchmark.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3966 2024-04-10 20:41:22.000000 pyquickbench-0.2.1/pyquickbench/_defaults.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     8514 2024-04-10 17:43:44.000000 pyquickbench-0.2.1/pyquickbench/_time_train.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)    17042 2024-04-10 17:43:11.000000 pyquickbench-0.2.1/pyquickbench/_utils.py
-drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-04-10 21:01:32.687987 pyquickbench-0.2.1/pyquickbench.egg-info/
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     6278 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/PKG-INFO
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)      444 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/SOURCES.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)        1 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/dependency_links.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)      260 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/requires.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)       13 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/top_level.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)      183 2024-01-18 10:03:43.000000 pyquickbench-0.2.1/requirements-docs.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)       25 2024-01-04 08:26:02.000000 pyquickbench-0.2.1/requirements-tests.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)       32 2024-01-10 08:42:41.000000 pyquickbench-0.2.1/requirements.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)       38 2024-04-10 21:01:32.700391 pyquickbench-0.2.1/setup.cfg
-drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-04-10 21:01:32.673478 pyquickbench-0.2.1/tests/
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     2886 2024-01-30 15:39:33.000000 pyquickbench-0.2.1/tests/test_config.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3400 2024-03-12 21:59:12.000000 pyquickbench-0.2.1/tests/test_simple.py
+drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-05-21 16:20:14.594988 pyquickbench-0.2.2/
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     1326 2023-02-10 09:29:15.000000 pyquickbench-0.2.2/LICENSE
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     6278 2024-05-21 16:20:14.594988 pyquickbench-0.2.2/PKG-INFO
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     2785 2024-05-21 15:22:36.000000 pyquickbench-0.2.2/README.md
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     1860 2024-05-21 16:19:43.000000 pyquickbench-0.2.2/pyproject.toml
+drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-05-21 16:20:14.521934 pyquickbench-0.2.2/pyquickbench/
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3885 2024-05-21 16:18:42.000000 pyquickbench-0.2.2/pyquickbench/__init__.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)    50566 2024-05-10 10:00:11.000000 pyquickbench-0.2.2/pyquickbench/_benchmark.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     4248 2024-05-21 16:18:42.000000 pyquickbench-0.2.2/pyquickbench/_defaults.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)    11956 2024-05-21 16:18:42.000000 pyquickbench-0.2.2/pyquickbench/_time_train.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)    17063 2024-05-17 09:31:06.000000 pyquickbench-0.2.2/pyquickbench/_utils.py
+drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-05-21 16:20:14.594988 pyquickbench-0.2.2/pyquickbench.egg-info/
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     6278 2024-05-21 16:20:14.000000 pyquickbench-0.2.2/pyquickbench.egg-info/PKG-INFO
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)      444 2024-05-21 16:20:14.000000 pyquickbench-0.2.2/pyquickbench.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)        1 2024-05-21 16:20:14.000000 pyquickbench-0.2.2/pyquickbench.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)      260 2024-05-21 16:20:14.000000 pyquickbench-0.2.2/pyquickbench.egg-info/requires.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)       13 2024-05-21 16:20:14.000000 pyquickbench-0.2.2/pyquickbench.egg-info/top_level.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)      183 2024-05-17 10:17:42.000000 pyquickbench-0.2.2/requirements-docs.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)       25 2024-01-04 08:26:02.000000 pyquickbench-0.2.2/requirements-tests.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)       32 2024-01-10 08:42:41.000000 pyquickbench-0.2.2/requirements.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)       38 2024-05-21 16:20:14.594988 pyquickbench-0.2.2/setup.cfg
+drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-05-21 16:20:14.583810 pyquickbench-0.2.2/tests/
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     2886 2024-01-30 15:39:33.000000 pyquickbench-0.2.2/tests/test_config.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3400 2024-03-12 21:59:12.000000 pyquickbench-0.2.2/tests/test_simple.py
```

### Comparing `pyquickbench-0.2.1/LICENSE` & `pyquickbench-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquickbench-0.2.1/PKG-INFO` & `pyquickbench-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquickbench
-Version: 0.2.1
+Version: 0.2.2
 Summary: A pure Pyton tool to perform time and accuracy benchmarks
 Author-email: Gabriel Fougeron <gabriel.fougeron@hotmail.fr>
 License: BSD 2-Clause License
         
         Copyright (c) 2021, Gabriel Fougeron
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyquickbench Version: 0.2.1 Summary: A pure Pyton
+Metadata-Version: 2.1 Name: pyquickbench Version: 0.2.2 Summary: A pure Pyton
 tool to perform time and accuracy benchmarks Author-email: Gabriel Fougeron
 hotmail.fr> License: BSD 2-Clause License Copyright (c) 2021, Gabriel Fougeron
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
```

### Comparing `pyquickbench-0.2.1/README.md` & `pyquickbench-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyquickbench-0.2.1/pyproject.toml` & `pyquickbench-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "build",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyquickbench"
-version = "0.2.1"
+version = "0.2.2"
 description = "A pure Pyton tool to perform time and accuracy benchmarks"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["Python", "benchmark"]
 authors = [
   {name = "Gabriel Fougeron", email = "gabriel.fougeron@hotmail.fr"},
 ]
```

### Comparing `pyquickbench-0.2.1/pyquickbench/__init__.py` & `pyquickbench-0.2.2/pyquickbench/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 .. autosummary::
    :toctree: generated/
    :nosignatures:
    :recursive:
 
    TimeTrain
    TimeTrain.toc
+   TimeTrain.tictoc
    TimeTrain.to_dict
    
 =========
 Constants
 =========
 
 A few named constants and default values in :mod:`pyquickbench`.
@@ -115,15 +116,15 @@
 
 all_transforms = all_transforms
 """Available data transformations.
 
    List of all available data transformations to be used in :func:`pyquickbench.plot_benchmark`.
 
    * "pol_growth_order"  : Plots an estimate of :math:`\\alpha` based on consecutive measured values if the data scales as :math:`\\approx n^\\alpha`.
-   * "pol_cvgence_order" :  Plots an estimate of :math:`\\alpha` based on consecutive measured values if the data scales as :math:`\\approx n^{-\\alpha}`.
+   * "pol_cvgence_order" : Plots an estimate of :math:`\\alpha` based on consecutive measured values if the data scales as :math:`\\approx n^{-\\alpha}`.
 
    See :ref:`sphx_glr__build_auto_examples_tutorial_06-Transforming_values.py` for usage example.
 
    .. rubric:: See Also
 
    * :func:`pyquickbench.plot_benchmark` : Plot benchmarks
```

### Comparing `pyquickbench-0.2.1/pyquickbench/_benchmark.py` & `pyquickbench-0.2.2/pyquickbench/_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import math
 import itertools
 import typing
 import warnings
-import multiprocessing
-
+    
 import numpy as np
 import numpy.typing
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import matplotlib.figure
 import tqdm
 import tqdm.notebook
@@ -74,17 +73,14 @@
     setup : callable, optional
         Function that prepares the inputs for the functions to be benchmarked.\n
         See :ref:`sphx_glr__build_auto_examples_tutorial_03-Preparing_inputs.py` for usage example.\n
         By default ``lambda n: {pyquickbench.default_ax_name: n}``.
     n_repeat : int, optional
         Number of times to repeat the benchmark for variability studies.\n
         By default ``1``.
-    n_repeat : int, optional
-        Length of function output.\n
-        By default ``1``.
     nproc : int, optional
         Number of workers in PoolExecutor.\n
         By default :func:`python:multiprocessing.cpu_count()`.
     pooltype : str, optional
         Type of PoolExecutor.\n
         Possible values: ``"phony"``, ``"thread"`` or ``"process"``.\n  
         By default ``"phony"``.
@@ -195,15 +191,18 @@
         if pooltype ==  None:
             if nproc is None:
                 pooltype = "phony"
             else:
                 pooltype = "process"                
         else:
             if nproc is None:
-                nproc = multiprocessing.cpu_count()
+                if MULTIPROCESSING_AVAILABLE:
+                    nproc = multiprocessing.cpu_count()
+                else:
+                    nproc = 1
                     
         try:
             PoolExecutor = AllPoolExecutors[pooltype]
         except KeyError:
             raise ValueError(f"Unknown pooltype {pooltype}. Available pootypes: {list(AllPoolExecutors.keys())}")
                     
         if mode == "timings":
```

### Comparing `pyquickbench-0.2.1/pyquickbench/_defaults.py` & `pyquickbench-0.2.2/pyquickbench/_defaults.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 import matplotlib as mpl
 import numpy as np
+try:
+    import multiprocessing
+    import _multiprocessing
+    import concurrent.futures
+    MULTIPROCESSING_AVAILABLE = True
+except:
+    MULTIPROCESSING_AVAILABLE = False
 
 default_ax_name = "n"
 fun_ax_name = "function"
 repeat_ax_name = "repeat"
 out_ax_name = "out"
 
 default_color_list = list(mpl.colors.TABLEAU_COLORS)
@@ -129,8 +136,14 @@
 ]
 
 all_plot_intents.extend([f'reduction_{name}' for name in all_reductions])
 
 all_transforms = [
     'pol_growth_order'  ,
     'pol_cvgence_order' ,
-]
+]
+
+tictoc_sync_name = "pyquickbench_sync"
+
+default_TimeTrain_ignore_names = set((
+    tictoc_sync_name    ,
+))
```

### Comparing `pyquickbench-0.2.1/pyquickbench/_utils.py` & `pyquickbench-0.2.2/pyquickbench/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import timeit
 import math
 import inspect
-import concurrent.futures
 import copy
 import itertools
 
 import numpy as np
 
 from pyquickbench._defaults import *
 from pyquickbench._time_train import TimeTrain
@@ -391,18 +390,20 @@
         pass
     
     def submit(self, fn, *args):
         return FakeFuture(fn, *args)
 
 AllPoolExecutors = {
     "phony"         :   PhonyProcessPoolExecutor                ,
-    "thread"        :   concurrent.futures.ThreadPoolExecutor   ,
-    "process"       :   concurrent.futures.ProcessPoolExecutor  ,
 }
 
+if MULTIPROCESSING_AVAILABLE:
+    AllPoolExecutors["thread"] = concurrent.futures.ThreadPoolExecutor
+    AllPoolExecutors["process"] = concurrent.futures.ProcessPoolExecutor
+    
 def _values_reduction(all_vals, idx_vals, idx_points, idx_all_reduction):
 
     idx_vals = idx_vals.copy()
     idx_vals[idx_points] = slice(None)
 
     idx_to_reduction = {idx_points:"points"}
```

### Comparing `pyquickbench-0.2.1/pyquickbench.egg-info/PKG-INFO` & `pyquickbench-0.2.2/pyquickbench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquickbench
-Version: 0.2.1
+Version: 0.2.2
 Summary: A pure Pyton tool to perform time and accuracy benchmarks
 Author-email: Gabriel Fougeron <gabriel.fougeron@hotmail.fr>
 License: BSD 2-Clause License
         
         Copyright (c) 2021, Gabriel Fougeron
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyquickbench Version: 0.2.1 Summary: A pure Pyton
+Metadata-Version: 2.1 Name: pyquickbench Version: 0.2.2 Summary: A pure Pyton
 tool to perform time and accuracy benchmarks Author-email: Gabriel Fougeron
 hotmail.fr> License: BSD 2-Clause License Copyright (c) 2021, Gabriel Fougeron
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
```

### Comparing `pyquickbench-0.2.1/tests/test_config.py` & `pyquickbench-0.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyquickbench-0.2.1/tests/test_simple.py` & `pyquickbench-0.2.2/tests/test_simple.py`

 * *Files identical despite different names*

