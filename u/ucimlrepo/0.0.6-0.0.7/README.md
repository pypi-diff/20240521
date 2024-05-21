# Comparing `tmp/ucimlrepo-0.0.6.tar.gz` & `tmp/ucimlrepo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ucimlrepo-0.0.6.tar", last modified: Wed Mar 20 07:13:58 2024, max compression
+gzip compressed data, was "ucimlrepo-0.0.7.tar", last modified: Tue May 21 06:04:43 2024, max compression
```

## Comparing `ucimlrepo-0.0.6.tar` & `ucimlrepo-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-07-18 01:17:59.000000 ucimlrepo-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5468 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4773 2024-03-20 06:52:00.000000 ucimlrepo-0.0.6/README.md
--rw-rw-rw-   0        0        0      699 2024-03-20 07:13:03.000000 ucimlrepo-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      416 2024-03-20 07:13:05.000000 ucimlrepo-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/src/ucimlrepo/
--rw-rw-rw-   0        0        0       29 2023-07-24 22:55:12.000000 ucimlrepo-0.0.6/src/ucimlrepo/__init__.py
--rw-rw-rw-   0        0        0      176 2023-08-03 19:08:31.000000 ucimlrepo-0.0.6/src/ucimlrepo/dotdict.py
--rw-rw-rw-   0        0        0     8338 2024-03-20 07:10:52.000000 ucimlrepo-0.0.6/src/ucimlrepo/fetch.py
--rw-rw-rw-   0        0        0     1926 2024-03-20 07:10:54.000000 ucimlrepo-0.0.6/src/ucimlrepo/test.py
-drwxrwxrwx   0        0        0        0 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/src/ucimlrepo.egg-info/
--rw-rw-rw-   0        0        0     5468 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/src/ucimlrepo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/src/ucimlrepo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/src/ucimlrepo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/src/ucimlrepo.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-20 07:13:58.000000 ucimlrepo-0.0.6/tests/
--rw-rw-rw-   0        0        0     2212 2024-03-20 06:52:59.000000 ucimlrepo-0.0.6/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:04:43.654160 ucimlrepo-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-07-18 01:17:59.000000 ucimlrepo-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5533 2024-05-21 06:04:43.650561 ucimlrepo-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4773 2024-05-21 05:52:44.000000 ucimlrepo-0.0.7/README.md
+-rw-rw-rw-   0        0        0      771 2024-05-21 06:02:40.000000 ucimlrepo-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:04:43.655501 ucimlrepo-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      416 2024-05-21 05:52:43.000000 ucimlrepo-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:04:43.555521 ucimlrepo-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 06:04:43.583061 ucimlrepo-0.0.7/src/ucimlrepo/
+-rw-rw-rw-   0        0        0       29 2023-07-24 22:55:12.000000 ucimlrepo-0.0.7/src/ucimlrepo/__init__.py
+-rw-rw-rw-   0        0        0      176 2023-08-03 19:08:31.000000 ucimlrepo-0.0.7/src/ucimlrepo/dotdict.py
+-rw-rw-rw-   0        0        0     8402 2024-03-20 07:18:10.000000 ucimlrepo-0.0.7/src/ucimlrepo/fetch.py
+-rw-rw-rw-   0        0        0     1926 2024-03-20 07:10:54.000000 ucimlrepo-0.0.7/src/ucimlrepo/test.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:04:43.646638 ucimlrepo-0.0.7/src/ucimlrepo.egg-info/
+-rw-rw-rw-   0        0        0     5533 2024-05-21 06:04:43.000000 ucimlrepo-0.0.7/src/ucimlrepo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-05-21 06:04:43.000000 ucimlrepo-0.0.7/src/ucimlrepo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:04:43.000000 ucimlrepo-0.0.7/src/ucimlrepo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-21 06:04:43.000000 ucimlrepo-0.0.7/src/ucimlrepo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 06:04:43.000000 ucimlrepo-0.0.7/src/ucimlrepo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 06:04:43.638328 ucimlrepo-0.0.7/tests/
+-rw-rw-rw-   0        0        0     2212 2024-03-20 06:52:59.000000 ucimlrepo-0.0.7/tests/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ucimlrepo-0.0.6/LICENSE` & `ucimlrepo-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ucimlrepo-0.0.6/PKG-INFO` & `ucimlrepo-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: ucimlrepo
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package to easily import datasets from the UC Irvine Machine Learning Repository into scripts and notebooks.
 Home-page: https://github.com/uci-ml-repo/ucimlrepo
 Author: Philip Truong
 Author-email: Philip Truong <ucirepository@gmail.com>
 Project-URL: Homepage, https://github.com/uci-ml-repo/ucimlrepo/tree/main
 Project-URL: Bug Tracker, https://github.com/uci-ml-repo/ucimlrepo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: certifi>=2020.12.5
 
 # `ucimlrepo` package
 Package to easily import datasets from the UC Irvine Machine Learning Repository into scripts and notebooks. 
 <br>
-**Current Version: 0.0.4**
+**Current Version: 0.0.7**
 
 ## Installation
 In a Jupyter notebook, install with the command 
 
     !pip3 install -U ucimlrepo 
     
 Restart the kernel and import the module `ucimlrepo`.
```

### Comparing `ucimlrepo-0.0.6/README.md` & `ucimlrepo-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # `ucimlrepo` package
 Package to easily import datasets from the UC Irvine Machine Learning Repository into scripts and notebooks. 
 <br>
-**Current Version: 0.0.4**
+**Current Version: 0.0.7**
 
 ## Installation
 In a Jupyter notebook, install with the command 
 
     !pip3 install -U ucimlrepo 
     
 Restart the kernel and import the module `ucimlrepo`.
```

### Comparing `ucimlrepo-0.0.6/pyproject.toml` & `ucimlrepo-0.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ucimlrepo"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Philip Truong", email="ucirepository@gmail.com" },
 ]
 description = "Package to easily import datasets from the UC Irvine Machine Learning Repository into scripts and notebooks."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "pandas >= 1.0.0",
+  "certifi >= 2020.12.5",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/uci-ml-repo/ucimlrepo/tree/main"
-"Bug Tracker" = "https://github.com/uci-ml-repo/ucimlrepo/issues"
+"Bug Tracker" = "https://github.com/uci-ml-repo/ucimlrepo/issues"
```

### Comparing `ucimlrepo-0.0.6/src/ucimlrepo/fetch.py` & `ucimlrepo-0.0.7/src/ucimlrepo/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,16 @@
     # column width for dataset name
     maxNameLen = max(max([len(dataset['name']) for dataset in data]) + 3, 15)
 
     # print table title
     title = 'The following {}datasets are available{}:'.format(filter + ' ' if filter else '', ' for search query "{}"'.format(search) if search else '')
     print('-' * len(title))
     print(title)
+    if area:
+        print('For subject area: {}'.format(area))
     print('-' * len(title))
 
     # print table headers
     header_str = '{:<{width}} {:<6}'.format('Dataset Name', 'ID', width=maxNameLen)
     underline_str = '{:<{width}} {:<6}'.format('------------', '--', width=maxNameLen)
     if len(data) > 0 and 'description' in data[0]:
         header_str += ' {:<100}'.format('Prediction Task')
```

### Comparing `ucimlrepo-0.0.6/src/ucimlrepo/test.py` & `ucimlrepo-0.0.7/src/ucimlrepo/test.py`

 * *Files identical despite different names*

### Comparing `ucimlrepo-0.0.6/src/ucimlrepo.egg-info/PKG-INFO` & `ucimlrepo-0.0.7/src/ucimlrepo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: ucimlrepo
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package to easily import datasets from the UC Irvine Machine Learning Repository into scripts and notebooks.
 Home-page: https://github.com/uci-ml-repo/ucimlrepo
 Author: Philip Truong
 Author-email: Philip Truong <ucirepository@gmail.com>
 Project-URL: Homepage, https://github.com/uci-ml-repo/ucimlrepo/tree/main
 Project-URL: Bug Tracker, https://github.com/uci-ml-repo/ucimlrepo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: certifi>=2020.12.5
 
 # `ucimlrepo` package
 Package to easily import datasets from the UC Irvine Machine Learning Repository into scripts and notebooks. 
 <br>
-**Current Version: 0.0.4**
+**Current Version: 0.0.7**
 
 ## Installation
 In a Jupyter notebook, install with the command 
 
     !pip3 install -U ucimlrepo 
     
 Restart the kernel and import the module `ucimlrepo`.
```

### Comparing `ucimlrepo-0.0.6/tests/test.py` & `ucimlrepo-0.0.7/tests/test.py`

 * *Files identical despite different names*

