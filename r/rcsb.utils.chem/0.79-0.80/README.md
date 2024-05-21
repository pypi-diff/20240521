# Comparing `tmp/rcsb.utils.chem-0.79.tar.gz` & `tmp/rcsb_utils_chem-0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.chem-0.79.tar", last modified: Tue Feb  6 21:28:42 2024, max compression
+gzip compressed data, was "rcsb_utils_chem-0.80.tar", last modified: Tue May 21 18:05:42 2024, max compression
```

## Comparing `rcsb.utils.chem-0.79.tar` & `rcsb_utils_chem-0.80.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-06 21:28:42.462463 rcsb.utils.chem-0.79/
--rw-r--r--   0 vsts      (1001) docker     (127)     5611 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2261 2024-02-06 21:28:42.462463 rcsb.utils.chem-0.79/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1307 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-06 21:28:42.454463 rcsb.utils.chem-0.79/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-06 21:28:42.454463 rcsb.utils.chem-0.79/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-06 21:28:42.462463 rcsb.utils.chem-0.79/rcsb/utils/chem/
--rw-r--r--   0 vsts      (1001) docker     (127)     9130 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/BatchChemSearch.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5041 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/CactvsMoleculeFactory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10127 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/ChemAxonDescriptorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13794 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompDepictWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13364 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompIndexProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7909 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompMoleculeProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16727 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompSearchIndexProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27265 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompSearchWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    96737 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/FailList.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5204 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/IoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2721 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/MolecularFormula.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13176 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/MoleculeAnnotationsCompare.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5106 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/ObMoleculeFactory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22814 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeAlignUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15861 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeChemCompUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3861 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeCommonUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9851 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49180 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeDepictAlign.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31812 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50250 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeMoleculeFactory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10831 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeMoleculeProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11322 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeSearchMoleculeProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12387 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11525 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/OeSubStructSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15773 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/PdbxChemComp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1959 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/PdbxChemCompConstants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6738 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/RdMoleculeFactory.py
--rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3964 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/rcsb/utils/chem/cactvsAnnotateMol.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-06 21:28:42.462463 rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2261 2024-02-06 21:28:42.000000 rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1460 2024-02-06 21:28:42.000000 rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-06 21:28:42.000000 rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-02-06 21:28:42.000000 rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-06 21:28:41.000000 rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      156 2024-02-06 21:28:42.000000 rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-02-06 21:28:42.000000 rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      185 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-02-06 21:28:42.462463 rcsb.utils.chem-0.79/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2397 2024-02-06 21:12:31.000000 rcsb.utils.chem-0.79/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 18:05:42.379550 rcsb_utils_chem-0.80/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5646 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2261 2024-05-21 18:05:42.379550 rcsb_utils_chem-0.80/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1307 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 18:05:42.371550 rcsb_utils_chem-0.80/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 18:05:42.371550 rcsb_utils_chem-0.80/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 18:05:42.375550 rcsb_utils_chem-0.80/rcsb/utils/chem/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9130 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/BatchChemSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5041 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/CactvsMoleculeFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10127 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/ChemAxonDescriptorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13858 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompDepictWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13364 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompIndexProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7909 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompMoleculeProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16727 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompSearchIndexProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27265 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompSearchWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    96737 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/FailList.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5204 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/IoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2721 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/MolecularFormula.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13176 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/MoleculeAnnotationsCompare.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5106 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/ObMoleculeFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22814 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeAlignUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15861 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeChemCompUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3861 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeCommonUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9851 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49180 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeDepictAlign.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31812 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50300 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeMoleculeFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10831 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeMoleculeProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11322 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeSearchMoleculeProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12387 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11525 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/OeSubStructSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15773 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/PdbxChemComp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1959 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/PdbxChemCompConstants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6738 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/RdMoleculeFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3964 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/rcsb/utils/chem/cactvsAnnotateMol.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 18:05:42.375550 rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2261 2024-05-21 18:05:42.000000 rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1460 2024-05-21 18:05:42.000000 rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 18:05:42.000000 rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-05-21 18:05:42.000000 rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 18:05:41.000000 rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      156 2024-05-21 18:05:42.000000 rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-21 18:05:42.000000 rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      185 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-21 18:05:42.379550 rcsb_utils_chem-0.80/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2397 2024-05-21 17:50:48.000000 rcsb_utils_chem-0.80/setup.py
```

### Comparing `rcsb.utils.chem-0.79/HISTORY.txt` & `rcsb_utils_chem-0.80/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,8 +64,9 @@
  9-Jun-2021 - V0.73 Update manifest files
 22-Aug-2021 - V0.74 Add ChemAxonDescriptorProvider and associated tests.  Add ChemAxon smiles to search index build.
 26-Aug-2021 - V0.75 Add filter for obsolete definitions in ChemCompMoleculeProvider and ChemCompSearchIndexProvider modules
 23-Sep-2021 - V0.76 Set default for skipObsolete to True
  9-Jan-2023 - V0.77 Configuration changes to support tox 4
 19-May-2023 - V0.78 Update DNS to PDB archive
  6-Feb-2024 - V0.79 Update Azure testing pipelines to use MacOS 13;
-                    Suppress errors logged for UNL (UNknown Ligand) chemical component
+                    Suppress errors logged for UNL (UNknown Ligand) chemical component
+21-May-2024 - V0.80 Fix pylinting
```

### Comparing `rcsb.utils.chem-0.79/LICENSE` & `rcsb_utils_chem-0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/PKG-INFO` & `rcsb_utils_chem-0.80/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chem
-Version: 0.79
+Version: 0.80
 Summary: RCSB Python Chemical Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chem
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chem-0.79/README.md` & `rcsb_utils_chem-0.80/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/BatchChemSearch.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/BatchChemSearch.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/CactvsMoleculeFactory.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/CactvsMoleculeFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/ChemAxonDescriptorProvider.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/ChemAxonDescriptorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompDepictWrapper.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompDepictWrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         imagePath = os.path.join(imageDirPath, "image-%s.svg" % ic)
         return imagePath
 
     def depictMolecule(self, identifier, identifierType, imagePath=None, **kwargs):
         """Create depiction from InChI, SMILES descriptors or PDB identifier."""
         try:
             imagePath = imagePath if imagePath else self.__makeImagePath()
+            oeMol = None
             oeio = OeIoUtils()
             if identifierType.lower() in ["smiles"]:
                 oeMol = oeio.smilesToMol(identifier)
             elif identifierType.lower() in ["inchi"]:
                 oeMol = oeio.inchiToMol(identifier)
             elif identifierType.lower() in ["identifierpdb"]:
                 ccsw = ChemCompSearchWrapper()
@@ -206,14 +207,15 @@
     def alignMoleculePair(self, refIdentifier, refIdentifierType, fitIdentifier, fitIdentifierType, imagePath=None, **kwargs):
         """Create aligned depiction for a target molecule InChI, SMILES descriptors or PDB identifier."""
         try:
             imagePath = imagePath if imagePath else self.__makeImagePath()
             oeio = OeIoUtils()
             ccsw = ChemCompSearchWrapper()
             oesmP = ccsw.getSearchMoleculeProvider()
+            oeMolRef = oeMolFit = None
             # ---
             if refIdentifierType.lower() in ["smiles"]:
                 oeMolRef = oeio.smilesToMol(refIdentifier)
             elif refIdentifierType.lower() in ["inchi"]:
                 oeMolRef = oeio.inchiToMol(refIdentifier)
             elif refIdentifierType.lower() in ["identifierpdb"]:
                 oeMolRef = oesmP.getMol(refIdentifier)
```

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompIndexProvider.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompIndexProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompMoleculeProvider.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompMoleculeProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompSearchIndexProvider.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompSearchIndexProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/ChemCompSearchWrapper.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/ChemCompSearchWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/FailList.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/FailList.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/IoUtils.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/IoUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/MolecularFormula.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/MolecularFormula.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/MoleculeAnnotationsCompare.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/MoleculeAnnotationsCompare.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/ObMoleculeFactory.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/ObMoleculeFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeAlignUtils.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeAlignUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeChemCompUtils.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeChemCompUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeCommonUtils.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeCommonUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeDepict.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeDepict.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeDepictAlign.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeDepictAlign.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeIoUtils.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeIoUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeMoleculeFactory.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeMoleculeFactory.py`

 * *Files 0% similar despite different names*

```diff
@@ -749,14 +749,15 @@
 
     def __buildFromExternalDescriptors(self, ccId, limitPerceptions=False):
         oeMolTupList = []
         if not self.__externalDescriptorTupList:
             return oeMolTupList
 
         for descrType, descriptor, label in self.__externalDescriptorTupList:
+            oeMol = None
             if "inchi" in descrType.lower():
                 oeMol = self.__inchiToMol(ccId, descriptor, limitPerceptions=limitPerceptions)
             elif "smiles" in descrType.lower():
                 oeMol = self.__smilesToMol(ccId, descriptor, limitPerceptions=limitPerceptions)
             if oeMol:
                 oeMolTupList.append((oeMol, label))
         logger.debug("Extra descriptor molecule count (%d)", len(oeMolTupList))
@@ -784,14 +785,15 @@
             descr = self.__getDescriptor(ccId, molBuildType, fallBackBuildType=fallBackBuildType)
             if not descr:
                 if not self.__quietMode:
                     logger.warning("%r molBuildType %r missing descriptor", ccId, molBuildType)
                 return None
             #
             logger.debug("Building with molBuildType %r descr %r ", molBuildType, descr)
+            oeMol = None
             if molBuildType in ["oe-smiles", "oe-iso-smiles", "acdlabs-smiles", "cactvs-smiles", "cactvs-iso-smiles"]:
                 oeMol = self.__smilesToMol(ccId, descr, limitPerceptions=limitPerceptions)
             elif molBuildType in ["inchi"]:
                 oeMol = self.__inchiToMol(ccId, descr, limitPerceptions=limitPerceptions)
             #
             return oeMol
         except Exception as e:
```

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeMoleculeProvider.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeMoleculeProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeSearchMoleculeProvider.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeSearchMoleculeProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeSearchUtils.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeSearchUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/OeSubStructSearchUtils.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/OeSubStructSearchUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/PdbxChemComp.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/PdbxChemComp.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/PdbxChemCompConstants.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/PdbxChemCompConstants.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/RdMoleculeFactory.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/RdMoleculeFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb/utils/chem/cactvsAnnotateMol.py` & `rcsb_utils_chem-0.80/rcsb/utils/chem/cactvsAnnotateMol.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/PKG-INFO` & `rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chem
-Version: 0.79
+Version: 0.80
 Summary: RCSB Python Chemical Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chem
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chem-0.79/rcsb.utils.chem.egg-info/SOURCES.txt` & `rcsb_utils_chem-0.80/rcsb.utils.chem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chem-0.79/setup.py` & `rcsb_utils_chem-0.80/setup.py`

 * *Files identical despite different names*

