# Comparing `tmp/df_analyze-0.1.0-py3-none-any.whl.zip` & `tmp/df_analyze-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 161976 bytes, number of entries: 54
+Zip file size: 161986 bytes, number of entries: 54
 -rw-r--r--  2.0 unx      107 b- defN 20-Feb-02 00:00 df_analyze/__init__.py
 -rw-r--r--  2.0 unx       59 b- defN 20-Feb-02 00:00 df_analyze/__main__.py
 -rw-r--r--  2.0 unx     6054 b- defN 20-Feb-02 00:00 df_analyze/_constants.py
 -rw-r--r--  2.0 unx     5441 b- defN 20-Feb-02 00:00 df_analyze/_main.py
 -rw-r--r--  2.0 unx     2126 b- defN 20-Feb-02 00:00 df_analyze/_setup.py
 -rw-r--r--  2.0 unx     1005 b- defN 20-Feb-02 00:00 df_analyze/_types.py
 -rw-r--r--  2.0 unx    17108 b- defN 20-Feb-02 00:00 df_analyze/enumerables.py
@@ -45,12 +45,12 @@
 -rw-r--r--  2.0 unx    13801 b- defN 20-Feb-02 00:00 df_analyze/selection/filter.py
 -rw-r--r--  2.0 unx     2270 b- defN 20-Feb-02 00:00 df_analyze/selection/models.py
 -rw-r--r--  2.0 unx    11378 b- defN 20-Feb-02 00:00 df_analyze/selection/stepwise.py
 -rw-r--r--  2.0 unx     5065 b- defN 20-Feb-02 00:00 df_analyze/selection/wrapper.py
 -rw-r--r--  2.0 unx    10433 b- defN 20-Feb-02 00:00 df_analyze/sklearn_pasta/_sequential.py
 -rw-r--r--  2.0 unx     2190 b- defN 20-Feb-02 00:00 df_analyze/sklearn_pasta/_tags.py
 -rw-r--r--  2.0 unx    15635 b- defN 20-Feb-02 00:00 df_analyze/testing/datasets.py
-?rw-r--r--  2.0 unx    43786 b- defN 20-Feb-02 00:00 df_analyze-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 df_analyze-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 df_analyze-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     4680 b- defN 20-Feb-02 00:00 df_analyze-0.1.0.dist-info/RECORD
-54 files, 547796 bytes uncompressed, 154562 bytes compressed:  71.8%
+?rw-r--r--  2.0 unx    43815 b- defN 20-Feb-02 00:00 df_analyze-0.1.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 df_analyze-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 df_analyze-0.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     4680 b- defN 20-Feb-02 00:00 df_analyze-0.1.1.dist-info/RECORD
+54 files, 547825 bytes uncompressed, 154572 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: df_analyze/sklearn_pasta/_tags.py
 Comment: 
 
 Filename: df_analyze/testing/datasets.py
 Comment: 
 
-Filename: df_analyze-0.1.0.dist-info/METADATA
+Filename: df_analyze-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: df_analyze-0.1.0.dist-info/WHEEL
+Filename: df_analyze-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: df_analyze-0.1.0.dist-info/entry_points.txt
+Filename: df_analyze-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: df_analyze-0.1.0.dist-info/RECORD
+Filename: df_analyze-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `df_analyze-0.1.0.dist-info/METADATA` & `df_analyze-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.3
 Name: df-analyze
-Version: 0.1.0
+Version: 0.1.1
 Summary: Add your description here
 Author-email: Derek Berger <dmberger.dev@gmail.com>
 Requires-Python: >=3.9
 Requires-Dist: joblib>=1.4.2
 Requires-Dist: jsonpickle>=3.0.4
 Requires-Dist: lightgbm>=4.3.0
 Requires-Dist: matplotlib>=3.9.0
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: openml>=0.14.2
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: optuna>=3.6.1
 Requires-Dist: pandas>=2.2.2
+Requires-Dist: pytest>=8.2.1
 Requires-Dist: scikit-learn>=1.4.2
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: skorch>=0.15.0
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: torch>=2.3.0
 Requires-Dist: torchvision>=0.18.0
 Requires-Dist: tqdm>=4.64.1
```

## Comparing `df_analyze-0.1.0.dist-info/RECORD` & `df_analyze-0.1.1.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -44,11 +44,11 @@
 df_analyze/selection/filter.py,sha256=XgUei3oxnM_p1E4Pbpjp1Xl3XSzycGZtlxBICuNKUuA,13801
 df_analyze/selection/models.py,sha256=f79nCRQFRfho6g2nVpuSEHL-uU2WmSxhKUjLpTbuoQg,2270
 df_analyze/selection/stepwise.py,sha256=io_g2p6a_SMc6L2MmXozhQNR89KaT5edAfjWZT0B8x0,11378
 df_analyze/selection/wrapper.py,sha256=hw9BpIJhNYqplJ3n_rAxAnrh0hfRVAAs32cx8eD5iNM,5065
 df_analyze/sklearn_pasta/_sequential.py,sha256=pBMfjpTlhj-8Rm3_49iRSs8rvCnG25bmGO5uiMHGjFA,10433
 df_analyze/sklearn_pasta/_tags.py,sha256=dt3r7baK1SXkQ1XCfYIoa8iZ6pMkoQVPUN6kCHBN4fQ,2190
 df_analyze/testing/datasets.py,sha256=7YG1gZpVQj7OGcgu965Nb4hZ5vgQPLsgRMfC7vYHXiE,15635
-df_analyze-0.1.0.dist-info/METADATA,sha256=poWegy2ccnwphLzFoPofl4VLHJNErgX5GraYK2yVrNk,43786
-df_analyze-0.1.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-df_analyze-0.1.0.dist-info/entry_points.txt,sha256=qHXW3wVtLlyTIG-YzV_czgFsLsFb4zGRefnszJZyXsg,47
-df_analyze-0.1.0.dist-info/RECORD,,
+df_analyze-0.1.1.dist-info/METADATA,sha256=hopPvTH74Un1_Iy4KjXeRj-N9CfUhnWarnd-yQFVSmU,43815
+df_analyze-0.1.1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+df_analyze-0.1.1.dist-info/entry_points.txt,sha256=qHXW3wVtLlyTIG-YzV_czgFsLsFb4zGRefnszJZyXsg,47
+df_analyze-0.1.1.dist-info/RECORD,,
```

