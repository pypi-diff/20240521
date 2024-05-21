# Comparing `tmp/tscluster-1.0.2.tar.gz` & `tmp/tscluster-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tscluster-1.0.2.tar", last modified: Tue Apr  9 01:22:42 2024, max compression
+gzip compressed data, was "tscluster-1.0.3.tar", last modified: Tue May 21 13:41:45 2024, max compression
```

## Comparing `tscluster-1.0.2.tar` & `tscluster-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 01:22:42.916412 tscluster-1.0.2/
--rw-rw-rw-   0        0        0      528 2024-04-09 01:22:42.915412 tscluster-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-04-01 13:24:00.000000 tscluster-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 01:22:42.917413 tscluster-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      864 2024-04-09 01:22:25.000000 tscluster-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:22:42.837457 tscluster-1.0.2/tscluster/
--rw-rw-rw-   0        0        0        0 2024-03-26 05:37:01.000000 tscluster-1.0.2/tscluster/__init__.py
--rw-rw-rw-   0        0        0     8005 2024-04-08 21:19:03.000000 tscluster-1.0.2/tscluster/base.py
--rw-rw-rw-   0        0        0     7733 2024-04-08 20:21:14.000000 tscluster-1.0.2/tscluster/interface.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:22:42.874436 tscluster-1.0.2/tscluster/metrics/
--rw-rw-rw-   0        0        0       55 2024-03-25 06:31:54.000000 tscluster-1.0.2/tscluster/metrics/__init__.py
--rw-rw-rw-   0        0        0     5905 2024-04-08 10:53:03.000000 tscluster-1.0.2/tscluster/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:22:42.883432 tscluster-1.0.2/tscluster/opttscluster/
--rw-rw-rw-   0        0        0       61 2024-03-24 06:02:16.000000 tscluster-1.0.2/tscluster/opttscluster/__init__.py
--rw-rw-rw-   0        0        0     9457 2024-03-24 06:02:16.000000 tscluster-1.0.2/tscluster/opttscluster/optcluster.py
--rw-rw-rw-   0        0        0    32670 2024-04-09 01:19:56.000000 tscluster-1.0.2/tscluster/opttscluster/opttscluster.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:22:42.896425 tscluster-1.0.2/tscluster/preprocessing/
--rw-rw-rw-   0        0        0       75 2024-03-24 06:02:16.000000 tscluster-1.0.2/tscluster/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2289 2024-04-06 08:25:25.000000 tscluster-1.0.2/tscluster/preprocessing/interface.py
--rw-rw-rw-   0        0        0     5695 2024-04-06 08:32:11.000000 tscluster-1.0.2/tscluster/preprocessing/scaler.py
--rw-rw-rw-   0        0        0    19702 2024-04-08 10:11:53.000000 tscluster-1.0.2/tscluster/preprocessing/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:22:42.909417 tscluster-1.0.2/tscluster/tskmeans/
--rw-rw-rw-   0        0        0      110 2024-03-24 06:02:16.000000 tscluster-1.0.2/tscluster/tskmeans/__init__.py
--rw-rw-rw-   0        0        0     7024 2024-04-08 19:48:30.000000 tscluster-1.0.2/tscluster/tskmeans/tsglobalkmeans.py
--rw-rw-rw-   0        0        0     6658 2024-04-08 19:48:26.000000 tscluster-1.0.2/tscluster/tskmeans/tskmeans.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:22:42.912414 tscluster-1.0.2/tscluster/tsplot/
--rw-rw-rw-   0        0        0       56 2024-04-07 01:33:17.000000 tscluster-1.0.2/tscluster/tsplot/__init__.py
--rw-rw-rw-   0        0        0    17064 2024-04-09 00:21:12.000000 tscluster-1.0.2/tscluster/tsplot/tsplot.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:22:42.864441 tscluster-1.0.2/tscluster.egg-info/
--rw-rw-rw-   0        0        0      528 2024-04-09 01:22:42.000000 tscluster-1.0.2/tscluster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-04-09 01:22:42.000000 tscluster-1.0.2/tscluster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 01:22:42.000000 tscluster-1.0.2/tscluster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2024-04-09 01:22:42.000000 tscluster-1.0.2/tscluster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 01:22:42.000000 tscluster-1.0.2/tscluster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 13:41:45.904612 tscluster-1.0.3/
+-rw-rw-rw-   0        0        0     4557 2024-05-21 13:41:45.892620 tscluster-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4291 2024-04-29 10:03:56.000000 tscluster-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:41:45.905612 tscluster-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      864 2024-05-21 13:40:34.000000 tscluster-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:41:45.246991 tscluster-1.0.3/tscluster/
+-rw-rw-rw-   0        0        0        0 2024-03-26 05:37:01.000000 tscluster-1.0.3/tscluster/__init__.py
+-rw-rw-rw-   0        0        0    10319 2024-05-21 12:41:26.000000 tscluster-1.0.3/tscluster/base.py
+-rw-rw-rw-   0        0        0     7733 2024-04-08 20:21:14.000000 tscluster-1.0.3/tscluster/interface.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:41:45.510837 tscluster-1.0.3/tscluster/metrics/
+-rw-rw-rw-   0        0        0       55 2024-03-25 06:31:54.000000 tscluster-1.0.3/tscluster/metrics/__init__.py
+-rw-rw-rw-   0        0        0     5905 2024-04-08 10:53:03.000000 tscluster-1.0.3/tscluster/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:41:45.614780 tscluster-1.0.3/tscluster/opttscluster/
+-rw-rw-rw-   0        0        0       61 2024-03-24 06:02:16.000000 tscluster-1.0.3/tscluster/opttscluster/__init__.py
+-rw-rw-rw-   0        0        0     9457 2024-03-24 06:02:16.000000 tscluster-1.0.3/tscluster/opttscluster/optcluster.py
+-rw-rw-rw-   0        0        0    32370 2024-05-21 11:46:34.000000 tscluster-1.0.3/tscluster/opttscluster/opttscluster.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:41:45.705726 tscluster-1.0.3/tscluster/preprocessing/
+-rw-rw-rw-   0        0        0       75 2024-03-24 06:02:16.000000 tscluster-1.0.3/tscluster/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2289 2024-04-06 08:25:25.000000 tscluster-1.0.3/tscluster/preprocessing/interface.py
+-rw-rw-rw-   0        0        0     5695 2024-04-06 08:32:11.000000 tscluster-1.0.3/tscluster/preprocessing/scaler.py
+-rw-rw-rw-   0        0        0    19702 2024-04-08 10:11:53.000000 tscluster-1.0.3/tscluster/preprocessing/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:41:45.839650 tscluster-1.0.3/tscluster/tskmeans/
+-rw-rw-rw-   0        0        0      110 2024-03-24 06:02:16.000000 tscluster-1.0.3/tscluster/tskmeans/__init__.py
+-rw-rw-rw-   0        0        0     7024 2024-04-08 19:48:30.000000 tscluster-1.0.3/tscluster/tskmeans/tsglobalkmeans.py
+-rw-rw-rw-   0        0        0     6658 2024-04-08 19:48:26.000000 tscluster-1.0.3/tscluster/tskmeans/tskmeans.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:41:45.888622 tscluster-1.0.3/tscluster/tsplot/
+-rw-rw-rw-   0        0        0       56 2024-04-07 01:33:17.000000 tscluster-1.0.3/tscluster/tsplot/__init__.py
+-rw-rw-rw-   0        0        0    17067 2024-05-21 13:26:02.000000 tscluster-1.0.3/tscluster/tsplot/tsplot.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:41:45.417891 tscluster-1.0.3/tscluster.egg-info/
+-rw-rw-rw-   0        0        0     4557 2024-05-21 13:41:44.000000 tscluster-1.0.3/tscluster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-21 13:41:45.000000 tscluster-1.0.3/tscluster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:41:44.000000 tscluster-1.0.3/tscluster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-05-21 13:41:44.000000 tscluster-1.0.3/tscluster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 13:41:44.000000 tscluster-1.0.3/tscluster.egg-info/top_level.txt
```

### Comparing `tscluster-1.0.2/setup.py` & `tscluster-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setup(
    name='tscluster',
-   version='1.0.2',
+   version='1.0.3',
    description='A useful package for temporal clustering',
    license="MIT",
    long_description=long_description,
    long_description_content_type="text/markdown",
    author='Jolomi Tosanwumi',
    author_email='tjolomi@gmail.com',
    #url="...",
```

### Comparing `tscluster-1.0.2/tscluster/base.py` & `tscluster-1.0.3/tscluster/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                         label_dict: dict|None = None
                         ) -> pd.DataFrame:
         """
         Method to return the a data frame of the label assignments with custom names of time steps and entities.
 
         Parameters
         -----------
-        label_dict dict, default=None
+        label_dict : dict, default=None
             a dictionary whose keys are 'T', 'N', and 'F' (which are the number of time steps, entities, and features respectively). Value of each key is a list such that the value of key:
             - 'T' is a list of names/labels of each time step to be used as index of each dataframe. If None, range(0, T) is used. Where T is the number of time steps in the fitted data
             - 'N' is a list of names/labels of each entity to be used as index of the dataframe. If None, range(0, N) is used. Where N is the number of entities/observations in the fitted data 
             - 'F' is a list of names/labels of each feature to be used as column of each dataframe. If None, range(0, F) is used. Where F is the number of features in the fitted data 
             If label_dict is None, the result of self.label_dict_ is used.
 
         Returns
@@ -139,28 +139,72 @@
     def get_dynamic_entities(self) -> Tuple[List[np.int64], List[np.int64]]:
         """
         returns the dynamic entities and their number of changes. Both lists are sorted by the number of cluster changes in descending order.
 
         Returns
         -------
         dynamic entities : list
-            a 1-D array of the indices of the entities that change cluster at least once.
+            a 1-D array of the indexes of the entities that change cluster at least once.
         number of changes : list
             a 1-D array of the number of changes for each dynamic entity such that the i-th element is the number of cluster changes for the i-th dynamic entity
         """
         
         n_changes = self._get_changes()
         changes = n_changes > 0
 
         entities = self.label_dict_['N']
         dynamic_entities = np.where(changes)[0]
 
         sort_filter = np.argsort(n_changes[changes])[::-1]
 
         return [entities[i] for i in dynamic_entities[sort_filter]], list(np.sort(n_changes[changes])[::-1])
 
+    def get_index_of_label(self, labels: List[str], axis: str = 'N') -> List[int]:
+        """
+        function to return the integer indexes of some given labelled items in `self.label_dict_`. The indexes are assumed to be 0-indexed.
+
+        Parameters
+        ----------
+        labels : list
+            a list of the label(s) whose integer indexes should be returned.
+        axis : str, default='N'
+            can be any of {'T', 'N', 'F'}. 
+            - If 'T', the values in the `labels` parameter are interpreted as time labels (as stored in `self.label_dict_['T']`). 
+            - If 'N', the values in the `labels` parameter are interpreted as entity labels (as stored in `self.label_dict_['N']`). 
+            - If 'F', the values in the `labels` parameter are interpreted as feature labels (as stored in `self.label_dict_['F']`). 
+    
+        Returns
+        -------
+        list
+            a list of the integer indexes of the labels in the given axis dimension.
+        """ 
+
+        return [self.label_dict_[axis].index(label) for label in labels]
+
+    def get_label_of_index(self, indexes: List[int], axis: str = 'N') -> List[str]:
+        """
+        function to return the labels of some given integer indexes as labelled in `self.label_dict_`. The indexes are assumed to be 0-indexed.
+
+        Parameters
+        ----------
+        indexes : list
+            a list of the index(es) whose labels should be returned.
+        axis : str, default='N'
+            can be any of {'T', 'N', 'F'}. 
+            - If 'T', the values in the `indexes` parameter are interpreted as the time indexes whose labels (as stored in `self.label_dict_['T']`) should be returned. 
+            - If 'N', the values in the `indexes` parameter are interpreted as the entity indexes whose labels (as stored in `self.label_dict_['N']`) should be returned. 
+            - If 'F', the values in the `indexes` parameter are interpreted as the feature indexes whose labels (as stored in `self.label_dict_['F']`) should be returned. 
+    
+        Returns
+        -------
+        list
+            a list of the labels of the given integer indexes in the given axis dimension.
+        """ 
+        
+        return list(pd.Series(self.label_dict_[axis]).values[indexes])
+    
     @property
     def n_changes_(self) -> int:
         """
         returns the total number of label changes
         """
         return np.sum(self._get_changes())
```

### Comparing `tscluster-1.0.2/tscluster/interface.py` & `tscluster-1.0.3/tscluster/interface.py`

 * *Files identical despite different names*

### Comparing `tscluster-1.0.2/tscluster/metrics/metrics.py` & `tscluster-1.0.3/tscluster/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `tscluster-1.0.2/tscluster/opttscluster/optcluster.py` & `tscluster-1.0.3/tscluster/opttscluster/optcluster.py`

 * *Files identical despite different names*

### Comparing `tscluster-1.0.2/tscluster/opttscluster/opttscluster.py` & `tscluster-1.0.3/tscluster/opttscluster/opttscluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,27 +19,25 @@
 
     """
     Class for optimal time-series clustering. Throughout this doc and code, 'z' refers to cluster centers, while 'c' to label assignment.
     This creates an OptTSCluster object
 
     Parameters
     -----------
-    k: int
+    n_clusters: int
         number of clusters
     scheme: {'z0c0', 'z0c1', 'z1c0', 'z1c1'}, default='z1c0'
         The scheme to use for tsclustering. Could be one of:
             - 'z0c0' means fixed center, fixed assignment
             - 'z0c1' means fixed center, changing assignment
             - 'z1c0' means changing center, fixed assignment
             - 'z1c1' means changing center, changing assignment
         Scheme needs to be a dynamic label assignment scheme (either 'z1c1' or 'z0c1') when using constrained cluster change (either with `n_allow_assignment_change` or `lagrangian_multiplier`)
     n_allow_assignment_change: int or None, default=None
         total number of label changes to allow
-    lagrangian_multiplier: float, default=0.0
-        The penalty term for constrained label changes. Value should be in range [0, np.inf], the higher the value, the less the number of label changes allowed. When used, `n_allow_assignment_change` is ignored.
     use_sum_distance: bool, default=False
         Indicate if to use sum of distance to cluster as the objective. This is the sum of the distances between points in a time series
         and their centroids. 
     warm_start: bool, default=True
         Indicates if to use k-means to initialize the centroids (Z) and their assignments (C).
     use_MILP_centroid: bool, default=True
         If True, cluster_centers_ atrribute will be cluster centers obtained from MILP solution, else the average of the 
@@ -55,31 +53,30 @@
     label_dict_
     n_changes_
     
     """
 
     def __init__(
             self, 
-            k: int, 
+            n_clusters: int, 
             scheme: str = 'z1c0', 
             *,
-            n_allow_assignment_change: None|int = None, 
-            lagrangian_multiplier: float = 0.0, 
+            n_allow_assignment_change: None|int = None,  
             use_sum_distance: bool = False,
             warm_start: bool = True, 
             use_MILP_centroid: bool = True,
             random_state: None|int = None
             ) -> None:
 
-        self.k = k
+        self.k = n_clusters
         self.scheme = scheme.lower()
         self.n_allow_assignment_change = n_allow_assignment_change
         self.is_Z_positive = True
         self.is_tight_constraints = True 
-        self.lagrangian_multiplier = lagrangian_multiplier
+        self.lagrangian_multiplier = 0.0
         self.use_sum_distance = use_sum_distance
         self.warm_start = warm_start
         self.normalise_assignment_penalty = True
         self.strictly_n_allow_assignment_change = False
         self.use_MILP_centroid = use_MILP_centroid
         self.use_full_constraints = True
         self.IFrac = 0.2
@@ -461,15 +458,15 @@
     def get_model_size(self,
             X: npt.NDArray[np.float64]
             ) -> Tuple:
         
         """
         Method to return the size of the model as a tuple of (v, c). Wehre v is the number of variables, and c is the number of constraints
 
-        Paramters
+        Parameters
         ---------
         X : numpy array
             Input time series data. Should be a 3 dimensional array in TNF fromat.        
 
         Returns
         -------
         number of variable
```

### Comparing `tscluster-1.0.2/tscluster/preprocessing/interface.py` & `tscluster-1.0.3/tscluster/preprocessing/interface.py`

 * *Files identical despite different names*

### Comparing `tscluster-1.0.2/tscluster/preprocessing/scaler.py` & `tscluster-1.0.3/tscluster/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `tscluster-1.0.2/tscluster/preprocessing/utils.py` & `tscluster-1.0.3/tscluster/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `tscluster-1.0.2/tscluster/tskmeans/tsglobalkmeans.py` & `tscluster-1.0.3/tscluster/tskmeans/tsglobalkmeans.py`

 * *Files identical despite different names*

### Comparing `tscluster-1.0.2/tscluster/tskmeans/tskmeans.py` & `tscluster-1.0.3/tscluster/tskmeans/tskmeans.py`

 * *Files identical despite different names*

### Comparing `tscluster-1.0.2/tscluster/tsplot/tsplot.py` & `tscluster-1.0.3/tscluster/tsplot/tsplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         entities_labels: List[str]|None = None,
         label_dict: dict|None = None,
         annot_fontsize: float|int = 10,
         show_all_entities: bool = True,
         figsize: Tuple[float, float] | None = None,
         shape_of_subplot: Tuple[int, int]|None = None, 
         xlabel: str|None = 'timesteps', 
-        ylabel: str|None = 'val',
+        ylabel: str|None = 'value',
         cluster_labels: List[str]|None = None,
         title_list: List[str]|None = None,
         show_all_xticklabels: bool = True, 
         x_rotation: float|int = 45,
         show_X_marker: bool = False,
         show_cluster_center_marker: bool = False,
         ) -> Tuple[matplotlib.figure.Figure, List[matplotlib.axes.Axes]]:
@@ -110,15 +110,15 @@
     X : numpy array, default=None
         The time series data in TNF format.
     cluster_centers : numpy array, default=None
         If numpy array, it is expected to be a 3D in TNF format. Here, N is the number of clusters. 
         If 2-D array, then it is interpreted as a K x F array where K is the number of clusters, and F is the number of features. Suitable for fixed cluster centers clustering.
     labels : numpy array, default=None
         It is expected to be a 2D array of shape (N, T) . Where N is the number of entities and T is the number of time steps. The value of the ith row at the t-th column is the label (cluster index) entity i was assigned to at time t.
-        If 1-D array, it is interpreted as an array of length N. Where N is the number of entities. In such case, the i-th element is the cluster the i-th entit was assigned to across all time steps. Suitable for fixed assignment clustering.
+        If 1-D array, it is interpreted as an array of length N. Where N is the number of entities. In such case, the i-th element is the cluster the i-th entity was assigned to across all time steps. Suitable for fixed assignment clustering.
     entity_idx : list, default=None 
         list of index of entities to display in the plot. If `show_all_entities` is True, `entity_idx` will be interpreted as the index of entities to be annonated.
     entities_labels : list, default=None
         list of labels for annotating the entities in `entity_idx`. If None, then labels of `entity_idx` in `label_dict` are used.
     label_dict dict, default=None
         a dictionary whose keys are 'T', 'N', and 'F' (which are the number of time steps, entities, and features respectively). Value of each key is a list such that the value of key:
         - 'T' is a list of names/labels of each time step to be used as index of each dataframe. If None, range(0, T) is used. Where T is the number of time steps in the fitted data
```

### Comparing `tscluster-1.0.2/tscluster.egg-info/SOURCES.txt` & `tscluster-1.0.3/tscluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

