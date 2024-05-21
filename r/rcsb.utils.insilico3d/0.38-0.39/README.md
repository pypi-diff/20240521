# Comparing `tmp/rcsb.utils.insilico3d-0.38.tar.gz` & `tmp/rcsb_utils_insilico3d-0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.insilico3d-0.38.tar", last modified: Tue Mar  5 14:24:37 2024, max compression
+gzip compressed data, was "rcsb_utils_insilico3d-0.39.tar", last modified: Tue May 21 16:46:03 2024, max compression
```

## Comparing `rcsb.utils.insilico3d-0.38.tar` & `rcsb_utils_insilico3d-0.39.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-05 14:24:37.676525 rcsb.utils.insilico3d-0.38/
--rw-r--r--   0 vsts      (1001) docker     (127)     4245 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     3626 2024-03-05 14:24:37.676525 rcsb.utils.insilico3d-0.38/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2555 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-05 14:24:37.672525 rcsb.utils.insilico3d-0.38/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-05 14:24:37.672525 rcsb.utils.insilico3d-0.38/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-05 14:24:37.676525 rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/
--rw-r--r--   0 vsts      (1001) docker     (127)    22907 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/AlphaFoldModelCloudProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18006 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/AlphaFoldModelProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24072 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/ModelArchiveModelProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10284 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/ModelHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7574 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/ModelProviderWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)    48385 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/ModelReorganizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-05 14:24:37.676525 rcsb.utils.insilico3d-0.38/rcsb.utils.insilico3d.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     3626 2024-03-05 14:24:37.000000 rcsb.utils.insilico3d-0.38/rcsb.utils.insilico3d.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      707 2024-03-05 14:24:37.000000 rcsb.utils.insilico3d-0.38/rcsb.utils.insilico3d.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-05 14:24:37.000000 rcsb.utils.insilico3d-0.38/rcsb.utils.insilico3d.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-05 14:23:15.000000 rcsb.utils.insilico3d-0.38/rcsb.utils.insilico3d.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-03-05 14:24:37.000000 rcsb.utils.insilico3d-0.38/rcsb.utils.insilico3d.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-03-05 14:24:37.000000 rcsb.utils.insilico3d-0.38/rcsb.utils.insilico3d.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      175 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-03-05 14:24:37.676525 rcsb.utils.insilico3d-0.38/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     2263 2024-03-05 14:20:36.000000 rcsb.utils.insilico3d-0.38/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:46:03.246588 rcsb_utils_insilico3d-0.39/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4282 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     3626 2024-05-21 16:46:03.246588 rcsb_utils_insilico3d-0.39/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2555 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:46:03.242588 rcsb_utils_insilico3d-0.39/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:46:03.242588 rcsb_utils_insilico3d-0.39/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:46:03.246588 rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/
+-rw-r--r--   0 vsts      (1001) docker     (127)    22907 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/AlphaFoldModelCloudProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18006 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/AlphaFoldModelProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24221 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/ModelArchiveModelProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10284 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/ModelHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7574 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/ModelProviderWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    48385 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/ModelReorganizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:46:03.246588 rcsb_utils_insilico3d-0.39/rcsb.utils.insilico3d.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3626 2024-05-21 16:46:03.000000 rcsb_utils_insilico3d-0.39/rcsb.utils.insilico3d.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      707 2024-05-21 16:46:03.000000 rcsb_utils_insilico3d-0.39/rcsb.utils.insilico3d.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 16:46:03.000000 rcsb_utils_insilico3d-0.39/rcsb.utils.insilico3d.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 16:44:18.000000 rcsb_utils_insilico3d-0.39/rcsb.utils.insilico3d.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-05-21 16:46:03.000000 rcsb_utils_insilico3d-0.39/rcsb.utils.insilico3d.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-21 16:46:03.000000 rcsb_utils_insilico3d-0.39/rcsb.utils.insilico3d.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      175 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-21 16:46:03.246588 rcsb_utils_insilico3d-0.39/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     2263 2024-05-21 16:41:35.000000 rcsb_utils_insilico3d-0.39/setup.py
```

### Comparing `rcsb.utils.insilico3d-0.38/HISTORY.txt` & `rcsb_utils_insilico3d-0.39/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,9 @@
                        Add methods to insert release dates to models lacking these details
                        Adjust ModelArchiveProvider to fetch model files individually (instead of the full bulk download)
   23-Dec-2022  - V0.34 Configuration changes to support tox 4
    9-Jan-2023  - V0.35 Improvements to ModelArchiveModelProvider, and addition of more ModelArchive data sets
   20-Mar-2023  - V0.36 Assign NCBI ID to ma-ornl-sphdiv files to enable organism metadata population
   27-Feb-2024  - V0.37 Update AlphaFoldModelCloudProvider and ModelArchiveProvider;
                        Adjust ModelReorganizer to handle bulk cloud datasets and write out models as BCIF.gz
-   5-Mar-2024  - V0.38 Renamed ModelCacheProvider to ModelHoldingsProvider; Added support for CSM scaling (use of multiple holdings files)
+   5-Mar-2024  - V0.38 Renamed ModelCacheProvider to ModelHoldingsProvider; Added support for CSM scaling (use of multiple holdings files)
+  21-May-2024  - V0.39 Fix pylinting
```

### Comparing `rcsb.utils.insilico3d-0.38/LICENSE` & `rcsb_utils_insilico3d-0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.insilico3d-0.38/PKG-INFO` & `rcsb_utils_insilico3d-0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.insilico3d
-Version: 0.38
+Version: 0.39
 Summary: RCSB Python In Silico Model Access Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_insilico3d
 Author: Dennis Piehl
 Author-email: dennis.piehl@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.insilico3d-0.38/README.md` & `rcsb_utils_insilico3d-0.39/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/AlphaFoldModelCloudProvider.py` & `rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/AlphaFoldModelCloudProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/AlphaFoldModelProvider.py` & `rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/AlphaFoldModelProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/ModelArchiveModelProvider.py` & `rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/ModelArchiveModelProvider.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,15 @@
                 cacheD = {}
                 cacheD.update({"created": startDateTime, "data": {}})
                 for dataSet, pathD in modelArchiveRequestedDatasetD.items():
                     try:
                         sD = {}
                         numModelsToDownload = pathD.get("numModels", None)  # Used for testing purposes, defaults to total number of models
                         bulkFileName = pathD.get("bulkFileName", None)
+                        numModelsDownloaded = 0
                         if bulkFileName:
                             # Download bulk model archive file (contains associated local pairwise quality data and a3m files)
                             sD.update({"downloadMethod": "bulk"})
                             sD.update({"bulkArchiveFileName": bulkFileName})
                             dataSetFilePath = os.path.join(baseUrl, dataSet + self.__modelArchiveBulkDownloadUrlEnd)
                             dataSetDataDumpDir = os.path.join(self.__workPath, dataSet.replace(" ", "_"))
                             self.__fU.mkdir(dataSetDataDumpDir)
@@ -176,14 +177,15 @@
                             logger.info("Completed unbundle (%r) at %s (%.4f seconds)", ok, time.strftime("%Y %m %d %H:%M:%S", time.localtime()), time.time() - startTime)
                             #
                             logger.info("Clearing non-model files from extracted zip bundle...")
                             for nonModelFile in Path(dataSetDataDumpDir).glob("*.a3m"):
                                 nonModelFile.unlink()
                             for nonModelFile in Path(dataSetDataDumpDir).glob("*_local_pairwise_qa.cif"):
                                 nonModelFile.unlink()
+                            numModelsDownloaded = len(list(Path(dataSetDataDumpDir).glob("*.cif*")))
                         else:
                             # Download model files individually
                             sD.update({"downloadMethod": "individual"})
                             dataSetDataDumpDir = os.path.join(self.__workPath, dataSet.replace(" ", "_"))
                             self.__fU.mkdir(dataSetDataDumpDir)
                             logger.info("Fetching files for %s from server to local path %s", dataSet, dataSetDataDumpDir)
                             ok, numModelsDownloaded = asyncio.run(self.downloadIndividualModelFiles(
```

### Comparing `rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/ModelHoldingsProvider.py` & `rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/ModelHoldingsProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/ModelProviderWorkflow.py` & `rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/ModelProviderWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.insilico3d-0.38/rcsb/utils/insilico3d/ModelReorganizer.py` & `rcsb_utils_insilico3d-0.39/rcsb/utils/insilico3d/ModelReorganizer.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.insilico3d-0.38/rcsb.utils.insilico3d.egg-info/PKG-INFO` & `rcsb_utils_insilico3d-0.39/rcsb.utils.insilico3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.insilico3d
-Version: 0.38
+Version: 0.39
 Summary: RCSB Python In Silico Model Access Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_insilico3d
 Author: Dennis Piehl
 Author-email: dennis.piehl@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.insilico3d-0.38/rcsb.utils.insilico3d.egg-info/SOURCES.txt` & `rcsb_utils_insilico3d-0.39/rcsb.utils.insilico3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.insilico3d-0.38/setup.py` & `rcsb_utils_insilico3d-0.39/setup.py`

 * *Files identical despite different names*

