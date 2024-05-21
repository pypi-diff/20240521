# Comparing `tmp/gene_trajectory-1.0.2.tar.gz` & `tmp/gene_trajectory-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene_trajectory-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gene_trajectory-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gene_trajectory-1.0.2.tar` & `gene_trajectory-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1070 2024-05-05 12:17:27.743010 gene_trajectory-1.0.2/LICENSE
--rw-r--r--   0        0        0     3441 2024-05-05 12:17:27.743010 gene_trajectory-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/__init__.py
--rw-r--r--   0        0        0     1861 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/add_gene_bin_score.py
--rw-r--r--   0        0        0     4642 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/coarse_grain.py
--rw-r--r--   0        0        0     2846 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/compute_gene_distance_cmd.py
--rw-r--r--   0        0        0     2337 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/diffusion_map.py
--rw-r--r--   0        0        0     5583 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/extract_gene_trajectory.py
--rw-r--r--   0        0        0     3845 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/gene_distance_shared.py
--rw-r--r--   0        0        0     1497 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/get_graph_distance.py
--rw-r--r--   0        0        0        0 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/plot/__init__.py
--rw-r--r--   0        0        0     3531 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/plot/gene_trajectory_plots.py
--rw-r--r--   0        0        0     1593 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/run_dm.py
--rw-r--r--   0        0        0        0 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/util/__init__.py
--rw-r--r--   0        0        0     1331 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/util/download_file.py
--rw-r--r--   0        0        0     3053 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/util/shared_array.py
--rw-r--r--   0        0        0       95 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/widgets/__init__.py
--rw-r--r--   0        0        0     5024 2024-05-05 12:17:27.787011 gene_trajectory-1.0.2/gene_trajectory/widgets/extract_gene_trajectory_widget.py
--rw-r--r--   0        0        0     1360 2024-05-05 12:17:27.815010 gene_trajectory-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4793 1970-01-01 00:00:00.000000 gene_trajectory-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-21 09:45:41.277046 gene_trajectory-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3441 2024-05-21 09:45:41.277046 gene_trajectory-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/__init__.py
+-rw-r--r--   0        0        0     1861 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/add_gene_bin_score.py
+-rw-r--r--   0        0        0     4915 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/coarse_grain.py
+-rw-r--r--   0        0        0     2846 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/compute_gene_distance_cmd.py
+-rw-r--r--   0        0        0     2442 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/diffusion_map.py
+-rw-r--r--   0        0        0     5774 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/extract_gene_trajectory.py
+-rw-r--r--   0        0        0     4120 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/gene_distance_shared.py
+-rw-r--r--   0        0        0     1497 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/get_graph_distance.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/plot/__init__.py
+-rw-r--r--   0        0        0     3531 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/plot/gene_trajectory_plots.py
+-rw-r--r--   0        0        0     1593 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/run_dm.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/util/__init__.py
+-rw-r--r--   0        0        0     1331 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/util/download_file.py
+-rw-r--r--   0        0        0     2534 2024-05-21 09:45:41.341047 gene_trajectory-1.0.3/gene_trajectory/util/input_validation.py
+-rw-r--r--   0        0        0     3053 2024-05-21 09:45:41.345047 gene_trajectory-1.0.3/gene_trajectory/util/shared_array.py
+-rw-r--r--   0        0        0       95 2024-05-21 09:45:41.345047 gene_trajectory-1.0.3/gene_trajectory/widgets/__init__.py
+-rw-r--r--   0        0        0     5024 2024-05-21 09:45:41.345047 gene_trajectory-1.0.3/gene_trajectory/widgets/extract_gene_trajectory_widget.py
+-rw-r--r--   0        0        0     1360 2024-05-21 09:45:41.369047 gene_trajectory-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4793 1970-01-01 00:00:00.000000 gene_trajectory-1.0.3/PKG-INFO
```

### Comparing `gene_trajectory-1.0.2/LICENSE` & `gene_trajectory-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/README.md` & `gene_trajectory-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/gene_trajectory/add_gene_bin_score.py` & `gene_trajectory-1.0.3/gene_trajectory/add_gene_bin_score.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/gene_trajectory/coarse_grain.py` & `gene_trajectory-1.0.3/gene_trajectory/coarse_grain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Optional
 
 import numpy as np
 import scanpy as sc
 from sklearn.cluster import KMeans
 
+from gene_trajectory.util.input_validation import validate_matrix
+
 
 def select_top_genes(
         adata: sc.AnnData,
         layer: str = None,
         min_expr_percent: float = 0.01,
         max_expr_percent: float = 0.5,
         n_variable_genes: int = 2000,
@@ -60,14 +62,18 @@
     :param gene_expression: the gene expression matrix
     :param graph_dist: the graph distance matrix
     :param n: number of cells to keep
     :param cluster: specify an array to use precomputed clusters. If not specified a KMeans clustering will be performed
     :param random_seed: the random seed
     :return: the updated cell embedding and gene expression matrices
     """
+    validate_matrix(gene_expression, obj_name='Gene Expression Matrix', min_value=0)
+    ncells, ngenes = gene_expression.shape
+    validate_matrix(cell_embedding, obj_name='Cell embedding', nrows=ncells)
+
     if cluster is None:
         k_means = KMeans(n_clusters=n, random_state=random_seed).fit(cell_embedding)
         cluster = k_means.labels_ # noqa
 
     knn_membership = np.zeros((n, cell_embedding.shape[0]))
     for i, c in enumerate(cluster):
         knn_membership[c, i] = 1
```

### Comparing `gene_trajectory-1.0.2/gene_trajectory/compute_gene_distance_cmd.py` & `gene_trajectory-1.0.3/gene_trajectory/compute_gene_distance_cmd.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/gene_trajectory/diffusion_map.py` & `gene_trajectory-1.0.3/gene_trajectory/diffusion_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Union
 import numpy as np
 
+from gene_trajectory.util.input_validation import validate_matrix
+
 
 def diffusion_map(
         dist_mat: np.array,
         k: int = 10,
         sigma: Union[float, np.array, list] = None,
         n_ev: int = 30,
         t: int = 1,
@@ -15,14 +17,16 @@
     :param dist_mat: Precomputed distance matrix (symmetric)
     :param k: Adaptive kernel bandwidth for each point set to be the distance to its `K`-th nearest neighbor
     :param sigma: Fixed kernel bandwidth, `sigma` will be ignored if `K` is specified
     :param n_ev: Number of leading eigenvectors to export
     :param t: Number of diffusion times
     :return: the diffusion embedding and the eigenvalues
     """
+    validate_matrix(dist_mat, square=True)
+
     affinity_matrix_symm = get_symmetrized_affinity_matrix(dist_mat=dist_mat, k=k, sigma=sigma)
     normalized_vec = np.sqrt(1 / affinity_matrix_symm.sum(axis=1))
     affinity_matrix_norm = (affinity_matrix_symm * normalized_vec * normalized_vec[:, None])
 
     n_ev = min(n_ev, affinity_matrix_norm.shape[0])
     eigs = np.linalg.eigh(affinity_matrix_norm, )
 
@@ -46,15 +50,16 @@
     Computes the symmetrized distance matrix
     :param dist_mat: Precomputed distance matrix (symmetric)
     :param k: Adaptive kernel bandwidth for each point set to be the distance to its `K`-th nearest neighbor
     :param sigma: Fixed kernel bandwidth, `sigma` will be ignored if `k` is specified
 
     :return:
     """
-    assert dist_mat.shape[0] == dist_mat.shape[1]
+    validate_matrix(dist_mat, square=True)
+
     dists = np.nan_to_num(dist_mat, 1e-6) # noqa
     k = min(k, dist_mat.shape[0])
 
     if sigma is None:
         sigma = np.apply_along_axis(func1d=sorted, axis=1, arr=dists)[:, k - 1]  # noqa
     elif np.isscalar(sigma):
         sigma = np.full(dists.shape[0], sigma)
```

### Comparing `gene_trajectory-1.0.2/gene_trajectory/extract_gene_trajectory.py` & `gene_trajectory-1.0.3/gene_trajectory/extract_gene_trajectory.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional
 
 from scipy.stats import rankdata
 import numpy as np
 import pandas as pd
 
 from gene_trajectory.diffusion_map import diffusion_map, get_symmetrized_affinity_matrix
+from gene_trajectory.util.input_validation import validate_matrix
 
 logger = logging.getLogger()
 
 
 def get_gene_embedding(
         dist_mat: np.array,
         k: int = 10,
@@ -24,14 +25,16 @@
     :param dist_mat: dist.mat matrix; Gene-gene Wasserstein distance matrix (symmetric)
     :param k: Adaptive kernel bandwidth for each point set to be the distance to its `K`-th nearest neighbor
     :param sigma: Fixed kernel bandwidth, `sigma` will be ignored if `K` is specified
     :param n_ev: Number of leading eigenvectors to export
     :param t: Number of diffusion times
     :return: the diffusion embedding and the eigenvalues
     """
+    validate_matrix(dist_mat, square=True)
+
     k = min(k, dist_mat.shape[0])
     n_ev = min(n_ev + 1, dist_mat.shape[0])
     diffu_emb, eigen_vals = diffusion_map(dist_mat=dist_mat, k=k, sigma=sigma, n_ev=n_ev, t=t)
     diffu_emb = diffu_emb[:, 1:n_ev + 1]
     eigen_vals = eigen_vals[1:n_ev + 1]
     return diffu_emb, eigen_vals
 
@@ -43,14 +46,16 @@
     """
     Convert a distance matrix into a random-walk matrix based on adaptive Gaussian kernel
 
     :param dist_mat: Precomputed distance matrix (symmetric)
     :param k: Adaptive kernel bandwidth for each point set to be the distance to its `K`-th nearest neighbor
     :return: Random-walk matrix
     """
+    validate_matrix(dist_mat, square=True)
+
     affinity_matrix_symm = get_symmetrized_affinity_matrix(dist_mat=dist_mat, k=k)
     normalized_vec = 1 / affinity_matrix_symm.sum(axis=1)
     affinity_matrix_norm = (affinity_matrix_symm * normalized_vec[:, None])
 
     return affinity_matrix_norm
 
 
@@ -63,15 +68,15 @@
     Order genes along a given trajectory
 
     :param dist_mat: Gene-gene Wasserstein distance matrix (symmetric)
     :param subset: Genes in a given trajectory
     :param max_id: Index of the terminal gene
     :return: The pseudoorder
     """
-    assert dist_mat.shape[0] == dist_mat.shape[1]
+    validate_matrix(dist_mat, square=True)
 
     emd = dist_mat[subset][:, subset]
     dm_emb, _ = diffusion_map(emd)
     pseudoorder = rankdata(dm_emb[:, 1])
 
     if max_id is not None and max_id in subset:
         n = len(subset)
@@ -104,14 +109,16 @@
     :param n: Number of gene trajectories to retrieve. Will be set to the length of t_list
     :param dims: Dimensions of gene embedding to use to identify terminal genes (extrema)
     :param k: Adaptive kernel bandwidth for each point set to be the distance to its `K`-th nearest neighbor
     :param quantile: Thresholding parameter to extract genes for each trajectory. Default: 0.02
     :param other: Label for genes not in a trajectory. Default: 'Other'
     :return: A data frame indicating gene trajectories and gene ordering along each trajectory
     """
+    validate_matrix(dist_mat, square=True)
+
     if np.isscalar(t_list):
         if n is None:
             raise ValueError(f'n should be specified if t_list is a number: {t_list}')
         t_list = np.full(n, t_list)
     elif n is None:
         n = len(t_list)
     if n != len(t_list):
```

### Comparing `gene_trajectory-1.0.2/gene_trajectory/gene_distance_shared.py` & `gene_trajectory-1.0.3/gene_trajectory/gene_distance_shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from multiprocessing.managers import SharedMemoryManager
 from typing import Optional, Sized
 
 import numpy as np
 import ot
 from tqdm import tqdm
 
+from gene_trajectory.util.input_validation import validate_matrix
 from gene_trajectory.util.shared_array import SharedArray, PartialStarApply
 
 logger = logging.getLogger()
 _DEFAULT_NUMITERMAX = 50000
 
 # Implementation notes:
 # - The matrices can get relatively large so they are kept in memory as shared objects
@@ -38,26 +39,28 @@
            the distance entry for missing pairs will be set to 1000*max(computed_gene_distances)
     :param num_iter_max: the max number of iterations when computing the distance (see ot.emd2)
     :param show_progress_bar: shows a progress bar while running the computation (default: True)
     :param processes:the number of processes to use (defaults to the number of CPUs available)
     :return: the distance matrix
     """
     processes = int(processes) if isinstance(processes, float) else os.cpu_count()
-    n = gene_expr.shape[1]
+    validate_matrix(gene_expr, obj_name='Gene Expression Matrix', min_value=0)
+    ncells, ngenes = gene_expr.shape
+    validate_matrix(ot_cost, obj_name='Cost Matrix', shape=(ncells, ncells), min_value=0)
+
     if show_progress_bar:
         logger.info(f'Computing emd distance..')
 
     if gene_pairs is None:
-        pairs = ((i, j) for i in range(0, n - 1) for j in range(i + 1, n))
-        npairs = (n * (n - 1)) // 2
+        pairs = ((i, j) for i in range(0, ngenes - 1) for j in range(i + 1, ngenes))
+        npairs = (ngenes * (ngenes - 1)) // 2
     else:
         pairs = gene_pairs
         npairs = len(gene_pairs)
-
-    emd_mat = np.full((n, n), fill_value=np.NaN)
+    emd_mat = np.full((ngenes, ngenes), fill_value=np.NaN)
 
     with SharedMemoryManager() as manager:
         start_time = time.perf_counter()
         # create and configure the process pool
 
         with ThreadPoolExecutor(max_workers=processes) as pool:
             # prepare shared environment
```

### Comparing `gene_trajectory-1.0.2/gene_trajectory/get_graph_distance.py` & `gene_trajectory-1.0.3/gene_trajectory/get_graph_distance.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/gene_trajectory/plot/gene_trajectory_plots.py` & `gene_trajectory-1.0.3/gene_trajectory/plot/gene_trajectory_plots.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/gene_trajectory/run_dm.py` & `gene_trajectory-1.0.3/gene_trajectory/run_dm.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/gene_trajectory/util/download_file.py` & `gene_trajectory-1.0.3/gene_trajectory/util/download_file.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/gene_trajectory/util/shared_array.py` & `gene_trajectory-1.0.3/gene_trajectory/util/shared_array.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/gene_trajectory/widgets/extract_gene_trajectory_widget.py` & `gene_trajectory-1.0.3/gene_trajectory/widgets/extract_gene_trajectory_widget.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.2/pyproject.toml` & `gene_trajectory-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "gene-trajectory"
-version = "1.0.2"
+version = "1.0.3"
 description = "Compute gene trajectories"
 license = {file = "LICENSE"}
 readme = "README.md"
 
 authors = [
     {name = "Francesco Strino", email = "francesco.strino@pcmgf.com"},
     {name = "Rihao Qu", email = "rihao.qu@yale.edu"},
```

### Comparing `gene_trajectory-1.0.2/PKG-INFO` & `gene_trajectory-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene-trajectory
-Version: 1.0.2
+Version: 1.0.3
 Summary: Compute gene trajectories
 Keywords: Gene trajectory,scRNA-seq
 Author-email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
 Maintainer-email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
```

