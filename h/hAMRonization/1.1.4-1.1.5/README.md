# Comparing `tmp/hAMRonization-1.1.4.tar.gz` & `tmp/hamronization-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hAMRonization-1.1.4.tar", last modified: Wed Oct 18 01:17:32 2023, max compression
+gzip compressed data, was "hamronization-1.1.5.tar", last modified: Tue May 21 21:10:32 2024, max compression
```

## Comparing `hAMRonization-1.1.4.tar` & `hamronization-1.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 01:17:32.688992 hAMRonization-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17841 2023-10-18 01:17:32.692992 hAMRonization-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16626 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 01:17:32.688992 hAMRonization-1.1.4/hAMRonization/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/AbricateIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/AmrFinderPlusIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/AmrPlusPlusIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/AribaIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/CSStarIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/DeepArgIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/FARGeneIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/GrootIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/Interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/KmerResistanceIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/MykrobeIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/PointFinderIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/ResFamsIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/ResFinderIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/RgiIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/SraxIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/Srst2IO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/StarAmrIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/TBProfilerIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/hAMRonizedResult.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/hamronize.py
--rw-r--r--   0 runner    (1001) docker     (127)    31901 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/hAMRonization/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 01:17:32.688992 hAMRonization-1.1.4/hAMRonization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17841 2023-10-18 01:17:32.000000 hAMRonization-1.1.4/hAMRonization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-10-18 01:17:32.000000 hAMRonization-1.1.4/hAMRonization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 01:17:32.000000 hAMRonization-1.1.4/hAMRonization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-18 01:17:32.000000 hAMRonization-1.1.4/hAMRonization.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-18 01:17:32.000000 hAMRonization-1.1.4/hAMRonization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-18 01:17:32.000000 hAMRonization-1.1.4/hAMRonization.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 01:17:32.000000 hAMRonization-1.1.4/hAMRonization.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-10-18 01:17:32.692992 hAMRonization-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 01:17:32.688992 hAMRonization-1.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/test/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    37514 2023-10-18 01:16:54.000000 hAMRonization-1.1.4/test/test_parsing_validity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:10:32.083994 hamronization-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-21 21:10:28.000000 hamronization-1.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17863 2024-05-21 21:10:32.083994 hamronization-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-05-21 21:10:28.000000 hamronization-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:10:32.079994 hamronization-1.1.5/hAMRonization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/AbricateIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/AmrFinderPlusIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/AmrPlusPlusIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/AribaIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/CSStarIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/DeepArgIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/FARGeneIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/GrootIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/Interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/KmerResistanceIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/MykrobeIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/PointFinderIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/ResFamsIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/ResFinderIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/RgiIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/SraxIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/Srst2IO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/StarAmrIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/TBProfilerIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/hAMRonizedResult.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/hamronize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31901 2024-05-21 21:10:28.000000 hamronization-1.1.5/hAMRonization/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:10:32.083994 hamronization-1.1.5/hAMRonization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17863 2024-05-21 21:10:32.000000 hamronization-1.1.5/hAMRonization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-21 21:10:32.000000 hamronization-1.1.5/hAMRonization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:10:32.000000 hamronization-1.1.5/hAMRonization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 21:10:32.000000 hamronization-1.1.5/hAMRonization.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 21:10:32.000000 hamronization-1.1.5/hAMRonization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 21:10:32.000000 hamronization-1.1.5/hAMRonization.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:10:32.000000 hamronization-1.1.5/hAMRonization.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-21 21:10:32.083994 hamronization-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-21 21:10:28.000000 hamronization-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:10:32.083994 hamronization-1.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-21 21:10:29.000000 hamronization-1.1.5/test/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38311 2024-05-21 21:10:29.000000 hamronization-1.1.5/test/test_parsing_validity.py
```

### Comparing `hAMRonization-1.1.4/LICENSE.txt` & `hamronization-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/PKG-INFO` & `hamronization-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hAMRonization
-Version: 1.1.4
+Version: 1.1.5
 Summary: Tool to convert and summarize AMR gene detection outputs using the hAMRonization specification
 Home-page: https://github.com/pha4ge/hAMRonization
-Download-URL: https://github.com/pha4ge/archive/v1.1.4.tar.gz
+Download-URL: https://github.com/pha4ge/archive/v1.1.5.tar.gz
 Author: Finlay Maguire
 Author-email: finlaymaguire@gmail.com
 License: LGPLv3
 Keywords: Genomics,Antimicrobial resistance,Antibiotic,Standardization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pandas
 
 ![Python package](https://github.com/pha4ge/hAMRonization/workflows/test_package/badge.svg)
 [![DOI](https://zenodo.org/badge/248040662.svg)](https://zenodo.org/badge/latestdoi/248040662)
 [![Docs English](https://img.shields.io/badge/Documentation-English-blue)](https://github.com/pha4ge/hAMRonization/blob/master/docs/subgrant/PHA4GE_AMR_SubGrant_Documentation.pdf)
 [![Docs English](https://img.shields.io/badge/Documentation-Español-blue)](https://github.com/pha4ge/hAMRonization/blob/master/docs/subgrant/PHA4GE_hAMRonization_espan%CC%83ol.pdf)
```

### Comparing `hAMRonization-1.1.4/README.md` & `hamronization-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/AbricateIO.py` & `hamronization-1.1.5/hAMRonization/AbricateIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/AmrFinderPlusIO.py` & `hamronization-1.1.5/hAMRonization/AmrFinderPlusIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/AmrPlusPlusIO.py` & `hamronization-1.1.5/hAMRonization/AmrPlusPlusIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/AribaIO.py` & `hamronization-1.1.5/hAMRonization/AribaIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/CSStarIO.py` & `hamronization-1.1.5/hAMRonization/CSStarIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/DeepArgIO.py` & `hamronization-1.1.5/hAMRonization/DeepArgIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/FARGeneIO.py` & `hamronization-1.1.5/hAMRonization/FARGeneIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/GrootIO.py` & `hamronization-1.1.5/hAMRonization/GrootIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/Interfaces.py` & `hamronization-1.1.5/hAMRonization/Interfaces.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/KmerResistanceIO.py` & `hamronization-1.1.5/hAMRonization/KmerResistanceIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/MykrobeIO.py` & `hamronization-1.1.5/hAMRonization/MykrobeIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/PointFinderIO.py` & `hamronization-1.1.5/hAMRonization/PointFinderIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/ResFamsIO.py` & `hamronization-1.1.5/hAMRonization/ResFamsIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/ResFinderIO.py` & `hamronization-1.1.5/hAMRonization/ResFinderIO.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,21 +52,36 @@
     def parse(self, handle):
         """
         Read each and return it
         """
         reader = csv.DictReader(handle, delimiter="\t")
         for result in reader:
             result["_gene_name"] = result["Resistance gene"]
-            _start, _stop = result["Position in contig"].split("..")
-            if _start > _stop:
-                _strand = "-"
+            # Removes fields that have NA and NA..NA this is typical in the 4.5.0 resfinder when the --inputfastq is implimented
+            for field, value in result.items():
+                if value == "NA":
+                    result[field] = None
+                if value == "NA..NA":
+                    result[field] = None
+            # If result["Position in contig"] == None then make _start, _stop and _strand = None
+            if result["Position in contig"] != None:
+                _start, _stop = result["Position in contig"].split("..")
+                if _start > _stop :
+                    _strand = "-"
+                else:
+                    _strand = "+"
+                    
+                result["_start"] = _start
+                result["_stop"] = _stop
+                result["_strand"] = _strand
             else:
-                _strand = "+"
-            result["_start"] = _start
-            result["_stop"] = _stop
-            result["_strand"] = _strand
+                _strand = None
+                result["_start"] = None
+                result["_stop"] = None
+                result["_strand"] = None
+                
             _reference_gene_length = result["Alignment Length/Gene Length"].split("/")[
                 0
             ]
             result["_reference_gene_length"] = _reference_gene_length
             yield self.hAMRonize(result, self.metadata)
             result = {}
```

### Comparing `hAMRonization-1.1.4/hAMRonization/RgiIO.py` & `hamronization-1.1.5/hAMRonization/RgiIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/SraxIO.py` & `hamronization-1.1.5/hAMRonization/SraxIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/Srst2IO.py` & `hamronization-1.1.5/hAMRonization/Srst2IO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/StarAmrIO.py` & `hamronization-1.1.5/hAMRonization/StarAmrIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/TBProfilerIO.py` & `hamronization-1.1.5/hAMRonization/TBProfilerIO.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/__init__.py` & `hamronization-1.1.5/hAMRonization/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 
 from hAMRonization import AbricateIO
 from hAMRonization import AmrFinderPlusIO
 from hAMRonization import AribaIO
 from hAMRonization import RgiIO
 from hAMRonization import ResFinderIO
 from hAMRonization import SraxIO
```

### Comparing `hAMRonization-1.1.4/hAMRonization/hAMRonizedResult.py` & `hamronization-1.1.5/hAMRonization/hAMRonizedResult.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization/summarize.py` & `hamronization-1.1.5/hAMRonization/summarize.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/hAMRonization.egg-info/PKG-INFO` & `hamronization-1.1.5/hAMRonization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hAMRonization
-Version: 1.1.4
+Version: 1.1.5
 Summary: Tool to convert and summarize AMR gene detection outputs using the hAMRonization specification
 Home-page: https://github.com/pha4ge/hAMRonization
-Download-URL: https://github.com/pha4ge/archive/v1.1.4.tar.gz
+Download-URL: https://github.com/pha4ge/archive/v1.1.5.tar.gz
 Author: Finlay Maguire
 Author-email: finlaymaguire@gmail.com
 License: LGPLv3
 Keywords: Genomics,Antimicrobial resistance,Antibiotic,Standardization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pandas
 
 ![Python package](https://github.com/pha4ge/hAMRonization/workflows/test_package/badge.svg)
 [![DOI](https://zenodo.org/badge/248040662.svg)](https://zenodo.org/badge/latestdoi/248040662)
 [![Docs English](https://img.shields.io/badge/Documentation-English-blue)](https://github.com/pha4ge/hAMRonization/blob/master/docs/subgrant/PHA4GE_AMR_SubGrant_Documentation.pdf)
 [![Docs English](https://img.shields.io/badge/Documentation-Español-blue)](https://github.com/pha4ge/hAMRonization/blob/master/docs/subgrant/PHA4GE_hAMRonization_espan%CC%83ol.pdf)
```

### Comparing `hAMRonization-1.1.4/hAMRonization.egg-info/SOURCES.txt` & `hamronization-1.1.5/hAMRonization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/setup.py` & `hamronization-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/test/test_interfaces.py` & `hamronization-1.1.5/test/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `hAMRonization-1.1.4/test/test_parsing_validity.py` & `hamronization-1.1.5/test/test_parsing_validity.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         assert result.input_protein_stop is None
         assert result.reference_protein_start is None
         assert result.reference_protein_stop is None
         assert result.reference_gene_start is None
         assert result.reference_gene_stop is None
 
 
-def test_resfinder():
+def test_pointfinder():
     metadata = {
         "analysis_software_version": "4.1.0",
         "reference_database_version": "2021-02-01",
         "input_file_name": "Dummy",
     }
     parsed_report = hAMRonization.parse(
         "data/dummy/pointfinder/PointFinder_results.txt", metadata, "pointfinder"
@@ -314,25 +314,40 @@
         assert result.analysis_software_version == "4.1.0"
         assert result.genetic_variation_type == "protein_variant_detected"
 
         assert result.drug_class == "Ciprofloxacin,Nalidixic acid,Ciprofloxacin"
         assert result.nucleotide_mutation == "GGT -> GAT"
         assert result.amino_acid_mutation == "p.G81D"
 
-
-def test_pointfinder():
+def test_resfinder_fastq():
     metadata = {
-        "analysis_software_version": "4.1.0",
-        "reference_database_version": "2019-Jul-28",
+        "analysis_software_version": "4.5.0",
+        "reference_database_version": "2021-02-01",
         "input_file_name": "Dummy",
     }
     parsed_report = hAMRonization.parse(
-        "data/dummy/resfinder/ResFinder_results_tab.txt", metadata, "resfinder"
+        "data/dummy/resfinder/resfinder_inputfastq_inputfasta.txt", metadata, "resfinder"
     )
 
+    for result in parsed_report:
+        # assert mandatory fields
+        assert result.input_file_name == "Dummy"
+        assert result.gene_symbol == "aph(6)-Id"
+        assert result.gene_name == "aph(6)-Id"
+        assert result.reference_database_name == "resfinder"
+        assert result.reference_database_version == "2021-02-01"
+        assert result.reference_accession == "M28829"
+        assert result.analysis_software_name == "resfinder"
+        assert result.analysis_software_version == "4.5.0"
+        assert result.genetic_variation_type == "gene_presence_detected"
+        assert result.coverage_percentage == 100
+        assert result.drug_class == "Streptomycin"
+        assert result.reference_gene_length == 837
+        assert result.sequence_identity == 100
+
 
 def test_rgi_variants():
     metadata = {
         "analysis_software_version": "5.2.0",
         "reference_database_version": "3.2.4",
         "input_file_name": "Dummy",
     }
```

