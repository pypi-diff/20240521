# Comparing `tmp/newyorkfed_pandas-0.0.1.tar.gz` & `tmp/newyorkfed_pandas-0.0.2.tar.gz`

## Comparing `newyorkfed_pandas-0.0.1.tar` & `newyorkfed_pandas-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.1/src/archive/test.ps1
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.1/src/newyorkfed_pandas/__init__.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.1/src/newyorkfed_pandas/rrp.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.1/LICENSE
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.1/README.md
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.2/src/newyorkfed_pandas/__init__.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.2/src/newyorkfed_pandas/rrp.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.2/LICENSE
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.2/README.md
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 newyorkfed_pandas-0.0.2/PKG-INFO
```

### Comparing `newyorkfed_pandas-0.0.1/src/newyorkfed_pandas/rrp.py` & `newyorkfed_pandas-0.0.2/src/newyorkfed_pandas/rrp.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,8 +92,13 @@
 
         print(f'No {path} found. Downloading all records after {start_date}.')
 
         df = download_records_after(start_date)
 
         df.to_pickle(path)
 
-        return df
+        return df
+
+# ----------------------------------------------------------------------
+
+if __name__ == '__main__':
+    load_records('1900-01-01', update=True)
```

### Comparing `newyorkfed_pandas-0.0.1/LICENSE` & `newyorkfed_pandas-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `newyorkfed_pandas-0.0.1/pyproject.toml` & `newyorkfed_pandas-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "newyorkfed_pandas"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Eduardo Cavazos", email="wayo.cavazos@gmail.com" },
 ]
 description = "Library for downloading data from the markets.newyorkfed API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `newyorkfed_pandas-0.0.1/PKG-INFO` & `newyorkfed_pandas-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: newyorkfed_pandas
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for downloading data from the markets.newyorkfed API
 Project-URL: Homepage, https://github.com/dharmatech/newyorkfed_pandas.py
 Project-URL: Issues, https://github.com/dharmatech/newyorkfed_pandas.py/issues
 Author-email: Eduardo Cavazos <wayo.cavazos@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,8 +20,8 @@
 
 The first time you request data, the data is retrieved and saved locally. Subsequent requests for the data only download newly available records plus a few others to ensure continuity.
 
 Currently, only the RRP endpoint is available.
 
 pypi package:
 
-
+https://pypi.org/project/newyorkfed-pandas/
```

