# Comparing `tmp/notebooks_and_scripts-4.449.1.tar.gz` & `tmp/notebooks_and_scripts-4.450.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebooks_and_scripts-4.449.1.tar", last modified: Sun May 19 23:06:02 2024, max compression
+gzip compressed data, was "notebooks_and_scripts-4.450.1.tar", last modified: Mon May 20 04:53:07 2024, max compression
```

## Comparing `notebooks_and_scripts-4.449.1.tar` & `notebooks_and_scripts-4.450.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:06:02.222477 notebooks_and_scripts-4.449.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.449.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)     4943 2024-05-19 23:06:02.220676 notebooks_and_scripts-4.449.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4141 2024-05-19 23:00:17.000000 notebooks_and_scripts-4.449.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:06:02.205664 notebooks_and_scripts-4.449.1/notebooks_and_scripts/
--rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-19 23:05:56.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      898 2024-04-27 03:49:23.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:06:02.207953 notebooks_and_scripts-4.449.1/notebooks_and_scripts/sagemaker/
--rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts/sagemaker/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:06:02.213872 notebooks_and_scripts-4.449.1/notebooks_and_scripts.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4943 2024-05-19 23:06:02.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      442 2024-05-19 23:06:02.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 23:06:02.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-19 23:06:02.000000 notebooks_and_scripts-4.449.1/notebooks_and_scripts.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 23:06:02.222631 notebooks_and_scripts-4.449.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      624 2024-05-19 22:57:54.000000 notebooks_and_scripts-4.449.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 04:53:07.484332 notebooks_and_scripts-4.450.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.450.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:51:23.000000 notebooks_and_scripts-4.450.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     5601 2024-05-20 04:53:07.483315 notebooks_and_scripts-4.450.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4141 2024-05-19 23:00:17.000000 notebooks_and_scripts-4.450.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 04:53:07.468155 notebooks_and_scripts-4.450.1/notebooks_and_scripts/
+-rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-20 04:53:03.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      898 2024-04-27 03:49:23.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 04:53:07.474399 notebooks_and_scripts-4.450.1/notebooks_and_scripts/sagemaker/
+-rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts/sagemaker/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 04:53:07.475827 notebooks_and_scripts-4.450.1/notebooks_and_scripts.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     5601 2024-05-20 04:53:07.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      515 2024-05-20 04:53:07.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-20 04:53:07.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      155 2024-05-20 04:53:07.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-20 04:53:07.000000 notebooks_and_scripts-4.450.1/notebooks_and_scripts.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      357 2024-05-17 03:47:04.000000 notebooks_and_scripts-4.450.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-20 04:53:07.484494 notebooks_and_scripts-4.450.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)     1076 2024-05-20 04:52:45.000000 notebooks_and_scripts-4.450.1/setup.py
```

### Comparing `notebooks_and_scripts-4.449.1/LICENSE` & `notebooks_and_scripts-4.450.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.449.1/PKG-INFO` & `notebooks_and_scripts-4.450.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,36 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.449.1
+Version: 4.450.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
+Home-page: https://github.com/kamangir/notebooks-and-scripts
 Author: arash@kamangir.net
+License: Public Domain
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Unix Shell
+Classifier: License :: Public Domain
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: abcli
+Requires-Dist: beautifulsoup4
+Requires-Dist: boto3
+Requires-Dist: geojson
+Requires-Dist: geopandas
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: opencv-python
+Requires-Dist: pydot
+Requires-Dist: pylint
+Requires-Dist: pymysql==0.10.1
+Requires-Dist: pytest
+Requires-Dist: python-dotenv[cli]
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: tqdm
 
 # 📜 notebooks & [meta] scripts
 
 [notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for ai experiments and aws batch jobs.
 
 ---
```

### Comparing `notebooks_and_scripts-4.449.1/README.md` & `notebooks_and_scripts-4.450.1/README.md`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.449.1/notebooks_and_scripts/__main__.py` & `notebooks_and_scripts-4.450.1/notebooks_and_scripts/__main__.py`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.449.1/notebooks_and_scripts.egg-info/PKG-INFO` & `notebooks_and_scripts-4.450.1/notebooks_and_scripts.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,36 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.449.1
+Version: 4.450.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
+Home-page: https://github.com/kamangir/notebooks-and-scripts
 Author: arash@kamangir.net
+License: Public Domain
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Unix Shell
+Classifier: License :: Public Domain
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: abcli
+Requires-Dist: beautifulsoup4
+Requires-Dist: boto3
+Requires-Dist: geojson
+Requires-Dist: geopandas
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: opencv-python
+Requires-Dist: pydot
+Requires-Dist: pylint
+Requires-Dist: pymysql==0.10.1
+Requires-Dist: pytest
+Requires-Dist: python-dotenv[cli]
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: tqdm
 
 # 📜 notebooks & [meta] scripts
 
 [notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for ai experiments and aws batch jobs.
 
 ---
```

