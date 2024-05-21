# Comparing `tmp/SimTissue-0.0.2.tar.gz` & `tmp/simtissue-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimTissue-0.0.2.tar", last modified: Tue Dec 26 15:59:11 2023, max compression
+gzip compressed data, was "simtissue-0.0.3.tar", last modified: Tue May 21 13:39:57 2024, max compression
```

## Comparing `SimTissue-0.0.2.tar` & `simtissue-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-12-26 15:59:11.548811 SimTissue-0.0.2/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1073 2023-11-19 14:50:32.000000 SimTissue-0.0.2/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      760 2023-12-26 15:59:11.548811 SimTissue-0.0.2/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      324 2023-11-19 15:55:35.000000 SimTissue-0.0.2/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      532 2023-12-26 15:45:07.000000 SimTissue-0.0.2/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       51 2023-11-19 15:27:36.000000 SimTissue-0.0.2/requirements.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-12-26 15:59:11.548811 SimTissue-0.0.2/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-12-26 15:59:11.548811 SimTissue-0.0.2/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-12-26 15:59:11.548811 SimTissue-0.0.2/src/SimTissue.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      760 2023-12-26 15:59:11.000000 SimTissue-0.0.2/src/SimTissue.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      413 2023-12-26 15:59:11.000000 SimTissue-0.0.2/src/SimTissue.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-12-26 15:59:11.000000 SimTissue-0.0.2/src/SimTissue.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       43 2023-12-26 15:59:11.000000 SimTissue-0.0.2/src/SimTissue.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       19 2023-12-26 15:59:11.000000 SimTissue-0.0.2/src/SimTissue.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-12-12 09:56:55.000000 SimTissue-0.0.2/src/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-12-26 15:59:11.548811 SimTissue-0.0.2/src/simtissue/
--rw-rw-r--   0 tom       (1000) tom       (1000)       62 2023-12-18 15:16:47.000000 SimTissue-0.0.2/src/simtissue/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5644 2023-11-19 14:23:09.000000 SimTissue-0.0.2/src/simtissue/arbitrary_shape.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12369 2023-12-12 10:03:20.000000 SimTissue-0.0.2/src/simtissue/control_expression.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2850 2023-11-19 14:23:09.000000 SimTissue-0.0.2/src/simtissue/plot.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2539 2023-12-18 10:27:35.000000 SimTissue-0.0.2/src/simtissue/tissue.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3149 2023-11-19 14:23:09.000000 SimTissue-0.0.2/src/simtissue/utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-21 13:39:57.864361 simtissue-0.0.3/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1073 2023-11-19 14:50:32.000000 simtissue-0.0.3/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      760 2024-05-21 13:39:57.864361 simtissue-0.0.3/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      324 2023-11-19 15:55:35.000000 simtissue-0.0.3/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      532 2024-05-21 13:39:53.000000 simtissue-0.0.3/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       51 2023-11-19 15:27:36.000000 simtissue-0.0.3/requirements.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-05-21 13:39:57.864361 simtissue-0.0.3/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-21 13:39:57.860361 simtissue-0.0.3/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-21 13:39:57.864361 simtissue-0.0.3/src/SimTissue.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      760 2024-05-21 13:39:57.000000 simtissue-0.0.3/src/SimTissue.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      413 2024-05-21 13:39:57.000000 simtissue-0.0.3/src/SimTissue.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-05-21 13:39:57.000000 simtissue-0.0.3/src/SimTissue.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       43 2024-05-21 13:39:57.000000 simtissue-0.0.3/src/SimTissue.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       19 2024-05-21 13:39:57.000000 simtissue-0.0.3/src/SimTissue.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-12-12 09:56:55.000000 simtissue-0.0.3/src/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-21 13:39:57.864361 simtissue-0.0.3/src/simtissue/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       62 2024-05-21 13:39:31.000000 simtissue-0.0.3/src/simtissue/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9059 2024-05-21 13:20:36.000000 simtissue-0.0.3/src/simtissue/arbitrary_shape.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11246 2024-05-21 13:37:40.000000 simtissue-0.0.3/src/simtissue/control_expression.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3419 2024-05-21 11:00:13.000000 simtissue-0.0.3/src/simtissue/plot.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2539 2023-12-18 10:27:35.000000 simtissue-0.0.3/src/simtissue/tissue.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3149 2023-11-19 14:23:09.000000 simtissue-0.0.3/src/simtissue/utils.py
```

### Comparing `SimTissue-0.0.2/LICENSE` & `simtissue-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SimTissue-0.0.2/PKG-INFO` & `simtissue-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimTissue
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Thomas Defard <thomas.defard@mines-paristech.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `SimTissue-0.0.2/pyproject.toml` & `simtissue-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "SimTissue"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Thomas Defard", email="thomas.defard@mines-paristech.fr" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `SimTissue-0.0.2/src/SimTissue.egg-info/PKG-INFO` & `simtissue-0.0.3/src/SimTissue.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimTissue
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Thomas Defard <thomas.defard@mines-paristech.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `SimTissue-0.0.2/src/simtissue/control_expression.py` & `simtissue-0.0.3/src/simtissue/control_expression.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,31 +10,28 @@
 import numpy as np
 import pandas as pd
 from sklearn.neighbors import NearestNeighbors
 from sklearn.utils.random import sample_without_replacement
 import anndata as ad
 from .utils import get_dict_coord_map
 
-def test():
-    print("test")
-
 
 def create_fix_profile(dict_profile={'typeA': [120, 0],
                                      'typeB': [0, 10]},
                        cell_type_distribution={'typeA': list(range(0, 110, 2)),
                                                'typeB': list(range(1, 110, 2))}):
     """
-
-    :param dict_profile: dictionary of the expression profile of each cell type e.g. {'typeA': [120, 0], 'typeB': [0, 10]}
+    Associate each cell index to a fixed RNA profile
+    :param dict_profile: dictionary defining the RNA profile of each cell type e.g. {'typeA': [120, 0], 'typeB': [0, 10]}
     :type dict_profile: dict
     :param cell_type_distribution: dictionary of the cell type distribution e.g. {'typeA': list(range(0, 110, 2)), 'typeB': list(range(1, 110, 2))}
     :type cell_type_distribution: dict
     :return:
         - dict_cell_type_label_rna - {cell_type : {cell_id : expression vector}
-        - dico_cell_index - {cell_id : {type:, rnaseq : expression vector}}
+        - dico_cell_index - {cell_id : {type: cell_type, rnaseq : expression vector}}
     """
     dico_cell_type_label_rna = {}  # {cell_type : {cell number : expression vector}
     dico_cell_index = {}  # {cell number : {type:, rnaseq : expression vector}}
     for cell_type in cell_type_distribution:
         dico_cell_type_label_rna[cell_type] = {cell_id: dict_profile[cell_type] for cell_id in
                                                cell_type_distribution[cell_type]}
         for cell_id in cell_type_distribution[cell_type]:
@@ -48,26 +45,30 @@
         dict_profile : dict,
         cell_type_distribution : dict,
         mask_cyto : np.ndarray,
         genes_list_to_simulate  : list,
         image_name : str = 'img0' ):
 
     """
-    simulate the expression of a list of genes in a mask of cytoplasm
+
+    This function simulate the expression of a list of genes in a mask of cytoplasm.
+     The rna position are sample from a uniform spatial distribution in the cytoplasm.
 
     :param dict_profile: dictionary of the expression profile of each cell type e.g. {'typeA': [120, 0], 'typeB': [0, 10]}
     :type dict_profile: dict
     :param cell_type_distribution: dictionary of the cell type distribution e.g. {'typeA': list(range(0, 110, 2)), 'typeB': list(range(1, 110, 2))}
     :type cell_type_distribution: dict
     :param mask_cyto: cytoplasm mask
     :type mask_cyto: np.ndarray
     :param genes_list_to_simulate: list of genes to simulate e.g. ['gene1', 'gene2']
     :param image_name: name of the image to add in annData
     :return: anndata object with the simulated expression profile and coordinates
     :rtype anndata: anndata object
+
+
     """
 
     dico_cell_type_label_rna, dico_cell_index = create_fix_profile(
         dict_profile=dict_profile,
         cell_type_distribution=cell_type_distribution
                 )
 
@@ -110,15 +111,15 @@
 
 
 def filter_simulation(spots_position : list,
                       max_dist: float = 3,
                       dict_scale : dict = {"x": 1, 'y': 1, "z": 1}):
     """
 
-    Merge overlapping spots
+    This function Merge overlapping spots as a single spot
     :param spots_position: list of spots position
     :type spots_position: list
     :param max_dist: max distance between spots to merge in the scale of dict_scale
     :type max_dist: int
     :param dict_scale:
     :return: list of spots position with merged spots
     """
@@ -144,39 +145,51 @@
 def sim_spots_from_ref_anndata(
         ref_anndata,
         cell_mask,
         selected_gene,
         image_name='',
         annotation_column="cell_ID",
         remove_neighbors=True,
-        max_dist=3,
+        max_dist=0.3,
         dict_scale={"x": 0.103, 'y': 0.103, "z": 0.300},
         random_indice : list = None,
+        scaling_factor=3
 
-        ):
-    """
+):
 
+    """
+    This function simulate the expression of a list of genes in a mask of cytoplasm.
+    It sample each RNA profile from a reference anndata object. The RNA molecule are then sampled from a uniform spatial distribution in each cell
     :param ref_anndata: andata object with the reference expression profile to sample
+    :type ref_anndata: anndata object
     :param cell_mask:  cell mask
-    :param selected_gene:
-    :param image_name:
-    :param annotation_column:
-    :param remove_neighbors:
-    :param max_dist:
-    :param random_indice:
-    :param dict_scale:
+    :type cell_mask: np.ndarray
+    :param selected_gene: list of genes to simulate e.g. ['gene1', 'gene2'] from the reference anndata
+    :type selected_gene: list
+    :param image_name: name of the image to add in annData
+    :type image_name: str
+    :param annotation_column: column name of the cell type in the reference anndata
+    :type annotation_column: str
+    :param remove_neighbors: if True remove the RNA molecules that are too close
+    :type remove_neighbors: bool
+    :param max_dist: max distance between spots to merge if remove_neighbors is True
+    :type max_dist: int
+    :param dict_scale: scale of the image in z,y,x in µm
+    :type dict_scale: dict
+    :param random_indice: if not None, list of cell index to sample from the reference anndata
+    :type random_indice: list
     :return:
     """
+
     dico_coord_map = get_dict_coord_map(cell_mask)
     if random_indice is None:
         random_indice = sample_without_replacement(len(ref_anndata),
                                                    len(dico_coord_map))  # return a list
     list_index_cell = list(dico_coord_map.keys())
 
-    scaling_factor = 3
     count_matrix = ref_anndata[random_indice, selected_gene].X
     print(ref_anndata[random_indice, selected_gene])
     list_cell_type = list(ref_anndata[random_indice, selected_gene].obs[annotation_column])
 
     if not isinstance(count_matrix, np.ndarray):
         count_matrix = count_matrix.toarray()
 
@@ -240,60 +253,7 @@
                              "x": csv_list_x,
                              "gene": csv_list_gene,
                              "cell": csv_list_cell,
                              'cell_type': csv_list_cell_type})
     anndata.uns["df_spots"] = df_spots
     return anndata, df_spots
 
-
-if __name__ == '__main__':
-
-    ### DEFINE THE TRANSCRIPTOMIC PROFILE OF EACH CELL
-    cell_index_typeA = [i for i in range(1, 111) if i % 2 == 0]
-    cell_index_typeB = [i for i in range(1, 111) if i % 2 == 0]
-    genes_list_to_simulate = ['A', 'B']
-    dico_cell_type_label_rna, dico_cell_index = create_fix_profile(
-        dico_profile={'typeA': [50, 0],
-                      'typeB': [0, 200]},
-        cell_type_distribution={'typeA': cell_index_typeA,
-                                'typeB': cell_index_typeB, }
-    )
-
-    ### simulate spots coordinate
-    dict_coord_map = get_dict_coord_map(mask_cell=mask_cyto,
-                                        )
-    list_index_cell = list(dict_coord_map.keys())
-
-    for cell in list_index_cell:
-        dico_cell_index[cell]["ground_truth"] = {}
-    list_list_gene = []
-    list_list_coord = []
-    for cell in list_index_cell:
-        list_gene = []
-        list_coord = []
-        for gene in genes_list_to_simulate:
-            gene_index = genes_list_to_simulate.index(gene)
-            nb_rna = int(dico_cell_index[cell]["rnaseq"][gene_index] * dico_gene_scaling[gene])
-            out_ind = dict_coord_map[cell]
-            spots_postion = out_ind[sample_without_replacement(len(out_ind), min(nb_rna, len(out_ind)))]
-            #dico_cell_index[cell]["ground_truth"][gene] = list(spots_postion)
-            #dico_fish_channel[gene]["ground_truth"] += list(spots_postion)
-            list_coord += list(spots_postion)
-            list_gene += [gene] * len(spots_postion)
-        list_list_gene.append(list_gene)
-        list_list_coord.append(list_coord)
-
-## gene expression vector
-    list_expression_vector = []
-    for cell_index in list_index_cell:
-        list_expression_vector.append(dico_cell_index[cell_index]["rnaseq"])
-
-    ### generate the list_expression_vectoranndata
-
-    adata = ad.AnnData(csr_matrix(list_expression_vector))
-    adata.var["features"] = genes_list_to_simulate
-    adata.var_names = genes_list_to_simulate
-    adata.obs["image_name"] = list_image_name
-    adata.obs["genes"] = list_list_gene
-    adata.obs["coordinate"] = list_list_coord
-    adata.obs["cell_index"] = list_index_cell
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `SimTissue-0.0.2/src/simtissue/plot.py` & `simtissue-0.0.3/src/simtissue/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,32 @@
 def plot_contour(mask_cyto=None,
                  mask_nuclei=None,
                  figsize=(15, 15),
                  anndata=None,
                  dico_color={"A": "r", "B": "b"},
                  spot_size=3,
                  linewidth=1):
+    """
+    plot the contour of the mask_cyto and mask_nuclei
+    :param mask_cyto: 3D/2D mask of the cytoplasm
+    :param mask_nuclei: 3D/ 2D mask of the nuclei
+    :param figsize:
+    :param anndata: With  anndata.obs["gene"] containing the gene list  of each cell and anndata.obs["coordinate"] as the coordinate of each gene
+    :param dico_color: dictionnary of color for each gene
+    :param spot_size: size of the spot
+    :param linewidth: width of the cell /nuclei contour
+    :return:
+    """
+
+
     fig, ax = plt.subplots(figsize=figsize)
 
-    if mask_cyto.ndim == 3:
+    if mask_cyto is not None and mask_cyto.ndim == 3:
         mask_cyto = np.amax(mask_cyto, axis=0)
-    if mask_nuclei.ndim == 3:
+    if mask_nuclei is not None and mask_nuclei.ndim == 3:
         mask_nuclei = np.amax(mask_nuclei, axis=0)
 
 
     if mask_cyto is not None:
         cyto_list = np.unique(mask_cyto)
         for nuc_id in cyto_list:
             countour = skimage.measure.find_contours(mask_cyto, nuc_id)
@@ -34,25 +47,25 @@
         contour_nuclei = (mask_nuclei  > 0).astype(int) - ndi.minimum_filter((mask_nuclei > 0).astype(int), size=3)
         contour_nuclei = np.array(list(zip(*np.nonzero(contour_nuclei))))
         plt.scatter(contour_nuclei[:, 1], contour_nuclei[:, 0],
                     s=linewidth,
                     linewidths = linewidth, c='black')
 
     ### plot cell border
-    contour_nuclei = [[0, i] for i in
-                      range(mask_nuclei.shape[-1])] + [[i, 0] for i
-                                                  in range(mask_nuclei.shape[-2])] + [[mask_nuclei.shape[-2] - 1, i] for i
-                                                                                 in range(mask_nuclei.shape[-1])] + [
-                         [i, mask_nuclei.shape[-1] - 1] for i
-                         in range(mask_nuclei.shape[-2])]
-    contour_nuclei = np.array(contour_nuclei)
-    plt.scatter(contour_nuclei[:, 1], contour_nuclei[:, 0],
-                linewidths=linewidth,
-                s=linewidth,
-                c='black')
+    #contour_nuclei = [[0, i] for i in
+    #                  range(mask_nuclei.shape[-1])] + [[i, 0] for i
+     #                                             in range(mask_nuclei.shape[-2])] + [[mask_nuclei.shape[-2] - 1, i] for i
+     #                                                                            in range(mask_nuclei.shape[-1])] + [
+      #                   [i, mask_nuclei.shape[-1] - 1] for i
+       #                  in range(mask_nuclei.shape[-2])]
+    #contour_nuclei = np.array(contour_nuclei)
+    #plt.scatter(contour_nuclei[:, 1], contour_nuclei[:, 0],
+     #           linewidths=linewidth,
+      #          s=linewidth,
+       #         c='black')
 
     if anndata is not None:
         list_list_gene = list(anndata.obs["genes"])
         list_list_coord = list(anndata.obs["coordinate"])
         list_unique_gene = np.unique(np.concatenate(list_list_gene))
         dico_gene_coord = {}
         for gene in list_unique_gene:
```

### Comparing `SimTissue-0.0.2/src/simtissue/tissue.py` & `simtissue-0.0.3/src/simtissue/tissue.py`

 * *Files identical despite different names*

### Comparing `SimTissue-0.0.2/src/simtissue/utils.py` & `simtissue-0.0.3/src/simtissue/utils.py`

 * *Files identical despite different names*

