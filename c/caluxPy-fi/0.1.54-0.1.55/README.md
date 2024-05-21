# Comparing `tmp/caluxpy_fi-0.1.54.tar.gz` & `tmp/caluxpy_fi-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluxpy_fi-0.1.54.tar", last modified: Fri May 17 14:14:24 2024, max compression
+gzip compressed data, was "caluxpy_fi-0.1.55.tar", last modified: Tue May 21 13:42:41 2024, max compression
```

## Comparing `caluxpy_fi-0.1.54.tar` & `caluxpy_fi-0.1.55.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 14:14:24.438005 caluxpy_fi-0.1.54/
--rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.54/LICENSE.txt
--rw-rw-rw-   0        0        0     4738 2024-05-17 14:14:24.438005 caluxpy_fi-0.1.54/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.54/README.md
--rw-rw-rw-   0        0        0      824 2024-05-17 14:13:06.000000 caluxpy_fi-0.1.54/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 14:14:24.438005 caluxpy_fi-0.1.54/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 14:14:24.314716 caluxpy_fi-0.1.54/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 14:14:24.422306 caluxpy_fi-0.1.54/src/caluxPy_fi/
--rw-rw-rw-   0        0        0     9533 2024-05-17 14:12:38.000000 caluxpy_fi-0.1.54/src/caluxPy_fi/Convexity.py
--rw-rw-rw-   0        0        0     1189 2024-05-06 14:57:42.000000 caluxpy_fi-0.1.54/src/caluxPy_fi/DataBase.py
--rw-rw-rw-   0        0        0     4215 2024-05-06 14:57:19.000000 caluxpy_fi-0.1.54/src/caluxPy_fi/ExternalImport.py
--rw-rw-rw-   0        0        0    10568 2024-05-06 14:54:58.000000 caluxpy_fi-0.1.54/src/caluxPy_fi/ExternalImport2.py
--rw-rw-rw-   0        0        0    58790 2024-05-06 14:47:32.000000 caluxpy_fi-0.1.54/src/caluxPy_fi/FixedIncome.py
--rw-rw-rw-   0        0        0     5781 2024-05-06 14:55:12.000000 caluxpy_fi-0.1.54/src/caluxPy_fi/Multiple.py
--rw-rw-rw-   0        0        0    13098 2024-05-06 14:51:25.000000 caluxpy_fi-0.1.54/src/caluxPy_fi/Portfolio.py
--rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.54/src/caluxPy_fi/Support.py
--rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.54/src/caluxPy_fi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:14:24.438005 caluxpy_fi-0.1.54/src/caluxPy_fi.egg-info/
--rw-rw-rw-   0        0        0     4738 2024-05-17 14:14:24.000000 caluxpy_fi-0.1.54/src/caluxPy_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2024-05-17 14:14:24.000000 caluxpy_fi-0.1.54/src/caluxPy_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 14:14:24.000000 caluxpy_fi-0.1.54/src/caluxPy_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-05-17 14:14:24.000000 caluxpy_fi-0.1.54/src/caluxPy_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 14:14:24.000000 caluxpy_fi-0.1.54/src/caluxPy_fi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 13:42:41.573713 caluxpy_fi-0.1.55/
+-rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.55/LICENSE.txt
+-rw-rw-rw-   0        0        0     4738 2024-05-21 13:42:41.571046 caluxpy_fi-0.1.55/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.55/README.md
+-rw-rw-rw-   0        0        0      824 2024-05-21 13:41:34.000000 caluxpy_fi-0.1.55/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:42:41.573713 caluxpy_fi-0.1.55/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 13:42:41.460066 caluxpy_fi-0.1.55/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 13:42:41.550717 caluxpy_fi-0.1.55/src/caluxPy_fi/
+-rw-rw-rw-   0        0        0     9625 2024-05-21 13:41:29.000000 caluxpy_fi-0.1.55/src/caluxPy_fi/Convexity.py
+-rw-rw-rw-   0        0        0     1189 2024-05-06 14:57:42.000000 caluxpy_fi-0.1.55/src/caluxPy_fi/DataBase.py
+-rw-rw-rw-   0        0        0     4215 2024-05-06 14:57:19.000000 caluxpy_fi-0.1.55/src/caluxPy_fi/ExternalImport.py
+-rw-rw-rw-   0        0        0    10568 2024-05-06 14:54:58.000000 caluxpy_fi-0.1.55/src/caluxPy_fi/ExternalImport2.py
+-rw-rw-rw-   0        0        0    58790 2024-05-06 14:47:32.000000 caluxpy_fi-0.1.55/src/caluxPy_fi/FixedIncome.py
+-rw-rw-rw-   0        0        0     5781 2024-05-06 14:55:12.000000 caluxpy_fi-0.1.55/src/caluxPy_fi/Multiple.py
+-rw-rw-rw-   0        0        0    13098 2024-05-06 14:51:25.000000 caluxpy_fi-0.1.55/src/caluxPy_fi/Portfolio.py
+-rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.55/src/caluxPy_fi/Support.py
+-rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.55/src/caluxPy_fi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:42:41.568167 caluxpy_fi-0.1.55/src/caluxPy_fi.egg-info/
+-rw-rw-rw-   0        0        0     4738 2024-05-21 13:42:41.000000 caluxpy_fi-0.1.55/src/caluxPy_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2024-05-21 13:42:41.000000 caluxpy_fi-0.1.55/src/caluxPy_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:42:41.000000 caluxpy_fi-0.1.55/src/caluxPy_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-21 13:42:41.000000 caluxpy_fi-0.1.55/src/caluxPy_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-21 13:42:41.000000 caluxpy_fi-0.1.55/src/caluxPy_fi.egg-info/top_level.txt
```

### Comparing `caluxpy_fi-0.1.54/LICENSE.txt` & `caluxpy_fi-0.1.55/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.54/PKG-INFO` & `caluxpy_fi-0.1.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.54
+Version: 0.1.55
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxpy_fi-0.1.54/README.md` & `caluxpy_fi-0.1.55/README.md`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.54/pyproject.toml` & `caluxpy_fi-0.1.55/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caluxPy_fi"
-version = "0.1.54"
+version = "0.1.55"
 authors = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 maintainers = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 description = "Fixed Income Valuation and Analysis"
```

### Comparing `caluxpy_fi-0.1.54/src/caluxPy_fi/Convexity.py` & `caluxpy_fi-0.1.55/src/caluxPy_fi/Convexity.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,18 +102,21 @@
         self.avg_dv01 = (first_neg + first_pos) / 2 # Get an averaged dv01 with the first occurrence of a marginal increase, because it can go both ways
         
         #Concatenating the dfs to form the complete one
         final = pd.concat([negatives, positives[1:]]) # Concatenate both results of gains and losses
         final.reset_index(drop = True, inplace = True) # Reset indexes so it can be incorporated into the original DataFrame
         self.df_convex[['dv01', 'gains/losses', 'Duration', 'Convexity']] = final[['dv01', 'gains/losses', 'Duration', 'Convexity']] # Incorporate gains and losses into the original DataFrame
         
-        final['Negative'] = final['pbs'] < 0 # Add a boolean column where True is if value of pbs is negative
-        max_values_by_category = final.groupby('Negative')['dv01'].max() # Group the data by the boolean column, having 2 groups (True and False) then getting max values of box, resulting into a list
-        avg_values_by_category = final.groupby('Negative')['dv01'].mean() # Get a list with the average means of both groups
-        std_values_by_category = final.groupby('Negative')['dv01'].std() # Get a list with the standard deviations of both groups
+        final_copy = final.copy()
+        final_copy['Negative'] = final_copy['pbs'] < 0 # Add a boolean column where True is if value of pbs is negative
+        #take out the 0
+        
+        max_values_by_category = final_copy.groupby('Negative')['dv01'].max() # Group the data by the boolean column, having 2 groups (True and False) then getting max values of box, resulting into a list
+        avg_values_by_category = final_copy.groupby('Negative')['dv01'].mean() # Get a list with the average means of both groups
+        std_values_by_category = final_copy.groupby('Negative')['dv01'].std() # Get a list with the standard deviations of both groups
 
         # Assigning values to the usable variables
         self.max_gain = max_values_by_category[True] 
         self.max_loss = max_values_by_category[False]
         self.avg_gain = avg_values_by_category[True]
         self.avg_loss = avg_values_by_category[False]
         self.std_gain = std_values_by_category[True]
```

### Comparing `caluxpy_fi-0.1.54/src/caluxPy_fi/DataBase.py` & `caluxpy_fi-0.1.55/src/caluxPy_fi/DataBase.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.54/src/caluxPy_fi/ExternalImport.py` & `caluxpy_fi-0.1.55/src/caluxPy_fi/ExternalImport.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.54/src/caluxPy_fi/ExternalImport2.py` & `caluxpy_fi-0.1.55/src/caluxPy_fi/ExternalImport2.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.54/src/caluxPy_fi/FixedIncome.py` & `caluxpy_fi-0.1.55/src/caluxPy_fi/FixedIncome.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.54/src/caluxPy_fi/Multiple.py` & `caluxpy_fi-0.1.55/src/caluxPy_fi/Multiple.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.54/src/caluxPy_fi/Portfolio.py` & `caluxpy_fi-0.1.55/src/caluxPy_fi/Portfolio.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.54/src/caluxPy_fi/Support.py` & `caluxpy_fi-0.1.55/src/caluxPy_fi/Support.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.54/src/caluxPy_fi.egg-info/PKG-INFO` & `caluxpy_fi-0.1.55/src/caluxPy_fi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.54
+Version: 0.1.55
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

