# Comparing `tmp/timeseries_shaper-0.0.0.2-py3-none-any.whl.zip` & `tmp/timeseries_shaper-0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 19032 bytes, number of entries: 31
+Zip file size: 19083 bytes, number of entries: 31
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 16:00 timeseries-shaper/__init__.py
 -rw-rw-rw-  2.0 fat      289 b- defN 24-May-04 15:57 timeseries-shaper/base.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 16:00 timeseries-shaper/events/__init__.py
 -rw-rw-rw-  2.0 fat     5351 b- defN 24-May-04 14:49 timeseries-shaper/events/tolerance_deviation.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 16:00 timeseries-shaper/filter/__init__.py
 -rw-rw-rw-  2.0 fat     1341 b- defN 24-May-04 16:23 timeseries-shaper/filter/boolean_filter.py
 -rw-rw-rw-  2.0 fat     1479 b- defN 24-May-04 16:23 timeseries-shaper/filter/custom_filter.py
@@ -20,14 +20,14 @@
 -rw-rw-rw-  2.0 fat     5177 b- defN 24-May-04 19:49 timeseries_shaper/filter/datetime_filter.py
 -rw-rw-rw-  2.0 fat     4387 b- defN 24-May-04 16:23 timeseries_shaper/filter/datetime_filters.py
 -rw-rw-rw-  2.0 fat     2540 b- defN 24-May-04 19:54 timeseries_shaper/filter/numeric_filter.py
 -rw-rw-rw-  2.0 fat      757 b- defN 24-May-04 16:23 timeseries_shaper/filter/numeric_filters.py
 -rw-rw-rw-  2.0 fat     2791 b- defN 24-May-04 19:51 timeseries_shaper/filter/string_filter.py
 -rw-rw-rw-  2.0 fat     1722 b- defN 24-May-04 16:23 timeseries_shaper/filter/string_filters.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 16:00 timeseries_shaper/stats/__init__.py
--rw-rw-rw-  2.0 fat     1402 b- defN 24-May-04 19:19 timeseries_shaper/stats/numeric_stats.py
--rw-rw-rw-  2.0 fat     1093 b- defN 24-May-04 19:59 timeseries_shaper-0.0.0.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2715 b- defN 24-May-04 19:59 timeseries_shaper-0.0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-04 19:59 timeseries_shaper-0.0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 24-May-04 19:59 timeseries_shaper-0.0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2910 b- defN 24-May-04 19:59 timeseries_shaper-0.0.0.2.dist-info/RECORD
-31 files, 50691 bytes uncompressed, 14196 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat     1854 b- defN 24-May-10 13:41 timeseries_shaper/stats/numeric_stats.py
+-rw-rw-rw-  2.0 fat     1093 b- defN 24-May-21 14:22 timeseries_shaper-0.0.0.3.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2715 b- defN 24-May-21 14:22 timeseries_shaper-0.0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-21 14:22 timeseries_shaper-0.0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 24-May-21 14:22 timeseries_shaper-0.0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2910 b- defN 24-May-21 14:22 timeseries_shaper-0.0.0.3.dist-info/RECORD
+31 files, 51143 bytes uncompressed, 14247 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -72,23 +72,23 @@
 
 Filename: timeseries_shaper/stats/__init__.py
 Comment: 
 
 Filename: timeseries_shaper/stats/numeric_stats.py
 Comment: 
 
-Filename: timeseries_shaper-0.0.0.2.dist-info/LICENSE.txt
+Filename: timeseries_shaper-0.0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: timeseries_shaper-0.0.0.2.dist-info/METADATA
+Filename: timeseries_shaper-0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: timeseries_shaper-0.0.0.2.dist-info/WHEEL
+Filename: timeseries_shaper-0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: timeseries_shaper-0.0.0.2.dist-info/top_level.txt
+Filename: timeseries_shaper-0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: timeseries_shaper-0.0.0.2.dist-info/RECORD
+Filename: timeseries_shaper-0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## timeseries_shaper/stats/numeric_stats.py

```diff
@@ -17,22 +17,34 @@
         """Calculate the median of a specified column."""
         return self.dataframe[self.column_name].median()
 
     def column_std(self):
         """Calculate the standard deviation of a specified column."""
         return self.dataframe[self.column_name].std()
 
+    def column_variance(self):
+        """Calculate the variance of a specified column."""
+        return self.dataframe[self.column_name].var()
+
     def column_min(self):
         """Calculate the minimum value of a specified column."""
         return self.dataframe[self.column_name].min()
 
     def column_max(self):
         """Calculate the maximum value of a specified column."""
         return self.dataframe[self.column_name].max()
 
     def column_sum(self):
         """Calculate the sum of a specified column."""
         return self.dataframe[self.column_name].sum()
 
+    def column_kurtosis(self):
+        """Calculate the kurtosis of a specified column."""
+        return self.dataframe[self.column_name].kurt()
+
+    def column_skewness(self):
+        """Calculate the skewness of a specified column."""
+        return self.dataframe[self.column_name].skew()
+
     def describe(self) -> pd.DataFrame:
         """Provide a statistical summary for numeric columns in the DataFrame."""
         return self.dataframe.describe()
```

## Comparing `timeseries_shaper-0.0.0.2.dist-info/LICENSE.txt` & `timeseries_shaper-0.0.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `timeseries_shaper-0.0.0.2.dist-info/METADATA` & `timeseries_shaper-0.0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseries-shaper
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: timeseries-shaper filters, transforms and abstracts your timeseries dataframe
 Home-page: https://jakobgabriel.github.io/timeseries-shaper/
 Author: Jakob Gabriel
 Author-email: jakob.gabriel5@googlemail.com
 Project-URL: Bug Tracker, https://github.com/jakobgabriel/timeseries-shaper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `timeseries_shaper-0.0.0.2.dist-info/RECORD` & `timeseries_shaper-0.0.0.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 timeseries_shaper/filter/datetime_filter.py,sha256=f95ZuDKIkFJE7CSfP_rGP_07U_aXS-AJLB-_Ci6_g30,5177
 timeseries_shaper/filter/datetime_filters.py,sha256=HjNMNCOtV4Q7equBEqNGxA2p3wgFonRCvqsKnURTahI,4387
 timeseries_shaper/filter/numeric_filter.py,sha256=uBJ5Fse9GTqmDpfrHyOFDBCaMQtnJdzjrWP4CHcPVPU,2540
 timeseries_shaper/filter/numeric_filters.py,sha256=c9wtarJovOJCFAYPrckl4rXvD2NjJLCJZafAOc6yQ8k,757
 timeseries_shaper/filter/string_filter.py,sha256=qhqKgid8j_5ts-KQWaXS0E6TdK3r8X_WtdX5cX5Wcm8,2791
 timeseries_shaper/filter/string_filters.py,sha256=oUIETyDBXdrIHSoR5YKF3pjVz3XA9zvppAo3J8KrX2c,1722
 timeseries_shaper/stats/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-timeseries_shaper/stats/numeric_stats.py,sha256=BzSAUhx_g1wqDCSHEyWWFZXDObxPCzOgxI9Z5fSqn1Q,1402
-timeseries_shaper-0.0.0.2.dist-info/LICENSE.txt,sha256=4QpeB3LkTiXXMQwSy9JzuY4S4PV48dcn01N_9qKZdys,1093
-timeseries_shaper-0.0.0.2.dist-info/METADATA,sha256=bpsMtuPz0rE7DBMrh8rX4BIOEqVLygAj1NJy8JxHKEk,2715
-timeseries_shaper-0.0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-timeseries_shaper-0.0.0.2.dist-info/top_level.txt,sha256=vzJVAg5J3PrZU28OKNmXElGh5W7X-BqDP3wJrn70Ouc,18
-timeseries_shaper-0.0.0.2.dist-info/RECORD,,
+timeseries_shaper/stats/numeric_stats.py,sha256=KeXNuvca9hj9m311BWv-_bmRtwN1H_mFm9iPPcCDE2U,1854
+timeseries_shaper-0.0.0.3.dist-info/LICENSE.txt,sha256=4QpeB3LkTiXXMQwSy9JzuY4S4PV48dcn01N_9qKZdys,1093
+timeseries_shaper-0.0.0.3.dist-info/METADATA,sha256=JgGh7yycFOxVj5EtNT7MRSFpYd52pntZMNXvsZDDgk0,2715
+timeseries_shaper-0.0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+timeseries_shaper-0.0.0.3.dist-info/top_level.txt,sha256=vzJVAg5J3PrZU28OKNmXElGh5W7X-BqDP3wJrn70Ouc,18
+timeseries_shaper-0.0.0.3.dist-info/RECORD,,
```

