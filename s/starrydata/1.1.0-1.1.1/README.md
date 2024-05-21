# Comparing `tmp/starrydata-1.1.0.tar.gz` & `tmp/starrydata-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrydata-1.1.0.tar", last modified: Tue May 21 07:54:05 2024, max compression
+gzip compressed data, was "starrydata-1.1.1.tar", last modified: Tue May 21 08:04:24 2024, max compression
```

## Comparing `starrydata-1.1.0.tar` & `starrydata-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 07:54:05.075660 starrydata-1.1.0/
--rw-r--r--   0 matotomoya   (501) staff       (20)     1073 2023-12-12 10:27:13.000000 starrydata-1.1.0/LICENSE
--rw-r--r--   0 matotomoya   (501) staff       (20)     2724 2024-05-21 07:54:05.075344 starrydata-1.1.0/PKG-INFO
--rw-r--r--   0 matotomoya   (501) staff       (20)     2132 2024-05-21 07:17:33.000000 starrydata-1.1.0/README.md
--rw-r--r--   0 matotomoya   (501) staff       (20)      576 2024-05-21 07:54:02.000000 starrydata-1.1.0/pyproject.toml
--rw-r--r--   0 matotomoya   (501) staff       (20)       38 2024-05-21 07:54:05.075737 starrydata-1.1.0/setup.cfg
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 07:54:05.072834 starrydata-1.1.0/src/
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 07:54:05.073886 starrydata-1.1.0/src/starrydata/
--rw-r--r--   0 matotomoya   (501) staff       (20)      183 2024-05-21 06:08:13.000000 starrydata-1.1.0/src/starrydata/__init__.py
--rw-r--r--   0 matotomoya   (501) staff       (20)     6532 2024-05-21 07:16:15.000000 starrydata-1.1.0/src/starrydata/dataset.py
--rw-r--r--   0 matotomoya   (501) staff       (20)     4914 2024-05-12 10:10:09.000000 starrydata-1.1.0/src/starrydata/test_dataset.py
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 07:54:05.075038 starrydata-1.1.0/src/starrydata.egg-info/
--rw-r--r--   0 matotomoya   (501) staff       (20)     2724 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/PKG-INFO
--rw-r--r--   0 matotomoya   (501) staff       (20)      305 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/SOURCES.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)        1 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/dependency_links.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)       21 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/requires.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)       11 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/top_level.txt
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:04:24.462881 starrydata-1.1.1/
+-rw-r--r--   0 matotomoya   (501) staff       (20)     1073 2023-12-12 10:27:13.000000 starrydata-1.1.1/LICENSE
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2790 2024-05-21 08:04:24.462542 starrydata-1.1.1/PKG-INFO
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2198 2024-05-21 07:56:14.000000 starrydata-1.1.1/README.md
+-rw-r--r--   0 matotomoya   (501) staff       (20)      576 2024-05-21 08:04:22.000000 starrydata-1.1.1/pyproject.toml
+-rw-r--r--   0 matotomoya   (501) staff       (20)       38 2024-05-21 08:04:24.462967 starrydata-1.1.1/setup.cfg
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:04:24.459452 starrydata-1.1.1/src/
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:04:24.460490 starrydata-1.1.1/src/starrydata/
+-rw-r--r--   0 matotomoya   (501) staff       (20)      183 2024-05-21 06:08:13.000000 starrydata-1.1.1/src/starrydata/__init__.py
+-rw-r--r--   0 matotomoya   (501) staff       (20)     6532 2024-05-21 07:16:15.000000 starrydata-1.1.1/src/starrydata/dataset.py
+-rw-r--r--   0 matotomoya   (501) staff       (20)     4914 2024-05-12 10:10:09.000000 starrydata-1.1.1/src/starrydata/test_dataset.py
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:04:24.462181 starrydata-1.1.1/src/starrydata.egg-info/
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2790 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/PKG-INFO
+-rw-r--r--   0 matotomoya   (501) staff       (20)      305 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/SOURCES.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)        1 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/dependency_links.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)       21 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/requires.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)       11 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/top_level.txt
```

### Comparing `starrydata-1.1.0/LICENSE` & `starrydata-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starrydata-1.1.0/PKG-INFO` & `starrydata-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrydata
-Version: 1.1.0
+Version: 1.1.1
 Summary: Starrydata Python useful tools 
 Author-email: MATO Tomoya <tomoya.matou@gmail.com>
 Project-URL: Homepage, https://github.com/starrydata/starrydata-python-library
 Project-URL: Issues, https://github.com/starrydata/starrydata-python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -50,15 +50,15 @@
 # Read the 'all_samples.csv' file from the dataset and convert it to a pandas DataFrame
 df_samples = pd.read_csv(sd_dataset.samples_csv)
 
 # Read the 'all_papers.json' file from the dataset and convert it to a pandas DataFrame
 df_papers = pd.read_json(sd_dataset.papers_json)
 ```
 
-More details is [1_how_to_use.ipynb](example_notebooks/1_how_to_use.ipynb)
+More details is [1_how_to_use.ipynb](https://github.com/starrydata/starrydata-python-library/blob/main/example_notebooks/1_how_to_use.ipynb)
 
 ## Documentation
 
 For more detailed documentation and usage examples, please refer to the [official documentation](https://pypi.org/project/starrydata/).
 
 ## Contributing
```

### Comparing `starrydata-1.1.0/README.md` & `starrydata-1.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # Read the 'all_samples.csv' file from the dataset and convert it to a pandas DataFrame
 df_samples = pd.read_csv(sd_dataset.samples_csv)
 
 # Read the 'all_papers.json' file from the dataset and convert it to a pandas DataFrame
 df_papers = pd.read_json(sd_dataset.papers_json)
 ```
 
-More details is [1_how_to_use.ipynb](example_notebooks/1_how_to_use.ipynb)
+More details is [1_how_to_use.ipynb](https://github.com/starrydata/starrydata-python-library/blob/main/example_notebooks/1_how_to_use.ipynb)
 
 ## Documentation
 
 For more detailed documentation and usage examples, please refer to the [official documentation](https://pypi.org/project/starrydata/).
 
 ## Contributing
```

### Comparing `starrydata-1.1.0/pyproject.toml` & `starrydata-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "starrydata"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="MATO Tomoya", email="tomoya.matou@gmail.com" },
 ]
 description = "Starrydata Python useful tools "
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `starrydata-1.1.0/src/starrydata/dataset.py` & `starrydata-1.1.1/src/starrydata/dataset.py`

 * *Files identical despite different names*

### Comparing `starrydata-1.1.0/src/starrydata/test_dataset.py` & `starrydata-1.1.1/src/starrydata/test_dataset.py`

 * *Files identical despite different names*

### Comparing `starrydata-1.1.0/src/starrydata.egg-info/PKG-INFO` & `starrydata-1.1.1/src/starrydata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrydata
-Version: 1.1.0
+Version: 1.1.1
 Summary: Starrydata Python useful tools 
 Author-email: MATO Tomoya <tomoya.matou@gmail.com>
 Project-URL: Homepage, https://github.com/starrydata/starrydata-python-library
 Project-URL: Issues, https://github.com/starrydata/starrydata-python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -50,15 +50,15 @@
 # Read the 'all_samples.csv' file from the dataset and convert it to a pandas DataFrame
 df_samples = pd.read_csv(sd_dataset.samples_csv)
 
 # Read the 'all_papers.json' file from the dataset and convert it to a pandas DataFrame
 df_papers = pd.read_json(sd_dataset.papers_json)
 ```
 
-More details is [1_how_to_use.ipynb](example_notebooks/1_how_to_use.ipynb)
+More details is [1_how_to_use.ipynb](https://github.com/starrydata/starrydata-python-library/blob/main/example_notebooks/1_how_to_use.ipynb)
 
 ## Documentation
 
 For more detailed documentation and usage examples, please refer to the [official documentation](https://pypi.org/project/starrydata/).
 
 ## Contributing
```

