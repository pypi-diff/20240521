# Comparing `tmp/scbsp-0.2.5.tar.gz` & `tmp/scbsp-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scbsp-0.2.5.tar", last modified: Mon Apr  8 05:35:17 2024, max compression
+gzip compressed data, was "scbsp-0.2.6.tar", last modified: Tue May 21 08:35:07 2024, max compression
```

## Comparing `scbsp-0.2.5.tar` & `scbsp-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:35:17.448954 scbsp-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 05:35:13.000000 scbsp-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-08 05:35:17.448954 scbsp-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-08 05:35:13.000000 scbsp-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:35:17.444954 scbsp-0.2.5/scbsp/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-08 05:35:13.000000 scbsp-0.2.5/scbsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-04-08 05:35:13.000000 scbsp-0.2.5/scbsp/scbsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:35:17.444954 scbsp-0.2.5/scbsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-08 05:35:17.000000 scbsp-0.2.5/scbsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-08 05:35:17.000000 scbsp-0.2.5/scbsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:35:17.000000 scbsp-0.2.5/scbsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 05:35:17.000000 scbsp-0.2.5/scbsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 05:35:17.000000 scbsp-0.2.5/scbsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:35:17.448954 scbsp-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-08 05:35:16.000000 scbsp-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:35:17.448954 scbsp-0.2.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-08 05:35:13.000000 scbsp-0.2.5/test/test_scbsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:35:07.536422 scbsp-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 08:35:04.000000 scbsp-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-21 08:35:07.536422 scbsp-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-21 08:35:04.000000 scbsp-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:35:07.532422 scbsp-0.2.6/scbsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 08:35:04.000000 scbsp-0.2.6/scbsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-21 08:35:04.000000 scbsp-0.2.6/scbsp/scbsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:35:07.536422 scbsp-0.2.6/scbsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-21 08:35:07.000000 scbsp-0.2.6/scbsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-21 08:35:07.000000 scbsp-0.2.6/scbsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:35:07.000000 scbsp-0.2.6/scbsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 08:35:07.000000 scbsp-0.2.6/scbsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 08:35:07.000000 scbsp-0.2.6/scbsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:35:07.536422 scbsp-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-21 08:35:06.000000 scbsp-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:35:07.536422 scbsp-0.2.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-21 08:35:04.000000 scbsp-0.2.6/test/test_scbsp.py
```

### Comparing `scbsp-0.2.5/LICENSE` & `scbsp-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scbsp-0.2.5/PKG-INFO` & `scbsp-0.2.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,12 @@
-Metadata-Version: 2.1
-Name: scbsp
-Version: 0.2.5
-Summary: A package that efficiently computes p-values for a given set of genes based on input matrices representing cell coordinates and gene expression data
-Home-page: https://github.com/YQ-Wang/scBSP
-Author: Yiqing Wang, Jinpu Li
-Author-email: yqw@wangemail.com, lijinp@health.missouri.edu
-License: GPLv3
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: hnsw
-License-File: LICENSE
+# scBSP - A Fast Tool for Single-Cell Spatially Variable Genes Identifications on Large-Scale Spatially Resolved Transcriptomics Data
 
-\n# scBSP - A Fast Tool for Single-Cell Spatially Variable Genes Identifications on Large-Scale Spatially Resolved Transcriptomics Data
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11123268.svg)](https://doi.org/10.5281/zenodo.11123268)
 
-scBSP is a dedicated software package crafted for the nuanced domain of biological data processing, emphasizing gene expression analysis and cell coordinate evaluation. It offers a streamlined method to calculate p-values for a set of genes by leveraging input matrices that encapsulate cell coordinates and gene expression data.
+This package utilizes a granularity-based dimension-agnostic tool, single-cell big-small patch (scBSP), implementing sparse matrix operation and KD-tree/balltree method for distance calculation, for the identification of spatially variable genes on large-scale data.
 
 ## Installation
 
 ### Dependencies
 To ensure scBSP functions optimally, the following dependencies are required:
 - Python (>= 3.8)
 - NumPy (>= 1.24.4)
@@ -84,8 +64,11 @@
 p_values = scbsp.granp(input_sp_mat, input_exp_mat_raw, d1, d2)
 ```
 
 ## Output
 
 The function returns a Pandas DataFrame, featuring two columns: `gene_names` and `p_values`. Each row within this DataFrame represents a unique gene from the input gene expression matrix. The `gene_names` column specifies the identifier for each gene, while the `p_values` column quantifies the statistical significance of the expression differences observed across various cell coordinates. This structured format enhances the ease of conducting sophisticated biological analyses, allowing for straightforward identification and investigation of genes with significant expression variability.
 
+## Reference
+- Li, Jinpu, Yiqing Wang, Mauminah Azam Raina, Chunhui Xu, Li Su, Qi Guo, Qin Ma, Juexin Wang, and Dong Xu. "scBSP: A fast and accurate tool for identifying spatially variable genes from spatial transcriptomic data." bioRxiv (2024).
 
+- Wang, Juexin, Jinpu Li, Skyler T. Kramer, Li Su, Yuzhou Chang, Chunhui Xu, Michael T. Eadon, Krzysztof Kiryluk, Qin Ma, and Dong Xu. "Dimension-agnostic and granularity-based spatially variable gene identification using BSP." Nature Communications 14, no. 1 (2023): 7367.
```

### Comparing `scbsp-0.2.5/scbsp/scbsp.py` & `scbsp-0.2.6/scbsp/scbsp.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 on large-scale data.
 """
 
 from typing import List, Tuple, Union
 
 import numpy as np
 import pandas as pd  # type: ignore
+import scipy
+import torch
 from scipy.sparse import csr_matrix, diags, identity, isspmatrix_csr  # type: ignore
 from scipy.stats import gmean, lognorm
 
 try:
     import hnswlib
-
     use_hnsw = True
 except ImportError:
     from sklearn.neighbors import BallTree
-
     use_hnsw = False
 
 
 def _scale_sparse_matrix(input_exp_mat: csr_matrix) -> csr_matrix:
     """
     Scales a sparse matrix such that each row is divided by its maximum value.
 
@@ -93,17 +93,18 @@
     # Construct binary csr_matrix
     data = np.ones_like(rows)
 
     sparse_mat = csr_matrix(
         (data, (rows, cols)),
         shape=(input_sparse_mat_array.shape[0], input_sparse_mat_array.shape[0]),
     )
-    sparse_mat += identity(input_sparse_mat_array.shape[0], format="csr", dtype=bool)
 
-    return sparse_mat
+    return sparse_mat + identity(
+        input_sparse_mat_array.shape[0], format="csr", dtype=bool
+    )
 
 
 def _calculate_sparse_variances(input_csr_mat: csr_matrix, axis: int) -> List[float]:
     """
     Calculates the variances along a given axis for a csr_matrix.
 
     Args:
@@ -184,15 +185,34 @@
             (patches_cells.sum(axis=1) > 1).astype(float).A.ravel(),
             offsets=0,
             format="csr",
         )
         patches_cells -= patches_cells_centroid
         sum_axis_0 = patches_cells.sum(axis=0).A.ravel()
         diag_matrix_sparse = _get_inverted_diag_matrix(sum_axis_0)
-        x_kj = input_exp_mat_norm.dot(patches_cells.dot(diag_matrix_sparse))
+
+        if torch.cuda.is_available():
+
+            # Convert the csr_matrix to PyTorch tensors and move to GPU
+            input_exp_mat_norm_torch = torch.tensor(
+                input_exp_mat_norm.toarray(), device="cuda"
+            )
+            patches_cells_torch = torch.tensor(patches_cells.toarray(), device="cuda")
+            diag_matrix_sparse_torch = torch.tensor(
+                diag_matrix_sparse.toarray(), device="cuda"
+            )
+
+            result = torch.matmul(
+                input_exp_mat_norm_torch,
+                torch.matmul(patches_cells_torch, diag_matrix_sparse_torch),
+            )
+            x_kj = scipy.sparse.csr_matrix(result.cpu().numpy())
+        else:
+            x_kj = input_exp_mat_norm.dot(patches_cells.dot(diag_matrix_sparse))
+
         return _calculate_sparse_variances(x_kj, axis=1)
 
     var_x = np.column_stack([_var_local_means(input_sp_mat, d_val, input_exp_mat_norm, leaf_size).A.ravel() for d_val in (d1, d2)])  # type: ignore
     var_x_0_add = _calculate_sparse_variances(input_exp_mat_raw, axis=1).A.ravel()  # type: ignore
     var_x_0_add /= max(var_x_0_add)
     t_matrix = (var_x[:, 1] / var_x[:, 0]) * var_x_0_add
     return t_matrix.tolist()
@@ -219,16 +239,20 @@
         A Pandas DataFrame with columns ['gene_names', 'p_values'].
     """
     # Extract column names if input_exp_mat_raw is a Pandas DataFrame, else use indices
     if isinstance(input_exp_mat_raw, pd.DataFrame):
         gene_names = input_exp_mat_raw.columns.astype(str).tolist()
         input_exp_mat_raw = csr_matrix(input_exp_mat_raw)
     else:
-        gene_names = [f'Gene_{i}' for i in range(input_exp_mat_raw.shape[1])]
-        input_exp_mat_raw = input_exp_mat_raw if isspmatrix_csr(input_exp_mat_raw) else csr_matrix(input_exp_mat_raw)
+        gene_names = [f"Gene_{i}" for i in range(input_exp_mat_raw.shape[1])]
+        input_exp_mat_raw = (
+            input_exp_mat_raw
+            if isspmatrix_csr(input_exp_mat_raw)
+            else csr_matrix(input_exp_mat_raw)
+        )
 
     # Scale the distance thresholds according to the geometric mean of data spread.
     scale_factor = (
         gmean(
             np.quantile(input_sp_mat, 0.975, axis=0)
             - np.quantile(input_sp_mat, 0.025, axis=0)
         )
@@ -247,11 +271,8 @@
     log_norm_params = (log_t_matrix_sum_mid.mean(), log_t_matrix_sum_mid.std(ddof=1))
 
     # Calculate p-values using the log-normal distribution.
     p_values = 1 - lognorm.cdf(
         t_matrix_sum, scale=np.exp(log_norm_params[0]), s=log_norm_params[1]
     )
 
-    return pd.DataFrame({
-        'gene_names': gene_names,
-        'p_values': p_values
-    })
+    return pd.DataFrame({"gene_names": gene_names, "p_values": p_values})
```

### Comparing `scbsp-0.2.5/scbsp.egg-info/PKG-INFO` & `scbsp-0.2.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scbsp
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package that efficiently computes p-values for a given set of genes based on input matrices representing cell coordinates and gene expression data
 Home-page: https://github.com/YQ-Wang/scBSP
 Author: Yiqing Wang, Jinpu Li
 Author-email: yqw@wangemail.com, lijinp@health.missouri.edu
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,19 +14,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: hnsw
+Provides-Extra: gpu
 License-File: LICENSE
 
 \n# scBSP - A Fast Tool for Single-Cell Spatially Variable Genes Identifications on Large-Scale Spatially Resolved Transcriptomics Data
 
-scBSP is a dedicated software package crafted for the nuanced domain of biological data processing, emphasizing gene expression analysis and cell coordinate evaluation. It offers a streamlined method to calculate p-values for a set of genes by leveraging input matrices that encapsulate cell coordinates and gene expression data.
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11123268.svg)](https://doi.org/10.5281/zenodo.11123268)
+
+This package utilizes a granularity-based dimension-agnostic tool, single-cell big-small patch (scBSP), implementing sparse matrix operation and KD-tree/balltree method for distance calculation, for the identification of spatially variable genes on large-scale data.
 
 ## Installation
 
 ### Dependencies
 To ensure scBSP functions optimally, the following dependencies are required:
 - Python (>= 3.8)
 - NumPy (>= 1.24.4)
@@ -84,8 +87,13 @@
 p_values = scbsp.granp(input_sp_mat, input_exp_mat_raw, d1, d2)
 ```
 
 ## Output
 
 The function returns a Pandas DataFrame, featuring two columns: `gene_names` and `p_values`. Each row within this DataFrame represents a unique gene from the input gene expression matrix. The `gene_names` column specifies the identifier for each gene, while the `p_values` column quantifies the statistical significance of the expression differences observed across various cell coordinates. This structured format enhances the ease of conducting sophisticated biological analyses, allowing for straightforward identification and investigation of genes with significant expression variability.
 
+## Reference
+- Li, Jinpu, Yiqing Wang, Mauminah Azam Raina, Chunhui Xu, Li Su, Qi Guo, Qin Ma, Juexin Wang, and Dong Xu. "scBSP: A fast and accurate tool for identifying spatially variable genes from spatial transcriptomic data." bioRxiv (2024).
+
+- Wang, Juexin, Jinpu Li, Skyler T. Kramer, Li Su, Yuzhou Chang, Chunhui Xu, Michael T. Eadon, Krzysztof Kiryluk, Qin Ma, and Dong Xu. "Dimension-agnostic and granularity-based spatially variable gene identification using BSP." Nature Communications 14, no. 1 (2023): 7367.
+
```

### Comparing `scbsp-0.2.5/setup.py` & `scbsp-0.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="scbsp",
-    version="0.2.5",
+    version="0.2.6",
     description="A package that efficiently computes p-values for a given set of genes based on input matrices representing cell coordinates and gene expression data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["scbsp"],
     url="https://github.com/YQ-Wang/scBSP",
     author="Yiqing Wang, Jinpu Li",
     author_email="yqw@wangemail.com, lijinp@health.missouri.edu",
@@ -27,10 +27,11 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
     install_requires=["numpy >= 1.24.4", "pandas >= 1.3.5", "scipy >= 1.10.1", "scikit-learn>=1.3.2"],
     extras_require={
         "hnsw": ["hnswlib >= 0.8.0"],
+        "gpu": ["torch >= 1.10.0"],
     },
     python_requires=">=3.8",
 )
```

### Comparing `scbsp-0.2.5/test/test_scbsp.py` & `scbsp-0.2.6/test/test_scbsp.py`

 * *Files identical despite different names*

