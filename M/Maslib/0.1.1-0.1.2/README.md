# Comparing `tmp/Maslib-0.1.1.tar.gz` & `tmp/Maslib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Maslib-0.1.1.tar", last modified: Mon May 20 16:41:12 2024, max compression
+gzip compressed data, was "Maslib-0.1.2.tar", last modified: Tue May 21 16:50:50 2024, max compression
```

## Comparing `Maslib-0.1.1.tar` & `Maslib-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 16:41:12.883592 Maslib-0.1.1/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.1.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-20 16:41:12.860987 Maslib-0.1.1/MasLib/
--rw-rw-rw-   0        0        0      661 2024-05-20 16:39:40.000000 Maslib-0.1.1/MasLib/__init__.py
--rw-rw-rw-   0        0        0     4174 2024-05-19 12:40:05.000000 Maslib-0.1.1/MasLib/clustering.py
--rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.1.1/MasLib/correlation.py
--rw-rw-rw-   0        0        0     2545 2024-05-20 16:39:17.000000 Maslib-0.1.1/MasLib/encoding.py
--rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.1.1/MasLib/grid_search_optimization.py
--rw-rw-rw-   0        0        0      465 2024-05-19 11:52:03.000000 Maslib-0.1.1/MasLib/loading.py
--rw-rw-rw-   0        0        0     5232 2024-05-19 11:16:36.000000 Maslib-0.1.1/MasLib/regressions.py
--rw-rw-rw-   0        0        0     8283 2024-05-20 16:40:21.000000 Maslib-0.1.1/MasLib/text_coding.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:41:12.880589 Maslib-0.1.1/Maslib.egg-info/
--rw-rw-rw-   0        0        0      848 2024-05-20 16:41:12.000000 Maslib-0.1.1/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2024-05-20 16:41:12.000000 Maslib-0.1.1/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 16:41:12.000000 Maslib-0.1.1/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-20 16:41:12.000000 Maslib-0.1.1/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 16:41:12.000000 Maslib-0.1.1/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      848 2024-05-20 16:41:12.882591 Maslib-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-19 12:47:41.000000 Maslib-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-20 16:41:12.883592 Maslib-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-05-20 16:40:14.000000 Maslib-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:41:12.877586 Maslib-0.1.1/tests/
--rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 Maslib-0.1.1/tests/test_clustering.py
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.1.1/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.1.1/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.1.1/tests/test_grid_search.py
--rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 Maslib-0.1.1/tests/test_loading.py
--rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 Maslib-0.1.1/tests/test_regression.py
--rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 Maslib-0.1.1/tests/test_text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:50:50.017732 Maslib-0.1.2/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.1.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-21 16:50:49.996714 Maslib-0.1.2/MasLib/
+-rw-rw-rw-   0        0        0      854 2024-05-21 16:49:15.000000 Maslib-0.1.2/MasLib/__init__.py
+-rw-rw-rw-   0        0        0     3909 2024-05-21 16:48:27.000000 Maslib-0.1.2/MasLib/classification.py
+-rw-rw-rw-   0        0        0     4174 2024-05-19 12:40:05.000000 Maslib-0.1.2/MasLib/clustering.py
+-rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.1.2/MasLib/correlation.py
+-rw-rw-rw-   0        0        0     3197 2024-05-21 16:49:28.000000 Maslib-0.1.2/MasLib/encoding.py
+-rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.1.2/MasLib/grid_search_optimization.py
+-rw-rw-rw-   0        0        0      465 2024-05-19 11:52:03.000000 Maslib-0.1.2/MasLib/loading.py
+-rw-rw-rw-   0        0        0     5232 2024-05-19 11:16:36.000000 Maslib-0.1.2/MasLib/regressions.py
+-rw-rw-rw-   0        0        0    11608 2024-05-21 16:48:29.000000 Maslib-0.1.2/MasLib/text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:50:50.014731 Maslib-0.1.2/Maslib.egg-info/
+-rw-rw-rw-   0        0        0      848 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      848 2024-05-21 16:50:50.015732 Maslib-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-05-19 12:47:41.000000 Maslib-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:50:50.017732 Maslib-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-05-21 16:49:53.000000 Maslib-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:50:50.012728 Maslib-0.1.2/tests/
+-rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 Maslib-0.1.2/tests/test_clustering.py
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.1.2/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.1.2/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.1.2/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 Maslib-0.1.2/tests/test_loading.py
+-rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 Maslib-0.1.2/tests/test_regression.py
+-rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 Maslib-0.1.2/tests/test_text_coding.py
```

### Comparing `Maslib-0.1.1/MasLib/__init__.py` & `Maslib-0.1.2/MasLib/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-from .encoding import number_encode_features, process_column_and_merge
+from .encoding import number_encode_features, process_column_and_merge,json_to_dataframe
 from .correlation import compute_phik_matrix, plot_phik_correlation_matrix
 from .regressions import gb_regression, rf_regression, lr_regression, catboost_regression, cross_val_evaluate
 from .grid_search_optimization import grid_search_gb_boost, grid_search_rf, grid_search_lr, grid_search_catboost
 from .loading import save_model
-from .text_coding import vectorize_text, lda_model, nmf_model, lsa_model, tfidf_vectorize_texts, elbow_method_tfidf
-from .clustering import scale_data, kmeans_clustering, hierarchical_clustering, dbscan_clustering, calculate_metrics, visualize_clustering
+from .text_coding import vectorize_text, lda_model, nmf_model, lsa_model, tfidf_vectorize_texts, elbow_method_tfidf, tfidf_vectorization, bert_topic_modeling, lda_topic_modeling
+from .clustering import scale_data, kmeans_clustering, hierarchical_clustering, dbscan_clustering, calculate_metrics, visualize_clustering
+from .classification import classification_with_svc, classification_with_random_forest, classification_with_knn
```

### Comparing `Maslib-0.1.1/MasLib/clustering.py` & `Maslib-0.1.2/MasLib/clustering.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.1/MasLib/correlation.py` & `Maslib-0.1.2/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.1/MasLib/grid_search_optimization.py` & `Maslib-0.1.2/MasLib/grid_search_optimization.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.1/MasLib/regressions.py` & `Maslib-0.1.2/MasLib/regressions.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.1/Maslib.egg-info/PKG-INFO` & `Maslib-0.1.2/Maslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Это моя библиотека для оптимизации кода для python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Maslib-0.1.1/Maslib.egg-info/SOURCES.txt` & `Maslib-0.1.2/Maslib.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 setup.py
 MasLib/__init__.py
+MasLib/classification.py
 MasLib/clustering.py
 MasLib/correlation.py
 MasLib/encoding.py
 MasLib/grid_search_optimization.py
 MasLib/loading.py
 MasLib/regressions.py
 MasLib/text_coding.py
```

### Comparing `Maslib-0.1.1/PKG-INFO` & `Maslib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Это моя библиотека для оптимизации кода для python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Maslib-0.1.1/setup.py` & `Maslib-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'phik',
         'matplotlib',
         'scikit-learn',
```

### Comparing `Maslib-0.1.1/tests/test_clustering.py` & `Maslib-0.1.2/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.1/tests/test_correlation.py` & `Maslib-0.1.2/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.1/tests/test_encoding.py` & `Maslib-0.1.2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.1/tests/test_grid_search.py` & `Maslib-0.1.2/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.1/tests/test_regression.py` & `Maslib-0.1.2/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.1/tests/test_text_coding.py` & `Maslib-0.1.2/tests/test_text_coding.py`

 * *Files identical despite different names*

