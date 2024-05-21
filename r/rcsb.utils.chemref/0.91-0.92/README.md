# Comparing `tmp/rcsb.utils.chemref-0.91.tar.gz` & `tmp/rcsb_utils_chemref-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.chemref-0.91.tar", last modified: Fri Dec  1 03:08:50 2023, max compression
+gzip compressed data, was "rcsb_utils_chemref-0.92.tar", last modified: Tue May 21 16:55:52 2024, max compression
```

## Comparing `rcsb.utils.chemref-0.91.tar` & `rcsb_utils_chemref-0.92.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 03:08:50.346651 rcsb.utils.chemref-0.91/
--rw-r--r--   0 vsts      (1001) docker     (127)     5828 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      111 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2077 2023-12-01 03:08:50.346651 rcsb.utils.chemref-0.91/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 03:08:50.338651 rcsb.utils.chemref-0.91/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 03:08:50.342651 rcsb.utils.chemref-0.91/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 03:08:50.346651 rcsb.utils.chemref-0.91/rcsb/utils/chemref/
--rw-r--r--   0 vsts      (1001) docker     (127)    10179 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/AtcProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6625 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/BirdProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3616 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/CARDProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4726 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/CODProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12752 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/ChEMBLProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7749 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/ChemCompModelProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9678 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/ChemCompProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16593 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/DrugBankProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11256 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/DrugBankReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3674 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/DrugCentralProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3858 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/PharosProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2509 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/PharosReadSqlDump.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7494 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/PsiModProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4060 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/PubChemProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    56020 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/PubChemUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6478 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/RcsbLigandScoreProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6669 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/ResidProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1586 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/ResidReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)      144 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/rcsb/utils/chemref/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 03:08:50.346651 rcsb.utils.chemref-0.91/rcsb.utils.chemref.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2077 2023-12-01 03:08:50.000000 rcsb.utils.chemref-0.91/rcsb.utils.chemref.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1077 2023-12-01 03:08:50.000000 rcsb.utils.chemref-0.91/rcsb.utils.chemref.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-01 03:08:50.000000 rcsb.utils.chemref-0.91/rcsb.utils.chemref.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-01 02:52:58.000000 rcsb.utils.chemref-0.91/rcsb.utils.chemref.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      197 2023-12-01 03:08:50.000000 rcsb.utils.chemref-0.91/rcsb.utils.chemref.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2023-12-01 03:08:50.000000 rcsb.utils.chemref-0.91/rcsb.utils.chemref.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      166 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2023-12-01 03:08:50.350651 rcsb.utils.chemref-0.91/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2227 2023-12-01 02:52:01.000000 rcsb.utils.chemref-0.91/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:55:52.394638 rcsb_utils_chemref-0.92/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5864 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      111 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2077 2024-05-21 16:55:52.394638 rcsb_utils_chemref-0.92/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:55:52.386638 rcsb_utils_chemref-0.92/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:55:52.390638 rcsb_utils_chemref-0.92/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:55:52.394638 rcsb_utils_chemref-0.92/rcsb/utils/chemref/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10179 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/AtcProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6650 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/BirdProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3616 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/CARDProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4726 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/CODProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12752 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/ChEMBLProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7749 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/ChemCompModelProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9678 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/ChemCompProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16593 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/DrugBankProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11256 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/DrugBankReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3674 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/DrugCentralProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3858 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/PharosProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2509 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/PharosReadSqlDump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7494 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/PsiModProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4060 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/PubChemProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    56046 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/PubChemUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6478 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/RcsbLigandScoreProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6669 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/ResidProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/ResidReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/rcsb/utils/chemref/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:55:52.394638 rcsb_utils_chemref-0.92/rcsb.utils.chemref.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2077 2024-05-21 16:55:52.000000 rcsb_utils_chemref-0.92/rcsb.utils.chemref.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1077 2024-05-21 16:55:52.000000 rcsb_utils_chemref-0.92/rcsb.utils.chemref.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 16:55:52.000000 rcsb_utils_chemref-0.92/rcsb.utils.chemref.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 16:35:44.000000 rcsb_utils_chemref-0.92/rcsb.utils.chemref.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-05-21 16:55:52.000000 rcsb_utils_chemref-0.92/rcsb.utils.chemref.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-21 16:55:52.000000 rcsb_utils_chemref-0.92/rcsb.utils.chemref.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-21 16:55:52.394638 rcsb_utils_chemref-0.92/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2227 2024-05-21 16:34:48.000000 rcsb_utils_chemref-0.92/setup.py
```

### Comparing `rcsb.utils.chemref-0.91/HISTORY.txt` & `rcsb_utils_chemref-0.92/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -77,7 +77,8 @@
   9-Jan-2023  - V0.85 Configuration changes to support tox 4
  22-Mar-2023  - V0.86 Update references to py-rcsb_exdb_assets master branch
  19-Apr-2023  - V0.87 Update file path in ATCProvider
  19-May-2023  - V0.88 Update DNS to PDB archive
   5-Jun-2023  - V0.89 Include bond count in ChemCompProvider
  20-Sep-2023  - V0.90 Adjust request methods in PubChemUtils; Use HTTPS instead of FTP for ChEMBL data
  30-Nov-2023  - V0.91 Add drug product information (approved, country, dates of marketing, etc.)
+ 21-May-2024  - V0.92 Fix pylinting
```

### Comparing `rcsb.utils.chemref-0.91/LICENSE` & `rcsb_utils_chemref-0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/PKG-INFO` & `rcsb_utils_chemref-0.92/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chemref
-Version: 0.91
+Version: 0.92
 Summary: RCSB Python Chemical Reference Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chemref
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chemref-0.91/README.md` & `rcsb_utils_chemref-0.92/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/AtcProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/AtcProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/BirdProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/BirdProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             dataContainerL = self.__mU.doImport(birdFilePath, fmt="mmcif")
             endTime = time.time()
             logger.info("Read %s with %d BIRD definitions (%.4f seconds)", birdFilePath, len(dataContainerL), endTime - startTime)
             # -------
             startTime = time.time()
             dataContainerL = dataContainerL[:molLimit] if molLimit else dataContainerL
             for dataContainer in dataContainerL:
-                prdId = prdReleaseStatus = representAs = None
+                prdId = prdReleaseStatus = representAs = chemCompId = classType = None
                 if dataContainer.exists("pdbx_reference_molecule"):
                     prdObj = dataContainer.getObj("pdbx_reference_molecule")
                     prdId = prdObj.getValueOrDefault("prd_id", 0, defaultValue=None)
                     prdReleaseStatus = prdObj.getValueOrDefault("release_status", 0, defaultValue=None)
                     representAs = prdObj.getValueOrDefault("represent_as", 0, defaultValue=None)
                     chemCompId = prdObj.getValueOrDefault("chem_comp_id", 0, defaultValue=None)
                     classType = prdObj.getValueOrDefault("class", 0, defaultValue=None)
```

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/CARDProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/CARDProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/CODProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/CODProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/ChEMBLProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/ChEMBLProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/ChemCompModelProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/ChemCompModelProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/ChemCompProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/ChemCompProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/DrugBankProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/DrugBankProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/DrugBankReader.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/DrugBankReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/DrugCentralProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/DrugCentralProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/PharosProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/PharosProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/PharosReadSqlDump.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/PharosReadSqlDump.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/PsiModProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/PsiModProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/PubChemProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/PubChemProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/PubChemUtils.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/PubChemUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         """
         exportPath = kwargs.get("exportPath", None)
         exportIntermediates = kwargs.get("exportIntermediates", False)
         matchIdOnly = kwargs.get("matchIdOnly", False)
         contentTypes = kwargs.get("contentTypes", ["view", "classification", "property", "xrefs", "synonyms", "dgidb", "pathway", "fdaorangebook", "clinicaltrials", "bioactivity"])
 
         retStatus = False
+        searchType = None
         retD = {}
         assemDL = []
         # -- First identifier the PubChem compound CID for the input chemical identifier.
         if chemicalIdentifier.identifierType in ["smiles", "inchi"]:
             searchType = "fastidentity"
         elif chemicalIdentifier.identifierType in ["cid", "name", "inchikey"]:
             searchType = "lookup"
```

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/RcsbLigandScoreProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/RcsbLigandScoreProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/ResidProvider.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/ResidProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb/utils/chemref/ResidReader.py` & `rcsb_utils_chemref-0.92/rcsb/utils/chemref/ResidReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/rcsb.utils.chemref.egg-info/PKG-INFO` & `rcsb_utils_chemref-0.92/rcsb.utils.chemref.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chemref
-Version: 0.91
+Version: 0.92
 Summary: RCSB Python Chemical Reference Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chemref
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chemref-0.91/rcsb.utils.chemref.egg-info/SOURCES.txt` & `rcsb_utils_chemref-0.92/rcsb.utils.chemref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.91/setup.py` & `rcsb_utils_chemref-0.92/setup.py`

 * *Files identical despite different names*

