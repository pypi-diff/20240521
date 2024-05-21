# Comparing `tmp/rcsb.workflow-0.42.tar.gz` & `tmp/rcsb_workflow-0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.workflow-0.42.tar", last modified: Thu Sep 21 20:59:47 2023, max compression
+gzip compressed data, was "rcsb_workflow-0.43.tar", last modified: Tue May 21 20:51:41 2024, max compression
```

## Comparing `rcsb.workflow-0.42.tar` & `rcsb_workflow-0.43.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-21 20:59:47.123115 rcsb.workflow-0.42/
--rw-r--r--   0 vsts      (1001) docker     (127)     2713 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    11357 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2188 2023-09-21 20:59:47.123115 rcsb.workflow-0.42/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1143 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-21 20:59:47.119115 rcsb.workflow-0.42/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-21 20:59:47.119115 rcsb.workflow-0.42/rcsb/workflow/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/rcsb/workflow/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-21 20:59:47.123115 rcsb.workflow-0.42/rcsb/workflow/chem/
--rw-r--r--   0 vsts      (1001) docker     (127)     3781 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/rcsb/workflow/chem/ChemCompFileWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5191 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/rcsb/workflow/chem/ChemCompImageWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3928 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      144 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/rcsb/workflow/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-21 20:59:47.123115 rcsb.workflow-0.42/rcsb/workflow/targets/
--rw-r--r--   0 vsts      (1001) docker     (127)    11001 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30545 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/rcsb/workflow/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-21 20:59:47.119115 rcsb.workflow-0.42/rcsb.workflow.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2188 2023-09-21 20:59:47.000000 rcsb.workflow-0.42/rcsb.workflow.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      661 2023-09-21 20:59:47.000000 rcsb.workflow-0.42/rcsb.workflow.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-09-21 20:59:47.000000 rcsb.workflow-0.42/rcsb.workflow.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-09-21 20:59:46.000000 rcsb.workflow-0.42/rcsb.workflow.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      196 2023-09-21 20:59:47.000000 rcsb.workflow-0.42/rcsb.workflow.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2023-09-21 20:59:47.000000 rcsb.workflow-0.42/rcsb.workflow.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      230 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2023-09-21 20:59:47.123115 rcsb.workflow-0.42/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2447 2023-09-21 20:35:26.000000 rcsb.workflow-0.42/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 20:51:41.296406 rcsb_workflow-0.43/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2747 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2188 2024-05-21 20:51:41.296406 rcsb_workflow-0.43/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1143 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 20:51:41.296406 rcsb_workflow-0.43/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 20:51:41.296406 rcsb_workflow-0.43/rcsb/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/rcsb/workflow/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 20:51:41.296406 rcsb_workflow-0.43/rcsb/workflow/chem/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3781 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/rcsb/workflow/chem/ChemCompFileWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5191 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/rcsb/workflow/chem/ChemCompImageWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3928 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/rcsb/workflow/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 20:51:41.296406 rcsb_workflow-0.43/rcsb/workflow/targets/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11126 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30972 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/rcsb/workflow/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 20:51:41.296406 rcsb_workflow-0.43/rcsb.workflow.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2188 2024-05-21 20:51:41.000000 rcsb_workflow-0.43/rcsb.workflow.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      661 2024-05-21 20:51:41.000000 rcsb_workflow-0.43/rcsb.workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 20:51:41.000000 rcsb_workflow-0.43/rcsb.workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 20:51:40.000000 rcsb_workflow-0.43/rcsb.workflow.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-05-21 20:51:41.000000 rcsb_workflow-0.43/rcsb.workflow.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-21 20:51:41.000000 rcsb_workflow-0.43/rcsb.workflow.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      230 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-21 20:51:41.296406 rcsb_workflow-0.43/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2447 2024-05-21 20:25:06.000000 rcsb_workflow-0.43/setup.py
```

### Comparing `rcsb.workflow-0.42/HISTORY.txt` & `rcsb_workflow-0.43/HISTORY.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,7 +30,8 @@
  5-May-2023 - V0.38 Add fromDbPharos and reloadPharos parameters to ProteinTargetSequenceExecutionWorkflow.exportFasta()
 22-May-2023 - V0.39 Add retries to tox task for MMseqs2 download
  1-Jun-2023 - V0.40 Don't back up resources to GitHub during cache update workflows
 12-Jun-2023 - V0.41 Set useTaxonomy filter to False for CARD annotations
 19-Sep-2023 - V0.42 Don't overwrite Buildlocker files if there is no data;
                     Reduce resource footprint for Azure tests;
                     Make CARDTargetOntologyProvider stashable on Buildlocker
+21-May-2024 - V0.43 Fix pylinting
```

### Comparing `rcsb.workflow-0.42/LICENSE` & `rcsb_workflow-0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.42/PKG-INFO` & `rcsb_workflow-0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.42
+Version: 0.43
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.42/README.md` & `rcsb_workflow-0.43/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.42/rcsb/workflow/chem/ChemCompFileWorkflow.py` & `rcsb_workflow-0.43/rcsb/workflow/chem/ChemCompFileWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.42/rcsb/workflow/chem/ChemCompImageWorkflow.py` & `rcsb_workflow-0.43/rcsb/workflow/chem/ChemCompImageWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.42/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py` & `rcsb_workflow-0.43/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.42/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py` & `rcsb_workflow-0.43/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,15 @@
     logger.info("exportFasta status %r", ok)
     ok = ptsWf.createSearchDatabases() and ok
     logger.info("createSearchDatabases status %r", ok)
     ok = ptsWf.searchDatabases() and ok
     logger.info("searchDatabases status %r", ok)
     ok = ptsWf.buildFeatures() and ok
     logger.info("buildFeatures status %r", ok)
+    # To rebuild ChEMBL-target-activity data from scratch (non-incremental), set skip=None in fetchTargetActivityDataMulti()
     ok = ptsWf.buildActivityData() and ok
     logger.info("buildActivityData status %r", ok)
     ok = ptsWf.buildCofactorData() and ok
     logger.info("buildCofactorData status %r", ok)
     ptsWf.resourceCheck()
     return ok
```

### Comparing `rcsb.workflow-0.42/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py` & `rcsb_workflow-0.43/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,33 +65,35 @@
         return True
 
     def exportRCSBChemRefMapping(self):
         """Export RCSB chemical reference data identifier mapping data"""
         ok = False
         try:
             crmP = ChemRefMappingProvider(self.__cachePath, useCache=False)
-            okF = crmP.fetchChemRefMapping(self.__cfgOb)
+            ok = crmP.fetchChemRefMapping(self.__cfgOb)
+            logger.info("Completed fetch ChemRefMappingProvider (%r)", ok)
             crmP.reload()
-            if okF and crmP.testCache(minCount=1):
-                okB = crmP.backup(self.__cfgOb, self.__configName, useStash=True, useGit=False)
-            ok = okF and okB
+            if ok and crmP.testCache(minCount=1):
+                ok = crmP.backup(self.__cfgOb, self.__configName, useStash=True, useGit=False)
+                logger.info("Completed backup ChemRefMappingProvider (%r)", ok)
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ok
 
     def exportRCSBLigandNeighborMapping(self):
         """Export RCSB ligand neighbor mapping data"""
         ok = False
         try:
             crmP = LigandNeighborMappingProvider(self.__cachePath, useCache=False)
-            okF = crmP.fetchLigandNeighborMapping(self.__cfgOb)
+            ok = crmP.fetchLigandNeighborMapping(self.__cfgOb)
+            logger.info("Completed fetch LigandNeighborMappingProvider (%r)", ok)
             crmP.reload()
-            if okF and crmP.testCache(minCount=1):
-                okB = crmP.backup(self.__cfgOb, self.__configName, useStash=True, useGit=False)
-            ok = okF and okB
+            if ok and crmP.testCache(minCount=1):
+                ok = crmP.backup(self.__cfgOb, self.__configName, useStash=True, useGit=False)
+                logger.info("Completed backup LigandNeighborMappingProvider (%r)", ok)
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ok
 
     def exportRCSBProteinEntityFasta(self, resourceName="pdbprent"):
         """Export RCSB protein entity sequence data (FASTA, taxon mapping, and essential details)"""
         ok = False
@@ -119,19 +121,20 @@
         return ok
 
     def updateUniProtTaxonomy(self):
         """Update Uniprot taxonomy mapping data from source files"""
         startTime = time.time()
         umP = UniProtIdMappingProvider(cachePath=self.__cachePath)
         umP.clearCache()
-        ok1 = umP.reload(useCache=True, useLegacy=False, fmt="tdd", mapNames=["NCBI-taxon"])
-        logger.info("Completed building UniProt Id mapping (%r) at %s (%.4f seconds)", ok1, time.strftime("%Y %m %d %H:%M:%S", time.localtime()), time.time() - startTime)
-        if ok1 and umP.testCache():
-            ok2 = umP.backup(self.__cfgOb, self.__configName)
-        return ok1 & ok2
+        ok = umP.reload(useCache=True, useLegacy=False, fmt="tdd", mapNames=["NCBI-taxon"])
+        logger.info("Completed building UniProt Id mapping (%r) at %s (%.4f seconds)", ok, time.strftime("%Y %m %d %H:%M:%S", time.localtime()), time.time() - startTime)
+        if ok and umP.testCache():
+            ok = umP.backup(self.__cfgOb, self.__configName)
+            logger.info("Completed backup UniProt Id mapping (%r)", ok)
+        return ok
 
     def exportTargetsFasta(self, resourceNameList=None, useCache=True, addTaxonomy=False, reloadPharos=False, fromDbPharos=False, backupPharos=False, remotePrefix=None):
         """Export the target FASTA files for the input data resources.
 
         Args:
             resourceNameList (list, optional): list of data resources. Defaults to ["sabdab", "card", "drugbank", "chembl", "pharos", "pdbprent"].
             useCache (bool, optional): use cached data files. Defaults to True.
@@ -419,14 +422,15 @@
                 try:
                     aP.restore(self.__cfgOb, self.__configName, remotePrefix=remotePrefix)
                     aP.reload()
                 except Exception:
                     pass
                 targetIdList = aP.getTargetIdList(resultPath)
                 targetIdList = targetIdList[:maxTargets] if maxTargets else targetIdList
+                # To rebuild ChEMBL-target-activity data from scratch (non-incremental), change skip=None
                 ok = aP.fetchTargetActivityDataMulti(targetIdList, skip="tried", chunkSize=50, numProc=6)
                 #
                 aP.reload()
                 if ok and backup and aP.testCache():
                     okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r activity backup status (%r)", resourceName, okB)
             elif resourceName == "pharos":
```

### Comparing `rcsb.workflow-0.42/rcsb.workflow.egg-info/PKG-INFO` & `rcsb_workflow-0.43/rcsb.workflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.42
+Version: 0.43
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.42/rcsb.workflow.egg-info/SOURCES.txt` & `rcsb_workflow-0.43/rcsb.workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.42/setup.py` & `rcsb_workflow-0.43/setup.py`

 * *Files identical despite different names*

