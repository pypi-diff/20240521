# Comparing `tmp/rcsb.utils.seq-0.79.tar.gz` & `tmp/rcsb_utils_seq-0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.seq-0.79.tar", last modified: Tue Mar 19 16:29:18 2024, max compression
+gzip compressed data, was "rcsb_utils_seq-0.80.tar", last modified: Tue May 21 19:22:22 2024, max compression
```

## Comparing `rcsb.utils.seq-0.79.tar` & `rcsb_utils_seq-0.80.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-19 16:29:18.010787 rcsb.utils.seq-0.79/
--rw-r--r--   0 vsts      (1001) docker     (127)     5566 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1925 2024-03-19 16:29:18.010787 rcsb.utils.seq-0.79/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-19 16:29:18.006787 rcsb.utils.seq-0.79/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-19 16:29:18.006787 rcsb.utils.seq-0.79/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-19 16:29:18.010787 rcsb.utils.seq-0.79/rcsb/utils/seq/
--rw-r--r--   0 vsts      (1001) docker     (127)    11893 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/GlyGenProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3042 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/GlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8323 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/InterProProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7748 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/PfamProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4720 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/SeqAlign.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20465 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/SiftsSummaryProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15157 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/UniProtIdMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34943 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/UniProtReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32271 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/UniProtUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/rcsb/utils/seq/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-19 16:29:18.010787 rcsb.utils.seq-0.79/rcsb.utils.seq.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1925 2024-03-19 16:29:17.000000 rcsb.utils.seq-0.79/rcsb.utils.seq.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-03-19 16:29:17.000000 rcsb.utils.seq-0.79/rcsb.utils.seq.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-19 16:29:17.000000 rcsb.utils.seq-0.79/rcsb.utils.seq.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-19 16:19:53.000000 rcsb.utils.seq-0.79/rcsb.utils.seq.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      141 2024-03-19 16:29:17.000000 rcsb.utils.seq-0.79/rcsb.utils.seq.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-03-19 16:29:17.000000 rcsb.utils.seq-0.79/rcsb.utils.seq.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-03-19 16:29:18.014787 rcsb.utils.seq-0.79/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2263 2024-03-19 16:18:20.000000 rcsb.utils.seq-0.79/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 19:22:22.545532 rcsb_utils_seq-0.80/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5603 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1925 2024-05-21 19:22:22.545532 rcsb_utils_seq-0.80/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 19:22:22.545532 rcsb_utils_seq-0.80/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 19:22:22.545532 rcsb_utils_seq-0.80/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 19:22:22.545532 rcsb_utils_seq-0.80/rcsb/utils/seq/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11893 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/GlyGenProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3042 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/GlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8323 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/InterProProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7748 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/PfamProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4720 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/SeqAlign.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20465 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/SiftsSummaryProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15157 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/UniProtIdMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34996 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/UniProtReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32271 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/UniProtUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/rcsb/utils/seq/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 19:22:22.545532 rcsb_utils_seq-0.80/rcsb.utils.seq.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1925 2024-05-21 19:22:22.000000 rcsb_utils_seq-0.80/rcsb.utils.seq.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-05-21 19:22:22.000000 rcsb_utils_seq-0.80/rcsb.utils.seq.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 19:22:22.000000 rcsb_utils_seq-0.80/rcsb.utils.seq.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 19:13:58.000000 rcsb_utils_seq-0.80/rcsb.utils.seq.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      141 2024-05-21 19:22:22.000000 rcsb_utils_seq-0.80/rcsb.utils.seq.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-21 19:22:22.000000 rcsb_utils_seq-0.80/rcsb.utils.seq.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-21 19:22:22.545532 rcsb_utils_seq-0.80/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2263 2024-05-21 19:12:43.000000 rcsb_utils_seq-0.80/setup.py
```

### Comparing `rcsb.utils.seq-0.79/HISTORY.txt` & `rcsb_utils_seq-0.80/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,8 +66,9 @@
    6-Feb-2023    V0.73 Resolve pylint issues
   23-Feb-2023    V0.74 Fix UniProtUtils primary fetching service to handle cases with invalid UniProt IDs
    9-Mar-2023    V0.75 Lower default maxChunkSize to 10 for UniProt requests (UniProt API having trouble streaming XML responses)
   19-Sep-2023    V0.76 Use HTTP instead of FTP for InterPro and Pfam downloads;
                        RO-4033: Adjust logic used for processing and assigning sequence alignment details
    3-Oct-2023    V0.77 Update PfamProvider to use new Pfam mapping file
   14-Nov-2023    V0.78 Add SPARQL functionality and version information to GlyGenProvider
-  18-Mar-2024    V0.79 Add yeast and fruitfly datasets to GlyGenProvider
+  18-Mar-2024    V0.79 Add yeast and fruitfly datasets to GlyGenProvider
+  21-May-2024    V0.80 Fix pylinting
```

### Comparing `rcsb.utils.seq-0.79/LICENSE` & `rcsb_utils_seq-0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/PKG-INFO` & `rcsb_utils_seq-0.80/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.seq
-Version: 0.79
+Version: 0.80
 Summary: RCSB Python Linear Polymer Sequence Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.seq-0.79/README.md` & `rcsb_utils_seq-0.80/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/rcsb/utils/seq/GlyGenProvider.py` & `rcsb_utils_seq-0.80/rcsb/utils/seq/GlyGenProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/rcsb/utils/seq/GlycanProvider.py` & `rcsb_utils_seq-0.80/rcsb/utils/seq/GlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/rcsb/utils/seq/InterProProvider.py` & `rcsb_utils_seq-0.80/rcsb/utils/seq/InterProProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/rcsb/utils/seq/PfamProvider.py` & `rcsb_utils_seq-0.80/rcsb/utils/seq/PfamProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/rcsb/utils/seq/SeqAlign.py` & `rcsb_utils_seq-0.80/rcsb/utils/seq/SeqAlign.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/rcsb/utils/seq/SiftsSummaryProvider.py` & `rcsb_utils_seq-0.80/rcsb/utils/seq/SiftsSummaryProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/rcsb/utils/seq/UniProtIdMappingProvider.py` & `rcsb_utils_seq-0.80/rcsb/utils/seq/UniProtIdMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/rcsb/utils/seq/UniProtReader.py` & `rcsb_utils_seq-0.80/rcsb/utils/seq/UniProtReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -827,14 +827,15 @@
 
         newD.update({"evidence": evidenceD})
 
         commentsL = []
         for comment in resultsD["to"]["comments"]:
             if "commentType" in comment:
                 commentType = comment["commentType"].lower()
+                commentText = commentEvidence = None
                 if "texts" in comment:
                     commentText = comment["texts"][0]["value"]
                     commentEvidence = " ".join([str(evidenceFullD[(eD["evidenceCode"], eD.get("source", None), eD.get("id", None))]) for eD in comment["texts"][0]["evidences"]])
                 elif "note" in comment:
                     if isinstance(comment["note"], str):
                         commentText = comment["note"]
                         commentEvidence = " ".join([str(evidenceFullD[(eD["evidenceCode"], eD.get("source", None), eD.get("id", None))]) for eD in comment["evidences"]])
```

### Comparing `rcsb.utils.seq-0.79/rcsb/utils/seq/UniProtUtils.py` & `rcsb_utils_seq-0.80/rcsb/utils/seq/UniProtUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/rcsb.utils.seq.egg-info/PKG-INFO` & `rcsb_utils_seq-0.80/rcsb.utils.seq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.seq
-Version: 0.79
+Version: 0.80
 Summary: RCSB Python Linear Polymer Sequence Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.seq-0.79/rcsb.utils.seq.egg-info/SOURCES.txt` & `rcsb_utils_seq-0.80/rcsb.utils.seq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seq-0.79/setup.py` & `rcsb_utils_seq-0.80/setup.py`

 * *Files identical despite different names*

