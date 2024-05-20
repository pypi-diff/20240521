# Comparing `tmp/dolomite-ranges-0.1.1.tar.gz` & `tmp/dolomite_ranges-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolomite-ranges-0.1.1.tar", last modified: Fri Feb  9 16:08:40 2024, max compression
+gzip compressed data, was "dolomite_ranges-0.1.2.tar", last modified: Mon May 20 22:10:55 2024, max compression
```

## Comparing `dolomite-ranges-0.1.1.tar` & `dolomite_ranges-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:08:40.002776 dolomite-ranges-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:08:39.990775 dolomite-ranges-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:08:39.994776 dolomite-ranges-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-02-09 16:08:40.002776 dolomite-ranges-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:08:39.998776 dolomite-ranges-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:08:39.998776 dolomite-ranges-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-09 16:08:40.002776 dolomite-ranges-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:08:39.990775 dolomite-ranges-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:08:39.998776 dolomite-ranges-0.1.1/src/dolomite_ranges/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/src/dolomite_ranges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/src/dolomite_ranges/read_genomic_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/src/dolomite_ranges/read_genomic_ranges_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/src/dolomite_ranges/read_sequence_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/src/dolomite_ranges/save_genomic_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/src/dolomite_ranges/save_genomic_ranges_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/src/dolomite_ranges/save_sequence_information.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:08:40.002776 dolomite-ranges-0.1.1/src/dolomite_ranges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-02-09 16:08:39.000000 dolomite-ranges-0.1.1/src/dolomite_ranges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-09 16:08:39.000000 dolomite-ranges-0.1.1/src/dolomite_ranges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:08:39.000000 dolomite-ranges-0.1.1/src/dolomite_ranges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:08:39.000000 dolomite-ranges-0.1.1/src/dolomite_ranges.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-09 16:08:39.000000 dolomite-ranges-0.1.1/src/dolomite_ranges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-09 16:08:39.000000 dolomite-ranges-0.1.1/src/dolomite_ranges.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:08:40.002776 dolomite-ranges-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/tests/test_genomic_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/tests/test_granges_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/tests/test_sequence_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-09 16:07:43.000000 dolomite-ranges-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:55.814380 dolomite_ranges-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:55.806380 dolomite_ranges-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:55.810380 dolomite_ranges-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-20 22:10:55.814380 dolomite_ranges-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:55.810380 dolomite_ranges-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:55.810380 dolomite_ranges-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:10:55.814380 dolomite_ranges-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:55.806380 dolomite_ranges-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:55.810380 dolomite_ranges-0.1.2/src/dolomite_ranges/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/src/dolomite_ranges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/src/dolomite_ranges/read_genomic_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/src/dolomite_ranges/read_genomic_ranges_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/src/dolomite_ranges/read_sequence_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/src/dolomite_ranges/save_genomic_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/src/dolomite_ranges/save_genomic_ranges_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/src/dolomite_ranges/save_sequence_information.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:55.814380 dolomite_ranges-0.1.2/src/dolomite_ranges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-20 22:10:55.000000 dolomite_ranges-0.1.2/src/dolomite_ranges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 22:10:55.000000 dolomite_ranges-0.1.2/src/dolomite_ranges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:10:55.000000 dolomite_ranges-0.1.2/src/dolomite_ranges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:10:55.000000 dolomite_ranges-0.1.2/src/dolomite_ranges.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-20 22:10:55.000000 dolomite_ranges-0.1.2/src/dolomite_ranges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 22:10:55.000000 dolomite_ranges-0.1.2/src/dolomite_ranges.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:55.814380 dolomite_ranges-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/tests/test_genomic_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/tests/test_granges_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/tests/test_sequence_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-20 22:09:54.000000 dolomite_ranges-0.1.2/tox.ini
```

### Comparing `dolomite-ranges-0.1.1/.coveragerc` & `dolomite_ranges-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/.github/workflows/pypi-publish.yml` & `dolomite_ranges-0.1.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/.github/workflows/pypi-test.yml` & `dolomite_ranges-0.1.2/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/.gitignore` & `dolomite_ranges-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/.readthedocs.yml` & `dolomite_ranges-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/CONTRIBUTING.md` & `dolomite_ranges-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/LICENSE.txt` & `dolomite_ranges-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/PKG-INFO` & `dolomite_ranges-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolomite-ranges
-Version: 0.1.1
+Version: 0.1.2
 Summary: Stage and load genomic ranges from disk.
 Home-page: https://github.com/ArtifactDB/dolomite-ranges
 Author: LTLA
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-ranges
 Platform: any
```

### Comparing `dolomite-ranges-0.1.1/README.md` & `dolomite_ranges-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/docs/Makefile` & `dolomite_ranges-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/docs/conf.py` & `dolomite_ranges-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/docs/index.md` & `dolomite_ranges-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/setup.cfg` & `dolomite_ranges-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/setup.py` & `dolomite_ranges-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/src/dolomite_ranges/__init__.py` & `dolomite_ranges-0.1.2/src/dolomite_ranges/__init__.py`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/src/dolomite_ranges/read_genomic_ranges.py` & `dolomite_ranges-0.1.2/src/dolomite_ranges/read_genomic_ranges.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 import dolomite_base as dl
 import h5py
 from dolomite_base.read_object import read_object_registry
 from genomicranges import GenomicRanges
 from iranges import IRanges
 
-from .read_sequence_information import read_sequence_information
-
 read_object_registry["genomic_ranges"] = "dolomite_ranges.read_genomic_ranges"
 
 
 def read_genomic_ranges(path: str, metadata: Optional[dict], **kwargs) -> GenomicRanges:
     """Load genomic ranges into a
     :py:class:`~genomicranges.GenomicRanges.GenomicRanges` object.
 
@@ -30,15 +28,15 @@
         kwargs:
             Further arguments, ignored.
 
     Returns:
         A :py:class:`~genomicranges.GenomicRanges.GenomicRanges` object.
     """
     _seqinfo_path = os.path.join(path, "sequence_information")
-    seqinfo = read_sequence_information(path=_seqinfo_path, metadata=None)
+    seqinfo = dl.alt_read_object(path=_seqinfo_path, **kwargs)
 
     with h5py.File(os.path.join(path, "ranges.h5"), "r") as handle:
         ghandle = handle["genomic_ranges"]
 
         seqnames = dl.load_vector_from_hdf5(
             ghandle["sequence"], expected_type=int, report_1darray=True
         )
@@ -60,16 +58,16 @@
         ranges=IRanges(starts, widths),
         strand=strand,
         seqinfo=seqinfo,
     )
 
     _range_annotation_path = os.path.join(path, "range_annotations")
     if os.path.exists(_range_annotation_path):
-        _mcols = dl.read_object(_range_annotation_path)
+        _mcols = dl.alt_read_object(_range_annotation_path, **kwargs)
         gr = gr.set_mcols(_mcols)
 
     _meta_path = os.path.join(path, "other_annotations")
     if os.path.exists(_meta_path):
-        _meta = dl.read_object(_meta_path)
+        _meta = dl.alt_read_object(_meta_path, **kwargs)
         gr = gr.set_metadata(_meta.as_dict())
 
     return gr
```

### Comparing `dolomite-ranges-0.1.1/src/dolomite_ranges/read_genomic_ranges_list.py` & `dolomite_ranges-0.1.2/src/dolomite_ranges/read_genomic_ranges_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from typing import Optional
 
 import dolomite_base as dl
 import h5py
 from dolomite_base.read_object import read_object_registry
 from genomicranges import GenomicRangesList
 
-from .read_genomic_ranges import read_genomic_ranges
-
 read_object_registry["genomic_ranges_list"] = "dolomite_ranges.read_genomic_ranges_list"
 
 
 def read_genomic_ranges_list(
     path: str, metadata: Optional[dict], **kwargs
 ) -> GenomicRangesList:
     """Load genomic ranges into a
@@ -44,17 +42,15 @@
 
         names = None
         if "names" in ghandle:
             names = dl.load_vector_from_hdf5(
                 ghandle["names"], expected_type=str, report_1darray=True
             )
 
-    _all_granges = read_genomic_ranges(
-        path=os.path.join(path, "concatenated"), metadata=None
-    )
+    _all_granges = dl.alt_read_object(path=os.path.join(path, "concatenated"), **kwargs)
 
     counter = 0
     _split_granges = []
     if lengths.sum() == 0:
         _split_granges = _all_granges
     else:
         for ilen in lengths:
@@ -62,16 +58,16 @@
             _split_granges.append(_frag)
             counter += ilen
 
     grl = GenomicRangesList(names=names, range_lengths=lengths, ranges=_split_granges)
 
     _elem_annotation_path = os.path.join(path, "element_annotations")
     if os.path.exists(_elem_annotation_path):
-        _mcols = dl.read_object(_elem_annotation_path)
+        _mcols = dl.alt_read_object(_elem_annotation_path, **kwargs)
         grl = grl.set_mcols(_mcols)
 
     _meta_path = os.path.join(path, "other_annotations")
     if os.path.exists(_meta_path):
-        _meta = dl.read_object(_meta_path)
+        _meta = dl.alt_read_object(_meta_path, **kwargs)
         grl = grl.set_metadata(_meta.as_dict())
 
     return grl
```

### Comparing `dolomite-ranges-0.1.1/src/dolomite_ranges/read_sequence_information.py` & `dolomite_ranges-0.1.2/src/dolomite_ranges/read_sequence_information.py`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/src/dolomite_ranges/save_genomic_ranges.py` & `dolomite_ranges-0.1.2/src/dolomite_ranges/save_genomic_ranges.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,20 @@
         )
 
         if x.get_names() is not None:
             dl.write_string_vector_to_hdf5(ghandle, name="name", x=x.get_names())
 
     _range_annotation = x.get_mcols()
     if _range_annotation is not None and _range_annotation.shape[1] > 0:
-        dl.save_object(
+        dl.alt_save_object(
             _range_annotation,
             path=os.path.join(path, "range_annotations"),
             **data_frame_args
         )
 
     _meta = x.get_metadata()
     if _meta is not None and len(_meta) > 0:
-        dl.save_object(_meta, path=os.path.join(path, "other_annotations"))
+        dl.alt_save_object(
+            _meta, path=os.path.join(path, "other_annotations"), **kwargs
+        )
 
     return
```

### Comparing `dolomite-ranges-0.1.1/src/dolomite_ranges/save_genomic_ranges_list.py` & `dolomite_ranges-0.1.2/src/dolomite_ranges/save_genomic_ranges_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,22 +53,24 @@
         if x.get_names() is not None:
             dl.write_string_vector_to_hdf5(ghandle, name="names", x=x.get_names())
 
     _all_ranges = x.get_ranges()
     if isinstance(_all_ranges, list) and len(_all_ranges) > 1:
         _all_ranges = combine_sequences(*x.get_ranges())
 
-    dl.save_object(_all_ranges, path=os.path.join(path, "concatenated"))
+    dl.alt_save_object(_all_ranges, path=os.path.join(path, "concatenated"), **kwargs)
 
     _elem_annotation = x.get_mcols()
     if _elem_annotation is not None and _elem_annotation.shape[1] > 0:
-        dl.save_object(
+        dl.alt_save_object(
             _elem_annotation,
             path=os.path.join(path, "element_annotations"),
             **data_frame_args
         )
 
     _meta = x.get_metadata()
     if _meta is not None and len(_meta) > 0:
-        dl.save_object(_meta, path=os.path.join(path, "other_annotations"))
+        dl.alt_save_object(
+            _meta, path=os.path.join(path, "other_annotations"), **kwargs
+        )
 
     return
```

### Comparing `dolomite-ranges-0.1.1/src/dolomite_ranges/save_sequence_information.py` & `dolomite_ranges-0.1.2/src/dolomite_ranges/save_sequence_information.py`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/src/dolomite_ranges.egg-info/PKG-INFO` & `dolomite_ranges-0.1.2/src/dolomite_ranges.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolomite-ranges
-Version: 0.1.1
+Version: 0.1.2
 Summary: Stage and load genomic ranges from disk.
 Home-page: https://github.com/ArtifactDB/dolomite-ranges
 Author: LTLA
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-ranges
 Platform: any
```

### Comparing `dolomite-ranges-0.1.1/src/dolomite_ranges.egg-info/SOURCES.txt` & `dolomite_ranges-0.1.2/src/dolomite_ranges.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/tests/test_genomic_ranges.py` & `dolomite_ranges-0.1.2/tests/test_genomic_ranges.py`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/tests/test_granges_list.py` & `dolomite_ranges-0.1.2/tests/test_granges_list.py`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/tests/test_sequence_information.py` & `dolomite_ranges-0.1.2/tests/test_sequence_information.py`

 * *Files identical despite different names*

### Comparing `dolomite-ranges-0.1.1/tox.ini` & `dolomite_ranges-0.1.2/tox.ini`

 * *Files identical despite different names*

