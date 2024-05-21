# Comparing `tmp/dpkits-1.2.3.tar.gz` & `tmp/dpkits-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpkits-1.2.3.tar", last modified: Fri May 10 06:48:03 2024, max compression
+gzip compressed data, was "dpkits-1.2.4.tar", last modified: Tue May 21 08:46:58 2024, max compression
```

## Comparing `dpkits-1.2.3.tar` & `dpkits-1.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 06:48:03.610378 dpkits-1.2.3/
--rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.2.3/LICENSE
--rw-rw-rw-   0        0        0    12196 2024-05-10 06:48:03.608365 dpkits-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.2.3/README.md
--rw-rw-rw-   0        0        0      626 2024-05-10 06:47:15.000000 dpkits-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 06:48:03.610378 dpkits-1.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 06:48:03.538125 dpkits-1.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 06:48:03.573798 dpkits-1.2.3/src/dpkits/
--rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.2.3/src/dpkits/__init__.py
--rw-rw-rw-   0        0        0    28970 2024-03-29 03:25:00.000000 dpkits-1.2.3/src/dpkits/ap_data_converter.py
--rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.2.3/src/dpkits/calculate_lsm.py
--rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.2.3/src/dpkits/codeframe_reader.py
--rw-rw-rw-   0        0        0     5209 2024-05-06 08:45:27.000000 dpkits-1.2.3/src/dpkits/data_analysis.py
--rw-rw-rw-   0        0        0     2798 2024-04-09 06:58:27.000000 dpkits-1.2.3/src/dpkits/data_processing.py
--rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.2.3/src/dpkits/data_transpose.py
--rw-rw-rw-   0        0        0    26578 2024-05-10 06:33:30.000000 dpkits-1.2.3/src/dpkits/table_formater.py
--rw-rw-rw-   0        0        0    66039 2024-04-24 03:29:44.000000 dpkits-1.2.3/src/dpkits/table_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-10 06:48:03.606366 dpkits-1.2.3/src/dpkits.egg-info/
--rw-rw-rw-   0        0        0    12196 2024-05-10 06:48:03.000000 dpkits-1.2.3/src/dpkits.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-05-10 06:48:03.000000 dpkits-1.2.3/src/dpkits.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 06:48:03.000000 dpkits-1.2.3/src/dpkits.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-10 06:48:03.000000 dpkits-1.2.3/src/dpkits.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 08:46:58.211915 dpkits-1.2.4/
+-rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0    12196 2024-05-21 08:46:58.209912 dpkits-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.2.4/README.md
+-rw-rw-rw-   0        0        0      626 2024-05-21 08:44:34.000000 dpkits-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 08:46:58.211915 dpkits-1.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 08:46:58.138457 dpkits-1.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 08:46:58.173342 dpkits-1.2.4/src/dpkits/
+-rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.2.4/src/dpkits/__init__.py
+-rw-rw-rw-   0        0        0    28970 2024-05-15 03:48:44.000000 dpkits-1.2.4/src/dpkits/ap_data_converter.py
+-rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.2.4/src/dpkits/calculate_lsm.py
+-rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.2.4/src/dpkits/codeframe_reader.py
+-rw-rw-rw-   0        0        0     5209 2024-05-06 08:45:27.000000 dpkits-1.2.4/src/dpkits/data_analysis.py
+-rw-rw-rw-   0        0        0     3241 2024-05-16 11:03:27.000000 dpkits-1.2.4/src/dpkits/data_processing.py
+-rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.2.4/src/dpkits/data_transpose.py
+-rw-rw-rw-   0        0        0    26578 2024-05-10 10:00:29.000000 dpkits-1.2.4/src/dpkits/table_formater.py
+-rw-rw-rw-   0        0        0    66209 2024-05-21 07:59:21.000000 dpkits-1.2.4/src/dpkits/table_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:46:58.207917 dpkits-1.2.4/src/dpkits.egg-info/
+-rw-rw-rw-   0        0        0    12196 2024-05-21 08:46:58.000000 dpkits-1.2.4/src/dpkits.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-05-21 08:46:58.000000 dpkits-1.2.4/src/dpkits.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 08:46:58.000000 dpkits-1.2.4/src/dpkits.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 08:46:58.000000 dpkits-1.2.4/src/dpkits.egg-info/top_level.txt
```

### Comparing `dpkits-1.2.3/LICENSE` & `dpkits-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.3/PKG-INFO` & `dpkits-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.2.3
+Version: 1.2.4
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dpkits-1.2.3/README.md` & `dpkits-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.3/pyproject.toml` & `dpkits-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpkits"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Hung Dao", email="hung.daotuan.1991@gmail.com" },
 ]
 description = "A small package for data processing"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dpkits-1.2.3/src/dpkits/__init__.py` & `dpkits-1.2.4/src/dpkits/__init__.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.3/src/dpkits/ap_data_converter.py` & `dpkits-1.2.4/src/dpkits/ap_data_converter.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.3/src/dpkits/calculate_lsm.py` & `dpkits-1.2.4/src/dpkits/calculate_lsm.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.3/src/dpkits/codeframe_reader.py` & `dpkits-1.2.4/src/dpkits/codeframe_reader.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.3/src/dpkits/data_analysis.py` & `dpkits-1.2.4/src/dpkits/data_analysis.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.3/src/dpkits/data_processing.py` & `dpkits-1.2.4/src/dpkits/data_processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import pandas as pd
 import numpy as np
 
 
 
 class DataProcessing:
 
+    def __init__(self):
+        pass
+
+
     @staticmethod
     def add_qres(df_data: pd.DataFrame, df_info: pd.DataFrame, dict_add_new_qres: dict, is_add_oe_col: bool = False) -> (pd.DataFrame, pd.DataFrame):
         info_col_name = ['var_name', 'var_lbl', 'var_type', 'val_lbl']
 
         for key, val in dict_add_new_qres.items():
 
             if val[1] in ['MA']:
@@ -73,7 +77,22 @@
         df_data.reset_index(drop=True, inplace=True)
         df_info.reset_index(drop=True, inplace=True)
 
         return df_data, df_info
 
 
 
+    def concept_evaluate(self, cpt_filename: str, ) -> (pd.DataFrame, dict):
+        # Here: May 16
+        # 1. clean inputted concept
+        # 2. create codeframe for each word for concept
+        # 3. match verbatim to concept codeframe
+        # 4. return dataframe with codes of the words in concept
+
+
+
+        
+        return pd.DataFrame(), dict()  # dataframe & codelíst
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dpkits-1.2.3/src/dpkits/data_transpose.py` & `dpkits-1.2.4/src/dpkits/data_transpose.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.3/src/dpkits/table_formater.py` & `dpkits-1.2.4/src/dpkits/table_formater.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.3/src/dpkits/table_generator.py` & `dpkits-1.2.4/src/dpkits/table_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1512,27 +1512,28 @@
                             else:
                                 df_qre = self.add_ma_qre_val_to_tbl_sig(df_qre, qre_info, dict_header_col_name, lst_sig_pair, sig_type, lst_sig_lvl, net_cat, net_val, None, weight_var)
 
                     else:
                         df_qre = self.add_ma_qre_val_to_tbl_sig(df_qre, qre_info, dict_header_col_name, lst_sig_pair, sig_type, lst_sig_lvl, cat, lbl, None, weight_var)
 
 
+            # BUGGING!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
             # SORTING---------------------------------------------------------------------------------------------------
             sort_opt = df_info.at[idx, 'sort']
 
-            if sort_opt:
-                is_asc = True if sort_opt == 'asc' else False
-                base_val = -999_999_999 if sort_opt == 'asc' else 999_999_999
-
-                df_qre['sort_col'] = df_qre[df_qre.columns.tolist()[5]]
-                df_qre.loc[df_qre['cat_val'] == 'base', 'sort_col'] = base_val
-
-                df_qre.sort_values(by=['sort_col'], ascending=is_asc, inplace=True, ignore_index=True)
-                df_qre.drop(columns=['sort_col'], inplace=True)
+            # if sort_opt:
+            #     is_asc = True if sort_opt == 'asc' else False
+            #     base_val = -999_999_999 if sort_opt == 'asc' else 999_999_999
+            #
+            #     df_qre['sort_col'] = df_qre[df_qre.columns.tolist()[5]]
+            #     df_qre.loc[df_qre['cat_val'] == 'base', 'sort_col'] = base_val
+            #
+            #     df_qre.sort_values(by=['sort_col'], ascending=is_asc, inplace=True, ignore_index=True)
+            #     df_qre.drop(columns=['sort_col'], inplace=True)
 
             # END SORTING-----------------------------------------------------------------------------------------------
 
             df_tbl = pd.concat([df_tbl, df_qre], axis=0, ignore_index=True)
 
             print(f'\t- Create table for {qre_name}[{qre_type}]: Done')
-
+        
         return df_tbl
```

### Comparing `dpkits-1.2.3/src/dpkits.egg-info/PKG-INFO` & `dpkits-1.2.4/src/dpkits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.2.3
+Version: 1.2.4
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

