# Comparing `tmp/trustee-1.1.5.tar.gz` & `tmp/trustee-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustee-1.1.5.tar", max compression
+gzip compressed data, was "trustee-1.1.6.tar", max compression
```

## Comparing `trustee-1.1.5.tar` & `trustee-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35149 2020-09-22 21:40:48.095653 trustee-1.1.5/LICENSE
--rw-r--r--   0        0        0     4847 2023-04-14 15:25:36.814142 trustee-1.1.5/README.md
--rw-r--r--   0        0        0     1186 2023-10-18 23:10:28.716988 trustee-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       54 2022-08-27 20:26:35.936347 trustee-1.1.5/trustee/__init__.py
--rw-r--r--   0        0        0       22 2023-10-18 23:10:41.263779 trustee-1.1.5/trustee/_version.py
--rw-r--r--   0        0        0        0 2022-08-27 20:26:23.511700 trustee-1.1.5/trustee/enums/__init__.py
--rw-r--r--   0        0        0      191 2020-08-25 15:03:18.309208 trustee-1.1.5/trustee/enums/feature_type.py
--rw-r--r--   0        0        0    26751 2023-06-19 19:57:20.263960 trustee-1.1.5/trustee/main.py
--rw-r--r--   0        0        0        0 2022-08-27 20:26:16.668910 trustee-1.1.5/trustee/report/__init__.py
--rw-r--r--   0        0        0    24655 2022-08-28 00:39:48.253906 trustee-1.1.5/trustee/report/plot.py
--rw-r--r--   0        0        0    60660 2023-06-19 19:45:17.222256 trustee-1.1.5/trustee/report/trust.py
--rw-r--r--   0        0        0        0 2022-08-27 20:26:08.556222 trustee-1.1.5/trustee/utils/__init__.py
--rw-r--r--   0        0        0    15272 2023-06-19 18:18:04.426391 trustee-1.1.5/trustee/utils/const.py
--rw-r--r--   0        0        0     6170 2023-06-19 19:55:09.667376 trustee-1.1.5/trustee/utils/dataset.py
--rw-r--r--   0        0        0      966 2023-06-19 18:17:08.078947 trustee-1.1.5/trustee/utils/log.py
--rw-r--r--   0        0        0      880 2021-06-29 22:34:28.093972 trustee-1.1.5/trustee/utils/persist.py
--rw-r--r--   0        0        0    13134 2022-08-07 22:44:17.450841 trustee-1.1.5/trustee/utils/plot.py
--rw-r--r--   0        0        0     2972 2023-04-14 14:35:56.230834 trustee-1.1.5/trustee/utils/rootpath.py
--rw-r--r--   0        0        0     5808 2023-10-18 23:16:13.672224 trustee-1.1.5/trustee/utils/tree.py
--rw-r--r--   0        0        0     6035 1970-01-01 00:00:00.000000 trustee-1.1.5/setup.py
--rw-r--r--   0        0        0     6305 1970-01-01 00:00:00.000000 trustee-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-09-22 21:40:48.095653 trustee-1.1.6/LICENSE
+-rw-r--r--   0        0        0     4847 2023-04-14 15:25:36.814142 trustee-1.1.6/README.md
+-rw-r--r--   0        0        0     1186 2024-05-20 22:06:53.658030 trustee-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0       54 2022-08-27 20:26:35.936347 trustee-1.1.6/trustee/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-20 22:07:58.609250 trustee-1.1.6/trustee/_version.py
+-rw-r--r--   0        0        0        0 2022-08-27 20:26:23.511700 trustee-1.1.6/trustee/enums/__init__.py
+-rw-r--r--   0        0        0      191 2020-08-25 15:03:18.309208 trustee-1.1.6/trustee/enums/feature_type.py
+-rw-r--r--   0        0        0    26869 2024-05-20 22:06:53.659743 trustee-1.1.6/trustee/main.py
+-rw-r--r--   0        0        0        0 2022-08-27 20:26:16.668910 trustee-1.1.6/trustee/report/__init__.py
+-rw-r--r--   0        0        0    24767 2024-05-20 22:06:53.661094 trustee-1.1.6/trustee/report/plot.py
+-rw-r--r--   0        0        0    61403 2024-05-20 22:06:53.663353 trustee-1.1.6/trustee/report/trust.py
+-rw-r--r--   0        0        0        0 2022-08-27 20:26:08.556222 trustee-1.1.6/trustee/utils/__init__.py
+-rw-r--r--   0        0        0    15272 2023-06-19 18:18:04.426391 trustee-1.1.6/trustee/utils/const.py
+-rw-r--r--   0        0        0     6170 2023-06-19 19:55:09.667376 trustee-1.1.6/trustee/utils/dataset.py
+-rw-r--r--   0        0        0      966 2023-06-19 18:17:08.078947 trustee-1.1.6/trustee/utils/log.py
+-rw-r--r--   0        0        0      880 2021-06-29 22:34:28.093972 trustee-1.1.6/trustee/utils/persist.py
+-rw-r--r--   0        0        0    13134 2022-08-07 22:44:17.450841 trustee-1.1.6/trustee/utils/plot.py
+-rw-r--r--   0        0        0     2972 2023-04-14 14:35:56.230834 trustee-1.1.6/trustee/utils/rootpath.py
+-rw-r--r--   0        0        0     5808 2023-10-18 23:16:13.672224 trustee-1.1.6/trustee/utils/tree.py
+-rw-r--r--   0        0        0     6035 1970-01-01 00:00:00.000000 trustee-1.1.6/setup.py
+-rw-r--r--   0        0        0     6305 1970-01-01 00:00:00.000000 trustee-1.1.6/PKG-INFO
```

### Comparing `trustee-1.1.5/LICENSE` & `trustee-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trustee-1.1.5/README.md` & `trustee-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `trustee-1.1.5/pyproject.toml` & `trustee-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trustee"
-version = "1.1.5"
+version = "1.1.6"
 readme = "README.md"
 description = "This package implements the Trustee framework to extract decision tree explanation from black-box ML models."
 homepage = "https://trusteeml.github.io"
 repository = "https://github.com/TrusteeML/trustee"
 authors = ["Arthur Selle Jacobs <asjacobs@inf.ufrgs.br>"]
 packages = [ { include = "trustee"} ]
 classifiers = [
```

### Comparing `trustee-1.1.5/trustee/main.py` & `trustee-1.1.6/trustee/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,16 @@
         self._y_test = []
 
         self._best_student = None
         self._features = None
         self._nodes = None
         self._branches = None
 
+        self._student_use_features: np.array = []
+
     @abc.abstractmethod
     def _score(self, y_true, y_pred):
         """
         Score function for student models. Compares the ground-truth predictions
         of a blackbox model with the predictions of a student model.
 
         Parameters
@@ -198,14 +200,16 @@
         if len(X) != len(y):
             raise ValueError("Features (X) and target (y) values should have the same length.")
 
         # convert data to np array to facilitate processing
         X = convert_to_df(X)
         y = convert_to_series(y)
 
+        self._student_use_features = use_features if use_features is not None else np.arange(0, len(X.columns))
+
         # split input array to train DTs and evaluate agreement
         self._X_train, self._X_test, self._y_train, self._y_test = train_test_split(X, y, train_size=train_size)
 
         features = self._X_train
         targets = convert_to_series(getattr(self.expert, predict_method_name)(self._X_train))
 
         if hasattr(targets, "shape") and len(targets.shape) >= 2:
@@ -240,20 +244,16 @@
                     )
 
                 samples_idxs = np.random.choice(dataset_size, size=size, replace=False)
                 X_iter, y_iter = features.iloc[samples_idxs], targets.iloc[samples_idxs]
                 X_iter_train, X_iter_test, y_iter_train, y_iter_test = train_test_split(
                     X_iter, y_iter, train_size=train_size
                 )
-
-                X_train_student = X_iter_train
-                X_test_student = X_iter_test
-                if use_features is not None:
-                    X_train_student = X_iter_train.iloc[:, use_features]
-                    X_test_student = X_iter_test.iloc[:, use_features]
+                X_train_student = X_iter_train.iloc[:, self._student_use_features]
+                X_test_student = X_iter_test.iloc[:, self._student_use_features]
 
                 # Step 2: Training DecisionTreeRegressor with sampled data
                 student.fit(X_train_student.values, y_iter_train.values)
                 student_pred = student.predict(X_test_student.values)
 
                 if verbose:
                     self.log(
@@ -357,16 +357,16 @@
                 agreement.append([])
                 # Apply top-k pruning before calculating agreement
                 base_tree = top_k_prune(self._top_students[i][0], top_k=top_k)
                 for j, _ in enumerate(self._top_students):
                     # Apply top-k pruning before calculating agreement
                     iter_tree = top_k_prune(self._top_students[j][0], top_k=top_k)
 
-                    iter_y_pred = iter_tree.predict(self._X_test.values)
-                    base_y_pred = base_tree.predict(self._X_test.values)
+                    iter_y_pred = iter_tree.predict(self._X_test.iloc[:, self._student_use_features].values)
+                    base_y_pred = base_tree.predict(self._X_test.iloc[:, self._student_use_features].values)
 
                     agreement[i].append(self._score(iter_y_pred, base_y_pred))
 
                 # Save complete dt, top-k prune dt, mean agreement and fidelity
                 self._stable_students.append(
                     (
                         self._top_students[i][0],
```

### Comparing `trustee-1.1.5/trustee/report/plot.py` & `trustee-1.1.6/trustee/report/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,14 +495,19 @@
         ylabel="Metric (%)",
         labels=["Blackbox Score", "DT Fidelity"],
         path=f"{output_dir}/accuracy_by_feature_removed.pdf",
     )
 
 
 def plot_distribution(X, y, top_branches, output_dir, aggregate=False, feature_names=[], class_names=[]):
+    if isinstance(X, pd.DataFrame):
+        X = X.values
+    if isinstance(y, pd.Series):
+        y = y.values
+
     """Plots the distribution of the data based on the top branches"""
     if not np.array(X).size or not np.array(y).size or not np.array(top_branches).size:
         return
 
     plots_output_dir = f"{output_dir}/dist" if not aggregate else f"{output_dir}/aggr_dist"
     if not os.path.exists(plots_output_dir):
         os.makedirs(plots_output_dir)
```

### Comparing `trustee-1.1.5/trustee/report/trust.py` & `trustee-1.1.6/trustee/report/trust.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         skip_retrain=False,
         top_k=10,
         logger=None,
         verbose=False,
         class_names=None,
         feature_names=None,
         is_classify=True,
+        use_features=None,
     ):
         """
         Builds Trust Report for given blackbox model using the Trustee method
         to extract whitebox explanations as Decision Trees.
 
         Parameters
         ----------
@@ -171,14 +172,19 @@
             List of class names to use when plotting decision trees and graphs.
 
         feature_names: array-like of str, default=None,
             List of feature names to use when plotting decision trees and graphs.
 
         is_classify: bool, default=True,
             Whether given blackbox is a classifier or regressor. The outputted plots change depending on chosen value.
+
+        use_features: array-like, default=None
+            Array-like of integers representing the indexes of features from the `X` training samples.
+            If not None, only the features indicated by the provided indexes will be used to train the
+            student decision tree model.
         """
         self.blackbox = blackbox
         self.X = X
         self.y = y
         self.X_train = X_train
         self.X_test = X_test
         self.y_train = y_train
@@ -198,14 +204,15 @@
         self.skip_retrain = skip_retrain
         self.top_k = top_k
         self.logger = logger
         self.verbose = verbose
         self.class_names = class_names
         self.feature_names = feature_names
         self.is_classify = is_classify
+        self.use_features = use_features if use_features is not None else np.arange(0, X_train.shape[1])
 
         self.step = 0
         """
             Used for progress bar.
 
             total_steps = 
                 _prepare_data (1) + 
@@ -882,26 +889,27 @@
             num_stability_iter=stability_iter,
             samples_size=self.trustee_sample_size,
             predict_method_name=self.predict_method_name,
             max_leaf_nodes=trustee_max_leaf_nodes if trustee_max_leaf_nodes else self.trustee_max_leaf_nodes,
             max_depth=trustee_max_depth if trustee_max_depth else self.trustee_max_depth,
             ccp_alpha=trustee_ccp_alpha if trustee_ccp_alpha else self.trustee_ccp_alpha,
             verbose=self.verbose,
+            use_features=self.use_features,
         )
 
         if self.verbose:
             log("Done!")
 
         dt, min_dt, agreement, reward = trustee.explain()
         if self.verbose:
             log(f"Model explanation training (agreement, fidelity): ({agreement}, {reward})")
             log(f"Top-k Prunned explanation size: {min_dt.tree_.node_count}")
 
-        dt_y_pred = dt.predict(X_test.values)
-        min_dt_y_pred = min_dt.predict(X_test.values)
+        dt_y_pred = dt.predict(X_test.iloc[:, self.use_features].values)
+        min_dt_y_pred = min_dt.predict(X_test.iloc[:, self.use_features].values)
 
         if self.verbose:
             log("Model explanation global fidelity report:")
             log(self._score_report(y_pred, dt_y_pred))
             log("Top-k Model explanation global fidelity report:")
             log(self._score_report(y_pred, min_dt_y_pred))
 
@@ -938,15 +946,15 @@
 
     def _collect_blackbox(self):
         """Collects information on analyzed blackbox"""
         log = self.logger.log if self.logger else print
         if self.verbose:
             log("Collecting blackbox information...")
 
-        self.bb_n_input_features = len(self.X_train.columns)
+        self.bb_n_input_features = self.X_train.shape[1]
         self.bb_n_output_classes = len(np.unique(self.y_train))
         if self.verbose:
             log("Done!")
 
         self._progress()
 
     def _collect_trustee(self):
@@ -990,15 +998,15 @@
 
         self.branch_iter = []
         for top_k in np.arange(1, self.max_dt.get_n_leaves()):
             if self.verbose:
                 log(f"Iteration {top_k}/{self.max_dt.get_n_leaves()}")
 
             pruned_dt = self.trustee.prune(top_k=top_k)
-            pruned_dt_y_pred = pruned_dt.predict(self.X_test.values)
+            pruned_dt_y_pred = pruned_dt.predict(self.X_test.iloc[:, self.use_features].values)
 
             self.branch_iter.append(
                 {
                     "top_k": top_k,
                     "dt": pruned_dt,
                     "y_pred": self.y_pred,
                     "dt_y_pred": pruned_dt_y_pred,
@@ -1052,15 +1060,15 @@
 
         self.top_k_prune_iter = []
         for top_k in np.arange(1, self.num_pruning_iter + 1):
             if self.verbose:
                 log(f"Iteration {top_k}/{self.num_pruning_iter}")
 
             pruned_dt = self.trustee.prune(top_k=top_k)
-            pruned_dt_y_pred = pruned_dt.predict(self.X_test.values)
+            pruned_dt_y_pred = pruned_dt.predict(self.X_test.iloc[:, self.use_features].values)
 
             self.top_k_prune_iter.append(
                 {
                     "top_k": top_k,
                     "dt": pruned_dt,
                     "y_pred": self.y_pred,
                     "dt_y_pred": pruned_dt_y_pred,
@@ -1186,17 +1194,17 @@
 
         i = 0
         n_features_removed = 0
         top_feature_to_remove = self.max_dt_top_features[0][0]
         X_train_iter = self.X_train.copy()
         X_test_iter = self.X_test.copy()
 
-        while i < self.max_iter and n_features_removed < self.bb_n_input_features - 1:
+        while i < self.max_iter and n_features_removed < len(self.use_features) - 1:
             if self.verbose:
-                log(f"Iteration {i + 1}/{min(self.max_iter, self.bb_n_input_features)}")
+                log(f"Iteration {i + 1}/{min(self.max_iter, len(self.use_features))}")
 
             # remove most significant feature
             X_train_iter.iloc[:, top_feature_to_remove] = 0
             X_test_iter.iloc[:, top_feature_to_remove] = 0
 
             n_features_removed += 1
             _, y_pred, dt, dt_y_pred, _, _ = self._fit_and_explain(X_train=X_train_iter, X_test=X_test_iter)
@@ -1242,27 +1250,27 @@
         log = self.logger.log if self.logger else print
         if self.verbose:
             log("Saving decision trees...")
 
         dot_data = tree.export_graphviz(
             self.max_dt,
             class_names=self.class_names,
-            feature_names=self.feature_names,
+            feature_names=[self.feature_names[i] for i in self.use_features],
             filled=True,
             rounded=True,
             special_characters=True,
         )
         graph = graphviz.Source(dot_data)
         graph.render(f"{output_dir}/trust_report_dt")
 
         if self.min_dt:
             dot_data = tree.export_graphviz(
                 self.min_dt,
                 class_names=self.class_names,
-                feature_names=self.feature_names,
+                feature_names=[self.feature_names[i] for i in self.use_features],
                 filled=True,
                 rounded=True,
                 special_characters=True,
             )
             graph = graphviz.Source(dot_data)
             graph.render(f"{output_dir}/trust_report_pruned_dt")
 
@@ -1415,50 +1423,50 @@
             [{"type": "Top-k Branches", "iter": self.branch_iter}],
             plots_output_dir,
             filename="branches",
         )
 
         plot_stability(
             self.stability_iter,
-            self.X_test,
+            self.X_test.iloc[:, self.use_features],
             self.y_test,
             self.max_dt,
             "max_dt",
             self.max_dt_top_branches,
             plots_output_dir,
             class_names=self.class_names,
             is_classify=self.is_classify,
         )
 
         plot_stability(
             self.stability_iter,
-            self.X_test,
+            self.X_test.iloc[:, self.use_features],
             self.y_test,
             self.min_dt,
             "min_dt",
             self.max_dt_top_branches,
             plots_output_dir,
             class_names=self.class_names,
             is_classify=self.is_classify,
         )
 
         plot_stability_heatmap(
             self.stability_iter,
-            self.X_test,
+            self.X_test.iloc[:, self.use_features],
             self.y_test,
             "max_dt",
             self.max_dt_top_branches,
             plots_output_dir,
             class_names=self.class_names,
             is_classify=self.is_classify,
         )
 
         plot_stability_heatmap(
             self.stability_iter,
-            self.X_test,
+            self.X_test.iloc[:, self.use_features],
             self.y_test,
             "min_dt",
             self.max_dt_top_branches,
             plots_output_dir,
             class_names=self.class_names,
             is_classify=self.is_classify,
         )
```

### Comparing `trustee-1.1.5/trustee/utils/const.py` & `trustee-1.1.6/trustee/utils/const.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.5/trustee/utils/dataset.py` & `trustee-1.1.6/trustee/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.5/trustee/utils/log.py` & `trustee-1.1.6/trustee/utils/log.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.5/trustee/utils/persist.py` & `trustee-1.1.6/trustee/utils/persist.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.5/trustee/utils/plot.py` & `trustee-1.1.6/trustee/utils/plot.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.5/trustee/utils/rootpath.py` & `trustee-1.1.6/trustee/utils/rootpath.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.5/trustee/utils/tree.py` & `trustee-1.1.6/trustee/utils/tree.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.5/setup.py` & `trustee-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'setuptools>=57.0.0,<58.0.0',
  'sphinx-gallery>=0.11.1,<0.12.0',
  'sphinxemoji>=0.2.0,<0.3.0',
  'termcolor>=1.1.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'trustee',
-    'version': '1.1.5',
+    'version': '1.1.6',
     'description': 'This package implements the Trustee framework to extract decision tree explanation from black-box ML models.',
     'long_description': '<img src="https://github.com/TrusteeML/trustee/blob/master/docs/_static/logo.png?raw=true" alt="Trustee" width="400"/>\n\n[![Downloads](https://static.pepy.tech/personalized-badge/trustee?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/trustee)\n\n\nThis package implements the `trustee` framework to extract decision tree explanation from black-box ML models.\nFor more information, please visit the [documentation website](https://trusteeml.github.io).\n\nStandard AI/ML development pipeline extended by Trustee.\n<img alt="Trustee" src="https://github.com/TrusteeML/trustee/blob/master/docs/_static/flowchart.png?raw=true"  width="800">\n\nGetting Started\n---------------\n\nThis section contains basic information and instructions to get started with Trustee.\n\n### Python Version\n\nTrustee supports `Python >=3.7`.\n\n### Install Trustee\n\nUse the following command to install Trustee:\n\n```\n$ pip install trustee\n```\n\n### Sample Code\n\n```\nfrom sklearn import datasets\nfrom sklearn.ensemble import RandomForestClassifier\nfrom sklearn.model_selection import train_test_split\nfrom sklearn.metrics import classification_report\n\nfrom trustee import ClassificationTrustee\n\nX, y = datasets.load_iris(return_X_y=True)\nX_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.30)\n\nclf = RandomForestClassifier(n_estimators=100)\nclf.fit(X_train, y_train)\ny_pred = clf.predict(X_test)\n\ntrustee = ClassificationTrustee(expert=clf)\ntrustee.fit(X_train, y_train, num_iter=50, num_stability_iter=10, samples_size=0.3, verbose=True)\ndt, pruned_dt, agreement, reward = trustee.explain()\ndt_y_pred = dt.predict(X_test)\n\nprint("Model explanation global fidelity report:")\nprint(classification_report(y_pred, dt_y_pred))\nprint("Model explanation score report:")\nprint(classification_report(y_test, dt_y_pred))\n```\n\n### Usage Examples\n\nFor simple usage examples of Trustee and TrustReport, please check the `examples/` directory.\n\n### Other Use Cases\n\nFor other examples and use cases of how Trustee can used to scrutinize ML models, listed in the table below, please check our [Use Cases repository](https://github.com/TrusteeML/emperor).\n\n | Use Case           | Description                                                                                                                                                 |\n | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |\n | heartbleed\\_case/  | Trustee application to a Random Forest Classifier for an Intrustion Detection System, trained with CIC-IDS-2017 dataset pre-computed features.              |\n | kitsune\\_case/     | Trustee application to Kitsune model for anomaly detection in network traffic, trained with features extracted from Kitsune\\\'s Mirai attack trace.          |\n | iot\\_case/         | Trustee application to Random Forest Classifier to distguish IoT devices, trained with features extracted from the pcaps from the UNSW IoT Dataset.         |\n | moon\\_star\\_case/  | Trustee application to Neural Network Moon and Stars Shortcut learning toy example.                                                                         |\n | nprint\\_ids\\_case/ | Trustee application to the nPrintML AutoGluon Tabular Predictor for an Intrustion Detection System, also trained using pcaps from the CIC-IDS-2017 dataset. |\n | nprint\\_os\\_case/  | Trustee application to the nPrintML AutoGluon Tabular Predictor for OS Fingerprinting, also trained using with pcaps from the CIC-IDS-2017 dataset.         |\n | pensieve\\_case/    | Trustee application to the Pensieve RL model for adaptive bit-rate prediction, and comparison to related work Metis.                                        |\n | vpn\\_case/         | Trustee application the 1D-CNN trained to detect VPN traffic trained with the ISCX VPN-nonVPN dataset.                                                      |\n\n### Supported AI/ML Libraries\n\n | Library      | Supported          |\n | ------------ | ------------------ |\n | scikit-learn | :white_check_mark: |\n | Keras        | :white_check_mark: |\n | Tensorflow   | :white_check_mark: |\n | PyTorch      | :white_check_mark: |\n | AutoGluon    | :white_check_mark: |\n\n## Citing us\n\n```\n@inproceedings{Jacobs2022,\n\ttitle        = {AI/ML and Network Security: The Emperor has no Clothes},\n\tauthor       = {A. S. Jacobs and R. Beltiukov and W. Willinger and R. A. Ferreira and A. Gupta and L. Z. Granville},\n\tyear         = 2022,\n\tbooktitle    = {Proceedings of the 2022 ACM SIGSAC Conference on Computer and Communications Security},\n\tlocation     = {Los Angeles, CA, USA},\n\tpublisher    = {Association for Computing Machinery},\n\taddress      = {New York, NY, USA},\n\tseries       = {CCS \'22}\n}\n```\n',
     'author': 'Arthur Selle Jacobs',
     'author_email': 'asjacobs@inf.ufrgs.br',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://trusteeml.github.io',
```

### Comparing `trustee-1.1.5/PKG-INFO` & `trustee-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustee
-Version: 1.1.5
+Version: 1.1.6
 Summary: This package implements the Trustee framework to extract decision tree explanation from black-box ML models.
 Home-page: https://trusteeml.github.io
 Author: Arthur Selle Jacobs
 Author-email: asjacobs@inf.ufrgs.br
 Requires-Python: >=3.7
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

