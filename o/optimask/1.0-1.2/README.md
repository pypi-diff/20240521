# Comparing `tmp/optimask-1.0.tar.gz` & `tmp/optimask-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimask-1.0.tar", last modified: Sat Mar 16 21:48:52 2024, max compression
+gzip compressed data, was "optimask-1.2.tar", last modified: Tue May 21 14:31:13 2024, max compression
```

## Comparing `optimask-1.0.tar` & `optimask-1.2.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:48:52.601398 optimask-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-16 21:48:44.000000 optimask-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-16 21:48:52.601398 optimask-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-16 21:48:44.000000 optimask-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:48:52.601398 optimask-1.0/optimask/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-16 21:48:44.000000 optimask-1.0/optimask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-03-16 21:48:44.000000 optimask-1.0/optimask/_optimask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:48:52.601398 optimask-1.0/optimask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-16 21:48:52.000000 optimask-1.0/optimask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-16 21:48:52.000000 optimask-1.0/optimask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 21:48:52.000000 optimask-1.0/optimask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-16 21:48:52.000000 optimask-1.0/optimask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-16 21:48:52.000000 optimask-1.0/optimask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 21:48:52.601398 optimask-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-16 21:48:44.000000 optimask-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:31:13.729851 optimask-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 14:31:00.000000 optimask-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 14:31:00.000000 optimask-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-21 14:31:13.729851 optimask-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-21 14:31:00.000000 optimask-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:31:13.725851 optimask-1.2/optimask/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 14:31:00.000000 optimask-1.2/optimask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 14:31:00.000000 optimask-1.2/optimask/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-21 14:31:00.000000 optimask-1.2/optimask/_optimask.py
+-rw-r--r--   0 runner    (1001) docker     (127)   427048 2024-05-21 14:31:13.000000 optimask-1.2/optimask/optimask_cython.c
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-21 14:31:00.000000 optimask-1.2/optimask/optimask_cython.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:31:13.729851 optimask-1.2/optimask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:31:13.729851 optimask-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 14:31:00.000000 optimask-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:31:13.729851 optimask-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-21 14:31:00.000000 optimask-1.2/tests/test_optimask.py
```

### Comparing `optimask-1.0/LICENSE` & `optimask-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optimask-1.0/PKG-INFO` & `optimask-1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: optimask
-Version: 1.0
+Version: 1.2
 Summary: OptiMask: extracting the largest (non-contiguous) submatrix without NaN
 Home-page: https://github.com/CyrilJl/optimask
 Author: Cyril Joly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: cython
 
-# OptiMask: Efficient NaN Data Removal in Python
+# <img src="https://raw.githubusercontent.com/CyrilJl/OptiMask/main/docs/source/_static/icon.svg" alt="Logo OptiMask" width="35" height="35"> OptiMask: Efficient NaN Data Removal in Python
 
-[![PyPI Version](https://img.shields.io/pypi/v/optimask.svg)](https://pypi.org/project/optimask/)
+[![PyPI Version](https://img.shields.io/pypi/v/optimask.svg)](https://pypi.org/project/optimask/) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/optimask.svg)](https://anaconda.org/conda-forge/optimask)
 
 ## Introduction
 
 OptiMask is a Python package designed to facilitate the process of removing NaN (Not-a-Number) data from matrices while efficiently computing the largest (and not necessarily contiguous) submatrix without NaN values. This tool prioritizes practicality and compatibility with Numpy arrays and Pandas DataFrames.
 
 ## Key Features
 
@@ -29,14 +30,24 @@
 
 To employ OptiMask, install the `optimask` package via pip:
 
 ```bash
 pip install optimask
 ```
 
+OptiMask is also available on the conda-forge channel:
+
+```bash
+conda install -c conda-forge optimask
+```
+
+```bash
+mamba install optimask
+```
+
 ## Usage Example
 
 Import the `OptiMask` class from the `optimask` package and utilize its methods for efficient data masking:
 
 ```python
 from optimask import OptiMask
 import numpy as np
```

### Comparing `optimask-1.0/README.md` & `optimask-1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# OptiMask: Efficient NaN Data Removal in Python
+# <img src="https://raw.githubusercontent.com/CyrilJl/OptiMask/main/docs/source/_static/icon.svg" alt="Logo OptiMask" width="35" height="35"> OptiMask: Efficient NaN Data Removal in Python
 
-[![PyPI Version](https://img.shields.io/pypi/v/optimask.svg)](https://pypi.org/project/optimask/)
+[![PyPI Version](https://img.shields.io/pypi/v/optimask.svg)](https://pypi.org/project/optimask/) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/optimask.svg)](https://anaconda.org/conda-forge/optimask)
 
 ## Introduction
 
 OptiMask is a Python package designed to facilitate the process of removing NaN (Not-a-Number) data from matrices while efficiently computing the largest (and not necessarily contiguous) submatrix without NaN values. This tool prioritizes practicality and compatibility with Numpy arrays and Pandas DataFrames.
 
 ## Key Features
 
@@ -16,14 +16,24 @@
 
 To employ OptiMask, install the `optimask` package via pip:
 
 ```bash
 pip install optimask
 ```
 
+OptiMask is also available on the conda-forge channel:
+
+```bash
+conda install -c conda-forge optimask
+```
+
+```bash
+mamba install optimask
+```
+
 ## Usage Example
 
 Import the `OptiMask` class from the `optimask` package and utilize its methods for efficient data masking:
 
 ```python
 from optimask import OptiMask
 import numpy as np
```

### Comparing `optimask-1.0/optimask/_optimask.py` & `optimask-1.2/optimask/_optimask.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 """
 
 from typing import Tuple, Union
 
 import numpy as np
 import pandas as pd
 
+from ._misc import check_params, warning
+from .optimask_cython import groupby_max, is_decreasing, permutation_index
+
 __all__ = ["OptiMask"]
 
 
 class OptiMask:
     """
     OptiMask is a class for calculating the optimal rows and columns to retain in a 2D array or DataFrame
     to remove NaN values and preserve the maximum number of non-NaN cells.
@@ -46,155 +49,92 @@
         has_nan_values = np.isnan(data[rows][:, cols]).any()
 
         # Print or display the results
         print(f"Coverage Ratio: {coverage_ratio:.2f}, Has NaN Values: {has_nan_values}")
         # Output: Coverage Ratio: 0.85, Has NaN Values: False
     """
 
-    def __init__(self, n_tries=10, max_steps=32, random_state=None, verbose=False):
+    def __init__(self, n_tries=5, max_steps=32, random_state=None, verbose=False):
         self.n_tries = n_tries
         self.max_steps = max_steps
         self.random_state = random_state
         self.verbose = bool(verbose)
 
     def _verbose(self, msg):
-        """
-        Print verbose information if verbose is True.
-
-        Args:
-            msg (str): The message to print.
-        """
         if self.verbose:
-            print(msg)
-
-    @staticmethod
-    def _heights(df, axis=0):
-        """
-        Calculate heights along the specified axis.
-
-        Args:
-            df (pd.DataFrame): The DataFrame.
-            axis (int): The axis along which to calculate heights.
-
-        Returns:
-            np.ndarray: Heights along the specified axis.
-        """
-        return df.groupby(axis)[1 - axis].max().values + 1
+            warning(msg)
 
     @staticmethod
-    def _is_decreasing(x) -> bool:
-        return all(x[:-1] >= x[1:])
-
-    @classmethod
-    def _sort_by_na_max_index(cls, height) -> np.ndarray:
-        """
-        Sort array indices based on the maximum value of another array in descending order.
-
-        Args:
-            height (np.ndarray): The array to sort.
-
-        Returns:
-            np.ndarray: Sorted indices.
-        """
+    def _sort_by_na_max_index(height: np.ndarray) -> np.ndarray:
         return np.argsort(-height, kind='mergesort')
 
-    @classmethod
-    def _get_largest_rectangle(cls, heights, m, n):
+    @staticmethod
+    def _get_largest_rectangle(heights, m, n):
         areas = (m - heights) * (n - np.arange(len(heights)))
         i0 = np.argmax(areas)
         return i0, heights[i0], areas[i0]
 
-    @staticmethod
-    def _permutation_index(p):
-        inv = np.empty_like(p)
-        inv[p] = np.arange(len(inv), dtype=inv.dtype)
-        return inv
-
     @classmethod
     def _is_pareto_ordered(cls, hx, hy):
-        return cls._is_decreasing(hx) and cls._is_decreasing(hy)
+        return is_decreasing(hx) and is_decreasing(hy)
 
-    def _trial(self, rng, df, m, n, m_nan, n_nan):
-        """
-        Perform a single optimization trial.
-
-        Args:
-            rng (np.random.Generator): Random number generator.
-            df (pd.DataFrame): The DataFrame.
-            m (int): Total height of the input array.
-            n (int): Total width of the input array.
-            m_nan (int): Number of rows with NaN values.
-            n_nan (int): Number of columns with NaN values.
-
-        Returns:
-            Tuple[int, int, int, np.ndarray, np.ndarray]: Area, indices, and permutations.
-        """
+    def _trial(self, rng, m_nan, n_nan, iy, ix, m, n):
         p_rows = rng.permutation(m_nan)
         p_cols = rng.permutation(n_nan)
-
-        df_trial = pd.DataFrame()
-        df_trial[0] = self._permutation_index(p_rows)[df[0].values]
-        df_trial[1] = self._permutation_index(p_cols)[df[1].values]
+        iy_trial = permutation_index(p_rows)[iy]
+        ix_trial = permutation_index(p_cols)[ix]
 
         step = 0
-        heights = self._heights(df_trial, axis=0), self._heights(df_trial, axis=1)
-        while (not self._is_pareto_ordered(*heights)) and (step < self.max_steps):
+        h0, h1 = groupby_max(iy_trial, ix_trial, m_nan), groupby_max(ix_trial, iy_trial, n_nan)
+        while (not self._is_pareto_ordered(h0, h1)) and (step < self.max_steps):
             axis = (step % 2)
             step += 1
-            p_step = self._sort_by_na_max_index(heights[axis])
-            df_trial[axis] = self._permutation_index(p_step)[df_trial[axis].values]
             if axis == 0:
+                p_step = self._sort_by_na_max_index(h0)
+                iy_trial = permutation_index(p_step)[iy_trial]
                 p_rows = p_rows[p_step]
-                heights = (heights[0][p_step], self._heights(df_trial, axis=1))
+                h0, h1 = h0[p_step], groupby_max(ix_trial, iy_trial, n_nan)
             if axis == 1:
+                p_step = self._sort_by_na_max_index(h1)
+                ix_trial = permutation_index(p_step)[ix_trial]
                 p_cols = p_cols[p_step]
-                heights = (self._heights(df_trial, axis=0), heights[1][p_step])
+                h0, h1 = groupby_max(iy_trial, ix_trial, m_nan), h1[p_step]
 
-        if not self._is_pareto_ordered(*heights):
+        if not self._is_pareto_ordered(h0, h1):
             raise ValueError("An error occurred while calculating optimal permutations. "
                              "You can try again with a larger `max_steps` value.")
         else:
-            i0, j0, area = self._get_largest_rectangle(heights[1], m, n)
+            i0, j0, area = self._get_largest_rectangle(h1, m, n)
             return area, i0, j0, p_rows, p_cols
 
     def _solve(self, x):
-        """
-        Solve the optimal problem of removing NaNs for a 2D array.
-
-        Args:
-            x (np.ndarray): The input 2D array with NaN values.
-
-        Returns:
-            Tuple[np.ndarray, np.ndarray]: Rows and columns to retain.
-        """
         m, n = x.shape
-        df = pd.DataFrame()
         iy, ix = np.isnan(x).nonzero()
-        if len(iy)>0:
-            rows_with_nan, df[0] = np.unique(iy, return_inverse=True)
-            cols_with_nan, df[1] = np.unique(ix, return_inverse=True)
+        if len(iy) == 0:
+            return np.arange(m), np.arange(n)
+        else:
+            rng = np.random.default_rng(seed=self.random_state)
+            rows_with_nan, iy = np.unique(iy, return_inverse=True)
+            cols_with_nan, ix = np.unique(ix, return_inverse=True)
             m_nan, n_nan = len(rows_with_nan), len(cols_with_nan)
 
-            rng = np.random.default_rng(seed=self.random_state)
             area_max = -1
-            for k in range(self.n_tries):
-                area, i0, j0, p_rows, p_cols = self._trial(rng, df, m, n, m_nan, n_nan)
-                self._verbose(f"\tTrial {k + 1} : submatrix of size {m - j0}x{n - i0} ({area} elements) found.")
+            for k in range(self.n_tries):                
+                area, i0, j0, p_rows, p_cols = self._trial(rng, m_nan, n_nan, iy, ix, m, n)
+                self._verbose(f"\tTrial {k+1} : submatrix of size {m-j0}x{n-i0} ({area} elements) found.")
                 if area > area_max:
                     area_max = area
                     opt = i0, j0, p_rows, p_cols
 
             i0, j0, p_rows, p_cols = opt
-            self._verbose(f"Result: the largest submatrix found is of size {m - j0}x{n - i0} ({area_max} elements) found.")
+            self._verbose(f"Result: the largest submatrix found is of size {m-j0}x{n-i0} ({area_max} elements) found.")
 
             rows_to_keep = np.setdiff1d(np.arange(m), rows_with_nan[p_rows[:j0]])
             cols_to_keep = np.setdiff1d(np.arange(n), cols_with_nan[p_cols[:i0]])
             return rows_to_keep, cols_to_keep
-        else:
-            return np.arange(m), np.arange(n)
 
     def solve(self, X: Union[np.ndarray, pd.DataFrame], return_data: bool = False) -> Union[Tuple[np.ndarray, np.ndarray], Tuple[pd.Index, pd.Index]]:
         """
         Solves the optimal problem of removing NaNs for a 2D array or DataFrame.
 
         Args:
             X (Union[np.ndarray, pd.DataFrame]): The input 2D array or DataFrame with NaN values.
@@ -202,29 +142,30 @@
 
         Returns:
             Union[Tuple[np.ndarray, np.ndarray], Tuple[pd.Index, pd.Index]]: If return_data is True, returns the resulting 2D array or DataFrame; otherwise, returns the indices of rows and columns to retain.
 
         Raises:
             ValueError: If the input data is not a numpy array or a pandas DataFrame, or if the input numpy array does not have ndim==2, or if the OptiMask algorithm encounters an error during optimization.
         """
-        if not isinstance(X, (np.ndarray, pd.DataFrame)):
-            raise ValueError("Input 'X' must be a numpy array or a pandas DataFrame.")
+        check_params(X, types=(np.ndarray, pd.DataFrame))
 
         if isinstance(X, np.ndarray) and X.ndim != 2:
-            raise ValueError("For a numpy array, 'X' must have ndim==2.")
+            raise ValueError("For a numpy array, 'X' must have ndim == 2.")
 
         rows, cols = self._solve(np.asarray(X))
 
-        if np.isnan(np.asarray(X)[rows][:, cols]).any():
+        if np.isnan(np.asarray(X)[np.ix_(rows, cols)]).any():
             raise ValueError("The OptiMask algorithm encountered an error.")
 
         if isinstance(X, pd.DataFrame):
             if return_data:
                 return X.iloc[rows, cols].copy()
             else:
+                if not X.index.is_unique:
+                    raise ValueError("The index contains non-unique entries!")
                 return X.index[rows].copy(), X.columns[cols].copy()
 
         if isinstance(X, np.ndarray):
             if return_data:
                 return X[rows][:, cols].copy()
             else:
                 return rows, cols
```

### Comparing `optimask-1.0/optimask.egg-info/PKG-INFO` & `optimask-1.2/optimask.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: optimask
-Version: 1.0
+Version: 1.2
 Summary: OptiMask: extracting the largest (non-contiguous) submatrix without NaN
 Home-page: https://github.com/CyrilJl/optimask
 Author: Cyril Joly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: cython
 
-# OptiMask: Efficient NaN Data Removal in Python
+# <img src="https://raw.githubusercontent.com/CyrilJl/OptiMask/main/docs/source/_static/icon.svg" alt="Logo OptiMask" width="35" height="35"> OptiMask: Efficient NaN Data Removal in Python
 
-[![PyPI Version](https://img.shields.io/pypi/v/optimask.svg)](https://pypi.org/project/optimask/)
+[![PyPI Version](https://img.shields.io/pypi/v/optimask.svg)](https://pypi.org/project/optimask/) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/optimask.svg)](https://anaconda.org/conda-forge/optimask)
 
 ## Introduction
 
 OptiMask is a Python package designed to facilitate the process of removing NaN (Not-a-Number) data from matrices while efficiently computing the largest (and not necessarily contiguous) submatrix without NaN values. This tool prioritizes practicality and compatibility with Numpy arrays and Pandas DataFrames.
 
 ## Key Features
 
@@ -29,14 +30,24 @@
 
 To employ OptiMask, install the `optimask` package via pip:
 
 ```bash
 pip install optimask
 ```
 
+OptiMask is also available on the conda-forge channel:
+
+```bash
+conda install -c conda-forge optimask
+```
+
+```bash
+mamba install optimask
+```
+
 ## Usage Example
 
 Import the `OptiMask` class from the `optimask` package and utilize its methods for efficient data masking:
 
 ```python
 from optimask import OptiMask
 import numpy as np
```

