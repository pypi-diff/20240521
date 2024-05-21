# Comparing `tmp/glook-1.2.0b1.tar.gz` & `tmp/glook-1.2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glook-1.2.0b1.tar", last modified: Thu May  9 19:02:01 2024, max compression
+gzip compressed data, was "glook-1.2.1b1.tar", last modified: Tue May 21 16:27:47 2024, max compression
```

## Comparing `glook-1.2.0b1.tar` & `glook-1.2.1b1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.258134 glook-1.2.0b1/
--rw-rw-rw-   0        0        0     7228 2024-05-09 19:02:01.255138 glook-1.2.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     5322 2024-04-27 21:12:46.000000 glook-1.2.0b1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.012161 glook-1.2.0b1/glook/
--rw-rw-rw-   0        0        0     3502 2024-05-09 16:44:31.000000 glook-1.2.0b1/glook/GLook.py
--rw-rw-rw-   0        0        0       51 2024-03-25 17:39:42.000000 glook-1.2.0b1/glook/__init__.py
--rw-rw-rw-   0        0        0      339 2024-03-25 18:24:01.000000 glook-1.2.0b1/glook/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.224290 glook-1.2.0b1/glook/pages/
--rw-rw-rw-   0        0        0    26240 2024-05-05 06:31:15.000000 glook-1.2.0b1/glook/pages/10_Unsupervised_learning.py
--rw-rw-rw-   0        0        0   107673 2024-05-05 05:42:46.000000 glook-1.2.0b1/glook/pages/11_Custom_Model_Training.py
--rw-rw-rw-   0        0        0    31057 2024-05-05 18:13:44.000000 glook-1.2.0b1/glook/pages/12_Supervised_Deployment_Demo.py
--rw-rw-rw-   0        0        0    33654 2024-05-08 18:38:27.000000 glook-1.2.0b1/glook/pages/13_Unsupervised_Deployment_Demo.py
--rw-rw-rw-   0        0        0     6483 2024-05-09 16:55:20.000000 glook-1.2.0b1/glook/pages/1_General_Data_Insights.py
--rw-rw-rw-   0        0        0    20207 2024-05-09 18:30:57.000000 glook-1.2.0b1/glook/pages/2_Univariate_Analysis.py
--rw-rw-rw-   0        0        0     8173 2024-05-09 16:56:35.000000 glook-1.2.0b1/glook/pages/3_Bivariate_Analysis.py
--rw-rw-rw-   0        0        0     8067 2024-05-09 16:58:02.000000 glook-1.2.0b1/glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-   0        0        0   114361 2024-05-09 17:39:14.000000 glook-1.2.0b1/glook/pages/5_Pre_Processing.py
--rw-rw-rw-   0        0        0     4099 2024-05-09 17:41:15.000000 glook-1.2.0b1/glook/pages/6_Split_Data.py
--rw-rw-rw-   0        0        0     4588 2024-04-11 19:05:58.000000 glook-1.2.0b1/glook/pages/7_Dimensionality_Reduction.py
--rw-rw-rw-   0        0        0    60527 2024-05-05 17:49:18.000000 glook-1.2.0b1/glook/pages/8_Supervised_Learning.py
-drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.164924 glook-1.2.0b1/glook.egg-info/
--rw-rw-rw-   0        0        0     7228 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      888 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      211 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.234409 glook-1.2.0b1/look/
--rw-rw-rw-   0        0        0     3228 2024-05-02 17:40:02.000000 glook-1.2.0b1/look/GLook.py
--rw-rw-rw-   0        0        0       51 2024-03-25 17:39:42.000000 glook-1.2.0b1/look/__init__.py
--rw-rw-rw-   0        0        0      339 2024-03-25 18:24:01.000000 glook-1.2.0b1/look/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.248962 glook-1.2.0b1/look/pages/
--rw-rw-rw-   0        0        0     6157 2024-05-02 17:40:35.000000 glook-1.2.0b1/look/pages/1_General_Data_Insights.py
--rw-rw-rw-   0        0        0    19802 2024-05-02 17:43:01.000000 glook-1.2.0b1/look/pages/2_Univariate_Analysis.py
--rw-rw-rw-   0        0        0     7813 2024-05-02 17:43:17.000000 glook-1.2.0b1/look/pages/3_Bivariate_Analysis.py
--rw-rw-rw-   0        0        0     7707 2024-05-02 17:43:33.000000 glook-1.2.0b1/look/pages/4_Trivariate_Analysis.py
--rw-rw-rw-   0        0        0       42 2024-05-09 19:02:01.258134 glook-1.2.0b1/setup.cfg
--rw-rw-rw-   0        0        0     2507 2024-05-09 19:01:54.000000 glook-1.2.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:47.975306 glook-1.2.1b1/
+-rw-rw-rw-   0        0        0    11088 2024-05-21 16:27:47.972320 glook-1.2.1b1/PKG-INFO
+-rw-rw-rw-   0        0        0     9182 2024-05-21 16:10:20.000000 glook-1.2.1b1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:47.873099 glook-1.2.1b1/glook/
+-rw-rw-rw-   0        0        0     3501 2024-05-20 15:16:08.000000 glook-1.2.1b1/glook/GLook.py
+-rw-rw-rw-   0        0        0       51 2024-03-25 17:39:42.000000 glook-1.2.1b1/glook/__init__.py
+-rw-rw-rw-   0        0        0      339 2024-03-25 18:24:01.000000 glook-1.2.1b1/glook/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:47.946305 glook-1.2.1b1/glook/pages/
+-rw-rw-rw-   0        0        0    26541 2024-05-13 18:27:01.000000 glook-1.2.1b1/glook/pages/10_Unsupervised_learning.py
+-rw-rw-rw-   0        0        0   124762 2024-05-13 18:41:32.000000 glook-1.2.1b1/glook/pages/11_Custom_Model_Training.py
+-rw-rw-rw-   0        0        0    32015 2024-05-12 18:37:30.000000 glook-1.2.1b1/glook/pages/12_Supervised_Deployment_Demo.py
+-rw-rw-rw-   0        0        0    34782 2024-05-13 18:37:05.000000 glook-1.2.1b1/glook/pages/13_Unsupervised_Deployment_Demo.py
+-rw-rw-rw-   0        0        0     4690 2024-05-18 16:50:52.000000 glook-1.2.1b1/glook/pages/1_General_Data_Insights.py
+-rw-rw-rw-   0        0        0    20295 2024-05-12 06:38:30.000000 glook-1.2.1b1/glook/pages/2_Univariate_Analysis.py
+-rw-rw-rw-   0        0        0     4743 2024-05-11 18:53:32.000000 glook-1.2.1b1/glook/pages/3_Bivariate_Analysis.py
+-rw-rw-rw-   0        0        0     4384 2024-05-12 07:45:54.000000 glook-1.2.1b1/glook/pages/4_Trivariate_Analysis.py
+-rw-rw-rw-   0        0        0   114370 2024-05-13 18:20:30.000000 glook-1.2.1b1/glook/pages/5_Pre_Processing.py
+-rw-rw-rw-   0        0        0     5430 2024-05-12 19:21:16.000000 glook-1.2.1b1/glook/pages/6_Split_Data.py
+-rw-rw-rw-   0        0        0     4651 2024-05-12 10:50:25.000000 glook-1.2.1b1/glook/pages/7_Dimensionality_Reduction.py
+-rw-rw-rw-   0        0        0    60527 2024-05-05 17:49:18.000000 glook-1.2.1b1/glook/pages/8_Supervised_Learning.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:47.906103 glook-1.2.1b1/glook.egg-info/
+-rw-rw-rw-   0        0        0    11088 2024-05-21 16:27:47.000000 glook-1.2.1b1/glook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      888 2024-05-21 16:27:47.000000 glook-1.2.1b1/glook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:27:47.000000 glook-1.2.1b1/glook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-21 16:27:47.000000 glook-1.2.1b1/glook.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      211 2024-05-21 16:27:47.000000 glook-1.2.1b1/glook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-21 16:27:47.000000 glook-1.2.1b1/glook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:47.956305 glook-1.2.1b1/look/
+-rw-rw-rw-   0        0        0     3228 2024-05-02 17:40:02.000000 glook-1.2.1b1/look/GLook.py
+-rw-rw-rw-   0        0        0       51 2024-03-25 17:39:42.000000 glook-1.2.1b1/look/__init__.py
+-rw-rw-rw-   0        0        0      339 2024-03-25 18:24:01.000000 glook-1.2.1b1/look/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:27:47.967308 glook-1.2.1b1/look/pages/
+-rw-rw-rw-   0        0        0     4218 2024-05-12 07:33:45.000000 glook-1.2.1b1/look/pages/1_General_Data_Insights.py
+-rw-rw-rw-   0        0        0    19989 2024-05-12 06:32:36.000000 glook-1.2.1b1/look/pages/2_Univariate_Analysis.py
+-rw-rw-rw-   0        0        0     4385 2024-05-12 06:59:19.000000 glook-1.2.1b1/look/pages/3_Bivariate_Analysis.py
+-rw-rw-rw-   0        0        0     4435 2024-05-12 07:00:45.000000 glook-1.2.1b1/look/pages/4_Trivariate_Analysis.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:27:47.975306 glook-1.2.1b1/setup.cfg
+-rw-rw-rw-   0        0        0     2507 2024-05-21 16:27:43.000000 glook-1.2.1b1/setup.py
```

### Comparing `glook-1.2.0b1/glook/GLook.py` & `glook-1.2.1b1/glook/GLook.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 		)
 # import matplotlib.pyplot as plt
 # import matplotlib
 # matplotlib.use('TkAgg')
 if "shared" not in st.session_state:
 	st.session_state["shared"] = True
 
-st.title("G-Look Auto EDA",)
+st.title("G-Look Auto ML",)
 # st.write("`")
 gg = st.file_uploader("Input:", type=['csv', 'xlsx'])
 
 # df = None
 # if st.button("process", use_container_width=True):
 # 	try:
 # 		# Try reading as CSV
```

### Comparing `glook-1.2.0b1/glook/pages/10_Unsupervised_learning.py` & `glook-1.2.1b1/glook/pages/10_Unsupervised_learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,30 @@
 	silhouette_score, davies_bouldin_score, calinski_harabasz_score,
 	adjusted_rand_score, adjusted_mutual_info_score, completeness_score,
 	homogeneity_score, v_measure_score
 )
 import numpy as np
 from sklearn.metrics import explained_variance_score
 import joblib
+from sklearn.model_selection import train_test_split
 try:
 	st.write("Session State:->", st.session_state["shared"])
 	# Streamlit UI for data splitting
 	# st.title("Data Splitting Page")
 
 	# Display the modified DataFrame
 	# st.subheader("Modified DataFrame")
-	if "df" in st.session_state:
-		df = st.session_state.df
+	if "df_pre" in st.session_state:
+		# df = st.session_state.df
+		df_to_pre = st.session_state.df_pre
+		df = df_to_pre
+		
+		# Splitting the data into training and validation sets
+		df, validation_df = train_test_split(df, test_size=0.1, random_state=42)
+		st.session_state.uns_valid = validation_df
 		# Assuming df is your DataFrame
 		# df.to_csv('your_file.csv', index=False)
 		# Data split options
 		# st.write(df)
 		# target_column = st.sidebar.selectbox("Select the target column:", df.columns)
 		# test_size = st.sidebar.slider("Select the test size:", 0.1, 0.5, step=0.05)
 		# random_state = st.sidebar.number_input("Enter the random state:", min_value=0, max_value=10000, value=42)
```

### Comparing `glook-1.2.0b1/glook/pages/11_Custom_Model_Training.py` & `glook-1.2.1b1/glook/pages/11_Custom_Model_Training.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 	calinski_harabasz_score,
 	adjusted_rand_score, 
 	adjusted_mutual_info_score, 
 	completeness_score,
 	homogeneity_score, 
 	v_measure_score
 )
-
+from sklearn.model_selection import train_test_split
 from sklearn.metrics import explained_variance_score
 from sklearn.metrics import roc_curve, precision_recall_curve, confusion_matrix
 from sklearn.metrics import mean_squared_error, mean_absolute_error, mean_squared_log_error
 from sklearn.metrics import (
 	accuracy_score, f1_score, mean_squared_error, r2_score, roc_auc_score,
 	recall_score, precision_score, roc_curve, auc, confusion_matrix,
 	classification_report
@@ -1222,15 +1222,19 @@
 
 
 
 st.title("Custom Modle Building")
 
 st.write("Session State:->", st.session_state["shared"])
 if "X_train" in st.session_state or "X_test" in st.session_state or "y_train" in st.session_state or "y_test" in st.session_state or "df" in st.session_state:
-	df = st.session_state.df
+	# df = st.session_state.df
+	df_to_pre = st.session_state.df_pre
+	df = df_to_pre
+	df, validation_df = train_test_split(df, test_size=0.1, random_state=42)
+	st.session_state.uns_valid = validation_df
 	max_clusters = len(df) - 1
 	try:
 		X_train = st.session_state.X_train
 		X_test = st.session_state.X_test
 		y_train = st.session_state.y_train
 		y_test = st.session_state.y_test
 		X_test.replace({True: 1, False: 0}, inplace=True)
@@ -2248,14 +2252,55 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_kmeans_model(transformed_data, params)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 	
 	elif selected_models == "Birch":
 		print("train_decision_tree_classifier")
 		st.header("Birch Clustering Hyperparameters")
 		threshold = st.slider("Threshold", min_value=0.1, max_value=1.0, value=0.5, step=0.1)
 		branching_factor = st.slider("Branching Factor", min_value=50, max_value=500, value=100, step=50)
 		n_clusters = st.slider("Number of Clusters", min_value=2, max_value=10, value=2, step=1)
@@ -2271,14 +2316,55 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_birch_model(transformed_data, params)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 
 	elif selected_models == "DBSCAN":
 		print("train_decision_tree_classifier")
 
 
 		# Sidebar for DBSCAN parameters
 		st.header("DBSCAN Parameters")
@@ -2289,15 +2375,57 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_dbscan_model(transformed_data, eps, min_samples)
 		# Train the model with the selected parameters
 		# model, metrics = train_dbscan_model(df, eps, min_samples)
+		st.write("Model:", model)
 		st.write("Evaluation Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 
 	elif selected_models == "HDBSCAN":
 		print("train_decision_tree_classifier")
 
 		# Sidebar for parameter input
 		st.header("HDBSCAN Parameters")
 		min_samples = st.slider("Min Samples", min_value=1, max_value=100, value=5, step=1)
@@ -2308,14 +2436,55 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_hdbscan_model(transformed_data, min_samples, min_cluster_size, cluster_selection_epsilon)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 
 	elif selected_models == "Agglomerative Clustering":
 		print("train_decision_tree_classifier")
 
 		# Sidebar for hyperparameter input
 		st.header("Agglomerative Clustering Hyperparameters")
 		n_clusters = st.slider("Number of Clusters", min_value=2, max_value=20, value=2, step=1)
@@ -2333,14 +2502,55 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_agglomerative_clus_model(transformed_data, params)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 
 	elif selected_models == "Mean Shift":
 		print("train_decision_tree_classifier")
 
 
 		# Sidebar for bandwidth input
 		st.header("MeanShift Clustering Hyperparameters")
@@ -2351,14 +2561,55 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_mean_shift_model(transformed_data, bandwidth)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 
 	elif selected_models == "Affinity Propagation":
 		print("train_decision_tree_classifier")
 		# Sidebar for hyperparameter input
 		st.header("AffinityPropagation Hyperparameters")
 		damping = st.slider("Damping", min_value=0.5, max_value=1.0, value=0.9, step=0.05)
 		max_iter = st.slider("Max Iterations", min_value=100, max_value=1000, value=200, step=50)
@@ -2380,14 +2631,55 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_affinity_propo_model(transformed_data, params)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 
 	elif selected_models == "Spectral Clustering":
 		print("train_decision_tree_classifier")
 		# Sidebar for hyperparameter input
 		st.header("SpectralClustering Hyperparameters")
 		n_clusters = st.slider("Number of Clusters", min_value=2, max_value=10, value=3, step=1)
 		assign_labels = st.selectbox("Assign Labels Method", ["kmeans", "discretize"])
@@ -2411,14 +2703,55 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_spectral_clust_model(transformed_data, params)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 		
 
 		# st.write(metrics)
 
 	elif selected_models == "OPTICS":
 		print("train_decision_tree_classifier")
 		# Sidebar for hyperparameter input
@@ -2445,14 +2778,55 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_optics_model(transformed_data, params)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 
 
 
 	elif selected_models == "Mini Batch K-Means":
 		print("train_decision_tree_classifier")
 		# Sidebar for hyperparameter input
 		st.header("MiniBatchKMeans Hyperparameters")
@@ -2478,14 +2852,55 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_mini_batch_kmeans_model(transformed_data, params)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 
 		
 	elif selected_models == "Feature Agglomeration":
 		print("train_decision_tree_classifier")
 
 
 		# Sidebar for hyperparameter input
@@ -2505,20 +2920,62 @@
 		else:
 			method, transformed_data, variance_explained = decomposition(df, n_comp, model_name)
 			st.write("Decomposition Method", method)
 			st.write("variance_explained:", variance_explained)
 			model, metrics = train_feature_agglo_model(transformed_data, params)
 		st.write("Model:", model)
 		st.write("Metrics:", metrics)
+		st.write("Lables:⬇️")
+		distinct_labels = np.unique(model.labels_)
+		st.write(distinct_labels)
+		if st.button("Register Model"):
+			if selected_type == "Clustering":
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
+			else:
+				model_info = {
+					'model': model,  # The trained model
+					'metrics': metrics,
+					'decom_method': model_name,
+					'decomn_comp': n_comp,	
+					'variance_explained': variance_explained,
+					'model_name': selected_models,  # Name of the model
+					'labels': model.labels_,
+					'distinct_labels': distinct_labels,
+					'selected_type': selected_type
+				}
+
+				# Dump to a joblib file
+				model_filename = f"{selected_models}_decom_clust_model_registered.pkl"
+				model_filename = model_filename.replace(" ", "")
+				# Save the dictionary containing the model and its metrics
+				with open(model_filename, "wb") as f:
+					joblib.dump(model_info, f)
+				st.success("Model Registered Successfully ✅")
 
 
 		
 
 except Exception as e:
-	st.error(e)
+	# st.error(e)
 	print(e)
-	st.warning("Select custom model type for tuning")
+	
 	if "X_train" in str(e):
 		st.warning("Check if proper preprocessing and data splitting is done or not!")
-
+	else:
+		st.warning("Select custom model type for tuning")
 	# pass
```

### Comparing `glook-1.2.0b1/glook/pages/12_Supervised_Deployment_Demo.py` & `glook-1.2.1b1/glook/pages/12_Supervised_Deployment_Demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import joblib
 import matplotlib.pyplot as plt
 from sklearn.impute import SimpleImputer
 from sklearn.compose import ColumnTransformer
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, RobustScaler
 import glob
 import seaborn as sns
-st.write(os.getcwd())
+# st.write(os.getcwd())
 import numpy as np
 from scipy.stats.mstats import winsorize
 from scipy.stats import boxcox, yeojohnson
 from sklearn.preprocessing import LabelEncoder, KBinsDiscretizer
 
 
 if "X_test" in st.session_state:
+	
 	X_test0 = st.session_state.X_test0
 	X_test = st.session_state.X_test
 	y_name = st.session_state.y_name
-	 
+
 dfo = X_test0
 # print(X_test0)
 
 
 def apply_pipeline_d_tpye(df, pipeline):
 	try:
 		# Make a copy of the DataFrame to avoid warnings or unintentional changes
@@ -400,15 +401,16 @@
 					data = pd.read_csv(uploadedFile)
 				except:
 						try:
 							data = pd.read_excel(uploadedFile)
 						except:      
 							data = pd.DataFrame(uploadedFile)
 		elif choice == "Use Validation Data":
-			data = X_test
+			data = X_test0
+			# st.write(data)
 					
 		else:
 			st.sidebar.warning("You need to upload a csv or excel file.")
 	elif type_ == 'Manual Input':
 		print(1)
 		# Analyze each column to determine type and range
 		# Select a random row to use as default values
@@ -491,245 +493,264 @@
 	# pw = st.sidebar.text_input("password", "Type Here", type="password")
 	# db = st.sidebar.text_input("database", "Type Here")
 	
 	result = ""
 	# Get the current working directory
 	cwd = os.getcwd()
 	try:
-		# Find all files in the cwd ending with 'model.pkl'
+		reg_models = glob.glob(os.path.join(cwd, "*model_registered.pkl"))
 		model_files = glob.glob(os.path.join(cwd, "*model.pkl"))
+		all_models = reg_models + model_files
 		# Check if any such files exist
-		if model_files:
-			st.write("'model.pkl' found:", model_files)
+		with st.expander("Models Found"):
+			# st.write("More Info ⬇")
+			tab1, tab2, tab3 = st.tabs(["All Models", "Registered Models (From Custom Model Training)", "Multi Model Trained (From Unsupervised Learning)"])
+			with tab1:
+				if all_models:
+					st.write("All Models found:", all_models)
+			with tab2:
+				if reg_models:
+					st.write("'model_registered.pkl' found:", reg_models)
+			with tab3:
+				if model_files:
+					st.write("'model.pkl' found:", model_files)
 		select_model = st.selectbox("Select trained model:", model_files)
 
 		model_pipe = joblib.load(select_model)
 		st.write(model_pipe)
 	except Exception as e:
 		print("e13", e)
 	if type_ == 'Upload File':
-		try:
-			# Full path to the file you're looking for
-			drop_files = glob.glob(os.path.join(cwd, "*drop_pipeline.pkl"))
-			
-			st.write(drop_files)
-
-			for drop_file_path in drop_files:
-			# Check if the file exists
-				if os.path.isfile(drop_file_path):
-					st.write(f"File 'drop_pipeline.pkl' found at {drop_file_path}")
-					drop_pipe = joblib.load(drop_file_path)
-					st.write(drop_pipe)
-					try:
-						data = apply_pipeline_drop(data, drop_pipe)
-					except Exception as e:
-						print("e35", e)
-				else:
-					st.write("No file named 'drop_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e_:14=",e)
-
-		
-
+		if choice == "Upload '.csv' or '.xlsx'":
+			try:
+				# Full path to the file you're looking for
+				drop_files = glob.glob(os.path.join(cwd, "*drop_pipeline.pkl"))
+				
+				st.write(drop_files)
 
-		try:
-			# datatype_file_path = os.path.join(cwd, "datatype_pipeline.pkl")
-			datatype_files = glob.glob(os.path.join(cwd, "*datatype_pipeline.pkl"))
-			for datatype_file_path in datatype_files:
+				for drop_file_path in drop_files:
 				# Check if the file exists
-				if os.path.isfile(datatype_file_path):
-					st.write(f"File 'drop_pipeline.pkl' found at {datatype_file_path}")
-					datatype_pipe = joblib.load(datatype_file_path)
-					st.write(datatype_pipe)
-					try:
-						data = apply_pipeline_d_tpye(data, datatype_pipe)
-					except Exception as e:
-						print("e34", e)
-				else:
-					st.write("No file named 'datatype_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e15", e)
-		
+					if os.path.isfile(drop_file_path):
+						st.write(f"File 'drop_pipeline.pkl' found at {drop_file_path}")
+						drop_pipe = joblib.load(drop_file_path)
+						st.write(drop_pipe)
+						try:
+							data = apply_pipeline_drop(data, drop_pipe)
+						except Exception as e:
+							print("e35", e)
+					else:
+						st.write("No file named 'drop_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e_:14=",e)
 
-		try:
-			drop_dup_file_path = os.path.join(cwd, "drop_dup_pipeline.pkl")
-			if os.path.isfile(drop_dup_file_path):
-				st.write(f"File 'drop_dup_pipeline.pkl' found at {drop_dup_file_path}")
-				drop_dup_pipe = joblib.load(drop_dup_file_path)
-				st.write(drop_dup_pipe)
-				data = apply_pipeline_drop_dup(data, drop_dup_pipe)
-			else:
-				st.write("No file named 'drop_dup_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e16", e)
+			
 
 
-		try:
-			# outliers_for_col_file_path = os.path.join(cwd, "outliers_for_col_pipeline.pkl")
-			col_outliers_files = glob.glob(os.path.join(cwd, "*outliers_for_col_pipeline.pkl"))
-
-			for outliers_for_col_file_path in col_outliers_files:
-				if os.path.isfile(outliers_for_col_file_path):
-					st.write(f"File 'outliers_for_col_pipeline.pkl' found at {outliers_for_col_file_path}")
-					outliers_for_col_pipe = joblib.load(outliers_for_col_file_path)
-					st.write(outliers_for_col_pipe)
-					try:
-						data = apply_outliers_for_col(data, outliers_for_col_pipe)
-					except Exception as e:
-						print("e32", e)
+			try:
+				# datatype_file_path = os.path.join(cwd, "datatype_pipeline.pkl")
+				datatype_files = glob.glob(os.path.join(cwd, "*datatype_pipeline.pkl"))
+				for datatype_file_path in datatype_files:
+					# Check if the file exists
+					if os.path.isfile(datatype_file_path):
+						st.write(f"File 'drop_pipeline.pkl' found at {datatype_file_path}")
+						datatype_pipe = joblib.load(datatype_file_path)
+						st.write(datatype_pipe)
+						try:
+							data = apply_pipeline_d_tpye(data, datatype_pipe)
+						except Exception as e:
+							print("e34", e)
+					else:
+						st.write("No file named 'datatype_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e15", e)
+			
+
+			try:
+				drop_dup_file_path = os.path.join(cwd, "drop_dup_pipeline.pkl")
+				if os.path.isfile(drop_dup_file_path):
+					st.write(f"File 'drop_dup_pipeline.pkl' found at {drop_dup_file_path}")
+					drop_dup_pipe = joblib.load(drop_dup_file_path)
+					st.write(drop_dup_pipe)
+					data = apply_pipeline_drop_dup(data, drop_dup_pipe)
 				else:
-					st.write("No file named 'outliers_for_col_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e17", e)
-		
+					st.write("No file named 'drop_dup_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e16", e)
 
-		try:
-			outliers_for_full_df_file_path = os.path.join(cwd, "outliers_for_full_df_pipeline.pkl")
-			if os.path.isfile(outliers_for_full_df_file_path):
-				st.write(f"File 'outliers_for_full_df_pipeline.pkl' found at {outliers_for_full_df_file_path}")
-				outliers_for_full_df_pipe = joblib.load(outliers_for_full_df_file_path)
-				st.write(outliers_for_full_df_pipe)
-				data = apply_outliers_full_df(data, outliers_for_full_df_pipe)
-			else:
-				st.write("No file named 'outliers_for_full_df_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e18", e)
-		
 
-		try:
-			# treat_missing_vaues_for_col_file_path = os.path.join(cwd, "treat_missing_vaues_for_col.pkl")
-			col_missing_files = glob.glob(os.path.join(cwd, "*treat_missing_vaues_for_col.pkl"))
-			for treat_missing_vaues_for_col_file_path in col_missing_files:
-				if os.path.isfile(treat_missing_vaues_for_col_file_path):
-					st.write(f"File 'treat_missing_vaues_for_col.pkl' found at {treat_missing_vaues_for_col_file_path}")
-					treat_missing_vaues_for_col_pipe = joblib.load(treat_missing_vaues_for_col_file_path)
-					st.write(treat_missing_vaues_for_col_pipe)
-					try:
-						data = treat_missing_vaues_for_col(data, treat_missing_vaues_for_col_pipe)
-					except Exception as e:
-						print("e31", e)
+			try:
+				# outliers_for_col_file_path = os.path.join(cwd, "outliers_for_col_pipeline.pkl")
+				col_outliers_files = glob.glob(os.path.join(cwd, "*outliers_for_col_pipeline.pkl"))
+
+				for outliers_for_col_file_path in col_outliers_files:
+					if os.path.isfile(outliers_for_col_file_path):
+						st.write(f"File 'outliers_for_col_pipeline.pkl' found at {outliers_for_col_file_path}")
+						outliers_for_col_pipe = joblib.load(outliers_for_col_file_path)
+						st.write(outliers_for_col_pipe)
+						try:
+							data = apply_outliers_for_col(data, outliers_for_col_pipe)
+						except Exception as e:
+							print("e32", e)
+					else:
+						st.write("No file named 'outliers_for_col_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e17", e)
+			
+
+			try:
+				outliers_for_full_df_file_path = os.path.join(cwd, "outliers_for_full_df_pipeline.pkl")
+				if os.path.isfile(outliers_for_full_df_file_path):
+					st.write(f"File 'outliers_for_full_df_pipeline.pkl' found at {outliers_for_full_df_file_path}")
+					outliers_for_full_df_pipe = joblib.load(outliers_for_full_df_file_path)
+					st.write(outliers_for_full_df_pipe)
+					data = apply_outliers_full_df(data, outliers_for_full_df_pipe)
 				else:
-					st.write("No file named 'treat_missing_vaues_for_col.pkl' found in the current directory.")
-		except Exception as e:
-			print("e19", e)
+					st.write("No file named 'outliers_for_full_df_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e18", e)
+			
 
-		try:
-			treat_missing_vaues_in_full_df_file_path = os.path.join(cwd, "treat_missing_vaues_in_full_df.pkl")
-			if os.path.isfile(treat_missing_vaues_in_full_df_file_path):
-				st.write(f"File 'treat_missing_vaues_in_full_df.pkl' found at {treat_missing_vaues_in_full_df_file_path}")
-				treat_missing_vaues_in_full_df_pipe = joblib.load(treat_missing_vaues_in_full_df_file_path)
-				st.write(treat_missing_vaues_in_full_df_pipe)
-				data = treat_missing_values_in_full_df(data, treat_missing_vaues_in_full_df_pipe)
-			else:
-				st.write("No file named 'treat_missing_vaues_in_full_df.pkl' found in the current directory.")
-		except Exception as e:
-			print("e20", e)
+			try:
+				# treat_missing_vaues_for_col_file_path = os.path.join(cwd, "treat_missing_vaues_for_col.pkl")
+				col_missing_files = glob.glob(os.path.join(cwd, "*treat_missing_vaues_for_col.pkl"))
+				for treat_missing_vaues_for_col_file_path in col_missing_files:
+					if os.path.isfile(treat_missing_vaues_for_col_file_path):
+						st.write(f"File 'treat_missing_vaues_for_col.pkl' found at {treat_missing_vaues_for_col_file_path}")
+						treat_missing_vaues_for_col_pipe = joblib.load(treat_missing_vaues_for_col_file_path)
+						st.write(treat_missing_vaues_for_col_pipe)
+						try:
+							data = treat_missing_vaues_for_col(data, treat_missing_vaues_for_col_pipe)
+						except Exception as e:
+							print("e31", e)
+					else:
+						st.write("No file named 'treat_missing_vaues_for_col.pkl' found in the current directory.")
+			except Exception as e:
+				print("e19", e)
+
+			try:
+				treat_missing_vaues_in_full_df_file_path = os.path.join(cwd, "treat_missing_vaues_in_full_df.pkl")
+				if os.path.isfile(treat_missing_vaues_in_full_df_file_path):
+					st.write(f"File 'treat_missing_vaues_in_full_df.pkl' found at {treat_missing_vaues_in_full_df_file_path}")
+					treat_missing_vaues_in_full_df_pipe = joblib.load(treat_missing_vaues_in_full_df_file_path)
+					st.write(treat_missing_vaues_in_full_df_pipe)
+					data = treat_missing_values_in_full_df(data, treat_missing_vaues_in_full_df_pipe)
+				else:
+					st.write("No file named 'treat_missing_vaues_in_full_df.pkl' found in the current directory.")
+			except Exception as e:
+				print("e20", e)
 
 
-		try:
+			try:
+				# apply_transformation_on_col_file_path = os.path.join(cwd, "apply_transformation_on_col.pkl")
+				tran_files = glob.glob(os.path.join(cwd, "*apply_transformation_on_col.pkl"))
+				for apply_transformation_on_col_file_path in tran_files:
+					if os.path.isfile(apply_transformation_on_col_file_path):
+						st.write(f"File 'treat_missing_vaues_in_full_df.pkl' found at {apply_transformation_on_col_file_path}")
+						apply_transformation_on_col_pipe = joblib.load(apply_transformation_on_col_file_path)
+						st.write(apply_transformation_on_col_pipe)
+						try:
+							data = apply_transformation_on_col(data, apply_transformation_on_col_pipe)
+						except Exception as e:
+							print("e30", e)
+					else:
+						st.write("No file named 'apply_transformation_on_col.pkl' found in the current directory.")
+			except Exception as e:
+				print("e21", e)
+			
+			
 			# apply_transformation_on_col_file_path = os.path.join(cwd, "apply_transformation_on_col.pkl")
-			tran_files = glob.glob(os.path.join(cwd, "*apply_transformation_on_col.pkl"))
-			for apply_transformation_on_col_file_path in tran_files:
-				if os.path.isfile(apply_transformation_on_col_file_path):
-					st.write(f"File 'treat_missing_vaues_in_full_df.pkl' found at {apply_transformation_on_col_file_path}")
-					apply_transformation_on_col_pipe = joblib.load(apply_transformation_on_col_file_path)
-					st.write(apply_transformation_on_col_pipe)
-					try:
-						data = apply_transformation_on_col(data, apply_transformation_on_col_pipe)
-					except Exception as e:
-						print("e30", e)
-				else:
-					st.write("No file named 'apply_transformation_on_col.pkl' found in the current directory.")
-		except Exception as e:
-			print("e21", e)
-		
-		
-		# apply_transformation_on_col_file_path = os.path.join(cwd, "apply_transformation_on_col.pkl")
-		# if os.path.isfile(apply_transformation_on_col_file_path):
-		#     st.write(f"File 'apply_transformation_on_col.pkl' found at {apply_transformation_on_col_file_path}")
-		#     apply_transformation_on_col_pipe = joblib.load(apply_transformation_on_col_file_path)
-		#     st.write(apply_transformation_on_col_pipe)
-		# else:
-		#     st.write("No file named 'apply_transformation_on_col.pkl' found in the current directory.")
-		try:
-			# column_unique_value_replacement_file_path = os.path.join(cwd, "column_unique_value_replacement.pkl")
-			out_rplac_files = glob.glob(os.path.join(cwd, "*column_unique_value_replacement.pkl"))
-			for column_unique_value_replacement_file_path in out_rplac_files:
-				if os.path.isfile(column_unique_value_replacement_file_path):
-					st.write(f"File 'column_unique_value_replacement.pkl' found at {column_unique_value_replacement_file_path}")
-					column_unique_value_replacement_pipe = joblib.load(column_unique_value_replacement_file_path)
-					st.write(column_unique_value_replacement_pipe)
-					try:
-						data = column_unique_value_replacement(data, column_unique_value_replacement_pipe)
-					except Exception as e:
-						print("e29", e)
-				else:
-					st.write("No file named 'column_unique_value_replacement.pkl' found in the current directory.")
-		except Exception as e:
-			print("e22", e)
-
-		try:    
-			# discretize_output_col_file_path = os.path.join(cwd, "discretize_output_col.pkl")
-			discretize_output_col_files = glob.glob(os.path.join(cwd, "*discretize_output_col.pkl"))
-			for discretize_output_col_file_path in discretize_output_col_files:
-				if os.path.isfile(discretize_output_col_file_path):
-					st.write(f"File 'discretize_output_col.pkl' found at {discretize_output_col_file_path}")
-					discretize_output_col_pipe = joblib.load(discretize_output_col_file_path)
-					st.write(discretize_output_col_pipe)
-					try:
-						data = discretize_output_col(data, discretize_output_col_pipe)
-					except Exception as e:
-						print("e28", e)
+			# if os.path.isfile(apply_transformation_on_col_file_path):
+			#     st.write(f"File 'apply_transformation_on_col.pkl' found at {apply_transformation_on_col_file_path}")
+			#     apply_transformation_on_col_pipe = joblib.load(apply_transformation_on_col_file_path)
+			#     st.write(apply_transformation_on_col_pipe)
+			# else:
+			#     st.write("No file named 'apply_transformation_on_col.pkl' found in the current directory.")
+			try:
+				# column_unique_value_replacement_file_path = os.path.join(cwd, "column_unique_value_replacement.pkl")
+				out_rplac_files = glob.glob(os.path.join(cwd, "*column_unique_value_replacement.pkl"))
+				for column_unique_value_replacement_file_path in out_rplac_files:
+					if os.path.isfile(column_unique_value_replacement_file_path):
+						st.write(f"File 'column_unique_value_replacement.pkl' found at {column_unique_value_replacement_file_path}")
+						column_unique_value_replacement_pipe = joblib.load(column_unique_value_replacement_file_path)
+						st.write(column_unique_value_replacement_pipe)
+						try:
+							data = column_unique_value_replacement(data, column_unique_value_replacement_pipe)
+						except Exception as e:
+							print("e29", e)
+					else:
+						st.write("No file named 'column_unique_value_replacement.pkl' found in the current directory.")
+			except Exception as e:
+				print("e22", e)
+			# st.write(data)
+			try:    
+				# discretize_output_col_file_path = os.path.join(cwd, "discretize_output_col.pkl")
+				discretize_output_col_files = glob.glob(os.path.join(cwd, "*discretize_output_col.pkl"))
+				for discretize_output_col_file_path in discretize_output_col_files:
+					if os.path.isfile(discretize_output_col_file_path):
+						st.write(f"File 'discretize_output_col.pkl' found at {discretize_output_col_file_path}")
+						discretize_output_col_pipe = joblib.load(discretize_output_col_file_path)
+						st.write(discretize_output_col_pipe)
+						try:
+							data = discretize_output_col(data, discretize_output_col_pipe)
+						except Exception as e:
+							print("e28", e)
+					else:
+						st.write("No file named 'discretize_output_col.pkl' found in the current directory.")
+			except Exception as e:
+				print("e23", e)
+			# st.write(data)
+				
+			try:
+				apply_encoding_on_df_file_path = os.path.join(cwd, "apply_encoding_on_df.pkl")
+				if os.path.isfile(apply_encoding_on_df_file_path):
+					st.write(f"File 'apply_encoding_on_df.pkl' found at {apply_encoding_on_df_file_path}")
+					apply_encoding_on_df_pipe = joblib.load(apply_encoding_on_df_file_path)
+					st.write(apply_encoding_on_df_pipe)
+					data = apply_encoding_on_df(data, apply_encoding_on_df_pipe)
 				else:
-					st.write("No file named 'discretize_output_col.pkl' found in the current directory.")
-		except Exception as e:
-			print("e23", e)
-			
-		try:
-			apply_encoding_on_df_file_path = os.path.join(cwd, "apply_encoding_on_df.pkl")
-			if os.path.isfile(apply_encoding_on_df_file_path):
-				st.write(f"File 'apply_encoding_on_df.pkl' found at {apply_encoding_on_df_file_path}")
-				apply_encoding_on_df_pipe = joblib.load(apply_encoding_on_df_file_path)
-				st.write(apply_encoding_on_df_pipe)
-				data = apply_encoding_on_df(data, apply_encoding_on_df_pipe)
-			else:
-				st.write("No file named 'apply_encoding_on_df.pkl' found in the current directory.")
-		except Exception as e:
-			print("e24", e)
-
-		try:
-			col_dum_files = glob.glob(os.path.join(cwd, "*apply_encoding_on_col.pkl"))
-			for apply_encoding_on_col_file_path in col_dum_files:
-				if os.path.isfile(apply_encoding_on_col_file_path):
-					st.write(f"File 'apply_encoding_on_col.pkl' found at {apply_encoding_on_col_file_path}")
-					apply_encoding_on_col_pipe = joblib.load(apply_encoding_on_col_file_path)
-					st.write(apply_encoding_on_col_pipe)
+					st.write("No file named 'apply_encoding_on_df.pkl' found in the current directory.")
+			except Exception as e:
+				print("e24", e)
+			# st.write(data)
+
+			try:
+				col_dum_files = glob.glob(os.path.join(cwd, "*apply_encoding_on_col.pkl"))
+				for apply_encoding_on_col_file_path in col_dum_files:
+					if os.path.isfile(apply_encoding_on_col_file_path):
+						st.write(f"File 'apply_encoding_on_col.pkl' found at {apply_encoding_on_col_file_path}")
+						apply_encoding_on_col_pipe = joblib.load(apply_encoding_on_col_file_path)
+						st.write(apply_encoding_on_col_pipe)
+						try:
+							data = apply_encoding_on_col(data, apply_encoding_on_col_pipe)
+						except Exception as e:
+							print("e27", e)
+					else:
+						st.write("No file named 'apply_encoding_on_col.pkl' found in the current directory.")
+			except Exception as e:
+				print("e25", e)
+
+			try:
+				apply_scaling_on_df_file_path = os.path.join(cwd, "apply_scaling_on_df.pkl")
+				if os.path.isfile(apply_scaling_on_df_file_path):
+					st.write(f"File 'apply_scaling_on_df.pkl' found at {apply_scaling_on_df_file_path}")
+					apply_scaling_on_df_pipe = joblib.load(apply_scaling_on_df_file_path)
+					st.write(apply_scaling_on_df_pipe)
 					try:
-						data = apply_encoding_on_col(data, apply_encoding_on_col_pipe)
+						data = apply_scaling_on_df(data, apply_scaling_on_df_pipe)
 					except Exception as e:
-						print("e27", e)
+						print("e26", e)
 				else:
-					st.write("No file named 'apply_encoding_on_col.pkl' found in the current directory.")
-		except Exception as e:
-			print("e25", e)
-
-		try:
-			apply_scaling_on_df_file_path = os.path.join(cwd, "apply_scaling_on_df.pkl")
-			if os.path.isfile(apply_scaling_on_df_file_path):
-				st.write(f"File 'apply_scaling_on_df.pkl' found at {apply_scaling_on_df_file_path}")
-				apply_scaling_on_df_pipe = joblib.load(apply_scaling_on_df_file_path)
-				st.write(apply_scaling_on_df_pipe)
-				try:
-					data = apply_scaling_on_df(data, apply_scaling_on_df_pipe)
-				except Exception as e:
-					print("e26", e)
-			else:
-				st.write("No file named 'apply_scaling_on_df.pkl' found in the current directory.")
-		except Exception as e:
-			print("e26", e)
+					st.write("No file named 'apply_scaling_on_df.pkl' found in the current directory.")
+			except Exception as e:
+				print("e26", e)
+			# st.write(data)
+		elif choice == "Use Validation Data":
+			data = X_test0
+			data = data.reset_index(drop=True)
+			# st.write(data)
 
 	elif type_ == 'Manual Input':
 		# st.warning("hi1")
 		random_row = dfo.sample(1).iloc[0]
 
 		# Detect the data type and range of each column
 		column_details = {}
@@ -821,13 +842,14 @@
 				st.table(styled_result.background_gradient(cmap = cm).format(precision=2))
 			elif type_ == 'Manual Input':
 				st.warning("Not Yet Released")
 				st.success("Comming Soon 🔜 @ https://pypi.org/project/glook/")
 		except UnboundLocalError:
 			st.warning("Upload .csv or .xlsx")
 		except Exception as e:
+			print(e)
 			st.error(e)
 		
 if __name__=='__main__':
 	main()
```

### Comparing `glook-1.2.0b1/glook/pages/13_Unsupervised_Deployment_Demo.py` & `glook-1.2.1b1/glook/pages/13_Unsupervised_Deployment_Demo.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import joblib
 import matplotlib.pyplot as plt
 from sklearn.impute import SimpleImputer
 from sklearn.compose import ColumnTransformer
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, RobustScaler
 import glob
 import seaborn as sns
-st.write(os.getcwd())
+# st.write(os.getcwd())
 import numpy as np
 from scipy.stats.mstats import winsorize
 from scipy.stats import boxcox, yeojohnson
 from sklearn.preprocessing import LabelEncoder, KBinsDiscretizer
 import matplotlib.colors as mcolors
 from sklearn.decomposition import PCA, NMF, FastICA, FactorAnalysis, DictionaryLearning, TruncatedSVD
 
@@ -25,16 +25,20 @@
 		X_test = st.session_state.X_test
 	except:
 		pass
 	try:
 		df = st.session_state.df
 	except:
 		pass
+	# try:
+	# 	df0 = st.session_state.df0
+	# except:
+	# 	pass
 	try:
-		df0 = st.session_state.df0
+		df0 = st.session_state.uns_valid
 	except:
 		pass
 try:
 	dfo = X_test0
 except:
 	pass
 # print(X_test0)
@@ -356,14 +360,17 @@
 		
 		model1.fit(clean_data)
 		label = model1.labels_
 		predictions = pd.DataFrame(label, columns=["Clusters"])
 
 		# Combine predictions with the original data
 		final_result = pd.concat([predictions, data], axis=1)
+		# final_result.reset_index(inplace=True)
+
+		# final_result = final_result.iloc[:, 1:]
 	elif ttype__ == "Clustering by Decomposition":
 		clean_data = data
 		method_ = model_pipe['decom_method']
 		n_comp = model_pipe['decomn_comp']
 		if method_ == "PCA":
 			decomm_ = PCA(n_components=int(n_comp))
 		elif method_ == "NMF":
@@ -511,245 +518,267 @@
 	# db = st.sidebar.text_input("database", "Type Here")
 	
 	result = ""
 	# Get the current working directory
 	cwd = os.getcwd()
 	try:
 		# Find all files in the cwd ending with 'model.pkl'
+		reg_models = glob.glob(os.path.join(cwd, "*model_registered.pkl"))
 		model_files = glob.glob(os.path.join(cwd, "*model.pkl"))
+		all_models = reg_models + model_files
 		# Check if any such files exist
-		if model_files:
-			st.write("'model.pkl' found:", model_files)
-		select_model = st.selectbox("Select trained model:", model_files)
+		with st.expander("Models Found"):
+			# st.write("More Info ⬇")
+			tab1, tab2, tab3 = st.tabs(["All Models", "Registered Models (From Custom Model Training)", "Multi Model Trained (From Unsupervised Learning)"])
+			with tab1:
+				if all_models:
+					st.write("All Models found:", all_models)
+			with tab2:
+				if reg_models:
+					st.write("'model_registered.pkl' found:", reg_models)
+			with tab3:
+				if model_files:
+					st.write("'model.pkl' found:", model_files)
+
+		select_model = st.selectbox("Select from trained all model:", all_models)
 
 		model_pipe = joblib.load(select_model)
 		
 		st.write(model_pipe)
 	except Exception as e:
 		print("e13", e)
 	if type_ == 'Upload File':
-		try:
-			# Full path to the file you're looking for
-			drop_files = glob.glob(os.path.join(cwd, "*drop_pipeline.pkl"))
-			
-			st.write(drop_files)
-
-			for drop_file_path in drop_files:
-			# Check if the file exists
-				if os.path.isfile(drop_file_path):
-					st.write(f"File 'drop_pipeline.pkl' found at {drop_file_path}")
-					drop_pipe = joblib.load(drop_file_path)
-					st.write(drop_pipe)
-					try:
-						data = apply_pipeline_drop(data, drop_pipe)
-					except Exception as e:
-						print("e35", e)
-				else:
-					st.write("No file named 'drop_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e_:14=",e)
-
-		
-
+		if choice == "Upload '.csv' or '.xlsx'":
+			try:
+				# Full path to the file you're looking for
+				drop_files = glob.glob(os.path.join(cwd, "*drop_pipeline.pkl"))
+				
+				st.write(drop_files)
 
-		try:
-			# datatype_file_path = os.path.join(cwd, "datatype_pipeline.pkl")
-			datatype_files = glob.glob(os.path.join(cwd, "*datatype_pipeline.pkl"))
-			for datatype_file_path in datatype_files:
+				for drop_file_path in drop_files:
 				# Check if the file exists
-				if os.path.isfile(datatype_file_path):
-					st.write(f"File 'drop_pipeline.pkl' found at {datatype_file_path}")
-					datatype_pipe = joblib.load(datatype_file_path)
-					st.write(datatype_pipe)
-					try:
-						data = apply_pipeline_d_tpye(data, datatype_pipe)
-					except Exception as e:
-						print("e34", e)
-				else:
-					st.write("No file named 'datatype_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e15", e)
-		
+					if os.path.isfile(drop_file_path):
+						st.write(f"File 'drop_pipeline.pkl' found at {drop_file_path}")
+						drop_pipe = joblib.load(drop_file_path)
+						st.write(drop_pipe)
+						try:
+							data = apply_pipeline_drop(data, drop_pipe)
+						except Exception as e:
+							print("e35", e)
+					else:
+						st.write("No file named 'drop_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e_:14=",e)
 
-		try:
-			drop_dup_file_path = os.path.join(cwd, "drop_dup_pipeline.pkl")
-			if os.path.isfile(drop_dup_file_path):
-				st.write(f"File 'drop_dup_pipeline.pkl' found at {drop_dup_file_path}")
-				drop_dup_pipe = joblib.load(drop_dup_file_path)
-				st.write(drop_dup_pipe)
-				data = apply_pipeline_drop_dup(data, drop_dup_pipe)
-			else:
-				st.write("No file named 'drop_dup_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e16", e)
+			
 
 
-		try:
-			# outliers_for_col_file_path = os.path.join(cwd, "outliers_for_col_pipeline.pkl")
-			col_outliers_files = glob.glob(os.path.join(cwd, "*outliers_for_col_pipeline.pkl"))
+			try:
+				# datatype_file_path = os.path.join(cwd, "datatype_pipeline.pkl")
+				datatype_files = glob.glob(os.path.join(cwd, "*datatype_pipeline.pkl"))
+				for datatype_file_path in datatype_files:
+					# Check if the file exists
+					if os.path.isfile(datatype_file_path):
+						st.write(f"File 'drop_pipeline.pkl' found at {datatype_file_path}")
+						datatype_pipe = joblib.load(datatype_file_path)
+						st.write(datatype_pipe)
+						try:
+							data = apply_pipeline_d_tpye(data, datatype_pipe)
+						except Exception as e:
+							print("e34", e)
+					else:
+						st.write("No file named 'datatype_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e15", e)
+			
 
-			for outliers_for_col_file_path in col_outliers_files:
-				if os.path.isfile(outliers_for_col_file_path):
-					st.write(f"File 'outliers_for_col_pipeline.pkl' found at {outliers_for_col_file_path}")
-					outliers_for_col_pipe = joblib.load(outliers_for_col_file_path)
-					st.write(outliers_for_col_pipe)
-					try:
-						data = apply_outliers_for_col(data, outliers_for_col_pipe)
-					except Exception as e:
-						print("e32", e)
+			try:
+				drop_dup_file_path = os.path.join(cwd, "drop_dup_pipeline.pkl")
+				if os.path.isfile(drop_dup_file_path):
+					st.write(f"File 'drop_dup_pipeline.pkl' found at {drop_dup_file_path}")
+					drop_dup_pipe = joblib.load(drop_dup_file_path)
+					st.write(drop_dup_pipe)
+					data = apply_pipeline_drop_dup(data, drop_dup_pipe)
 				else:
-					st.write("No file named 'outliers_for_col_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e17", e)
-		
+					st.write("No file named 'drop_dup_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e16", e)
 
-		try:
-			outliers_for_full_df_file_path = os.path.join(cwd, "outliers_for_full_df_pipeline.pkl")
-			if os.path.isfile(outliers_for_full_df_file_path):
-				st.write(f"File 'outliers_for_full_df_pipeline.pkl' found at {outliers_for_full_df_file_path}")
-				outliers_for_full_df_pipe = joblib.load(outliers_for_full_df_file_path)
-				st.write(outliers_for_full_df_pipe)
-				data = apply_outliers_full_df(data, outliers_for_full_df_pipe)
-			else:
-				st.write("No file named 'outliers_for_full_df_pipeline.pkl' found in the current directory.")
-		except Exception as e:
-			print("e18", e)
-		
 
-		try:
-			# treat_missing_vaues_for_col_file_path = os.path.join(cwd, "treat_missing_vaues_for_col.pkl")
-			col_missing_files = glob.glob(os.path.join(cwd, "*treat_missing_vaues_for_col.pkl"))
-			for treat_missing_vaues_for_col_file_path in col_missing_files:
-				if os.path.isfile(treat_missing_vaues_for_col_file_path):
-					st.write(f"File 'treat_missing_vaues_for_col.pkl' found at {treat_missing_vaues_for_col_file_path}")
-					treat_missing_vaues_for_col_pipe = joblib.load(treat_missing_vaues_for_col_file_path)
-					st.write(treat_missing_vaues_for_col_pipe)
-					try:
-						data = treat_missing_vaues_for_col(data, treat_missing_vaues_for_col_pipe)
-					except Exception as e:
-						print("e31", e)
+			try:
+				# outliers_for_col_file_path = os.path.join(cwd, "outliers_for_col_pipeline.pkl")
+				col_outliers_files = glob.glob(os.path.join(cwd, "*outliers_for_col_pipeline.pkl"))
+
+				for outliers_for_col_file_path in col_outliers_files:
+					if os.path.isfile(outliers_for_col_file_path):
+						st.write(f"File 'outliers_for_col_pipeline.pkl' found at {outliers_for_col_file_path}")
+						outliers_for_col_pipe = joblib.load(outliers_for_col_file_path)
+						st.write(outliers_for_col_pipe)
+						try:
+							data = apply_outliers_for_col(data, outliers_for_col_pipe)
+						except Exception as e:
+							print("e32", e)
+					else:
+						st.write("No file named 'outliers_for_col_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e17", e)
+			
+
+			try:
+				outliers_for_full_df_file_path = os.path.join(cwd, "outliers_for_full_df_pipeline.pkl")
+				if os.path.isfile(outliers_for_full_df_file_path):
+					st.write(f"File 'outliers_for_full_df_pipeline.pkl' found at {outliers_for_full_df_file_path}")
+					outliers_for_full_df_pipe = joblib.load(outliers_for_full_df_file_path)
+					st.write(outliers_for_full_df_pipe)
+					data = apply_outliers_full_df(data, outliers_for_full_df_pipe)
 				else:
-					st.write("No file named 'treat_missing_vaues_for_col.pkl' found in the current directory.")
-		except Exception as e:
-			print("e19", e)
+					st.write("No file named 'outliers_for_full_df_pipeline.pkl' found in the current directory.")
+			except Exception as e:
+				print("e18", e)
+			
 
-		try:
-			treat_missing_vaues_in_full_df_file_path = os.path.join(cwd, "treat_missing_vaues_in_full_df.pkl")
-			if os.path.isfile(treat_missing_vaues_in_full_df_file_path):
-				st.write(f"File 'treat_missing_vaues_in_full_df.pkl' found at {treat_missing_vaues_in_full_df_file_path}")
-				treat_missing_vaues_in_full_df_pipe = joblib.load(treat_missing_vaues_in_full_df_file_path)
-				st.write(treat_missing_vaues_in_full_df_pipe)
-				data = treat_missing_values_in_full_df(data, treat_missing_vaues_in_full_df_pipe)
-			else:
-				st.write("No file named 'treat_missing_vaues_in_full_df.pkl' found in the current directory.")
-		except Exception as e:
-			print("e20", e)
+			try:
+				# treat_missing_vaues_for_col_file_path = os.path.join(cwd, "treat_missing_vaues_for_col.pkl")
+				col_missing_files = glob.glob(os.path.join(cwd, "*treat_missing_vaues_for_col.pkl"))
+				for treat_missing_vaues_for_col_file_path in col_missing_files:
+					if os.path.isfile(treat_missing_vaues_for_col_file_path):
+						st.write(f"File 'treat_missing_vaues_for_col.pkl' found at {treat_missing_vaues_for_col_file_path}")
+						treat_missing_vaues_for_col_pipe = joblib.load(treat_missing_vaues_for_col_file_path)
+						st.write(treat_missing_vaues_for_col_pipe)
+						try:
+							data = treat_missing_vaues_for_col(data, treat_missing_vaues_for_col_pipe)
+						except Exception as e:
+							print("e31", e)
+					else:
+						st.write("No file named 'treat_missing_vaues_for_col.pkl' found in the current directory.")
+			except Exception as e:
+				print("e19", e)
+
+			try:
+				treat_missing_vaues_in_full_df_file_path = os.path.join(cwd, "treat_missing_vaues_in_full_df.pkl")
+				if os.path.isfile(treat_missing_vaues_in_full_df_file_path):
+					st.write(f"File 'treat_missing_vaues_in_full_df.pkl' found at {treat_missing_vaues_in_full_df_file_path}")
+					treat_missing_vaues_in_full_df_pipe = joblib.load(treat_missing_vaues_in_full_df_file_path)
+					st.write(treat_missing_vaues_in_full_df_pipe)
+					data = treat_missing_values_in_full_df(data, treat_missing_vaues_in_full_df_pipe)
+				else:
+					st.write("No file named 'treat_missing_vaues_in_full_df.pkl' found in the current directory.")
+			except Exception as e:
+				print("e20", e)
 
 
-		try:
+			try:
+				# apply_transformation_on_col_file_path = os.path.join(cwd, "apply_transformation_on_col.pkl")
+				tran_files = glob.glob(os.path.join(cwd, "*apply_transformation_on_col.pkl"))
+				for apply_transformation_on_col_file_path in tran_files:
+					if os.path.isfile(apply_transformation_on_col_file_path):
+						st.write(f"File 'treat_missing_vaues_in_full_df.pkl' found at {apply_transformation_on_col_file_path}")
+						apply_transformation_on_col_pipe = joblib.load(apply_transformation_on_col_file_path)
+						st.write(apply_transformation_on_col_pipe)
+						try:
+							data = apply_transformation_on_col(data, apply_transformation_on_col_pipe)
+						except Exception as e:
+							print("e30", e)
+					else:
+						st.write("No file named 'apply_transformation_on_col.pkl' found in the current directory.")
+			except Exception as e:
+				print("e21", e)
+			
+			
 			# apply_transformation_on_col_file_path = os.path.join(cwd, "apply_transformation_on_col.pkl")
-			tran_files = glob.glob(os.path.join(cwd, "*apply_transformation_on_col.pkl"))
-			for apply_transformation_on_col_file_path in tran_files:
-				if os.path.isfile(apply_transformation_on_col_file_path):
-					st.write(f"File 'treat_missing_vaues_in_full_df.pkl' found at {apply_transformation_on_col_file_path}")
-					apply_transformation_on_col_pipe = joblib.load(apply_transformation_on_col_file_path)
-					st.write(apply_transformation_on_col_pipe)
-					try:
-						data = apply_transformation_on_col(data, apply_transformation_on_col_pipe)
-					except Exception as e:
-						print("e30", e)
-				else:
-					st.write("No file named 'apply_transformation_on_col.pkl' found in the current directory.")
-		except Exception as e:
-			print("e21", e)
-		
-		
-		# apply_transformation_on_col_file_path = os.path.join(cwd, "apply_transformation_on_col.pkl")
-		# if os.path.isfile(apply_transformation_on_col_file_path):
-		#     st.write(f"File 'apply_transformation_on_col.pkl' found at {apply_transformation_on_col_file_path}")
-		#     apply_transformation_on_col_pipe = joblib.load(apply_transformation_on_col_file_path)
-		#     st.write(apply_transformation_on_col_pipe)
-		# else:
-		#     st.write("No file named 'apply_transformation_on_col.pkl' found in the current directory.")
-		try:
-			# column_unique_value_replacement_file_path = os.path.join(cwd, "column_unique_value_replacement.pkl")
-			out_rplac_files = glob.glob(os.path.join(cwd, "*column_unique_value_replacement.pkl"))
-			for column_unique_value_replacement_file_path in out_rplac_files:
-				if os.path.isfile(column_unique_value_replacement_file_path):
-					st.write(f"File 'column_unique_value_replacement.pkl' found at {column_unique_value_replacement_file_path}")
-					column_unique_value_replacement_pipe = joblib.load(column_unique_value_replacement_file_path)
-					st.write(column_unique_value_replacement_pipe)
-					try:
-						data = column_unique_value_replacement(data, column_unique_value_replacement_pipe)
-					except Exception as e:
-						print("e29", e)
-				else:
-					st.write("No file named 'column_unique_value_replacement.pkl' found in the current directory.")
-		except Exception as e:
-			print("e22", e)
-
-		try:    
-			# discretize_output_col_file_path = os.path.join(cwd, "discretize_output_col.pkl")
-			discretize_output_col_files = glob.glob(os.path.join(cwd, "*discretize_output_col.pkl"))
-			for discretize_output_col_file_path in discretize_output_col_files:
-				if os.path.isfile(discretize_output_col_file_path):
-					st.write(f"File 'discretize_output_col.pkl' found at {discretize_output_col_file_path}")
-					discretize_output_col_pipe = joblib.load(discretize_output_col_file_path)
-					st.write(discretize_output_col_pipe)
-					try:
-						data = discretize_output_col(data, discretize_output_col_pipe)
-					except Exception as e:
-						print("e28", e)
+			# if os.path.isfile(apply_transformation_on_col_file_path):
+			#     st.write(f"File 'apply_transformation_on_col.pkl' found at {apply_transformation_on_col_file_path}")
+			#     apply_transformation_on_col_pipe = joblib.load(apply_transformation_on_col_file_path)
+			#     st.write(apply_transformation_on_col_pipe)
+			# else:
+			#     st.write("No file named 'apply_transformation_on_col.pkl' found in the current directory.")
+			try:
+				# column_unique_value_replacement_file_path = os.path.join(cwd, "column_unique_value_replacement.pkl")
+				out_rplac_files = glob.glob(os.path.join(cwd, "*column_unique_value_replacement.pkl"))
+				for column_unique_value_replacement_file_path in out_rplac_files:
+					if os.path.isfile(column_unique_value_replacement_file_path):
+						st.write(f"File 'column_unique_value_replacement.pkl' found at {column_unique_value_replacement_file_path}")
+						column_unique_value_replacement_pipe = joblib.load(column_unique_value_replacement_file_path)
+						st.write(column_unique_value_replacement_pipe)
+						try:
+							data = column_unique_value_replacement(data, column_unique_value_replacement_pipe)
+						except Exception as e:
+							print("e29", e)
+					else:
+						st.write("No file named 'column_unique_value_replacement.pkl' found in the current directory.")
+			except Exception as e:
+				print("e22", e)
+
+			try:    
+				# discretize_output_col_file_path = os.path.join(cwd, "discretize_output_col.pkl")
+				discretize_output_col_files = glob.glob(os.path.join(cwd, "*discretize_output_col.pkl"))
+				for discretize_output_col_file_path in discretize_output_col_files:
+					if os.path.isfile(discretize_output_col_file_path):
+						st.write(f"File 'discretize_output_col.pkl' found at {discretize_output_col_file_path}")
+						discretize_output_col_pipe = joblib.load(discretize_output_col_file_path)
+						st.write(discretize_output_col_pipe)
+						try:
+							data = discretize_output_col(data, discretize_output_col_pipe)
+						except Exception as e:
+							print("e28", e)
+					else:
+						st.write("No file named 'discretize_output_col.pkl' found in the current directory.")
+			except Exception as e:
+				print("e23", e)
+				
+			try:
+				apply_encoding_on_df_file_path = os.path.join(cwd, "apply_encoding_on_df.pkl")
+				if os.path.isfile(apply_encoding_on_df_file_path):
+					st.write(f"File 'apply_encoding_on_df.pkl' found at {apply_encoding_on_df_file_path}")
+					apply_encoding_on_df_pipe = joblib.load(apply_encoding_on_df_file_path)
+					st.write(apply_encoding_on_df_pipe)
+					data = apply_encoding_on_df(data, apply_encoding_on_df_pipe)
 				else:
-					st.write("No file named 'discretize_output_col.pkl' found in the current directory.")
-		except Exception as e:
-			print("e23", e)
-			
-		try:
-			apply_encoding_on_df_file_path = os.path.join(cwd, "apply_encoding_on_df.pkl")
-			if os.path.isfile(apply_encoding_on_df_file_path):
-				st.write(f"File 'apply_encoding_on_df.pkl' found at {apply_encoding_on_df_file_path}")
-				apply_encoding_on_df_pipe = joblib.load(apply_encoding_on_df_file_path)
-				st.write(apply_encoding_on_df_pipe)
-				data = apply_encoding_on_df(data, apply_encoding_on_df_pipe)
-			else:
-				st.write("No file named 'apply_encoding_on_df.pkl' found in the current directory.")
-		except Exception as e:
-			print("e24", e)
-
-		try:
-			col_dum_files = glob.glob(os.path.join(cwd, "*apply_encoding_on_col.pkl"))
-			for apply_encoding_on_col_file_path in col_dum_files:
-				if os.path.isfile(apply_encoding_on_col_file_path):
-					st.write(f"File 'apply_encoding_on_col.pkl' found at {apply_encoding_on_col_file_path}")
-					apply_encoding_on_col_pipe = joblib.load(apply_encoding_on_col_file_path)
-					st.write(apply_encoding_on_col_pipe)
+					st.write("No file named 'apply_encoding_on_df.pkl' found in the current directory.")
+			except Exception as e:
+				print("e24", e)
+
+			try:
+				col_dum_files = glob.glob(os.path.join(cwd, "*apply_encoding_on_col.pkl"))
+				for apply_encoding_on_col_file_path in col_dum_files:
+					if os.path.isfile(apply_encoding_on_col_file_path):
+						st.write(f"File 'apply_encoding_on_col.pkl' found at {apply_encoding_on_col_file_path}")
+						apply_encoding_on_col_pipe = joblib.load(apply_encoding_on_col_file_path)
+						st.write(apply_encoding_on_col_pipe)
+						try:
+							data = apply_encoding_on_col(data, apply_encoding_on_col_pipe)
+						except Exception as e:
+							print("e27", e)
+					else:
+						st.write("No file named 'apply_encoding_on_col.pkl' found in the current directory.")
+			except Exception as e:
+				print("e25", e)
+
+			try:
+				apply_scaling_on_df_file_path = os.path.join(cwd, "apply_scaling_on_df.pkl")
+				if os.path.isfile(apply_scaling_on_df_file_path):
+					st.write(f"File 'apply_scaling_on_df.pkl' found at {apply_scaling_on_df_file_path}")
+					apply_scaling_on_df_pipe = joblib.load(apply_scaling_on_df_file_path)
+					st.write(apply_scaling_on_df_pipe)
 					try:
-						data = apply_encoding_on_col(data, apply_encoding_on_col_pipe)
+						data = apply_scaling_on_df(data, apply_scaling_on_df_pipe)
 					except Exception as e:
-						print("e27", e)
+						print("e26", e)
 				else:
-					st.write("No file named 'apply_encoding_on_col.pkl' found in the current directory.")
-		except Exception as e:
-			print("e25", e)
-
-		try:
-			apply_scaling_on_df_file_path = os.path.join(cwd, "apply_scaling_on_df.pkl")
-			if os.path.isfile(apply_scaling_on_df_file_path):
-				st.write(f"File 'apply_scaling_on_df.pkl' found at {apply_scaling_on_df_file_path}")
-				apply_scaling_on_df_pipe = joblib.load(apply_scaling_on_df_file_path)
-				st.write(apply_scaling_on_df_pipe)
-				try:
-					data = apply_scaling_on_df(data, apply_scaling_on_df_pipe)
-				except Exception as e:
-					print("e26", e)
-			else:
-				st.write("No file named 'apply_scaling_on_df.pkl' found in the current directory.")
-		except Exception as e:
-			print("e26", e)
+					st.write("No file named 'apply_scaling_on_df.pkl' found in the current directory.")
+			except Exception as e:
+				print("e26", e)
+			try:
+				data = data.reset_index(drop=True)
+			except:
+				pass
+		elif choice == "Use Validation Data":
+			data = df0
+			data = data.reset_index(drop=True)
+		
 
 	elif type_ == 'Manual Input':
 		# st.warning("hi1")
 		random_row = dfo.sample(1).iloc[0]
 
 		# Detect the data type and range of each column
 		column_details = {}
@@ -905,12 +934,13 @@
 			elif type_ == 'Manual Input':
 				st.warning("Not Yet Released")
 				st.success("Comming Soon 🔜 @ https://pypi.org/project/glook/")
 		except UnboundLocalError:
 			st.warning("Upload .csv or .xlsx")
 		except Exception as e:
 			st.error(e)
+			print(e)
 		
 if __name__=='__main__':
 	main()
```

### Comparing `glook-1.2.0b1/glook/pages/1_General_Data_Insights.py` & `glook-1.2.1b1/glook/pages/1_General_Data_Insights.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 import streamlit as st
 import pandas as pd
 import plotly.graph_objects as go
 from io import StringIO
-st.set_page_config(page_title="GLook", layout="wide")
+st.set_page_config(
+	# page_title="ML-Automation", 
+	page_title="Auto - EDA", 
+	page_icon="👁️", 
+	layout="wide", 
+	initial_sidebar_state = "expanded",
+	menu_items={
+        'Get Help': 'https://github.com/gaurang157/glook/blob/main/README.md',
+        'Report a bug': "https://github.com/gaurang157/glook/issues",
+        'About': "# This is Auto EDA Library. This is an *extremely* cool app!"
+		}
+		)
 st.write("Session State:->", st.session_state["shared"])
 
 
 if "df" in st.session_state and st.session_state.df is not None:
 	# df = st.session_state.df
 	oragnial_df = st.session_state.df
 	df_to_pre = st.session_state.df_pre
@@ -37,68 +48,26 @@
 	num_features = len(df.columns)
 
 	# Get number of categorical features
 	num_categorical = len(df.select_dtypes(include=['object']).columns)
 
 	# Get number of numerical features
 	num_numerical = len(df.select_dtypes(include=['number']).columns)
-
 	
-	# st.dataframe(df)
-	# Exclude non-numeric columns
-	numeric_df = df.select_dtypes(include='number')
-
-	# Convert non-numeric values to NaN
-	numeric_df = numeric_df.apply(pd.to_numeric, errors='coerce')
-	st.header(":green[Correlation Coefficient]")
-	# Calculate the correlation matrix
-	correlation_matrix = numeric_df.corr()
-	# Define the list of colorscales
-	# colorscales = ['aggrnyl', 'agsunset', 'algae', 'amp', 'armyrose', 'balance', 'blackbody', 'bluered', 'blues', 'blugrn', 'bluyl', 'brbg', 'brwnyl', 'bugn', 'bupu', 'burg', 'burgyl', 'cividis', 'curl', 'darkmint', 'deep', 'delta', 'dense', 'earth', 'edge', 'electric', 'emrld', 'fall', 'geyser', 'gnbu', 'gray', 'greens', 'greys', 'haline', 'hot', 'hsv', 'ice', 'icefire', 'inferno', 'jet', 'magenta', 'magma', 'matter', 'mint', 'mrybm', 'mygbm', 'oranges', 'orrd', 'oryel', 'oxy', 'peach', 'phase', 'picnic', 'pinkyl', 'piyg', 'plasma', 'plotly3', 'portland', 'prgn', 'pubu', 'pubugn', 'puor', 'purd', 'purp', 'purples', 'purpor', 'rainbow', 'rdbu', 'rdgy', 'rdpu', 'rdylbu', 'rdylgn', 'redor', 'reds', 'solar', 'spectral', 'speed', 'sunset', 'sunsetdark', 'teal', 'tealgrn', 'tealrose', 'tempo', 'temps', 'thermal', 'tropic', 'turbid', 'turbo', 'twilight', 'viridis', 'ylgn', 'ylgnbu', 'ylorbr', 'ylorrd']
-	# Number input for selecting the colorscale index
-	# colorscale_index = st.number_input('Select a colorscale index:', min_value=0, max_value=len(colorscales)-1, value=0)
-	# st.write(colorscales[colorscale_index])
-	# Create the heatmap plot
-
-	fig = go.Figure(data=go.Heatmap(
-		z=correlation_matrix.values,
-		x=correlation_matrix.columns,
-		y=correlation_matrix.index,
-		# colorscale=colorscales[colorscale_index],  # You can choose any colorscale
-		colorscale='aggrnyl',
-		text=correlation_matrix.values,  # Values to display
-		texttemplate='%{text:.2f}',  # Format for displaying values
-		showscale=True  # Display the color scale on the side
-	))
-
-	# Add title and axis labels
-	fig.update_layout(
-		title='Correlation Coefficient Heatmap',
-		xaxis=dict(title='Columns'),
-		yaxis=dict(title='Columns'),
-		width=700,  # Adjust width
-		height=700,  # Adjust height
-
-	)
-
-	# Show the plot
-	st.plotly_chart(fig)
-
-	st.header(":green[Edit Data] to Suit Your Needs:")
-	df = st.data_editor(df)
-
-
-	# Capture the output of df.info()
-	info_buffer = StringIO()
-	df.info(buf=info_buffer)
-	info_str = info_buffer.getvalue()
-
-	# Display the info in Streamlit
-	st.subheader("DataFrame :green[Info:]")
-	st.code(info_str, language="neon")
+	# Display the insights
+	st.subheader(f"Data dimensions: :green[{num_rows} rows, {num_columns} columns]")
+	st.subheader(f"Number of rows: :green[{num_rows}]")
+	st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
+	st.subheader(f"Deep Memory usage: :green[{memory_usage:.3f} MB]")
+	st.subheader(f"Number of features: :green[{num_features}]")
+	st.subheader(f"Number of categorical features: :green[{num_categorical}]")
+	st.subheader(f"Number of numerical features: :green[{num_numerical}]")
+	st.subheader("Customize DataFrame Values to Fit Your Requirements:")
+	st.text("Note: Double tap to Change Values")
+	st.data_editor(df)
 
 
 	try:
 		st.header("Numerical :green[Data Overview]")
 		# df_info = df.describe().T
 		# styled_df_info = df_info.style.highlight_max(axis=0).highlight_min(axis=0).format("{:.2f}")
 		df_info = (
@@ -135,22 +104,24 @@
 			.highlight_min(axis=0, props='background-color: yellowgreen; color: black;')  # Highlight min values with another color
 			# .format("{:.2f}")
 		)
 
 		st.dataframe(styled_df_info1)
 	except ValueError:
 		st.dataframe()
-	# Display the insights
-	st.subheader(f"Data dimensions: :green[{num_rows} rows, {num_columns} columns]")
-	st.subheader(f"Number of rows: :green[{num_rows}]")
-	st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
-	st.subheader(f"Deep Memory usage: :green[{memory_usage:.3f} MB]")
-	st.subheader(f"Number of features: :green[{num_features}]")
-	st.subheader(f"Number of categorical features: :green[{num_categorical}]")
-	st.subheader(f"Number of numerical features: :green[{num_numerical}]")
+
+
+	# Capture the output of df.info()
+	info_buffer = StringIO()
+	df.info(buf=info_buffer)
+	info_str = info_buffer.getvalue()
+
+	# Display the info in Streamlit
+	st.subheader("DataFrame :green[Info:]")
+	st.code(info_str, language="neon")
 	
 
 
 else:
 	st.write("DataFrame not yet uploaded.")
 # if st.sidebar.button("Univariate Analysis"):
 	# st.switch_page("pages/2_Univariate_Analysis.py")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `glook-1.2.0b1/glook/pages/2_Univariate_Analysis.py` & `glook-1.2.1b1/glook/pages/2_Univariate_Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,14 +160,15 @@
 
 
 
 try:
 	# Assuming df is already defined and stored in session_state
 	
 	if "df" in st.session_state and st.session_state.df is not None:
+		st.title("1️⃣ Univariate Analysis")
 		oragnial_df = st.session_state.df
 		df_to_pre = st.session_state.df_pre
 		# st.warning("kl")
 		to_select = st.selectbox("Select Data Frame (Recommended Oragnial DF)", ["oragnial_df", "df_to_pre_process"], index=0)
 		if to_select == "oragnial_df":
 			df = oragnial_df
 		elif to_select == "df_to_pre_process":
@@ -201,15 +202,15 @@
 		# st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
 		# st.subheader(f"Memory usage: :green[{memory_usage:.1f} KB]")
 		# st.subheader(f"Number of features: :green[{num_features}]")
 		# st.subheader(f"Number of categorical features: :green[{num_categorical}]")
 		# st.subheader(f"Number of numerical features: :green[{num_numerical}]")
 		
 		# Display insights for each column
-		st.title("1️⃣ Univariate Analysis")                                                                  # PROBLEM
+		                                                                  # PROBLEM
 		# st.header(":green[Column Insights:]⤵️")
 		# html_content = ""
 		for idx, column in enumerate(df.columns):
 			# st.subheader(f':green[**Column {idx + 1}:** {column}]')
 			# subh = f""":green[Column {idx + 1}: {column}]"""
 			# st.subheader(subh)
 			# subh = f"**Column {idx + 1}:** `{column}`"
@@ -485,17 +486,18 @@
 							},
 							height=500,  # Set the plot height
 						)
 						st.plotly_chart(fig)
 
 					with tab3:
 						# plt.figure(figsize=(10, 6))  # Adjust figure size
-
+						missing_value = additional_stats.get('Missing')
+						if missing_value != 0:
+							st.write(":grey[Note: The theoretical line will be visible when there are no missing values.]")
 						# Generate QQ plot
-						st.write(":grey[Note: The theoretical line will be visible when there are no missing values.]")
 						qqplot_data = sm.qqplot(df[column], line='s').gca().lines
 
 						fig = go.Figure()
 						fig.add_trace({
 							'type': 'scatter',
 							'x': qqplot_data[0].get_xdata(),
 							'y': qqplot_data[0].get_ydata(),
```

### Comparing `glook-1.2.0b1/glook/pages/5_Pre_Processing.py` & `glook-1.2.1b1/glook/pages/5_Pre_Processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -2915,15 +2915,15 @@
 				st.session_state.col_dum = col_dum_no
 				st.rerun()
 				print(595)
 
 
 	elif preprocessing_action == 'Apply Scaling':
 		scaling_method = st.selectbox('Select scaling method', [
-			'Standardize Scaling', 'Min-Max Scaling', 'Robust Scaling'])
+			'Standardize Scaling', 'Min-Max Scaling', 'Robust Scaling'], index=1)
 		if st.button('Apply', on_click=callback
 			) or st.session_state.button_clicked:
 			modified_df = df.copy()
 			modified_df = apply_scaling(modified_df, scaling_method)
 			st.write('Modified DataFrame:')
 			print(596)
 			st.write(modified_df)
```

### Comparing `glook-1.2.0b1/glook/pages/7_Dimensionality_Reduction.py` & `glook-1.2.1b1/glook/pages/7_Dimensionality_Reduction.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 try:
 	st.write("Session State:->", st.session_state["shared"])
 	# Streamlit UI for data splitting
 	# st.title("Data Splitting Page")
 
 	# Display the modified DataFrame
 	# st.subheader("Modified DataFrame")
-	if "df" in st.session_state:
-		df = st.session_state.df
+	if "df_pre" in st.session_state:
+		# df = st.session_state.df
+		df_to_pre = st.session_state.df_pre
+		df = df_to_pre
 		# Assuming df is your DataFrame
 		# df.to_csv('your_file.csv', index=False)
 		# Data split options
 		# st.write(df)
 		# target_column = st.sidebar.selectbox("Select the target column:", df.columns)
 		# test_size = st.sidebar.slider("Select the test size:", 0.1, 0.5, step=0.05)
 		# random_state = st.sidebar.number_input("Enter the random state:", min_value=0, max_value=10000, value=42)
```

### Comparing `glook-1.2.0b1/glook/pages/8_Supervised_Learning.py` & `glook-1.2.1b1/glook/pages/8_Supervised_Learning.py`

 * *Files identical despite different names*

### Comparing `glook-1.2.0b1/glook.egg-info/SOURCES.txt` & `glook-1.2.1b1/glook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glook-1.2.0b1/look/GLook.py` & `glook-1.2.1b1/look/GLook.py`

 * *Files identical despite different names*

### Comparing `glook-1.2.0b1/look/pages/1_General_Data_Insights.py` & `glook-1.2.1b1/look/pages/1_General_Data_Insights.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 import streamlit as st
 import pandas as pd
 import plotly.graph_objects as go
 from io import StringIO
-st.set_page_config(page_title="GLook", layout="wide")
+st.set_page_config(
+	# page_title="ML-Automation", 
+	page_title="Auto - EDA", 
+	page_icon="👁️", 
+	layout="wide", 
+	initial_sidebar_state = "expanded",
+	menu_items={
+        'Get Help': 'https://github.com/gaurang157/glook/blob/main/README.md',
+        'Report a bug': "https://github.com/gaurang157/glook/issues",
+        'About': "# This is Auto EDA Library. This is an *extremely* cool app!"
+		}
+		)
 st.write("Session State:->", st.session_state["shared"])
 
 
 if "df" in st.session_state and st.session_state.df is not None:
 	df = st.session_state.df
 	# Get number of rows
 	num_rows = df.shape[0]
@@ -29,67 +40,23 @@
 
 	# Get number of categorical features
 	num_categorical = len(df.select_dtypes(include=['object']).columns)
 
 	# Get number of numerical features
 	num_numerical = len(df.select_dtypes(include=['number']).columns)
 
-	
-	# st.dataframe(df)
-	# Exclude non-numeric columns
-	numeric_df = df.select_dtypes(include='number')
-
-	# Convert non-numeric values to NaN
-	numeric_df = numeric_df.apply(pd.to_numeric, errors='coerce')
-	st.header("Correlation Coefficient :green[Heatmap]")
-	# Calculate the correlation matrix
-	correlation_matrix = numeric_df.corr()
-	# Define the list of colorscales
-	# colorscales = ['aggrnyl', 'agsunset', 'algae', 'amp', 'armyrose', 'balance', 'blackbody', 'bluered', 'blues', 'blugrn', 'bluyl', 'brbg', 'brwnyl', 'bugn', 'bupu', 'burg', 'burgyl', 'cividis', 'curl', 'darkmint', 'deep', 'delta', 'dense', 'earth', 'edge', 'electric', 'emrld', 'fall', 'geyser', 'gnbu', 'gray', 'greens', 'greys', 'haline', 'hot', 'hsv', 'ice', 'icefire', 'inferno', 'jet', 'magenta', 'magma', 'matter', 'mint', 'mrybm', 'mygbm', 'oranges', 'orrd', 'oryel', 'oxy', 'peach', 'phase', 'picnic', 'pinkyl', 'piyg', 'plasma', 'plotly3', 'portland', 'prgn', 'pubu', 'pubugn', 'puor', 'purd', 'purp', 'purples', 'purpor', 'rainbow', 'rdbu', 'rdgy', 'rdpu', 'rdylbu', 'rdylgn', 'redor', 'reds', 'solar', 'spectral', 'speed', 'sunset', 'sunsetdark', 'teal', 'tealgrn', 'tealrose', 'tempo', 'temps', 'thermal', 'tropic', 'turbid', 'turbo', 'twilight', 'viridis', 'ylgn', 'ylgnbu', 'ylorbr', 'ylorrd']
-	# Number input for selecting the colorscale index
-	# colorscale_index = st.number_input('Select a colorscale index:', min_value=0, max_value=len(colorscales)-1, value=0)
-	# st.write(colorscales[colorscale_index])
-	# Create the heatmap plot
-
-	fig = go.Figure(data=go.Heatmap(
-		z=correlation_matrix.values,
-		x=correlation_matrix.columns,
-		y=correlation_matrix.index,
-		# colorscale=colorscales[colorscale_index],  # You can choose any colorscale
-		colorscale='aggrnyl',
-		text=correlation_matrix.values,  # Values to display
-		texttemplate='%{text:.2f}',  # Format for displaying values
-		showscale=True  # Display the color scale on the side
-	))
-
-	# Add title and axis labels
-	fig.update_layout(
-		title='Correlation Coefficient Heatmap',
-		xaxis=dict(title='Columns'),
-		yaxis=dict(title='Columns'),
-		width=700,  # Adjust width
-		height=700,  # Adjust height
-
-	)
-
-	# Show the plot
-	st.plotly_chart(fig)
-
-	st.header(":green[Edit Data] to Suit Your Needs:")
-	df = st.data_editor(df)
-
-
-	# Capture the output of df.info()
-	info_buffer = StringIO()
-	df.info(buf=info_buffer)
-	info_str = info_buffer.getvalue()
 
-	# Display the info in Streamlit
-	st.subheader("DataFrame :green[Info:]")
-	st.code(info_str, language="neon")
+	# Display the insights
+	st.subheader(f"Data dimensions: :green[{num_rows} rows, {num_columns} columns]")
+	st.subheader(f"Number of rows: :green[{num_rows}]")
+	st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
+	st.subheader(f"Deep Memory usage: :green[{memory_usage:.3f} MB]")
+	st.subheader(f"Number of features: :green[{num_features}]")
+	st.subheader(f"Number of categorical features: :green[{num_categorical}]")
+	st.subheader(f"Number of numerical features: :green[{num_numerical}]")
 
 
 	try:
 		st.header("Numerical :green[Data Overview]")
 		# df_info = df.describe().T
 		# styled_df_info = df_info.style.highlight_max(axis=0).highlight_min(axis=0).format("{:.2f}")
 		df_info = (
@@ -126,22 +93,24 @@
 			.highlight_min(axis=0, props='background-color: yellowgreen; color: black;')  # Highlight min values with another color
 			# .format("{:.2f}")
 		)
 
 		st.dataframe(styled_df_info1)
 	except ValueError:
 		st.dataframe()
-	# Display the insights
-	st.subheader(f"Data dimensions: :green[{num_rows} rows, {num_columns} columns]")
-	st.subheader(f"Number of rows: :green[{num_rows}]")
-	st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
-	st.subheader(f"Deep Memory usage: :green[{memory_usage:.3f} MB]")
-	st.subheader(f"Number of features: :green[{num_features}]")
-	st.subheader(f"Number of categorical features: :green[{num_categorical}]")
-	st.subheader(f"Number of numerical features: :green[{num_numerical}]")
+
+
+	# Capture the output of df.info()
+	info_buffer = StringIO()
+	df.info(buf=info_buffer)
+	info_str = info_buffer.getvalue()
+
+	# Display the info in Streamlit
+	st.subheader("DataFrame :green[Info:]")
+	st.code(info_str, language="neon")
 	
 
 
 else:
 	st.write("DataFrame not yet uploaded.")
 # if st.sidebar.button("Univariate Analysis"):
 	# st.switch_page("pages/2_Univariate_Analysis.py")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `glook-1.2.0b1/look/pages/2_Univariate_Analysis.py` & `glook-1.2.1b1/look/pages/2_Univariate_Analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,15 +477,17 @@
 							},
 							height=500,  # Set the plot height
 						)
 						st.plotly_chart(fig)
 
 					with tab3:
 						# plt.figure(figsize=(10, 6))  # Adjust figure size
-
+						missing_value = additional_stats.get('Missing')
+						if missing_value != 0:
+							st.write(":grey[Note: The theoretical line will be visible when there are no missing values.]")
 						# Generate QQ plot
 						qqplot_data = sm.qqplot(df[column], line='s').gca().lines
 
 						fig = go.Figure()
 						fig.add_trace({
 							'type': 'scatter',
 							'x': qqplot_data[0].get_xdata(),
```

### Comparing `glook-1.2.0b1/setup.py` & `glook-1.2.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="glook",
-    version="1.2.0b1",
+    version="1.2.1b1",
     author="Gaurang Ingle",
     author_email="gaurang.ingle@gmail.com",
     description="Auto EDA.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaurang157/glook",
     packages=find_packages(),
```

