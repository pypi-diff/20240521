# Comparing `tmp/aiondata-0.4.6.tar.gz` & `tmp/aiondata-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiondata-0.4.6.tar", max compression
+gzip compressed data, was "aiondata-0.5.0.tar", max compression
```

## Comparing `aiondata-0.4.6.tar` & `aiondata-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11372 2024-05-19 13:00:50.817646 aiondata-0.4.6/LICENSE
--rw-r--r--   0        0        0     4606 2024-05-19 13:00:50.817646 aiondata-0.4.6/README.md
--rw-r--r--   0        0        0      419 2024-05-19 13:00:50.817646 aiondata-0.4.6/aiondata/__init__.py
--rw-r--r--   0        0        0     8538 2024-05-19 13:00:50.817646 aiondata-0.4.6/aiondata/bindingdb.py
--rw-r--r--   0        0        0     2326 2024-05-19 13:00:50.817646 aiondata-0.4.6/aiondata/datasets.py
--rw-r--r--   0        0        0     4714 2024-05-19 13:00:50.817646 aiondata-0.4.6/aiondata/moleculenet.py
--rw-r--r--   0        0        0     8692 2024-05-19 13:00:50.821646 aiondata-0.4.6/aiondata/protein_structure.py
--rw-r--r--   0        0        0     5413 2024-05-19 13:00:50.821646 aiondata-0.4.6/aiondata/weizmann_ccca.py
--rw-r--r--   0        0        0     1505 2024-05-19 13:00:50.821646 aiondata-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    11372 2024-05-21 14:11:42.805010 aiondata-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4606 2024-05-21 14:11:42.805010 aiondata-0.5.0/README.md
+-rw-r--r--   0        0        0      436 2024-05-21 14:11:42.805010 aiondata-0.5.0/aiondata/__init__.py
+-rw-r--r--   0        0        0     9582 2024-05-21 14:11:42.805010 aiondata-0.5.0/aiondata/bindingdb.py
+-rw-r--r--   0        0        0     2326 2024-05-21 14:11:42.805010 aiondata-0.5.0/aiondata/datasets.py
+-rw-r--r--   0        0        0     4714 2024-05-21 14:11:42.809010 aiondata-0.5.0/aiondata/moleculenet.py
+-rw-r--r--   0        0        0     8692 2024-05-21 14:11:42.809010 aiondata-0.5.0/aiondata/protein_structure.py
+-rw-r--r--   0        0        0     5413 2024-05-21 14:11:42.809010 aiondata-0.5.0/aiondata/weizmann_ccca.py
+-rw-r--r--   0        0        0     1505 2024-05-21 14:11:42.809010 aiondata-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.5.0/PKG-INFO
```

### Comparing `aiondata-0.4.6/LICENSE` & `aiondata-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.6/README.md` & `aiondata-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.6/aiondata/bindingdb.py` & `aiondata-0.5.0/aiondata/bindingdb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from collections import OrderedDict
 import io
 from typing import Optional, Generator, Union, Tuple
 import urllib.request
-from rdkit import Chem
-from rdkit import RDLogger
+from rdkit import Chem, RDLogger
 from tqdm.auto import tqdm
 import zipfile
 
-from .datasets import GeneratedDataset
+from .datasets import GeneratedDataset, CachedDataset
 import polars as pl
 
 
 class BindingDB(GeneratedDataset):
     """BindingDB
 
     A public, web-accessible database of measured binding affinities, focusing chiefly on the interactions of protein considered to be drug-targets with small, drug-like molecules.
@@ -228,7 +226,40 @@
         self.fd.close()
         if self.outer_fd is not None:
             self.outer_fd.close()
 
         # Re-enable logging
         RDLogger.EnableLog("rdApp.error")
         RDLogger.EnableLog("rdApp.warning")
+
+
+class BindingAffinity(CachedDataset):
+    def __init__(self, fd: Optional[io.BufferedReader] = None):
+        """
+        Initializes a BindingAffinity instance.
+
+        Args:
+            fd (Optional[io.BufferedReader]): The file-like object containing the BindingDB content.
+                If `fd` is not provided, the dataset content will be fetched from the default source.
+        """
+        self.bindingdb = BindingDB(fd)
+
+    def get_df(self) -> pl.DataFrame:
+        bdb_df = self.bindingdb.to_df()
+        ba_df = bdb_df.select(
+            [
+                "SMILES",
+                "BindingDB Target Chain Sequence",
+                "Ki (nM)",
+                "IC50 (nM)",
+                "Kd (nM)",
+                "EC50 (nM)",
+                "kon (M-1-s-1)",
+                "koff (s-1)",
+            ]
+        )
+        ba_df = ba_df.rename({"BindingDB Target Chain Sequence": "Sequence"})
+
+        # Remove spaces from BindingDB Target Chain Sequence column
+        ba_df = ba_df.with_columns(pl.col("Sequence").str.replace_all(" ", ""))
+
+        return ba_df
```

### Comparing `aiondata-0.4.6/aiondata/datasets.py` & `aiondata-0.5.0/aiondata/datasets.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.6/aiondata/moleculenet.py` & `aiondata-0.5.0/aiondata/moleculenet.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.6/aiondata/protein_structure.py` & `aiondata-0.5.0/aiondata/protein_structure.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.6/aiondata/weizmann_ccca.py` & `aiondata-0.5.0/aiondata/weizmann_ccca.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.6/pyproject.toml` & `aiondata-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiondata"
-version = "0.4.6"
+version = "0.5.0"
 description = "A common data access layer for AI-driven drug discovery."
 authors = ["JJ Ben-Joseph <jj@tensorspace.ai>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://www.github.com/aion-labs/aiondata"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `aiondata-0.4.6/PKG-INFO` & `aiondata-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiondata
-Version: 0.4.6
+Version: 0.5.0
 Summary: A common data access layer for AI-driven drug discovery.
 Home-page: https://www.github.com/aion-labs/aiondata
 License: Apache
 Author: JJ Ben-Joseph
 Author-email: jj@tensorspace.ai
 Requires-Python: >=3.10
 Classifier: Development Status :: 3 - Alpha
```

