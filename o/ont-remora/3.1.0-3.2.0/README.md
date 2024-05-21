# Comparing `tmp/ont-remora-3.1.0.tar.gz` & `tmp/ont_remora-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ont-remora-3.1.0.tar", last modified: Tue Dec  5 22:41:33 2023, max compression
+gzip compressed data, was "ont_remora-3.2.0.tar", last modified: Tue May 21 13:24:10 2024, max compression
```

## Comparing `ont-remora-3.1.0.tar` & `ont_remora-3.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-12-05 22:41:33.822591 ont-remora-3.1.0/
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    14471 2023-05-18 20:02:58.000000 ont-remora-3.1.0/LICENSE.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       45 2023-05-18 20:02:58.000000 ont-remora-3.1.0/MANIFEST.in
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    12707 2023-12-05 22:41:33.822707 ont-remora-3.1.0/PKG-INFO
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    12283 2023-11-14 14:31:18.000000 ont-remora-3.1.0/README.rst
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      343 2023-07-19 22:44:10.000000 ont-remora-3.1.0/pyproject.toml
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1588 2023-12-05 22:41:33.823532 ont-remora-3.1.0/setup.cfg
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      941 2023-09-14 14:55:45.000000 ont-remora-3.1.0/setup.py
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-12-05 22:41:33.810344 ont-remora-3.1.0/src/
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-12-05 22:41:33.814323 ont-remora-3.1.0/src/ont_remora.egg-info/
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    12707 2023-12-05 22:41:33.000000 ont-remora-3.1.0/src/ont_remora.egg-info/PKG-INFO
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      995 2023-12-05 22:41:33.000000 ont-remora-3.1.0/src/ont_remora.egg-info/SOURCES.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-12-05 22:41:33.000000 ont-remora-3.1.0/src/ont_remora.egg-info/dependency_links.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       43 2023-12-05 22:41:33.000000 ont-remora-3.1.0/src/ont_remora.egg-info/entry_points.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-05-18 20:26:40.000000 ont-remora-3.1.0/src/ont_remora.egg-info/not-zip-safe
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      208 2023-12-05 22:41:33.000000 ont-remora-3.1.0/src/ont_remora.egg-info/requires.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        7 2023-12-05 22:41:33.000000 ont-remora-3.1.0/src/ont_remora.egg-info/top_level.txt
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-12-05 22:41:33.820768 ont-remora-3.1.0/src/remora/
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      127 2023-12-05 22:34:39.000000 ont-remora-3.1.0/src/remora/__init__.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      508 2023-05-18 20:02:58.000000 ont-remora-3.1.0/src/remora/activations.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     6364 2023-12-05 22:20:25.000000 ont-remora-3.1.0/src/remora/constants.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    86495 2023-10-31 13:31:53.000000 ont-remora-3.1.0/src/remora/data_chunks.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1536 2023-09-14 14:55:45.000000 ont-remora-3.1.0/src/remora/data_chunks_core.pyx
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1670 2023-05-18 20:02:58.000000 ont-remora-3.1.0/src/remora/download.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3353 2023-11-15 04:57:49.000000 ont-remora-3.1.0/src/remora/duplex_utils.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1557 2023-09-14 14:55:45.000000 ont-remora-3.1.0/src/remora/encoded_kmers.pyx
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    30079 2023-11-15 04:31:31.000000 ont-remora-3.1.0/src/remora/inference.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    83044 2023-11-16 19:45:57.000000 ont-remora-3.1.0/src/remora/io.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2434 2023-09-14 14:55:45.000000 ont-remora-3.1.0/src/remora/log.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1901 2023-09-18 17:34:42.000000 ont-remora-3.1.0/src/remora/main.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3839 2023-05-18 20:02:58.000000 ont-remora-3.1.0/src/remora/metrics.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    22139 2023-11-08 00:34:52.000000 ont-remora-3.1.0/src/remora/model_util.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    68671 2023-11-14 14:31:18.000000 ont-remora-3.1.0/src/remora/parsers.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     8155 2023-11-14 14:31:18.000000 ont-remora-3.1.0/src/remora/prepare_train_data.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    31010 2023-11-21 19:34:56.000000 ont-remora-3.1.0/src/remora/refine_signal_map.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    19514 2023-12-05 19:28:17.000000 ont-remora-3.1.0/src/remora/refine_signal_map_core.pyx
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    18250 2023-09-18 17:33:56.000000 ont-remora-3.1.0/src/remora/train_model.py
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-12-05 22:41:33.821000 ont-remora-3.1.0/src/remora/trained_models/
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      338 2023-05-18 20:02:58.000000 ont-remora-3.1.0/src/remora/trained_models/readme.rst
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    24590 2023-11-14 14:31:18.000000 ont-remora-3.1.0/src/remora/util.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    20497 2023-11-14 14:31:18.000000 ont-remora-3.1.0/src/remora/validate.py
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-12-05 22:41:33.822408 ont-remora-3.1.0/tests/
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      679 2023-05-18 20:02:58.000000 ont-remora-3.1.0/tests/test_coding_standards.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    12174 2023-05-18 20:02:58.000000 ont-remora-3.1.0/tests/test_duplex.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    14199 2023-11-14 14:31:18.000000 ont-remora-3.1.0/tests/test_main.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      740 2023-11-02 23:04:50.000000 ont-remora-3.1.0/tests/test_notebooks.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2024-05-21 13:24:10.965494 ont_remora-3.2.0/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    14471 2023-05-18 20:02:58.000000 ont_remora-3.2.0/LICENSE.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       45 2023-05-18 20:02:58.000000 ont_remora-3.2.0/MANIFEST.in
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    14315 2024-05-21 13:24:10.965284 ont_remora-3.2.0/PKG-INFO
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    13185 2024-05-21 12:16:22.000000 ont_remora-3.2.0/README.rst
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      343 2023-07-19 22:44:10.000000 ont_remora-3.2.0/pyproject.toml
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1607 2024-05-21 13:24:10.965974 ont_remora-3.2.0/setup.cfg
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      941 2023-09-14 14:55:45.000000 ont_remora-3.2.0/setup.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2024-05-21 13:24:10.943155 ont_remora-3.2.0/src/
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2024-05-21 13:24:10.964445 ont_remora-3.2.0/src/ont_remora.egg-info/
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    14315 2024-05-21 13:24:10.000000 ont_remora-3.2.0/src/ont_remora.egg-info/PKG-INFO
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      995 2024-05-21 13:24:10.000000 ont_remora-3.2.0/src/ont_remora.egg-info/SOURCES.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2024-05-21 13:24:10.000000 ont_remora-3.2.0/src/ont_remora.egg-info/dependency_links.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       43 2024-05-21 13:24:10.000000 ont_remora-3.2.0/src/ont_remora.egg-info/entry_points.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-05-18 20:26:40.000000 ont_remora-3.2.0/src/ont_remora.egg-info/not-zip-safe
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      223 2024-05-21 13:24:10.000000 ont_remora-3.2.0/src/ont_remora.egg-info/requires.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        7 2024-05-21 13:24:10.000000 ont_remora-3.2.0/src/ont_remora.egg-info/top_level.txt
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2024-05-21 13:24:10.961353 ont_remora-3.2.0/src/remora/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      127 2024-05-21 13:10:23.000000 ont_remora-3.2.0/src/remora/__init__.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      508 2023-05-18 20:02:58.000000 ont_remora-3.2.0/src/remora/activations.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     7642 2024-05-19 18:25:35.000000 ont_remora-3.2.0/src/remora/constants.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    86949 2024-04-19 17:42:38.000000 ont_remora-3.2.0/src/remora/data_chunks.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1536 2023-09-14 14:55:45.000000 ont_remora-3.2.0/src/remora/data_chunks_core.pyx
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1670 2023-05-18 20:02:58.000000 ont_remora-3.2.0/src/remora/download.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3353 2024-03-13 22:29:18.000000 ont_remora-3.2.0/src/remora/duplex_utils.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1557 2023-09-14 14:55:45.000000 ont_remora-3.2.0/src/remora/encoded_kmers.pyx
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    34574 2024-05-18 01:21:58.000000 ont_remora-3.2.0/src/remora/inference.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    87927 2024-04-19 17:42:38.000000 ont_remora-3.2.0/src/remora/io.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2434 2023-09-14 14:55:45.000000 ont_remora-3.2.0/src/remora/log.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1901 2024-03-13 22:27:10.000000 ont_remora-3.2.0/src/remora/main.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3839 2023-05-18 20:02:58.000000 ont_remora-3.2.0/src/remora/metrics.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    24993 2024-03-29 22:25:43.000000 ont_remora-3.2.0/src/remora/model_util.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    78466 2024-05-21 12:16:22.000000 ont_remora-3.2.0/src/remora/parsers.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     8432 2024-05-21 10:43:27.000000 ont_remora-3.2.0/src/remora/prepare_train_data.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    31010 2024-03-13 22:27:10.000000 ont_remora-3.2.0/src/remora/refine_signal_map.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    19514 2024-03-13 22:28:32.000000 ont_remora-3.2.0/src/remora/refine_signal_map_core.pyx
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    22206 2024-05-18 01:21:58.000000 ont_remora-3.2.0/src/remora/train_model.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2024-05-21 13:24:10.961873 ont_remora-3.2.0/src/remora/trained_models/
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      338 2023-05-18 20:02:58.000000 ont_remora-3.2.0/src/remora/trained_models/readme.rst
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    25911 2024-03-29 22:25:43.000000 ont_remora-3.2.0/src/remora/util.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    20497 2024-03-13 22:27:10.000000 ont_remora-3.2.0/src/remora/validate.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2024-05-21 13:24:10.963962 ont_remora-3.2.0/tests/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      679 2023-05-18 20:02:58.000000 ont_remora-3.2.0/tests/test_coding_standards.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    12174 2023-05-18 20:02:58.000000 ont_remora-3.2.0/tests/test_duplex.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    14199 2024-03-13 22:27:10.000000 ont_remora-3.2.0/tests/test_main.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      740 2024-03-13 22:27:10.000000 ont_remora-3.2.0/tests/test_notebooks.py
```

### Comparing `ont-remora-3.1.0/LICENSE.txt` & `ont_remora-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/PKG-INFO` & `ont_remora-3.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,41 @@
 Metadata-Version: 2.1
 Name: ont-remora
-Version: 3.1.0
+Version: 3.2.0
 Summary: Nanopore methylation/modified base calling detached from basecalling
 Home-page: https://github.com/nanoporetech/remora
 License: ont_public_licence
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8; variant=GFM
-Provides-Extra: tests
 License-File: LICENSE.txt
+Requires-Dist: tqdm
+Requires-Dist: toml
+Requires-Dist: torch
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
+Requires-Dist: thop
+Requires-Dist: pod5>=0.2.8
+Requires-Dist: pysam>=0.20.0
+Requires-Dist: parasail
+Requires-Dist: requests
+Requires-Dist: polars
+Requires-Dist: plotnine==0.12.4
+Requires-Dist: importlib_resources
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: black==22.8.0; extra == "tests"
+Requires-Dist: flake8; extra == "tests"
+Requires-Dist: sphinx; extra == "tests"
+Requires-Dist: build; extra == "tests"
+Requires-Dist: jupyter; extra == "tests"
+Requires-Dist: patchworklib==0.6.3; extra == "tests"
+Requires-Dist: scipy; extra == "tests"
 
 .. image:: /ONT_logo.png
   :width: 800
   :alt: [Oxford Nanopore Technologies]
   :target: https://nanoporetech.com/
 
 Remora
@@ -74,15 +96,15 @@
    :alt: Neural network sequence encoding
 
 Data Preparation
 ----------------
 
 Remora data preparation begins from a POD5 file containing signal data and a BAM file containing basecalls from the POD5 file.
 Note that the BAM file must contain the move table (``--emit-moves`` in Dorado) and the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
-If using minimap2 for alignment use ``samtools fastq -T "*" [in.bam] | minimap2 -y -ax map-ont [ref.fa] - | samtools view -b -o [out.bam]`` in order to transfer the move table tags through the alignment step since minimap2 does not support SAM/BAM input.
+If using minimap2 for alignment use ``samtools fastq -T "*" [in.bam] | minimap2 -y -ax lr:hq [ref.fa] - | samtools view -b -o [out.bam]`` in order to transfer the move table tags through the alignment step since minimap2 does not support SAM/BAM input.
 
 The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the released 5mC CG-context models.
 Example reads can be found in the Remora repository (see ``test/data/`` directory).
 
 K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
 
 .. code-block:: bash
@@ -120,16 +142,20 @@
 The ``remora dataset make_config`` command creates these config files specifying the composition of the new dataset.
 When reading batches from these combined datasets, the default behavior will be to draw chunks randomly from the entire set of chunks.
 This setting is useful for multiple flowcells of the same condition.
 
 The ``--dataset-weights`` argument produces a config which generates batches with a fixed proportion of chunks from each input dataset.
 This setting is useful when combining different data types, for example control and modified datasets.
 
-In addition, the ``remora dataset merge`` command is supplied to merge datasets, copying the data into a new core Remora dataset.
-This may increase efficiency of data access for datasets composed of many core datasets, but only supports the default behavior from the ``make_config`` command.
+The ``remora dataset merge`` command is supplied to merge datasets, copying the data into a new core Remora dataset.
+This may increase efficiency of data access for datasets composed of many core datasets, but only supports the default behavior from the ``make_config`` command (sampling over all chunks).
+
+The ``remora dataset copy`` command is provided in order to move datasets to a new location.
+This can be useful when handling config datasets composed of many core datasets.
+Copying a dataset is especially useful to achieve higher training speeds when core datasets are stored on a network file system (NFS).
 
 Composed dataset config files can also be specified manually.
 Config files are JSON format files containing a single list, where each element is a list of two items.
 The first is the path to the dataset and the second is the weight (must be a positive value).
 The ``make_config`` output config file will also contain the dataset hash to ensure the contents of a dataset are unchanged, but this is an optional third field in the config.
 
 Metadata attributes from each core dataset are checked for compatibility and merged where applicable.
@@ -162,21 +188,21 @@
     train_dataset.jsn \
     --model remora/models/ConvLSTM_w_ref.py \
     --device 0 \
     --chunk-context 50 50 \
     --output-path train_results
 
 This command will produce a "best" model in torchscript format for use in Bonito, ``remora infer``, or ``remora validate`` commands.
-Models can be exported for use in Dorado with the ``remora model export train_results/model_best.pt`` command.
+Models can be exported for use in Dorado with the ``remora model export train_results/model_best.pt train_results_dorado_model`` command.
 
 Model Inference
 ---------------
 
 For testing purposes, inference within Remora is provided.
-For large scale using the exported Dorado model during basecalling is recommended.
+For standard model architectures and inference methods, using the exported Dorado model during basecalling is recommended.
 
 .. code-block:: bash
 
   remora \
     infer from_pod5_and_bam \
     can_signal.pod5 \
     can_mappings.bam \
@@ -189,43 +215,47 @@
     mod_signal.pod5 \
     mod_mappings.bam \
     --model train_results/model_best.pt \
     --out-file mod_infer.bam \
     --log-filename mod_infer.log \
     --device 0
 
-Finally, Remora provides tools to validate these results.
-Ground truth `BED files <http://useast.ensembl.org/info/website/upload/bed.html>`_ reference positions where each read should be called as the modified or canonical base listed in the BED name field.
-Note in the test files where the control file has a ``C`` in the name field, while the modified BED file has ``m`` (single letter code for 5mC) in the name field.
-
-WARNING: There is a bug in pysam which causes all-context (e.g. ``--motif C 0``) modified model calls to produce invalid results with this command.
-This issue is reported `here <https://github.com/pysam-developers/pysam/issues/1123>`_.
-We are investigating solutions to bypass this issue including dropping this command.
+The ``remora validate from_modbams`` command is deprecated and will be removed in a future version of Remora.
+The ``modkit validate`` command is now recommended for this purpose.
 
-.. code-block:: bash
+Reference-anchored Inference
+****************************
 
-  remora \
-    validate from_modbams \
-    --bam-and-bed can_infer.bam can_ground_truth.bed \
-    --bam-and-bed mod_infer.bam mod_ground_truth.bed \
-    --explicit-mod-tag-used
+Reference-anchored inference allows users to make per-read per-site modified base calls against the reference sequence to which a read is mapped.
+This is in contrast to standard Remora model inference where calls are made against the basecalls.
+This mode can be useful to explore modified bases around which the canonical basecaller does not perform well.
+This inference mode is toggled by the ``--reference-anchored`` argument to the ``remora infer from_pod5_and_bam`` command.
+
+The output BAM file from this command will take each mapped read and replace the basecalls with the mapped reference bases.
+The move table will be transferred to the mapped reference bases and interpolated over mapping reference deletions in order to make enable extraction of Remora chunks for inference.
+
+Note that this means that the canonical basecalls will show 0 errors over the entire output BAM file.
+The intended purpose of this output is only to store the modified base status for each read at each applicable base.
+Any analysis of basecall metrics should not use the output of this command.
 
 Pre-trained Models
 ------------------
 
 See the selection of current released models with ``remora model list_pretrained``.
 Pre-trained models are stored remotely and can be downloaded using the ``remora model download`` command or will be downloaded on demand when needed.
 
 Models may be run from `Bonito <https://github.com/nanoporetech/bonito>`_.
 See Bonito documentation to apply Remora models.
 
 More advanced research models may be supplied via `Rerio <https://github.com/nanoporetech/rerio>`_.
 These files require download from Rerio and then the path to this download must be provided to Remora.
 Note that older ONNX format models require Remora version < 2.0.
 
+Downloaded or trained models can be inspected with the ``remora model inspect`` command to view the metadata attributes of the model.
+
 Python API and Raw Signal Analysis
 ----------------------------------
 
 Raw signal plotting is available via the ``remora analyze plot ref_region`` command.
 
 The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
 As an example using the test data, the following command produces the plots below.
@@ -258,14 +288,14 @@
 
 This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
 Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
 Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
 Research releases may be unstable and subject to rapid change by Oxford Nanopore Technologies.
 
-© 2021-2023 Oxford Nanopore Technologies Ltd.
+© 2021-2024 Oxford Nanopore Technologies Ltd.
 Remora is distributed under the terms of the Oxford Nanopore Technologies' Public Licence.
 
 Research Release
 ----------------
 
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
```

### Comparing `ont-remora-3.1.0/README.rst` & `ont_remora-3.2.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -61,15 +61,15 @@
    :alt: Neural network sequence encoding
 
 Data Preparation
 ----------------
 
 Remora data preparation begins from a POD5 file containing signal data and a BAM file containing basecalls from the POD5 file.
 Note that the BAM file must contain the move table (``--emit-moves`` in Dorado) and the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
-If using minimap2 for alignment use ``samtools fastq -T "*" [in.bam] | minimap2 -y -ax map-ont [ref.fa] - | samtools view -b -o [out.bam]`` in order to transfer the move table tags through the alignment step since minimap2 does not support SAM/BAM input.
+If using minimap2 for alignment use ``samtools fastq -T "*" [in.bam] | minimap2 -y -ax lr:hq [ref.fa] - | samtools view -b -o [out.bam]`` in order to transfer the move table tags through the alignment step since minimap2 does not support SAM/BAM input.
 
 The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the released 5mC CG-context models.
 Example reads can be found in the Remora repository (see ``test/data/`` directory).
 
 K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
 
 .. code-block:: bash
@@ -107,16 +107,20 @@
 The ``remora dataset make_config`` command creates these config files specifying the composition of the new dataset.
 When reading batches from these combined datasets, the default behavior will be to draw chunks randomly from the entire set of chunks.
 This setting is useful for multiple flowcells of the same condition.
 
 The ``--dataset-weights`` argument produces a config which generates batches with a fixed proportion of chunks from each input dataset.
 This setting is useful when combining different data types, for example control and modified datasets.
 
-In addition, the ``remora dataset merge`` command is supplied to merge datasets, copying the data into a new core Remora dataset.
-This may increase efficiency of data access for datasets composed of many core datasets, but only supports the default behavior from the ``make_config`` command.
+The ``remora dataset merge`` command is supplied to merge datasets, copying the data into a new core Remora dataset.
+This may increase efficiency of data access for datasets composed of many core datasets, but only supports the default behavior from the ``make_config`` command (sampling over all chunks).
+
+The ``remora dataset copy`` command is provided in order to move datasets to a new location.
+This can be useful when handling config datasets composed of many core datasets.
+Copying a dataset is especially useful to achieve higher training speeds when core datasets are stored on a network file system (NFS).
 
 Composed dataset config files can also be specified manually.
 Config files are JSON format files containing a single list, where each element is a list of two items.
 The first is the path to the dataset and the second is the weight (must be a positive value).
 The ``make_config`` output config file will also contain the dataset hash to ensure the contents of a dataset are unchanged, but this is an optional third field in the config.
 
 Metadata attributes from each core dataset are checked for compatibility and merged where applicable.
@@ -149,21 +153,21 @@
     train_dataset.jsn \
     --model remora/models/ConvLSTM_w_ref.py \
     --device 0 \
     --chunk-context 50 50 \
     --output-path train_results
 
 This command will produce a "best" model in torchscript format for use in Bonito, ``remora infer``, or ``remora validate`` commands.
-Models can be exported for use in Dorado with the ``remora model export train_results/model_best.pt`` command.
+Models can be exported for use in Dorado with the ``remora model export train_results/model_best.pt train_results_dorado_model`` command.
 
 Model Inference
 ---------------
 
 For testing purposes, inference within Remora is provided.
-For large scale using the exported Dorado model during basecalling is recommended.
+For standard model architectures and inference methods, using the exported Dorado model during basecalling is recommended.
 
 .. code-block:: bash
 
   remora \
     infer from_pod5_and_bam \
     can_signal.pod5 \
     can_mappings.bam \
@@ -176,43 +180,47 @@
     mod_signal.pod5 \
     mod_mappings.bam \
     --model train_results/model_best.pt \
     --out-file mod_infer.bam \
     --log-filename mod_infer.log \
     --device 0
 
-Finally, Remora provides tools to validate these results.
-Ground truth `BED files <http://useast.ensembl.org/info/website/upload/bed.html>`_ reference positions where each read should be called as the modified or canonical base listed in the BED name field.
-Note in the test files where the control file has a ``C`` in the name field, while the modified BED file has ``m`` (single letter code for 5mC) in the name field.
-
-WARNING: There is a bug in pysam which causes all-context (e.g. ``--motif C 0``) modified model calls to produce invalid results with this command.
-This issue is reported `here <https://github.com/pysam-developers/pysam/issues/1123>`_.
-We are investigating solutions to bypass this issue including dropping this command.
+The ``remora validate from_modbams`` command is deprecated and will be removed in a future version of Remora.
+The ``modkit validate`` command is now recommended for this purpose.
 
-.. code-block:: bash
+Reference-anchored Inference
+****************************
 
-  remora \
-    validate from_modbams \
-    --bam-and-bed can_infer.bam can_ground_truth.bed \
-    --bam-and-bed mod_infer.bam mod_ground_truth.bed \
-    --explicit-mod-tag-used
+Reference-anchored inference allows users to make per-read per-site modified base calls against the reference sequence to which a read is mapped.
+This is in contrast to standard Remora model inference where calls are made against the basecalls.
+This mode can be useful to explore modified bases around which the canonical basecaller does not perform well.
+This inference mode is toggled by the ``--reference-anchored`` argument to the ``remora infer from_pod5_and_bam`` command.
+
+The output BAM file from this command will take each mapped read and replace the basecalls with the mapped reference bases.
+The move table will be transferred to the mapped reference bases and interpolated over mapping reference deletions in order to make enable extraction of Remora chunks for inference.
+
+Note that this means that the canonical basecalls will show 0 errors over the entire output BAM file.
+The intended purpose of this output is only to store the modified base status for each read at each applicable base.
+Any analysis of basecall metrics should not use the output of this command.
 
 Pre-trained Models
 ------------------
 
 See the selection of current released models with ``remora model list_pretrained``.
 Pre-trained models are stored remotely and can be downloaded using the ``remora model download`` command or will be downloaded on demand when needed.
 
 Models may be run from `Bonito <https://github.com/nanoporetech/bonito>`_.
 See Bonito documentation to apply Remora models.
 
 More advanced research models may be supplied via `Rerio <https://github.com/nanoporetech/rerio>`_.
 These files require download from Rerio and then the path to this download must be provided to Remora.
 Note that older ONNX format models require Remora version < 2.0.
 
+Downloaded or trained models can be inspected with the ``remora model inspect`` command to view the metadata attributes of the model.
+
 Python API and Raw Signal Analysis
 ----------------------------------
 
 Raw signal plotting is available via the ``remora analyze plot ref_region`` command.
 
 The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
 As an example using the test data, the following command produces the plots below.
@@ -245,14 +253,14 @@
 
 This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
 Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
 Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
 Research releases may be unstable and subject to rapid change by Oxford Nanopore Technologies.
 
-© 2021-2023 Oxford Nanopore Technologies Ltd.
+© 2021-2024 Oxford Nanopore Technologies Ltd.
 Remora is distributed under the terms of the Oxford Nanopore Technologies' Public Licence.
 
 Research Release
 ----------------
 
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
```

### Comparing `ont-remora-3.1.0/setup.cfg` & `ont_remora-3.2.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 	scikit-learn
 	thop
 	pod5 >= 0.2.8
 	pysam >= 0.20.0
 	parasail
 	requests
 	polars
-	plotnine
+	plotnine == 0.12.4
 	importlib_resources
 
 [options.extras_require]
 tests = 
 	pytest
 	pytest-cov
 	black==22.8.0
 	flake8
 	sphinx
 	build
 	jupyter
-	patchworklib
+	patchworklib == 0.6.3
 	scipy
 
 [options.packages.find]
 where = 
 	src/
 	src/remora
 exclude =
```

### Comparing `ont-remora-3.1.0/setup.py` & `ont_remora-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/ont_remora.egg-info/PKG-INFO` & `ont_remora-3.2.0/src/ont_remora.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,41 @@
 Metadata-Version: 2.1
 Name: ont-remora
-Version: 3.1.0
+Version: 3.2.0
 Summary: Nanopore methylation/modified base calling detached from basecalling
 Home-page: https://github.com/nanoporetech/remora
 License: ont_public_licence
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8; variant=GFM
-Provides-Extra: tests
 License-File: LICENSE.txt
+Requires-Dist: tqdm
+Requires-Dist: toml
+Requires-Dist: torch
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
+Requires-Dist: thop
+Requires-Dist: pod5>=0.2.8
+Requires-Dist: pysam>=0.20.0
+Requires-Dist: parasail
+Requires-Dist: requests
+Requires-Dist: polars
+Requires-Dist: plotnine==0.12.4
+Requires-Dist: importlib_resources
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: black==22.8.0; extra == "tests"
+Requires-Dist: flake8; extra == "tests"
+Requires-Dist: sphinx; extra == "tests"
+Requires-Dist: build; extra == "tests"
+Requires-Dist: jupyter; extra == "tests"
+Requires-Dist: patchworklib==0.6.3; extra == "tests"
+Requires-Dist: scipy; extra == "tests"
 
 .. image:: /ONT_logo.png
   :width: 800
   :alt: [Oxford Nanopore Technologies]
   :target: https://nanoporetech.com/
 
 Remora
@@ -74,15 +96,15 @@
    :alt: Neural network sequence encoding
 
 Data Preparation
 ----------------
 
 Remora data preparation begins from a POD5 file containing signal data and a BAM file containing basecalls from the POD5 file.
 Note that the BAM file must contain the move table (``--emit-moves`` in Dorado) and the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
-If using minimap2 for alignment use ``samtools fastq -T "*" [in.bam] | minimap2 -y -ax map-ont [ref.fa] - | samtools view -b -o [out.bam]`` in order to transfer the move table tags through the alignment step since minimap2 does not support SAM/BAM input.
+If using minimap2 for alignment use ``samtools fastq -T "*" [in.bam] | minimap2 -y -ax lr:hq [ref.fa] - | samtools view -b -o [out.bam]`` in order to transfer the move table tags through the alignment step since minimap2 does not support SAM/BAM input.
 
 The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the released 5mC CG-context models.
 Example reads can be found in the Remora repository (see ``test/data/`` directory).
 
 K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
 
 .. code-block:: bash
@@ -120,16 +142,20 @@
 The ``remora dataset make_config`` command creates these config files specifying the composition of the new dataset.
 When reading batches from these combined datasets, the default behavior will be to draw chunks randomly from the entire set of chunks.
 This setting is useful for multiple flowcells of the same condition.
 
 The ``--dataset-weights`` argument produces a config which generates batches with a fixed proportion of chunks from each input dataset.
 This setting is useful when combining different data types, for example control and modified datasets.
 
-In addition, the ``remora dataset merge`` command is supplied to merge datasets, copying the data into a new core Remora dataset.
-This may increase efficiency of data access for datasets composed of many core datasets, but only supports the default behavior from the ``make_config`` command.
+The ``remora dataset merge`` command is supplied to merge datasets, copying the data into a new core Remora dataset.
+This may increase efficiency of data access for datasets composed of many core datasets, but only supports the default behavior from the ``make_config`` command (sampling over all chunks).
+
+The ``remora dataset copy`` command is provided in order to move datasets to a new location.
+This can be useful when handling config datasets composed of many core datasets.
+Copying a dataset is especially useful to achieve higher training speeds when core datasets are stored on a network file system (NFS).
 
 Composed dataset config files can also be specified manually.
 Config files are JSON format files containing a single list, where each element is a list of two items.
 The first is the path to the dataset and the second is the weight (must be a positive value).
 The ``make_config`` output config file will also contain the dataset hash to ensure the contents of a dataset are unchanged, but this is an optional third field in the config.
 
 Metadata attributes from each core dataset are checked for compatibility and merged where applicable.
@@ -162,21 +188,21 @@
     train_dataset.jsn \
     --model remora/models/ConvLSTM_w_ref.py \
     --device 0 \
     --chunk-context 50 50 \
     --output-path train_results
 
 This command will produce a "best" model in torchscript format for use in Bonito, ``remora infer``, or ``remora validate`` commands.
-Models can be exported for use in Dorado with the ``remora model export train_results/model_best.pt`` command.
+Models can be exported for use in Dorado with the ``remora model export train_results/model_best.pt train_results_dorado_model`` command.
 
 Model Inference
 ---------------
 
 For testing purposes, inference within Remora is provided.
-For large scale using the exported Dorado model during basecalling is recommended.
+For standard model architectures and inference methods, using the exported Dorado model during basecalling is recommended.
 
 .. code-block:: bash
 
   remora \
     infer from_pod5_and_bam \
     can_signal.pod5 \
     can_mappings.bam \
@@ -189,43 +215,47 @@
     mod_signal.pod5 \
     mod_mappings.bam \
     --model train_results/model_best.pt \
     --out-file mod_infer.bam \
     --log-filename mod_infer.log \
     --device 0
 
-Finally, Remora provides tools to validate these results.
-Ground truth `BED files <http://useast.ensembl.org/info/website/upload/bed.html>`_ reference positions where each read should be called as the modified or canonical base listed in the BED name field.
-Note in the test files where the control file has a ``C`` in the name field, while the modified BED file has ``m`` (single letter code for 5mC) in the name field.
-
-WARNING: There is a bug in pysam which causes all-context (e.g. ``--motif C 0``) modified model calls to produce invalid results with this command.
-This issue is reported `here <https://github.com/pysam-developers/pysam/issues/1123>`_.
-We are investigating solutions to bypass this issue including dropping this command.
+The ``remora validate from_modbams`` command is deprecated and will be removed in a future version of Remora.
+The ``modkit validate`` command is now recommended for this purpose.
 
-.. code-block:: bash
+Reference-anchored Inference
+****************************
 
-  remora \
-    validate from_modbams \
-    --bam-and-bed can_infer.bam can_ground_truth.bed \
-    --bam-and-bed mod_infer.bam mod_ground_truth.bed \
-    --explicit-mod-tag-used
+Reference-anchored inference allows users to make per-read per-site modified base calls against the reference sequence to which a read is mapped.
+This is in contrast to standard Remora model inference where calls are made against the basecalls.
+This mode can be useful to explore modified bases around which the canonical basecaller does not perform well.
+This inference mode is toggled by the ``--reference-anchored`` argument to the ``remora infer from_pod5_and_bam`` command.
+
+The output BAM file from this command will take each mapped read and replace the basecalls with the mapped reference bases.
+The move table will be transferred to the mapped reference bases and interpolated over mapping reference deletions in order to make enable extraction of Remora chunks for inference.
+
+Note that this means that the canonical basecalls will show 0 errors over the entire output BAM file.
+The intended purpose of this output is only to store the modified base status for each read at each applicable base.
+Any analysis of basecall metrics should not use the output of this command.
 
 Pre-trained Models
 ------------------
 
 See the selection of current released models with ``remora model list_pretrained``.
 Pre-trained models are stored remotely and can be downloaded using the ``remora model download`` command or will be downloaded on demand when needed.
 
 Models may be run from `Bonito <https://github.com/nanoporetech/bonito>`_.
 See Bonito documentation to apply Remora models.
 
 More advanced research models may be supplied via `Rerio <https://github.com/nanoporetech/rerio>`_.
 These files require download from Rerio and then the path to this download must be provided to Remora.
 Note that older ONNX format models require Remora version < 2.0.
 
+Downloaded or trained models can be inspected with the ``remora model inspect`` command to view the metadata attributes of the model.
+
 Python API and Raw Signal Analysis
 ----------------------------------
 
 Raw signal plotting is available via the ``remora analyze plot ref_region`` command.
 
 The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
 As an example using the test data, the following command produces the plots below.
@@ -258,14 +288,14 @@
 
 This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
 Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
 Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
 Research releases may be unstable and subject to rapid change by Oxford Nanopore Technologies.
 
-© 2021-2023 Oxford Nanopore Technologies Ltd.
+© 2021-2024 Oxford Nanopore Technologies Ltd.
 Remora is distributed under the terms of the Oxford Nanopore Technologies' Public Licence.
 
 Research Release
 ----------------
 
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
```

### Comparing `ont-remora-3.1.0/src/ont_remora.egg-info/SOURCES.txt` & `ont_remora-3.2.0/src/ont_remora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/data_chunks.py` & `ont_remora-3.2.0/src/remora/data_chunks.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,14 @@
             focus_bases=None
             if self.focus_bases is None
             else self.focus_bases.copy(),
         )
 
     def refine_signal_mapping(self, sig_map_refiner, check_read=False):
         if not sig_map_refiner.is_loaded:
-            LOGGER.debug("no signal map refiner loaded skipping..")
             return
         if sig_map_refiner.do_rough_rescale:
             prev_shift, prev_scale = self.shift, self.scale
             self.shift, self.scale = sig_map_refiner.rough_rescale(
                 self.shift,
                 self.scale,
                 self.seq_to_sig_map,
@@ -278,15 +277,14 @@
                 self.dacs,
             )
             self._sig = None
             self._sig_cumsum = None
             self._base_levels = None
         if sig_map_refiner.scale_iters >= 0:
             prev_shift, prev_scale = self.shift, self.scale
-            prev_seq_to_sig_map = self.seq_to_sig_map.copy()
             try:
                 (
                     self.seq_to_sig_map,
                     self.shift,
                     self.scale,
                 ) = sig_map_refiner.refine_sig_map(
                     self.shift,
@@ -298,20 +296,17 @@
             except IndexError as e:
                 LOGGER.debug(f"refine_error {self.read_id} {e}")
             # reset computed values after refinement
             self._sig = None
             self._dwells = None
             self._sig_cumsum = None
             self._base_levels = None
-            LOGGER.debug(f"refine_mapping_shift: {prev_shift} {self.shift}")
-            LOGGER.debug(f"refine_mapping_scale: {prev_scale} {self.scale}")
-            sig_map_diffs = self.seq_to_sig_map - prev_seq_to_sig_map
             LOGGER.debug(
-                f"refine_mapping_median_adjust: {np.median(sig_map_diffs)} "
-                f"{self.read_id}"
+                f"Refine mapping ::: shift: {prev_shift} -> {self.shift} "
+                f"scale: {prev_scale} -> {self.scale}"
             )
         if check_read:
             self.check()
 
     def set_motif_focus_bases(self, motifs):
         """
         Mutates self. Sets self.focus_bases to all hits within self.int_seq.
@@ -337,14 +332,15 @@
         self,
         focus_sig_idx,
         chunk_context,
         kmer_context_bases,
         label=-1,
         read_focus_base=-1,
         check_chunk=False,
+        signal_padding=False,
     ):
         chunk_len = sum(chunk_context)
         sig_start = focus_sig_idx - chunk_context[0]
         sig_end = focus_sig_idx + chunk_context[1]
         seq_to_sig_offset = 0
         if sig_start >= 0 and sig_end <= self.sig.size:
             # chunk boundaries are within read signal
@@ -356,17 +352,24 @@
             fill_en = chunk_len
             if sig_start < 0:
                 fill_st = -sig_start
                 # record offset value by which to shift seq_to_sig_map
                 seq_to_sig_offset = -sig_start
                 sig_start = 0
             if sig_end > self.sig.size:
-                fill_en = self.sig.size - sig_start
+                fill_en = self.sig.size - sig_start + seq_to_sig_offset
                 sig_end = self.sig.size
             chunk_sig[fill_st:fill_en] = self.sig[sig_start:sig_end]
+            if signal_padding:
+                chunk_sig[:fill_st] = self.sig[
+                    sig_start + fill_st : sig_start : -1
+                ]
+                chunk_sig[fill_en:] = self.sig[
+                    sig_end : sig_end - chunk_sig.size + fill_en - 1 : -1
+                ]
 
         seq_start = (
             np.searchsorted(self.seq_to_sig_map, sig_start, side="right") - 1
         )
         seq_end = np.searchsorted(self.seq_to_sig_map, sig_end, side="left")
 
         # extract/compute sequence to signal mapping for this chunk
@@ -670,15 +673,17 @@
             before and after the central position.
         base_start_justify (bool): Extract chunk centered on start of base
         offset (int): Extract chunk centered on base offset from base of
             interest
         kmer_context_bases (tuple): 2-tuple containing the bases to include in
             the encoded k-mer presented as input.
         reverse_signal (bool): Is nanopore signal 3' to 5' orientation?
-            Primarily for directRNA
+            Primarily for direct RNA
+        pa_scaling (tuple): Zero-centered picoamp scaling factors. These should
+            be extracted from a Dorado (v4.3+) basecalling model.
         sig_map_refiner (remora.refine_signal_map.SigMapRefiner): Signal
             mapping refiner
     """
 
     # dataset attributes
     allocate_size: int
     max_seq_len: int
@@ -697,15 +702,16 @@
     extra_arrays: dict = None
     # chunk extract
     chunk_context: tuple = constants.DEFAULT_CHUNK_CONTEXT
     base_start_justify: bool = False
     offset: int = 0
     kmer_context_bases: tuple = constants.DEFAULT_KMER_CONTEXT_BASES
     reverse_signal: bool = False
-    # signal refinement
+    # signal scaling/refinement
+    pa_scaling: tuple = None
     sig_map_refiner: SigMapRefiner = None
     rough_rescale_method: str = constants.DEFAULT_ROUGH_RESCALE_METHOD
 
     _stored_kmer_context_bases: tuple = None
     _stored_chunk_context: tuple = None
 
     @property
@@ -1447,15 +1453,19 @@
             ]
             arr_copy = array.copy()
             for b_idx, (b_st, b_en) in enumerate(b_ranges):
                 array[b_st : min(b_en, self.size)] = arr_copy[
                     shuf_indices[b_st:b_en]
                 ]
                 array.flush()
-                LOGGER.debug(f"{b_idx + 1}/{len(b_ranges)} batches complete")
+                if b_idx % 10 == 9:
+                    # update every 10 batches
+                    LOGGER.debug(
+                        f"{b_idx + 1}/{len(b_ranges)} batches complete"
+                    )
                 if show_prog:
                     b_pb.update()
             if show_prog:
                 b_pb.close()
                 arr_pb.update()
 
     def adjust_batch_params(self):
@@ -1829,14 +1839,15 @@
             f"           mod_long_names : {self.metadata.mod_long_names}\n"
             f"       kmer_context_bases : {self.metadata.kmer_context_bases}\n"
             f"            chunk_context : {self.metadata.chunk_context}\n"
             f"                   motifs : {self.metadata.motifs}\n"
             f"           reverse_signal : {self.metadata.reverse_signal}\n"
             f" chunk_extract_base_start : {self.metadata.base_start_justify}\n"
             f"     chunk_extract_offset : {self.metadata.offset}\n"
+            f"               pa_scaling : {self.metadata.pa_scaling}\n"
             f"          sig_map_refiner : {self.metadata.sig_map_refiner}\n"
         )
 
     @property
     def init_kwargs(self):
         return {
             "proportions": self.props,
@@ -1867,14 +1878,15 @@
         for ds in self.datasets[1:]:
             # first check attrs for which exact match is required
             for attr_name in (
                 "modified_base_labels",
                 "base_start_justify",
                 "offset",
                 "reverse_signal",
+                "pa_scaling",
                 "sig_map_refiner",
             ):
                 if getattr(ds.metadata, attr_name) != getattr(
                     self.metadata, attr_name
                 ):
                     raise RemoraError(
                         f"All datasets must have same {attr_name} "
@@ -1981,14 +1993,15 @@
         self.metadata.mod_long_names = mod_long_names
 
     def update_metadata(self, other):
         for md_key in (
             "modified_base_labels",
             "offset",
             "reverse_signal",
+            "pa_scaling",
             "sig_map_refiner",
         ):
             if getattr(self.metadata, md_key) != getattr(
                 other.metadata, md_key
             ):
                 raise RemoraError(
                     f"Cannot update metadata with mismatching '{md_key}'. "
```

### Comparing `ont-remora-3.1.0/src/remora/data_chunks_core.pyx` & `ont_remora-3.2.0/src/remora/data_chunks_core.pyx`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/download.py` & `ont_remora-3.2.0/src/remora/download.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/duplex_utils.py` & `ont_remora-3.2.0/src/remora/duplex_utils.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/encoded_kmers.pyx` & `ont_remora-3.2.0/src/remora/encoded_kmers.pyx`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/inference.py` & `ont_remora-3.2.0/src/remora/inference.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import sys
+import array
 import torch
 from copy import copy
 import array as pyarray
 from pathlib import Path
 from threading import Thread
 from itertools import chain, islice
 from collections import defaultdict
@@ -45,35 +47,41 @@
 
 
 ################
 # POD5+BAM CLI #
 ################
 
 
-def mods_tags_to_str(mods_tags):
+def mods_tags_to_str(mm_tags, ml_arr):
     # TODO these operations are often quite slow
     return [
-        f"MM:Z:{mods_tags[0]}",
-        f"ML:B:C,{','.join(map(str, mods_tags[1]))}",
+        f"MM:Z:{''.join(mm_tags)}",
+        f"ML:B:C,{','.join(map(str, ml_arr))}",
     ]
 
 
-def prepare_reads(read_errs, model_metadata, ref_anchored):
+def prepare_reads(read_errs, models_metadata, ref_anchored):
     out_read_errs = []
-    motif_seqs, motif_offsets = zip(*model_metadata["motifs"])
-    motifs = [Motif(*mot) for mot in model_metadata["motifs"]]
-    md_kwargs = {
-        "mod_bases": model_metadata["mod_bases"],
-        "mod_long_names": model_metadata["mod_long_names"],
-        "motif_sequences": motif_seqs,
-        "motif_offsets": motif_offsets,
-        "chunk_context": model_metadata["chunk_context"],
-        "kmer_context_bases": model_metadata["kmer_context_bases"],
-        "extra_arrays": {"read_focus_bases": ("int64", "")},
-    }
+
+    models_kwargs = []
+    motifs = {}
+    for md in models_metadata:
+        motif_seqs, motif_offsets = zip(*md["motifs"])
+        motifs[md["can_base"]] = [Motif(*mot) for mot in md["motifs"]]
+        models_kwargs.append(
+            {
+                "mod_bases": md["mod_bases"],
+                "mod_long_names": md["mod_long_names"],
+                "motif_sequences": motif_seqs,
+                "motif_offsets": motif_offsets,
+                "chunk_context": md["chunk_context"],
+                "kmer_context_bases": md["kmer_context_bases"],
+                "extra_arrays": {"read_focus_bases": ("int64", "")},
+            }
+        )
     for io_read, err in read_errs:
         if err is not None:
             io_read.prune(drop_move_tag=False)
             out_read_errs.append((io_read, None, err))
             continue
         try:
             remora_read = io_read.into_remora_read(ref_anchored)
@@ -85,43 +93,51 @@
         except Exception as e:
             io_read.prune(drop_move_tag=False)
             LOGGER.debug(f"{io_read.child_read_id} Unexpected error: {e}")
             out_read_errs.append((io_read, None, f"Unexpected error: {e}"))
             continue
         # after creating remora read strip IO read of large arrays
         io_read.prune(drop_move_tag=False)
-        remora_read.set_motif_focus_bases(motifs)
-        remora_read.refine_signal_mapping(model_metadata["sig_map_refiner"])
-        chunks = list(
-            remora_read.iter_chunks(
-                model_metadata["chunk_context"],
-                model_metadata["kmer_context_bases"],
-                model_metadata["base_start_justify"],
-                model_metadata["offset"],
+        datasets = {}
+        for md, md_kwargs in zip(models_metadata, models_kwargs):
+            mdl_remora_read = remora_read.copy()
+            mdl_remora_read.set_motif_focus_bases(motifs[md["can_base"]])
+            mdl_remora_read.refine_signal_mapping(md["sig_map_refiner"])
+            chunks = list(
+                mdl_remora_read.iter_chunks(
+                    md["chunk_context"],
+                    md["kmer_context_bases"],
+                    md["base_start_justify"],
+                    md["offset"],
+                )
             )
-        )
-        if len(chunks) == 0:
-            LOGGER.debug(f"{io_read.child_read_id} No mod calls")
-            out_read_errs.append((io_read, None, "No mod calls"))
-            continue
-        # prepare in memory dataset to perform chunk extraction
-        num_chunks = len(chunks)
-        md_kwargs["allocate_size"] = num_chunks
-        md_kwargs["max_seq_len"] = max(c.seq_len for c in chunks)
-        # open in-memory dataset
-        dataset = CoreRemoraDataset(
-            mode="w",
-            metadata=DatasetMetadata(**md_kwargs),
-            batch_size=num_chunks,
-            super_batch_size=num_chunks,
-            infinite_iter=False,
-        )
-        for chunk in chunks:
-            dataset.write_chunk(chunk)
-        out_read_errs.append((io_read, dataset, None))
+            if len(chunks) == 0:
+                LOGGER.debug(
+                    f"{io_read.child_read_id} No {md['can_base']} mod calls"
+                )
+                out_read_errs.append(
+                    (io_read, None, f"No {md['can_base']} mod calls")
+                )
+                continue
+            # prepare in memory dataset to perform chunk extraction
+            num_chunks = len(chunks)
+            md_kwargs["allocate_size"] = num_chunks
+            md_kwargs["max_seq_len"] = max(c.seq_len for c in chunks)
+            # open in-memory dataset
+            dataset = CoreRemoraDataset(
+                mode="w",
+                metadata=DatasetMetadata(**md_kwargs),
+                batch_size=num_chunks,
+                super_batch_size=num_chunks,
+                infinite_iter=False,
+            )
+            for chunk in chunks:
+                dataset.write_chunk(chunk)
+            datasets[md["can_base"]] = dataset
+        out_read_errs.append((io_read, datasets, None))
     return out_read_errs
 
 
 if _PROF_PREP_FN:
     _prepare_reads_wrapper = prepare_reads
 
     def prepare_reads(*args, **kwargs):
@@ -135,89 +151,118 @@
 
 def prep_nn_input(read_errs):
     # TODO for basecall-anchored calls only call on first read and apply to
     # other mappings
     if len(read_errs) == 0:
         return [(None, None, "No valid mappings")]
     read_nn_inputs = []
-    for io_read, read_dataset, err in read_errs:
+    for io_read, read_datasets, err in read_errs:
         if err is not None:
             read_nn_inputs.append((io_read, None, err))
             continue
-        r_chunks = next(iter(read_dataset))
-        del r_chunks["labels"]
-        read_nn_inputs.append((io_read, r_chunks, None))
+        bases_chunks = {}
+        for can_base, ds in read_datasets.items():
+            base_chunks = next(iter(ds))
+            del base_chunks["labels"]
+            bases_chunks[can_base] = base_chunks
+        read_nn_inputs.append((io_read, bases_chunks, None))
     return read_nn_inputs
 
 
-def batch_reads(prepped_nn_inputs, batches_q, batch_size, model_metadata):
-    def new_arrays():
+def batch_reads(prepped_nn_inputs, batches_q, batch_size, models_metadata):
+    md_dict = dict((md["can_base"], md) for md in models_metadata)
+    can_bases = list(md_dict)
+
+    def new_arrays(can_base):
         return (
             np.empty(
-                (batch_size, 1, model_metadata["chunk_len"]),
+                (batch_size, 1, md_dict[can_base]["chunk_len"]),
                 dtype=np.float32,
             ),
             np.empty(
                 (
                     batch_size,
-                    model_metadata["kmer_len"] * 4,
-                    model_metadata["chunk_len"],
+                    md_dict[can_base]["kmer_len"] * 4,
+                    md_dict[can_base]["chunk_len"],
                 ),
                 dtype=np.float32,
             ),
             np.empty(batch_size, dtype=int),
         )
 
-    b_sigs, b_enc_kmers, b_read_pos = new_arrays()
+    arrs = dict((cb, new_arrays(cb)) for cb in can_bases)
     # position within current batch
-    b_pos = 0
-    b_reads = []
+    b_poss = dict((cb, 0) for cb in can_bases)
+    b_readss = dict((cb, []) for cb in can_bases)
     for read_nn_inputs in prepped_nn_inputs:
-        for io_read, r_chunks, err in read_nn_inputs:
+        for io_read, bases_chunks, err in read_nn_inputs:
             if err is not None:
-                b_reads.append([io_read, None, None, err])
+                for can_base in can_bases:
+                    b_readss[can_base].append([io_read, None, None, err])
                 continue
-            num_chunks = r_chunks["read_focus_bases"].size
-            # fill out and yield full batches
-            rb_consumed = 0
-            # while this read extends through a whole batch continue to
-            # supply batches from this read
-            while b_pos + num_chunks - rb_consumed >= batch_size:
-                rb_en = rb_consumed + batch_size - b_pos
-                b_sigs[b_pos:] = r_chunks["signal"][rb_consumed:rb_en]
-                b_enc_kmers[b_pos:] = r_chunks["enc_kmers"][rb_consumed:rb_en]
-                b_read_pos[b_pos:] = r_chunks["read_focus_bases"][
-                    rb_consumed:rb_en
+            for can_base, r_chunks in bases_chunks.items():
+                num_chunks = r_chunks["read_focus_bases"].size
+                # fill out and yield full batches
+                rb_consumed = 0
+                # while this read extends through a whole batch continue to
+                # supply batches from this read
+                while b_poss[can_base] + num_chunks - rb_consumed >= batch_size:
+                    rb_en = rb_consumed + batch_size - b_poss[can_base]
+                    arrs[can_base][0][b_poss[can_base] :] = r_chunks["signal"][
+                        rb_consumed:rb_en
+                    ]
+                    arrs[can_base][1][b_poss[can_base] :] = r_chunks[
+                        "enc_kmers"
+                    ][rb_consumed:rb_en]
+                    arrs[can_base][2][b_poss[can_base] :] = r_chunks[
+                        "read_focus_bases"
+                    ][rb_consumed:rb_en]
+                    # batch start is None once the first batch is complete
+                    # from this read
+                    b_st = b_poss[can_base] if rb_consumed == 0 else None
+                    b_readss[can_base].append([io_read, b_st, None, None])
+                    _put_item(
+                        (can_base, *arrs[can_base], b_readss[can_base]),
+                        batches_q,
+                    )
+                    rb_consumed += batch_size - b_poss[can_base]
+                    # new batch
+                    arrs[can_base] = new_arrays(can_base)
+                    b_poss[can_base] = 0
+                    b_readss[can_base] = []
+                # add rest of read to unfinished batch
+                b_en = b_poss[can_base] + num_chunks - rb_consumed
+                arrs[can_base][0][b_poss[can_base] : b_en] = r_chunks["signal"][
+                    rb_consumed:
                 ]
-                # batch start is None once the first batch is complete
-                # from this read
-                b_st = b_pos if rb_consumed == 0 else None
-                b_reads.append([io_read, b_st, None, None])
-                _put_item((b_sigs, b_enc_kmers, b_read_pos, b_reads), batches_q)
-                rb_consumed += batch_size - b_pos
-                # new batch
-                b_sigs, b_enc_kmers, b_read_pos = new_arrays()
-                b_pos = 0
-                b_reads = []
-            # add rest of read to unfinished batch
-            b_en = b_pos + num_chunks - rb_consumed
-            b_sigs[b_pos:b_en] = r_chunks["signal"][rb_consumed:]
-            b_enc_kmers[b_pos:b_en] = r_chunks["enc_kmers"][rb_consumed:]
-            b_read_pos[b_pos:b_en] = r_chunks["read_focus_bases"][rb_consumed:]
-            # if read continues from last batch set start to None
-            b_st = b_pos if rb_consumed == 0 else None
-            b_reads.append([io_read, b_st, b_en, None])
-            # set current batch position for next read
-            b_pos = b_en
-    if b_pos > 0:
-        # send last batch
-        _put_item(
-            (b_sigs[:b_pos], b_enc_kmers[:b_pos], b_read_pos[:b_pos], b_reads),
-            batches_q,
-        )
+                arrs[can_base][1][b_poss[can_base] : b_en] = r_chunks[
+                    "enc_kmers"
+                ][rb_consumed:]
+                arrs[can_base][2][b_poss[can_base] : b_en] = r_chunks[
+                    "read_focus_bases"
+                ][rb_consumed:]
+                # if read continues from last batch set start to None
+                b_st = b_poss[can_base] if rb_consumed == 0 else None
+                b_readss[can_base].append([io_read, b_st, b_en, None])
+                # set current batch position for next read
+                b_poss[can_base] = b_en
+    for can_base in can_bases:
+        if b_poss[can_base] > 0:
+            b_sigs, b_enc_kmers, b_read_pos = arrs[can_base]
+            # send last batch
+            _put_item(
+                (
+                    can_base,
+                    b_sigs[: b_poss[can_base]],
+                    b_enc_kmers[: b_poss[can_base]],
+                    b_read_pos[: b_poss[can_base]],
+                    b_readss[can_base],
+                ),
+                batches_q,
+            )
     _put_item(StopIteration, batches_q)
 
 
 if _PROF_BATCH_FN:
     _batch_reads_wrapper = batch_reads
 
     def batch_reads(*args, **kwargs):
@@ -226,41 +271,52 @@
         prof = cProfile.Profile()
         retval = prof.runcall(_batch_reads_wrapper, *args, **kwargs)
         prof.dump_stats(_PROF_BATCH_FN)
         return retval
 
 
 def run_model_batched(
-    batches_q, called_batches_q, model, model_metadata, batch_size
+    batches_q, called_batches_q, models, models_metadata, batch_size
 ):
-    device = next(model.parameters()).device
-    pin_memory = device.type == "cuda"
-    t_b_sigs = torch.empty(
-        (batch_size, 1, model_metadata["chunk_len"]),
-        dtype=torch.float32,
-        pin_memory=pin_memory,
-    )
-    t_b_enc_kmers = torch.empty(
-        (
-            batch_size,
-            model_metadata["kmer_len"] * 4,
-            model_metadata["chunk_len"],
-        ),
-        dtype=torch.float32,
-        pin_memory=pin_memory,
-    )
-    for b_sigs, b_enc_kmers, b_read_pos, b_reads in _queue_iter(batches_q):
+    md_dict = dict((md["can_base"], md) for md in models_metadata)
+    can_bases = list(md_dict)
+    devices = dict()
+    sig_arrs = dict()
+    enc_kmer_arrs = dict()
+    for can_base in can_bases:
+        devices[can_base] = next(models[can_base].parameters()).device
+        pin_memory = devices[can_base].type == "cuda"
+        sig_arrs[can_base] = torch.empty(
+            (batch_size, 1, md_dict[can_base]["chunk_len"]),
+            dtype=torch.float32,
+            pin_memory=pin_memory,
+        )
+        enc_kmer_arrs[can_base] = torch.empty(
+            (
+                batch_size,
+                md_dict[can_base]["kmer_len"] * 4,
+                md_dict[can_base]["chunk_len"],
+            ),
+            dtype=torch.float32,
+            pin_memory=pin_memory,
+        )
+    for can_base, b_sigs, b_enc_kmers, b_read_pos, b_reads in _queue_iter(
+        batches_q
+    ):
         if b_read_pos.size == batch_size:
-            t_b_sigs[:] = torch.from_numpy(b_sigs)
-            t_b_enc_kmers[:] = torch.from_numpy(b_enc_kmers)
+            sig_arrs[can_base][:] = torch.from_numpy(b_sigs)
+            enc_kmer_arrs[can_base][:] = torch.from_numpy(b_enc_kmers)
         else:
-            t_b_sigs = torch.from_numpy(b_sigs)
-            t_b_enc_kmers = torch.from_numpy(b_enc_kmers)
-        nn_out = model(t_b_sigs.to(device), t_b_enc_kmers.to(device))
-        _put_item((nn_out, b_read_pos, b_reads), called_batches_q)
+            sig_arrs[can_base] = torch.from_numpy(b_sigs)
+            enc_kmer_arrs[can_base] = torch.from_numpy(b_enc_kmers)
+        nn_out = models[can_base](
+            sig_arrs[can_base].to(devices[can_base]),
+            enc_kmer_arrs[can_base].to(devices[can_base]),
+        )
+        _put_item((can_base, nn_out, b_read_pos, b_reads), called_batches_q)
     _put_item(StopIteration, called_batches_q)
 
 
 if _PROF_MODEL_FN:
     _run_model_wrapper = run_model_batched
 
     def run_model_batched(*args, **kwargs):
@@ -307,24 +363,58 @@
                 b_nn_out[b_st:b_en],
                 b_read_pos[b_st:b_en],
                 None,
             )
     return comp_reads, curr_read
 
 
-def unbatch(called_batches_q, called_reads_q):
-    curr_read = None
-    for nn_out, b_read_pos, b_reads in _queue_iter(called_batches_q):
-        comp_reads, curr_read = unbatch_reads(
-            curr_read, nn_out.cpu().numpy(), b_read_pos, b_reads
-        )
-        for read in comp_reads:
-            _put_item(read, called_reads_q)
-    if curr_read is not None:
-        _put_item(curr_read, called_reads_q)
+def unbatch(called_batches_q, called_reads_q, models_metadata):
+    def get_return_read(reads):
+        mod_calls = []
+        r_errs = set()
+        for can_base, (io_read, nn_out, r_pos, err) in reads:
+            r_errs.add(err)
+            if err is None:
+                mod_calls.append((can_base, nn_out, r_pos))
+        if any(err is None for err in r_errs):
+            r_err = None
+        else:
+            r_err = ",".join(sorted(r_errs))
+        return io_read, mod_calls, r_err
+
+    can_bases = [md["can_base"] for md in models_metadata]
+    num_can_bases = len(can_bases)
+    curr_reads = dict((can_base, None) for can_base in can_bases)
+    comp_reads = defaultdict(list)
+    for can_base, nn_out, b_read_pos, b_reads in _queue_iter(called_batches_q):
+        cb_comp_reads, cb_curr_read = unbatch_reads(
+            curr_reads[can_base], nn_out.cpu().numpy(), b_read_pos, b_reads
+        )
+        curr_reads[can_base] = cb_curr_read
+        for comp_read in cb_comp_reads:
+            comp_reads[comp_read[0].read_id].append((can_base, comp_read))
+
+        # add reads which have completed through all canonical base model
+        full_comp_read_ids = [
+            rid
+            for rid, r_comp_reads in comp_reads.items()
+            if len(r_comp_reads) == num_can_bases
+        ]
+        for rid in full_comp_read_ids:
+            _put_item(
+                get_return_read(comp_reads[rid]),
+                called_reads_q,
+            )
+            # delete read from completed reads dict
+            del comp_reads[rid]
+    if curr_reads[can_bases[0]] is not None:
+        _put_item(
+            get_return_read([(cb, curr_reads[cb]) for cb in can_bases]),
+            called_reads_q,
+        )
     _put_item(StopIteration, called_reads_q)
 
 
 if _PROF_UNBATCH_FN:
     _unbatch_wrapper = unbatch
 
     def unbatch(*args, **kwargs):
@@ -332,88 +422,101 @@
 
         prof = cProfile.Profile()
         retval = prof.runcall(_unbatch_wrapper, *args, **kwargs)
         prof.dump_stats(_PROF_UNBATCH_FN)
         return retval
 
 
-def post_process_reads(read_mapping, model_metadata, ref_anchored):
-    io_read, nn_out, r_poss, err = read_mapping
+def post_process_reads(read_mapping, models_metadata, ref_anchored):
+    io_read, mod_calls, err = read_mapping
     if err is not None:
         return io_read, err
-    r_probs = softmax_axis1(nn_out)[:, 1:].astype(np.float64)
-    seq = io_read.ref_seq if ref_anchored else io_read.seq
-    mod_tags = mods_tags_to_str(
-        format_mm_ml_tags(
+
+    md_dict = dict((md["can_base"], md) for md in models_metadata)
+    mm_tags = []
+    ml_arr = array.array("B")
+    for can_base, nn_out, r_poss in mod_calls:
+        r_probs = softmax_axis1(nn_out)[:, 1:].astype(np.float64)
+        seq = io_read.ref_seq if ref_anchored else io_read.seq
+        cb_mm, cb_ml = format_mm_ml_tags(
             seq=seq,
             poss=r_poss,
             probs=r_probs,
-            mod_bases=model_metadata["mod_bases"],
-            can_base=model_metadata["can_base"],
+            mod_bases=md_dict[can_base]["mod_bases"],
+            can_base=can_base,
         )
-    )
-    io_read.full_align["tags"].extend(mod_tags)
+        mm_tags.append(cb_mm)
+        ml_arr.extend(cb_ml)
+
+    io_read.full_align["tags"].extend(mods_tags_to_str(mm_tags, ml_arr))
     if ref_anchored:
         io_read.full_align["cigar"] = f"{len(io_read.ref_seq)}M"
         io_read.full_align["seq"] = (
             io_read.ref_seq
             if io_read.ref_reg.strand == "+"
             else revcomp(io_read.ref_seq)
         )
         io_read.full_align["qual"] = "*"
     return io_read, None
 
 
 def infer_from_pod5_and_bam(
     pod5_path,
     in_bam_path,
-    model,
-    model_metadata,
+    models,
     out_bam_path,
     num_reads=None,
     queue_max=1_000,
     num_extract_alignment_workers=1,
     num_prep_read_workers=1,
     num_prep_nn_input_workers=1,
     num_post_process_workers=1,
     batch_size=constants.DEFAULT_BATCH_SIZE,
     skip_non_primary=True,
     ref_anchored=False,
 ):
     bam_idx = ReadIndexedBam(in_bam_path, skip_non_primary, req_tags={"mv"})
+    if bam_idx.num_records == 0:
+        LOGGER.info("No records found in BAM file.")
+        sys.exit()
     with DatasetReader(Path(pod5_path)) as pod5_dr:
         read_ids, num_reads = get_read_ids(bam_idx, pod5_dr, num_reads)
+    models_metadata = list(zip(*models))[1]
+    models = dict((md["can_base"], mdl) for mdl, md in models)
+    reverse_signal = models_metadata[0]["reverse_signal"]
+    pa_scaling = models_metadata[0]["pa_scaling"]
 
     signals = BackgroundIter(
         iter_signal,
         args=(pod5_path,),
         kwargs={
             "num_reads": num_reads,
             "read_ids": read_ids,
-            "rev_sig": model_metadata["reverse_signal"],
+            "rev_sig": reverse_signal,
+            "pa_scaling": pa_scaling,
         },
         name="ExtractSignal",
         use_process=True,
         q_maxsize=queue_max,
     )
     reads = MultitaskMap(
         extract_alignments,
         signals,
         num_workers=num_extract_alignment_workers,
-        args=(bam_idx, model_metadata["reverse_signal"]),
+        args=(bam_idx, reverse_signal),
         name="AddAlignments",
         use_process=True,
         use_mp_queue=True,
         q_maxsize=queue_max,
     )
     prepped_reads = MultitaskMap(
         prepare_reads,
         reads,
         num_workers=num_prep_read_workers,
-        args=(model_metadata, ref_anchored),
+        args=(models_metadata, ref_anchored),
         name="PrepReadData",
         use_process=True,
         use_mp_queue=True,
         q_maxsize=100,
     )
     prepped_nn_input = MultitaskMap(
         prep_nn_input,
@@ -427,44 +530,45 @@
     batches_q = NamedQueue(maxsize=4, name="Batches")
     batch_reads_p = Thread(
         target=batch_reads,
         args=(
             _queue_iter(prepped_nn_input.out_q, num_prep_nn_input_workers),
             batches_q,
             batch_size,
-            model_metadata,
+            models_metadata,
         ),
         name="batch_reads",
         daemon=True,
     )
     batch_reads_p.start()
     called_batches_q = NamedQueue(maxsize=4, name="CalledBatches")
     call_batches_t = Thread(
         target=run_model_batched,
-        args=(batches_q, called_batches_q, model, model_metadata, batch_size),
+        args=(batches_q, called_batches_q, models, models_metadata, batch_size),
         name="call_batches",
         daemon=True,
     )
     call_batches_t.start()
     called_reads_q = NamedMPQueue(maxsize=queue_max, name="Unbatch")
     unbatch_p = Thread(
         target=unbatch,
         args=(
             called_batches_q,
             called_reads_q,
+            models_metadata,
         ),
         name="unbatch",
         daemon=True,
     )
     unbatch_p.start()
     final_reads = MultitaskMap(
         post_process_reads,
         _queue_iter(called_reads_q),
         num_workers=num_post_process_workers,
-        args=(model_metadata, ref_anchored),
+        args=(models_metadata, ref_anchored),
         name="PostProcess",
         use_process=False,
         use_mp_queue=False,
         q_maxsize=queue_max,
     )
 
     all_qs = [
@@ -474,21 +578,21 @@
         prepped_nn_input.out_q,
         batches_q,
         called_batches_q,
         called_reads_q,
         final_reads.out_q,
     ]
     errs = defaultdict(int)
-    if bam_idx.num_non_primary > 0:
-        errs["Non-primary alignment skipped"] = bam_idx.num_non_primary
+    for err, cnt in bam_idx.skip_reasons.items():
+        errs[err] = cnt
     pysam_save = pysam.set_verbosity(0)
     sig_called = 0
     in_bam = out_bam = pbar = prev_rid = None
     try:
-        in_bam = pysam.AlignmentFile(in_bam_path, "rb")
+        in_bam = pysam.AlignmentFile(in_bam_path, "rb", check_sq=False)
         out_bam = pysam.AlignmentFile(out_bam_path, "wb", template=in_bam)
         pbar = tqdm(
             smoothing=0,
             total=num_reads,
             dynamic_ncols=True,
             unit=" Reads",
             desc="Inferring mods",
@@ -806,18 +910,24 @@
     LOGGER.info("Indexing Duplex BAM")
     duplex_bam_index = ReadIndexedBam(
         duplex_bam_path,
         skip_non_primary=skip_non_primary,
         req_tags=set(),
         read_id_converter=lambda k: k.split(duplex_deliminator)[0],
     )
+    if duplex_bam_index.num_records == 0:
+        LOGGER.info("No records found in duplex BAM file.")
+        sys.exit()
     LOGGER.info("Indexing Simplex BAM")
     simplex_bam_index = ReadIndexedBam(
         simplex_bam_path, skip_non_primary=True, req_tags={"mv"}
     )
+    if simplex_bam_index.num_records == 0:
+        LOGGER.info("No records found in simplex BAM file.")
+        sys.exit()
     with open(pairs_path, "r") as fh:
         pairs = [tuple(line.split()) for line in fh]
     valid_pairs, num_valid_reads = check_simplex_alignments(
         simplex_index=simplex_bam_index,
         duplex_index=duplex_bam_index,
         pairs=pairs,
     )
```

### Comparing `ont-remora-3.1.0/src/remora/io.py` & `ont_remora-3.2.0/src/remora/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,14 +198,16 @@
             (e.g. for concatenated duplex read ids).
     """
 
     bam_path: str
     skip_non_primary: bool = True
     req_tags: set = None
     read_id_converter: Callable = None
+    parent_read_id_subset: set = None
+    child_read_id_subset: set = None
 
     @property
     def reference_filename(self):
         """Alias to mimic AlignmentFile attribute"""
         return self.bam_path
 
     @property
@@ -258,35 +260,46 @@
         pbar = tqdm(
             smoothing=0,
             unit=" Reads",
             desc="Indexing BAM by parent read id",
             disable=os.environ.get("LOG_SAFE", False),
         )
         self.num_records = 0
-        self.num_non_primary = 0
+        self.skip_reasons = defaultdict(int)
         # iterating over file handle gives incorrect pointers
         while True:
             read_ptr = self.bam_fh.tell()
             try:
                 read = next(self.bam_fh)
             except StopIteration:
                 break
             pbar.update()
+            if (
+                self.child_read_id_subset is not None
+                and read.query_name not in self.child_read_id_subset
+            ):
+                self.skip_reasons["Child read ID filtered"] += 1
+                continue
             index_read_id = get_parent_id(read)
+            if (
+                self.parent_read_id_subset is not None
+                and index_read_id not in self.parent_read_id_subset
+            ):
+                self.skip_reasons["Parent read ID filtered"] += 1
+                continue
             if self.read_id_converter is not None:
                 index_read_id = self.read_id_converter(index_read_id)
             if self.req_tags is not None:
                 tags = set(tg[0] for tg in read.tags)
                 missing_tags = self.req_tags.difference(tags)
                 if len(missing_tags) > 0:
-                    LOGGER.debug(f"{index_read_id} missing tags {missing_tags}")
+                    self.skip_reasons["Missing BAM tags"] += 1
                     continue
             if self.skip_non_primary and not read_is_primary(read):
-                LOGGER.debug(f"{read.query_name} not primary")
-                self.num_non_primary += 1
+                self.skip_reasons["Non-primary alignment"] += 1
                 continue
             self.num_records += 1
             self._bam_idx[index_read_id].append(read_ptr)
         # close bam if it was closed at start of function call
         if bam_was_closed:
             self.close()
         pbar.close()
@@ -384,24 +397,16 @@
     stride = mv_tag[0]
     mv_table = np.array(mv_tag[1:])
     query_to_signal = np.nonzero(mv_table)[0] * stride
     query_to_signal = np.concatenate([query_to_signal, [sig_len]])
     if reverse_signal:
         query_to_signal = sig_len - query_to_signal[::-1]
     if check and seq_len is not None and query_to_signal.size - 1 != seq_len:
-        LOGGER.debug(
-            f"Move table (num moves: {query_to_signal.size - 1}) discordant "
-            f"with basecalls (seq len: {seq_len})"
-        )
         raise RemoraError("Move table discordant with basecalls")
     if check and mv_table.size != sig_len // stride:
-        LOGGER.debug(
-            f"Move table (len: {mv_table.size}) discordant with "
-            f"signal (sig len // stride: {sig_len // stride})"
-        )
         raise RemoraError("Move table discordant with signal")
     return query_to_signal, mv_table, stride
 
 
 #######################
 # POD5/BAM Extraction #
 #######################
@@ -429,37 +434,45 @@
                 )
                 return
 
             yield read
     LOGGER.debug("Completed pod5 signal worker")
 
 
-def iter_signal(pod5_path, num_reads=None, read_ids=None, rev_sig=False):
+def iter_signal(
+    pod5_path, num_reads=None, read_ids=None, rev_sig=False, pa_scaling=None
+):
     """Iterate io Read objects loaded from Pod5
 
     Args:
         pod5_path (str): Path to POD5 file
         num_reads (int): Maximum number of reads to iterate
         read_ids (iterable): Read IDs to extract
         rev_sig (bool): Should signal be reversed on reading
+        pa_scaling (tuple): picoamp to zero-centered picoamp shift and scale
 
     Yields:
         2-tuple:
             1. remora.io.Read object
             2. Error text or None if no errors
     """
+    pa_kwargs = {}
+    if pa_scaling is not None:
+        pa_kwargs["shift_pa_to_zc_pa"] = pa_scaling[0]
+        pa_kwargs["scale_pa_to_zc_pa"] = pa_scaling[1]
     for pod5_read in iter_pod5_reads(
         pod5_path=pod5_path, num_reads=num_reads, read_ids=read_ids
     ):
         dacs = pod5_read.signal[::-1] if rev_sig else pod5_read.signal
         read = Read(
             read_id=str(pod5_read.read_id),
             dacs=dacs,
             shift_dacs_to_pa=pod5_read.calibration.offset,
             scale_dacs_to_pa=pod5_read.calibration.scale,
+            **pa_kwargs,
         )
         yield read, None
     LOGGER.debug("Completed signal worker")
 
 
 if _SIG_PROF_FN:
     _iter_signal_wrapper = iter_signal
@@ -469,24 +482,26 @@
 
         sig_prof = cProfile.Profile()
         retval = sig_prof.runcall(_iter_signal_wrapper, *args, **kwargs)
         sig_prof.dump_stats(_SIG_PROF_FN)
         return retval
 
 
-def extract_alignments(read_err, bam_idx, rev_sig=False):
+def extract_alignments(read_err, bam_idx, rev_sig=False, pa_scaling=None):
     io_read, err = read_err
     if io_read is None:
         return [read_err]
     read_alignments = []
     try:
         for bam_read in bam_idx.get_alignments(io_read.read_id):
             align_read = io_read.copy()
             try:
-                align_read.add_alignment(bam_read, reverse_signal=rev_sig)
+                align_read.add_alignment(
+                    bam_read, reverse_signal=rev_sig, pa_scaling=pa_scaling
+                )
                 read_alignments.append((align_read, None))
             except RemoraError as e:
                 LOGGER.debug(f"{io_read.read_id} Extract alignment error: {e}")
                 read_alignments.append((align_read, str(e)))
     except RemoraError as e:
         LOGGER.debug(f"{io_read.read_id} Extract alignment error: {e}")
         return [(io_read, str(e))]
@@ -703,64 +718,78 @@
         ref_orient (bool): Should returned sequence and levels be reference
             oriented? This only effects the output for reverse strand ref_reg.
             Reference orientation will return the reference sequence and levels
             in the forward reference direction. Read orient (ref_orient=False)
             will return sequence and levels in 5' to 3' read direction on the
             reverse strand.
     """
-    # extract read oriented context seq
-    context_int_seq = get_ref_int_seq_from_reads(
-        ref_reg.adjust(
-            -sig_map_refiner.bases_before,
-            sig_map_refiner.bases_after,
+    if sig_map_refiner is None:
+        levels = None
+        context_int_seq = get_ref_int_seq_from_reads(
+            ref_reg,
+            bam_reads,
             ref_orient=False,
-        ),
-        bam_reads,
-        ref_orient=False,
-    )
-    # levels are read oriented
-    levels = sig_map_refiner.extract_levels(context_int_seq)
-    # convert sequence positions not in reads to nan and seq to N
-    levels[np.equal(context_int_seq, -2)] = np.NAN
-    context_int_seq[np.equal(context_int_seq, -2)] = -1
-    seq = util.int_to_seq(context_int_seq)
-    # trim seq and levels
-    seq = seq[
-        sig_map_refiner.bases_before : sig_map_refiner.bases_before
-        + ref_reg.len
-    ]
-    levels = levels[
-        sig_map_refiner.bases_before : sig_map_refiner.bases_before
-        + ref_reg.len
-    ]
+        )
+        context_int_seq[np.equal(context_int_seq, -2)] = -1
+        seq = util.int_to_seq(context_int_seq)
+    else:
+        # extract read oriented context seq
+        context_int_seq = get_ref_int_seq_from_reads(
+            ref_reg.adjust(
+                -sig_map_refiner.bases_before,
+                sig_map_refiner.bases_after,
+                ref_orient=False,
+            ),
+            bam_reads,
+            ref_orient=False,
+        )
+        # levels are read oriented
+        levels = sig_map_refiner.extract_levels(context_int_seq)
+        # convert sequence positions not in reads to nan and seq to N
+        levels[np.equal(context_int_seq, -2)] = np.NAN
+        context_int_seq[np.equal(context_int_seq, -2)] = -1
+        seq = util.int_to_seq(context_int_seq)
+        # trim seq and levels
+        seq = seq[
+            sig_map_refiner.bases_before : sig_map_refiner.bases_before
+            + ref_reg.len
+        ]
+        levels = levels[
+            sig_map_refiner.bases_before : sig_map_refiner.bases_before
+            + ref_reg.len
+        ]
 
     if ref_reg.strand == "-" and ref_orient:
         seq = seq[::-1]
-        levels = levels[::-1]
+        if levels is not None:
+            levels = levels[::-1]
     return seq, levels
 
 
 def get_pod5_reads(pod5_dr, read_ids):
     return dict(
         (str(pod5_read.read_id), pod5_read)
         for pod5_read in pod5_dr.reads(selection=read_ids, preload=["samples"])
     )
 
 
-def get_io_reads(bam_reads, pod5_dr, reverse_signal=False, missing_ok=False):
+def get_io_reads(
+    bam_reads, pod5_dr, reverse_signal=False, missing_ok=False, pa_scaling=None
+):
     pod5_reads = get_pod5_reads(
         pod5_dr, list(set(get_parent_id(bam_read) for bam_read in bam_reads))
     )
     io_reads = []
     for bam_read in bam_reads:
         try:
             io_read = Read.from_pod5_and_alignment(
                 pod5_read_record=pod5_reads[get_parent_id(bam_read)],
                 alignment_record=bam_read,
                 reverse_signal=reverse_signal,
+                pa_scaling=pa_scaling,
             )
         except Exception:
             if missing_ok:
                 continue
             else:
                 raise RemoraError("BAM record not found in POD5")
         io_reads.append(io_read)
@@ -770,53 +799,76 @@
 def get_reads_reference_regions(
     ref_reg,
     pod5_bam_pairs,
     sig_map_refiner=None,
     skip_sig_map_refine=False,
     max_reads=50,
     reverse_signal=False,
+    missing_ok=False,
+    pa_scaling=None,
+    signal_type="norm",
 ):
     all_bam_reads = []
     samples_read_ref_regs = []
     for pod5_dr, bam_fh in pod5_bam_pairs:
         sample_bam_reads = get_reg_bam_reads(ref_reg, bam_fh)
         if len(sample_bam_reads) == 0:
             raise RemoraError("No reads covering region")
         if max_reads is not None and len(sample_bam_reads) > max_reads:
             sample_bam_reads = random.sample(sample_bam_reads, max_reads)
         all_bam_reads.append(sample_bam_reads)
-        io_reads = get_io_reads(sample_bam_reads, pod5_dr, reverse_signal)
+        io_reads = get_io_reads(
+            sample_bam_reads,
+            pod5_dr,
+            reverse_signal,
+            missing_ok=missing_ok,
+            pa_scaling=pa_scaling,
+        )
         if sig_map_refiner is not None and not skip_sig_map_refine:
             for io_read in io_reads:
                 io_read.set_refine_signal_mapping(
                     sig_map_refiner, ref_mapping=True
                 )
         samples_read_ref_regs.append(
-            [io_read.extract_ref_reg(ref_reg) for io_read in io_reads]
+            [
+                io_read.extract_ref_reg(ref_reg, signal_type=signal_type)
+                for io_read in io_reads
+            ]
         )
     return samples_read_ref_regs, all_bam_reads
 
 
 def get_ref_reg_sample_metrics(
     ref_reg,
     pod5_dr,
     bam_reads,
     metric,
     sig_map_refiner,
     skip_sig_map_refine=False,
     reverse_signal=False,
     ref_orient=True,
+    missing_ok=False,
+    pa_scaling=None,
+    signal_type="norm",
     **kwargs,
 ):
-    io_reads = get_io_reads(bam_reads, pod5_dr, reverse_signal)
+    io_reads = get_io_reads(
+        bam_reads,
+        pod5_dr,
+        reverse_signal,
+        missing_ok=missing_ok,
+        pa_scaling=pa_scaling,
+    )
     if sig_map_refiner is not None and not skip_sig_map_refine:
         for io_read in io_reads:
             io_read.set_refine_signal_mapping(sig_map_refiner, ref_mapping=True)
     sample_metrics = [
-        io_read.compute_per_base_metric(metric, region=ref_reg, **kwargs)
+        io_read.compute_per_base_metric(
+            metric, region=ref_reg, signal_type=signal_type, **kwargs
+        )
         for io_read in io_reads
     ]
     if len(sample_metrics) <= 0:
         return
     reg_metrics = dict(
         (
             metric_name,
@@ -838,14 +890,15 @@
     ref_reg,
     pod5_bam_pairs,
     sig_map_refiner=None,
     skip_sig_map_refine=False,
     max_reads=None,
     reverse_signal=False,
     metric="dwell_trimmean",
+    missing_ok=False,
     **kwargs,
 ):
     all_bam_reads = []
     samples_metrics = []
     for pod5_dr, bam_fh in pod5_bam_pairs:
         sample_bam_reads = get_reg_bam_reads(ref_reg, bam_fh)
         if len(sample_bam_reads) == 0:
@@ -1004,14 +1057,15 @@
     sig_start=0,
     sig_lw=0.5,
     levels_lw=1,
     ylim=None,
     rev_strand=False,
     t_as_u=False,
     xlab="Signal Position",
+    ylab="Normalized Signal",
     base_dividers=False,
     sig_pctl_range=METRIC_PCTL_RANGE,
 ):
     """Plot a single read on signal coordinates.
 
     Args:
         seq (str): Sequence to plot
@@ -1060,28 +1114,30 @@
                 xmax="base_en",
                 fill="base",
                 ymin=sig_min,
                 ymax=sig_max,
             ),
             data=base_coords,
             alpha=0.1,
+            show_legend=False,
         )
         + p9.geom_text(
             p9.aes(x="base_st", label="base", color="base", y=sig_min),
             data=base_coords,
             va="bottom",
             ha="left",
             size=8,
             angle=180 if rev_strand else 0,
+            show_legend=False,
         )
-        + p9.scale_fill_manual(BASE_COLORS, guide=False)
-        + p9.scale_color_manual(BASE_COLORS, guide=False)
+        + p9.scale_fill_manual(BASE_COLORS)
+        + p9.scale_color_manual(BASE_COLORS)
         + p9.geom_line(p9.aes(x=xlab, y="Signal"), size=sig_lw, data=sig_df)
-        + p9.labels.ylab("Normalized Signal")
         + p9.labels.xlab(xlab)
+        + p9.labels.ylab(ylab)
         + p9.coords.coord_cartesian(ylim=ylim)
         + p9.theme(
             panel_grid_major_x=p9.element_blank(),
             panel_grid_minor_x=p9.element_blank(),
         )
     )
     if base_dividers:
@@ -1120,14 +1176,15 @@
     start_base=0,
     sig_lw=0.5,
     levels_lw=1,
     ylim=None,
     rev_strand=False,
     t_as_u=False,
     xlab="Base Position",
+    ylab="Normalized Signal",
     base_dividers=False,
     sig_pctl_range=METRIC_PCTL_RANGE,
 ):
     """Plot a single read on base/sequence coordinates.
 
     Args:
         start_base (int): Coordinate of first base in seq
@@ -1137,14 +1194,15 @@
         levels (np.array): Expected signal levels for bases in region
         sig_lw (int): Linewidth for signal lines
         levels_lw (int): Linewidth for level lines (if applicable)
         ylim (tuple): 2-tuple with y-axis limits
         rev_strand (bool): Plot bases upside down
         t_as_u (bool): Plot T bases as U (RNA)
         xlab (str): X-axis Label
+        ylab (str): Y-axis Label
         base_dividers (bool): Add vertical lines separating bases
 
     Returns:
         plotnine plot objects. Use print(return_value) to display plot in in
         a notebook or return_value.save("remora_plot.pdf") to save to file.
     """
     if ylim is None:
@@ -1179,28 +1237,30 @@
                 xmax="base_en",
                 fill="base",
                 ymin=sig_min,
                 ymax=sig_max,
             ),
             data=base_coords,
             alpha=0.1,
+            show_legend=False,
         )
         + p9.geom_text(
             p9.aes(x="base_st", label="base", color="base", y=sig_min),
             data=base_coords,
             va="bottom",
             ha="left",
             size=8,
             angle=180 if rev_strand else 0,
+            show_legend=False,
         )
-        + p9.scale_fill_manual(BASE_COLORS, guide=False)
-        + p9.scale_color_manual(BASE_COLORS, guide=False)
+        + p9.scale_fill_manual(BASE_COLORS)
+        + p9.scale_color_manual(BASE_COLORS)
         + p9.geom_line(p9.aes(x=xlab, y="Signal"), size=sig_lw, data=sig_df)
-        + p9.labels.ylab("Normalized Signal")
         + p9.labels.xlab(xlab)
+        + p9.labels.ylab(ylab)
         + p9.coords.coord_cartesian(ylim=ylim)
         + p9.theme(
             panel_grid_major_x=p9.element_blank(),
             panel_grid_minor_x=p9.element_blank(),
         )
     )
     if base_dividers:
@@ -1234,26 +1294,30 @@
 def plot_align(
     io_read,
     sig_st,
     sig_en,
     sig_mp=0,
     t_as_u=False,
     xlab="Signal Position",
+    ylab="Normalized Signal",
     sig_pctl_range=METRIC_PCTL_RANGE,
+    signal_type="norm",
 ):
     """Plot a single read in signal space with basecalls and reference
     alignment bases annotated.
 
     Args:
         io_read (Read): remora.io.Read object
         sig_st (int): Signal start coordinate
         sig_en (int): Signal end coordinate
         sig_mp (int): Signal midpoint (default 0)
         t_as_u (bool): Plot T bases as U (RNA)
         xlab (str): X-axis label
+        ylab (str): Y-axis label
+        signal_type (str): One of "norm" (default), "pa", "zc_pa", "dac"
 
     Returns:
         plotnine plot object. Use print(return_value) to display plot in in
         a notebook or return_value.save("remora_plot.pdf") to save to file.
     """
     ref_st = np.searchsorted(io_read.ref_to_signal[:-1], sig_st - 1)
     ref_en = np.searchsorted(io_read.ref_to_signal[:-1], sig_en)
@@ -1280,15 +1344,15 @@
             io_read.query_to_signal[bc_st + 1 : bc_en + 1].clip(sig_st, sig_en),
             list(bc_seq),
         ],
         schema=["sig_st", "sig_en", "base"],
         orient="col",
     )
 
-    sig = io_read.norm_signal[sig_st:sig_en]
+    sig = io_read.get_sig_type(signal_type)[sig_st:sig_en]
     sig_min, sig_max = np.percentile(sig, sig_pctl_range)
     sig_diff = sig_max - sig_min
     ylim = (sig_min - sig_diff * 0.02, sig_max + sig_diff * 0.03)
     if sig_mp is None:
         sig_mp = sum(ylim) / 2
 
     return (
@@ -1299,74 +1363,81 @@
                 xmax="sig_en",
                 fill="base",
                 ymin=sig_mp,
                 ymax=sig_max,
             ),
             data=ref_coords,
             alpha=0.3,
-        )
-        + p9.geom_text(
-            p9.aes(x="sig_st", label="base", color="base", y=sig_max),
-            data=ref_coords,
-            va="top",
-            ha="left",
+            show_legend=False,
         )
         + p9.geom_rect(
             p9.aes(
                 xmin="sig_st",
                 xmax="sig_en",
                 fill="base",
                 ymin=sig_min,
                 ymax=sig_mp,
             ),
             data=bc_coords,
             alpha=0.3,
+            show_legend=False,
+        )
+        + p9.geom_text(
+            p9.aes(x="sig_st", label="base", color="base", y=sig_max),
+            data=ref_coords,
+            va="top",
+            ha="left",
+            show_legend=False,
         )
         + p9.geom_text(
             p9.aes(x="sig_st", label="base", color="base", y=sig_min),
             data=bc_coords,
             va="bottom",
             ha="left",
+            show_legend=False,
         )
-        + p9.scale_fill_manual(BASE_COLORS, guide=False)
-        + p9.scale_color_manual(BASE_COLORS, guide=False)
+        + p9.scale_fill_manual(BASE_COLORS)
+        + p9.scale_color_manual(BASE_COLORS)
         + p9.geom_text(
             p9.aes(
                 y=[sig_min, sig_max],
                 label=["Basecalls", "Reference"],
                 va=["top", "bottom"],
             ),
             x=sig_st,
             ha="left",
         )
         + p9.geom_hline(yintercept=sig_mp, linetype="dashed", alpha=0.2)
         + p9.geom_line(p9.aes(x=np.arange(sig_st, sig_en), y=sig))
-        + p9.labels.ylab("Normalized Signal")
         + p9.labels.xlab(xlab)
+        + p9.labels.ylab(ylab)
         + p9.coords.coord_cartesian(ylim=ylim)
         + p9.theme(
             panel_grid_major_x=p9.element_blank(),
             panel_grid_minor_x=p9.element_blank(),
         )
     )
 
 
 def plot_ref_region_reads(
     ref_reg,
     samples_read_ref_regs,
     seq,
     levels,
     sig_lw=0.5,
+    sig_alpha=0.2,
     levels_lw=1,
     sample_names=None,
     sample_colors=None,
     ylim=None,
     highlight_ranges=None,
     t_as_u=False,
     sig_pctl_range=METRIC_PCTL_RANGE,
+    xlab="Reference Position",
+    ylab="Normalized Signal",
 ):
     """Plot read signals over reference region
 
     Args:
         sample_names (list): Sample names. Default: ["Sample1", "Sample2", ... ]
 
     Returns:
@@ -1396,23 +1467,24 @@
             ).with_columns(pl.lit(sample_name).alias("Sample"))
         )
     sig_df = pl.concat(sig_df)
     if ylim is None:
         sig_min, sig_max = np.percentile(sig_df["Signal"], sig_pctl_range)
         sig_diff = sig_max - sig_min
         ylim = (sig_min - sig_diff * 0.01, sig_max + sig_diff * 0.01)
-    level_df = pl.DataFrame(
-        [
-            np.arange(ref_reg.start, ref_reg.end),
-            np.arange(ref_reg.start + 1, ref_reg.end + 1),
-            levels,
-        ],
-        schema=["base_st", "base_en", "level"],
-        orient="col",
-    )
+    if levels is not None:
+        level_df = pl.DataFrame(
+            [
+                np.arange(ref_reg.start, ref_reg.end),
+                np.arange(ref_reg.start + 1, ref_reg.end + 1),
+                levels,
+            ],
+            schema=["base_st", "base_en", "level"],
+            orient="col",
+        )
     if t_as_u:
         seq = util.t_to_u(seq)
     base_coords = pl.DataFrame(
         [
             np.arange(ref_reg.start, ref_reg.end),
             seq,
         ],
@@ -1439,15 +1511,17 @@
                     ymax="sig_max",
                 ),
                 # keep fill out of legends (in case fill is used later)
                 fill=highlight_df["color"],
                 data=highlight_df,
                 alpha=0.2,
             )
-            + p9.scale_fill_manual(dict((c, c) for _, _, c in highlight_ranges))
+            + p9.scale_fill_manual(
+                dict((c, c) for _, _, c in highlight_ranges), guide=False
+            )
         )
     p = (
         p
         + p9.geom_text(
             p9.aes(x="pos", label="base", y=sig_min),
             # keep color out of legend (used for sample names in this plot)
             color=[BASE_COLORS[b] for b in seq],
@@ -1464,46 +1538,50 @@
             alpha=0.5,
             size=0.02,
         )
         + p9.geom_line(
             p9.aes(
                 x="Reference Position", y="Signal", color="Sample", group="Read"
             ),
-            alpha=0.2,
+            alpha=sig_alpha,
             size=sig_lw,
             data=sig_df,
         )
-        + p9.geom_segment(
-            p9.aes(x="base_st", xend="base_en", y="level", yend="level"),
-            color="orange",
-            alpha=0.5,
-            size=levels_lw,
-            data=level_df,
-        )
         + p9.ylim(*ylim)
         + p9.xlim(ref_reg.start, ref_reg.end)
-        + p9.labels.ylab("Normalized Signal")
-        + p9.labels.xlab("Reference Position")
+        + p9.labels.xlab(xlab)
+        + p9.labels.ylab(ylab)
         + p9.theme(
             panel_grid_major_x=p9.element_blank(),
             panel_grid_minor_x=p9.element_blank(),
         )
     )
+    if levels is not None:
+        p = p + p9.geom_segment(
+            p9.aes(x="base_st", xend="base_en", y="level", yend="level"),
+            color="orange",
+            alpha=0.5,
+            size=levels_lw,
+            data=level_df,
+        )
+
     if sample_colors is not None:
         p = p + p9.scale_color_manual(sample_colors, limits=sample_names)
     return p
 
 
 def plot_signal_at_ref_region(
     ref_reg,
     pod5_bam_pairs,
     sig_map_refiner=None,
     skip_sig_map_refine=False,
     max_reads=50,
     reverse_signal=False,
+    pa_scaling=None,
+    signal_type="norm",
     **kwargs,
 ):
     """Plot signal from reads at a reference region.
 
     Args:
         ref_reg (RefRegion): Reference position at which to plot signal
         pod5_bam_pairs (list): List of samples. Each element should be a
@@ -1521,14 +1599,16 @@
     samples_read_ref_regs, reg_bam_reads = get_reads_reference_regions(
         ref_reg,
         pod5_bam_pairs,
         sig_map_refiner=sig_map_refiner,
         skip_sig_map_refine=skip_sig_map_refine,
         max_reads=max_reads,
         reverse_signal=reverse_signal,
+        pa_scaling=pa_scaling,
+        signal_type=signal_type,
     )
     seq, levels = get_ref_seq_and_levels_from_reads(
         ref_reg, chain(*reg_bam_reads), sig_map_refiner
     )
     return plot_ref_region_reads(
         ref_reg,
         samples_read_ref_regs,
@@ -1543,14 +1623,15 @@
     samples_metrics,
     all_bam_reads,
     sample_names=None,
     sample_colors=None,
     geom=p9.geom_boxplot,
     geom_kwargs=None,
     metric_pctl_range=METRIC_PCTL_RANGE,
+    xlab="Reference Position",
 ):
     ref_pos = list(range(ref_reg.start, ref_reg.end))
     metric_names = list(samples_metrics[0].keys())
     if sample_names is None:
         sample_names = [f"Sample{idx}" for idx in range(len(samples_metrics))]
     dfs = dict((metric, []) for metric in metric_names)
     for samp_name, metric_arrs, samp_bam_reads in zip(
@@ -1595,15 +1676,15 @@
                 **geom_kwargs,
             )
             + p9.scale_x_discrete(
                 labels=[str(rp) if rp % 5 == 0 else "" for rp in ref_pos]
             )
             + p9.ylim(*ylim)
             + p9.labels.ylab(metric)
-            + p9.labels.xlab("Reference Position")
+            + p9.labels.xlab(xlab)
         )
         if sample_colors is not None:
             plots[-1] = plots[-1] + p9.scale_fill_manual(
                 sample_colors, limits=sample_names
             )
     return plots
 
@@ -1660,50 +1741,55 @@
 ###########
 # IO Read #
 ###########
 
 
 @dataclass
 class Read:
-    """Input/Output Read
+    """Input/Output Read. Contains signal, basecalls, mapping between the two,
+    various signal scaling parameters, and reference alignment.
 
-    Object to hold information related to signal, basecalls and mapping of a
-    nanopore read.
+    All scaling parameters use the following forumla:
+        output = (input - shift) / sca;e
 
     Args:
         read_id (str): Read identifier. Note that for split reads this should
             be the parent ID (original POD5 ID). See child_read_id for the
             read ID listed in the BAM file.
         dacs (np.ndarray): Data ACquisition signal values. As read from the
             pod5_read.signal attribute. Note for "reverse signal" reads (mostly
             RNA) signal should be in the 5' to 3' orientation (opposite of
             original sequencing 3' to 5' direction)
         seq (str): Basecalled sequence
         stride (int): Basecalling model stride. Move table (mv_table) entries
             occur at regular stride intervals through the signal.
-        num_trimmed (int): Number of signal points trimmed from the start of
-            the read. For split reads this is applied after split slicing.
         mv_table (np.array): Move table. `1` entries indicate base output
             position. See Dorado documentation/SAM.md.
         query_to_signal (np.ndarray): Array with length one longer than
             basecalled sequence (`len(io_read.seq) + 1`) where entries
             represent assigned position in io_read.dacs. This attribute is
             updated when io_read.set_refine_signal_mapping is called.
         shift_dacs_to_pa (float): Shift parameter to convert from DACs to
-            picoampere scaling. See io.Read.pa_signal for implementation.
+            picoamp scaling. See io.Read.pa_signal for implementation.
         scale_dacs_to_pa (float): Scale parameter to convert from DACs to
-            picoampere scaling. See io.Read.pa_signal for implementation.
-        shift_pa_to_norm (float): Shift parameter to convert from picoampere to
+            picoamp scaling. See io.Read.pa_signal for implementation.
+        shift_pa_to_norm (float): Shift parameter to convert from picoamp to
             norm scaling. Extracted from BAM record tags.
-        scale_pa_to_norm (float): Scale parameter to convert from picoampere to
+        scale_pa_to_norm (float): Scale parameter to convert from picoamp to
             norm scaling. Extracted from BAM record tags.
         shift_dacs_to_norm (float): Shift parameter to convert from DACs to
             norm scaling. See io.Read.norm_signal for implementation.
         scale_dacs_to_norm (float): Scale parameter to convert from DACs to
             norm scaling. See io.Read.norm_signal for implementation.
+        shift_pa_to_zc_pa (float): Shift parameter to convert from picoamp to
+            zero-centered picoamp scaling. Extracted from picoamp scaling
+            Dorado basecalling model
+        scale_pa_to_zc_pa (float): Scale parameter to convert from picoamp to
+            zero-centered picoamp scaling. Extracted from picoamp scaling
+            Dorado basecalling model
         ref_seq (str): Reference sequence for mapping.
         ref_reg (RefRegion): Reference mapping region coordinates.
         cigar (list): pysam.AlignedSegment.cigartuples
         ref_to_signal (np.ndarray): Array with length one longer than
             reference sequence (`len(io_read.ref_seq) + 1`) where entries
             represent assigned position in io_read.dacs. This attribute is
             updated when io_read.set_refine_signal_mapping(ref_mapping=True)
@@ -1711,40 +1797,50 @@
         full_align (dict): Dictionary representation of BAM record.
     """
 
     read_id: str
     dacs: np.ndarray = None
     seq: str = None
     stride: int = None
-    num_trimmed: int = None
     mv_table: np.array = None
     query_to_signal: np.ndarray = None
     shift_dacs_to_pa: float = None
     scale_dacs_to_pa: float = None
     shift_pa_to_norm: float = None
     scale_pa_to_norm: float = None
     shift_dacs_to_norm: float = None
     scale_dacs_to_norm: float = None
+    shift_pa_to_zc_pa: float = None
+    scale_pa_to_zc_pa: float = None
     ref_seq: str = None
     ref_reg: RefRegion = None
     cigar: list = None
     ref_to_signal: np.ndarray = None
     full_align: dict = None
     _child_read_id: str = None
     _sig_len: int = None
 
     @property
     def pa_signal(self):
-        """Picoampere convereted signal. Shift and scale values are determined
+        """Picoamp convereted signal. Shift and scale values are determined
         from the instrument. These values are generally not recommended for any
         type of analysis.
         """
         if self.scale_dacs_to_pa is None or self.shift_dacs_to_pa is None:
             raise RemoraError("pA scaling factors not set")
-        return self.scale_dacs_to_pa * (self.dacs + self.shift_dacs_to_pa)
+        return (self.dacs - self.shift_dacs_to_pa) / self.scale_dacs_to_pa
+
+    @property
+    def zero_centered_pa_signal(self):
+        """Zero-centered picoamp convereted signal. Shift and scale values
+        are determined from the instrument plus the basecalling model. These
+        values are linked to a basecalling model and should only be used with
+        these models.
+        """
+        return (self.dacs - self.shift_dacs_to_zc_pa) / self.scale_dacs_to_zc_pa
 
     @property
     def norm_signal(self):
         """Normalized signal, generally aiming to standardize the signal with
         mean=0 and SD=1, though different methods may be applied to perform
         this operation robustly.
         """
@@ -1783,14 +1879,34 @@
 
     @property
     def child_read_id(self):
         if self._child_read_id is None:
             return self.read_id
         return self._child_read_id
 
+    @property
+    def shift_dacs_to_zc_pa(self):
+        """Shift factor from DAC signal values to zero-centered picoamp"""
+        if (
+            self.shift_dacs_to_pa is None
+            or self.scale_dacs_to_pa is None
+            or self.shift_pa_to_zc_pa is None
+        ):
+            raise RemoraError("Zero-centered pA scaling factors not set")
+        return self.shift_dacs_to_pa + (
+            self.scale_dacs_to_pa * self.shift_pa_to_zc_pa
+        )
+
+    @property
+    def scale_dacs_to_zc_pa(self):
+        """Scale factor from DAC signal values to zero-centered picoamp"""
+        if self.scale_dacs_to_pa is None or self.scale_pa_to_zc_pa is None:
+            raise RemoraError("Zero-centered pA scaling factors not set")
+        return self.scale_dacs_to_pa * self.scale_pa_to_zc_pa
+
     def prune(self, drop_mod_tags=True, drop_move_tag=True):
         """Drop larger memory arrays: dacs, mv_table, *_to_signal"""
         drop_tags = set()
         if drop_mod_tags:
             drop_tags.update(("MM", "ML"))
         if drop_move_tag:
             drop_tags.add("mv")
@@ -1850,89 +1966,86 @@
 
         read.ref_seq = None
         read.ref_to_signal = None
         read.ref_reg = None
         return read, simplex_duplex_mapping.duplex_offset
 
     def add_alignment(
-        self, alignment_record, parse_ref_align=True, reverse_signal=False
+        self,
+        alignment_record,
+        parse_ref_align=True,
+        reverse_signal=False,
+        pa_scaling=None,
     ):
         """Add alignment to read object
 
         Args:
             alignment_record (pysam.AlignedSegment)
             parse_ref_align (bool): Should reference alignment be parsed
             reverse_signal (bool): Does this read derive from 3' to 5' signal
                 (RNA reads)
+            pa_scaling (tuple): picoamp to zero-centered picoamp shift and scale
         """
+        if pa_scaling is not None:
+            self.shift_pa_to_zc_pa = pa_scaling[0]
+            self.scale_pa_to_zc_pa = pa_scaling[1]
         if (
             alignment_record.reference_name is None
             and alignment_record.is_reverse
         ):
             raise RemoraError("Unmapped reads cannot map to reverse strand.")
         if self.dacs is None:
             raise RemoraError("Must add signal to io.Read before alignment.")
         self.full_align = alignment_record.to_dict()
 
         tags = dict(alignment_record.tags)
-        try:
-            parent_read_id = tags.get("pi", None)
-            if parent_read_id is None:
-                self.num_trimmed = tags["ts"]
-                if alignment_record.query_name != self.read_id:
-                    raise RemoraError("Read IDs mismatch")
-            else:
-                if parent_read_id != self.read_id:
-                    raise RemoraError("Split read IDs mismatch")
-                self._child_read_id = alignment_record.query_name
-                try:
-                    self.num_trimmed = tags["ts"] + tags["sp"]
-                    self._sig_len = tags["ns"] - tags["ts"]
-                except KeyError:
-                    LOGGER.debug(
-                        f"{self.child_read_id} Split read, missing sp tag."
-                    )
-                    raise RemoraError("Split read missing sp tag")
-            if self.num_trimmed > 0:
-                if reverse_signal:
-                    self.dacs = self.dacs[: -self.num_trimmed]
-                else:
-                    self.dacs = self.dacs[self.num_trimmed :]
-            if self._sig_len is not None:
-                if reverse_signal:
-                    self.dacs = self.dacs[-self._sig_len :]
-                else:
-                    self.dacs = self.dacs[: self._sig_len]
-        except KeyError:
-            self.num_trimmed = 0
+        if reverse_signal:
+            self.dacs = self.dacs[::-1]
+        # trim for split read sp tag
+        self.dacs = self.dacs[tags.get("sp", 0) :]
+        # trim for start and end read trimming
+        self.dacs = self.dacs[
+            tags.get("ts", 0) : tags.get("ns", self.dacs.size)
+        ]
+        if reverse_signal:
+            self.dacs = self.dacs[::-1]
+
+        parent_read_id = tags.get("pi", None)
+        if parent_read_id is None:
+            if alignment_record.query_name != self.read_id:
+                raise RemoraError("Read IDs mismatch")
+        else:
+            if parent_read_id != self.read_id:
+                raise RemoraError("Split read IDs mismatch")
+            self._child_read_id = alignment_record.query_name
 
         self.seq = alignment_record.query_sequence
         if alignment_record.is_reverse:
             self.seq = util.revcomp(self.seq)
         try:
             self.query_to_signal, self.mv_table, self.stride = parse_move_tag(
                 tags["mv"],
-                sig_len=self.dacs.size,
+                sig_len=self.sig_len,
                 seq_len=len(self.seq),
                 reverse_signal=reverse_signal,
             )
         except KeyError:
             LOGGER.debug(f"Move table not found for {self.child_read_id}")
             self.query_to_signal = self.mv_table = self.stride = None
 
         try:
             self.shift_pa_to_norm = tags["sm"]
             self.scale_pa_to_norm = tags["sd"]
         except KeyError:
             self.compute_pa_to_norm_scaling()
 
-        self.shift_dacs_to_norm = (
-            self.shift_pa_to_norm / self.scale_dacs_to_pa
-        ) - self.shift_dacs_to_pa
-        self.scale_dacs_to_norm = self.scale_pa_to_norm / self.scale_dacs_to_pa
+        self.shift_dacs_to_norm = self.shift_dacs_to_pa + (
+            self.scale_dacs_to_pa * self.shift_pa_to_norm
+        )
+        self.scale_dacs_to_norm = self.scale_dacs_to_pa * self.scale_pa_to_norm
 
         if not parse_ref_align or alignment_record.is_unmapped:
             return
 
         self.ref_reg = RefRegion(
             ctg=alignment_record.reference_name,
             strand="-" if alignment_record.is_reverse else "+",
@@ -1968,32 +2081,47 @@
                     f"ref_seq:{len(self.ref_seq)}"
                 )
                 raise RemoraError("Discordant ref seq lengths")
             self.ref_reg.end = self.ref_reg.start + self.ref_to_signal.size - 1
 
     @classmethod
     def from_pod5_and_alignment(
-        cls, pod5_read_record, alignment_record, reverse_signal=False
+        cls,
+        pod5_read_record,
+        alignment_record,
+        reverse_signal=False,
+        pa_scaling=None,
     ):
         """Initialize read from pod5 and pysam records
 
         Args:
             pod5_read_record (pod5.ReadRecord)
             alignment_record (pysam.AlignedSegment)
+            reverse_signal (bool): Is this 3' to 5' signal
+            pa_scaling (tuple): picoamp to zero-centered picoamp shift and scale
         """
         dacs = pod5_read_record.signal
         if reverse_signal:
             dacs = dacs[::-1]
+        # calibration offset and scale apply normalization as:
+        #     y=(x+a)/b
+        # while io.Read stores shfit and scale as:
+        #     y=c*(x-d)
+        # In other words, as shift=mean and scale=std. dev.
         read = Read(
             read_id=str(pod5_read_record.read_id),
             dacs=dacs,
-            shift_dacs_to_pa=pod5_read_record.calibration.offset,
-            scale_dacs_to_pa=pod5_read_record.calibration.scale,
+            shift_dacs_to_pa=-pod5_read_record.calibration.offset,
+            scale_dacs_to_pa=1 / pod5_read_record.calibration.scale,
+        )
+        read.add_alignment(
+            alignment_record,
+            reverse_signal=reverse_signal,
+            pa_scaling=pa_scaling,
         )
-        read.add_alignment(alignment_record, reverse_signal=reverse_signal)
         return read
 
     def into_remora_read(self, use_reference_anchor):
         """Extract RemoraRead object from io.Read.
 
         Args:
             use_reference_anchor (bool): Should remora read be reference
@@ -2024,21 +2152,30 @@
             if self.query_to_signal is None:
                 raise RemoraError("Missing query_to_signal (move table)")
             trim_dacs = self.dacs[
                 self.query_to_signal[0] : self.query_to_signal[-1]
             ]
             shift_seq_to_sig = self.query_to_signal - self.query_to_signal[0]
             seq = self.seq
+        if self.shift_pa_to_zc_pa is None or self.scale_pa_to_zc_pa is None:
+            scale_kwargs = {
+                "shift": self.shift_dacs_to_norm,
+                "scale": self.scale_dacs_to_norm,
+            }
+        else:
+            scale_kwargs = {
+                "shift": self.shift_dacs_to_zc_pa,
+                "scale": self.scale_dacs_to_zc_pa,
+            }
         remora_read = data_chunks.RemoraRead(
             dacs=trim_dacs,
-            shift=self.shift_dacs_to_norm,
-            scale=self.scale_dacs_to_norm,
             seq_to_sig_map=shift_seq_to_sig,
             str_seq=seq,
             read_id=self.read_id,
+            **scale_kwargs,
         )
         remora_read.check()
         return remora_read
 
     def set_refine_signal_mapping(self, sig_map_refiner, ref_mapping=False):
         """Refine signal mapping
 
@@ -2067,17 +2204,17 @@
             self.query_to_signal = (
                 remora_read.seq_to_sig_map + self.query_to_signal[0]
             )
 
         self.shift_dacs_to_norm = remora_read.shift
         self.scale_dacs_to_norm = remora_read.scale
         self.shift_pa_to_norm = (
-            self.shift_dacs_to_norm + self.shift_dacs_to_pa
-        ) * self.scale_dacs_to_pa
-        self.scale_pa_to_norm = self.scale_dacs_to_norm * self.scale_dacs_to_pa
+            self.shift_dacs_to_norm - self.shift_dacs_to_pa
+        ) / self.scale_dacs_to_pa
+        self.scale_pa_to_norm = self.scale_dacs_to_norm / self.scale_dacs_to_pa
 
     def get_filtered_focus_positions(self, select_focus_positions):
         """
         Args:
             select_focus_positions (dict): lookup table of (contig, strand)
             tuples (both strings) to a set of positions to include.
 
@@ -2150,46 +2287,68 @@
             ]
         )
         return base_call_focus_bases
 
     def copy(self):
         return deepcopy(self)
 
-    def extract_basecall_region(self, start_base=None, end_base=None):
+    def get_sig_type(self, signal_type):
+        """Get type of signal specified
+
+        Args:
+            signal_type (str): One of "norm" (default), "pa", "zc_pa", "dac"
+        """
+        if signal_type == "norm":
+            return self.norm_signal
+        elif signal_type == "pa":
+            return self.pa_signal
+        elif signal_type == "zc_pa":
+            return self.zero_centered_pa_signal
+        elif signal_type == "dac":
+            return self.dacs
+        raise RemoraError(f"Invalid signal_type: {signal_type}")
+
+    def extract_basecall_region(
+        self, start_base=None, end_base=None, signal_type="norm"
+    ):
         """Extract region of read from basecall coordinates.
 
         Args:
             start_base (int): Start coordinate for region
             end_base (int): End coordinate for region
+            signal_type (str): One of "norm" (default), "pa", "zc_pa", "dac"
 
         Returns:
             ReadBasecallRegion object
         """
         if self.query_to_signal is None:
             raise RemoraError("Missing query_to_signal (move table)")
         start_base = start_base or 0
         end_base = end_base or self.seq_len
         reg_seq_to_sig = self.query_to_signal[start_base : end_base + 1].copy()
-        reg_sig = self.norm_signal[reg_seq_to_sig[0] : reg_seq_to_sig[-1]]
+        reg_sig = self.get_sig_type(signal_type)[
+            reg_seq_to_sig[0] : reg_seq_to_sig[-1]
+        ]
         sig_start = reg_seq_to_sig[0]
         reg_seq_to_sig -= sig_start
         return ReadBasecallRegion(
             read_id=self.read_id,
             norm_signal=reg_sig,
             seq=self.seq[start_base:end_base],
             seq_to_sig_map=reg_seq_to_sig,
             start=start_base,
             sig_start=sig_start,
         )
 
-    def extract_ref_reg(self, ref_reg):
+    def extract_ref_reg(self, ref_reg, signal_type="norm"):
         """Extract region of read from reference coordinates.
 
         Args:
             ref_reg (RefRegion): Reference region
+            signal_type (str): One of "norm" (default), "pa", "zc_pa", "dac"
 
         Returns:
             ReadRefReg object
         """
         if self.ref_to_signal is None:
             raise RemoraError("Missing ref_to_signal (move table)")
         if ref_reg.start >= self.ref_reg.start + self.ref_seq_len:
@@ -2202,15 +2361,17 @@
             reg_en_within_read = ref_reg.end - self.ref_reg.start
         else:
             reg_st_within_read = max(0, self.ref_reg.end - ref_reg.end)
             reg_en_within_read = self.ref_reg.end - ref_reg.start
         reg_seq_to_sig = self.ref_to_signal[
             reg_st_within_read : reg_en_within_read + 1
         ].copy()
-        reg_sig = self.norm_signal[reg_seq_to_sig[0] : reg_seq_to_sig[-1]]
+        reg_sig = self.get_sig_type(signal_type)[
+            reg_seq_to_sig[0] : reg_seq_to_sig[-1]
+        ]
         reg_seq = self.ref_seq[reg_st_within_read:reg_en_within_read]
         sig_start = reg_seq_to_sig[0]
         reg_seq_to_sig -= sig_start
         read_reg_ref_st = max(self.ref_reg.start, ref_reg.start)
         # orient reverse strand reads on the reference
         if self.ref_reg.strand == "-":
             reg_sig = reg_sig[::-1]
@@ -2248,16 +2409,15 @@
                 a sequence to signal mapping and return a dict of metric names
                 to per base metric arrays.
             ref_anchored (bool): Compute metric against reference bases. If
                 False, return basecall anchored metrics.
             region (RefRegion): Reference region from which to extract metrics
                 of bases. If ref_anchored is False, start and end coordinates
                 are in basecall sequence coordinates.
-            signal_type (str): Type of signal. Should be one of: norm, pa, and
-                dac
+            signal_type (str): One of "norm" (default), "pa", "zc_pa", and "dac"
             **kwargs: Extra args to pass through to metric computations
 
         Returns:
             Result of metric_func. Preset metrics will return dict with metric
             name keys and a numpy array of per-base metric values.
         """
         if metric is not None:
@@ -2302,23 +2462,15 @@
                 if self.query_to_signal is None:
                     raise RemoraError("Missing query_to_signal (move table)")
                 if region.start < 0 or region.start > self.seq_len:
                     raise RemoraError("Region does not overlap read.")
                 # TODO deal with partially overlapping region
                 st_buf = en_buf = 0
                 seq_to_sig = self.query_to_signal[region.start : region.end]
-        if signal_type == "norm":
-            sig = self.norm_signal
-        elif signal_type == "pa":
-            sig = self.pa_signal
-        elif signal_type == "dac":
-            sig = self.dacs
-        else:
-            raise RemoraError("signal_type must be norm, pa or dac")
-
+        sig = self.get_sig_type(signal_type)
         metrics_vals = metric_func(sig, seq_to_sig, **kwargs)
         if max(st_buf, en_buf) > 0:
             tmp_metrics_vals = {}
             for metric_name, metric_vals in metrics_vals.items():
                 tmp_metrics_vals[metric_name] = np.full(region.len, np.NAN)
                 tmp_metrics_vals[metric_name][
                     st_buf : st_buf + metric_vals.size
```

### Comparing `ont-remora-3.1.0/src/remora/log.py` & `ont_remora-3.2.0/src/remora/log.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/main.py` & `ont_remora-3.2.0/src/remora/main.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/metrics.py` & `ont_remora-3.2.0/src/remora/metrics.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/model_util.py` & `ont_remora-3.2.0/src/remora/model_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import json
 import toml
 import datetime
 import importlib
 from os.path import isfile
+from dataclasses import dataclass
 
 import torch
 import numpy as np
 import polars as pl
 from torch import nn
 from torch.nn.utils.fusion import fuse_conv_bn_eval
 
@@ -20,14 +21,96 @@
     from importlib.resources import files as importlib_resources_files
 except ImportError:
     # python3.8 requires backport
     from importlib_resources import files as importlib_resources_files
 
 LOGGER = log.get_logger()
 
+
+####################
+# Training Options #
+####################
+
+
+class CustomPlusCoolDownScheduler:
+    def __init__(
+        self,
+        opt,
+        initial_lr,
+        lr_scheduler_str,
+        lr_scheduler_kwargs,
+        epochs,
+        cool_down_epochs,
+        cool_down_lr,
+    ):
+        self.last_epoch = -1
+        self.opt = opt
+        self.initial_lr = initial_lr
+        self.num_epochs = epochs
+        self.num_cool_down_epochs = cool_down_epochs
+        self.cool_down_lr = cool_down_lr
+        self.total_epochs = epochs + cool_down_epochs
+        self.custom_scheduler = getattr(
+            torch.optim.lr_scheduler, lr_scheduler_str
+        )(
+            self.opt,
+            **dict(
+                (lr_key, constants.TYPE_CONVERTERS[lr_type](lr_val))
+                for lr_key, lr_val, lr_type in lr_scheduler_kwargs
+            ),
+        )
+
+    def get_last_lr(self):
+        if self.last_epoch < self.num_epochs - 1:
+            return self.custom_scheduler.get_last_lr()
+        else:
+            return [self.cool_down_lr for _ in self.opt.param_groups]
+
+    def step(self):
+        self.last_epoch += 1
+        if self.last_epoch < self.num_epochs - 1:
+            return self.custom_scheduler.step()
+        else:
+            for pg in self.opt.param_groups:
+                pg["lr"] = self.cool_down_lr
+
+
+@dataclass
+class TrainOpts:
+    epochs: int = constants.DEFAULT_EPOCHS
+    early_stopping: int = constants.DEFAULT_EARLY_STOPPING
+    optimizer_str: str = constants.DEFAULT_OPTIMIZER
+    opt_kwargs: list = constants.DEFAULT_OPT_VALUES
+    learning_rate: float = constants.DEFAULT_LR
+    lr_scheduler_str: str = constants.DEFAULT_SCHEDULER
+    lr_scheduler_kwargs: list = constants.DEFAULT_SCH_VALUES
+    lr_cool_down_epochs: int = constants.DEFAULT_SCH_COOL_DOWN_EPOCHS
+    lr_cool_down_lr: float = constants.DEFAULT_SCH_COOL_DOWN_LR
+
+    def load_optimizer(self, model):
+        return getattr(torch.optim, self.optimizer_str)(
+            model.parameters(),
+            **dict(
+                (opt_key, constants.TYPE_CONVERTERS[opt_type](opt_val))
+                for opt_key, opt_val, opt_type in self.opt_kwargs
+            ),
+        )
+
+    def load_scheduler(self, opt):
+        return CustomPlusCoolDownScheduler(
+            opt,
+            self.learning_rate,
+            self.lr_scheduler_str,
+            self.lr_scheduler_kwargs,
+            epochs=self.epochs,
+            cool_down_epochs=self.lr_cool_down_epochs,
+            cool_down_lr=self.lr_cool_down_lr,
+        )
+
+
 #############
 # Exporting #
 #############
 
 
 def export_model_torchscript(ckpt, model, save_filename):
     model.eval()
@@ -47,14 +130,15 @@
         "refine_kmer_center_idx",
         "refine_do_rough_rescale",
         "refine_scale_iters",
         "refine_algo",
         "refine_half_bandwidth",
         "base_start_justify",
         "offset",
+        "pa_scaling",
         "model_params",
     ):
         meta[ckpt_key] = ckpt[ckpt_key]
 
     if ckpt["mod_bases"] is not None:
         for mod_idx in range(len(ckpt["mod_bases"])):
             meta[f"mod_long_names_{mod_idx}"] = str(
@@ -193,14 +277,15 @@
         )
 
     # add simple metadata
     for ckpt_key in (
         "mod_bases",
         "offset",
         "reverse_signal",
+        "pa_scaling",
     ):
         modbases[ckpt_key] = ckpt[ckpt_key]
 
     if ckpt["mod_bases"] is not None:
         for mod_idx in range(len(ckpt["mod_bases"])):
             modbases[f"mod_long_names_{mod_idx}"] = str(
                 ckpt["mod_long_names"][mod_idx]
@@ -255,14 +340,20 @@
 
 def add_derived_metadata(model_metadata):
     if "reverse_signal" not in model_metadata:
         LOGGER.warning(
             "reverse signal attribute not found in model. Assuming False"
         )
         model_metadata["reverse_signal"] = False
+    if "pa_scaling" not in model_metadata:
+        LOGGER.warning(
+            "Centered picoamp scaling attribute not found in model. "
+            "Assuming None"
+        )
+        model_metadata["pa_scaling"] = None
     if model_metadata["mod_bases"] == "None":
         model_metadata["mod_bases"] = None
         model_metadata["mod_long_names"] = None
     else:
         model_metadata["mod_long_names"] = []
         for mod_idx in range(len(model_metadata["mod_bases"])):
             model_metadata["mod_long_names"].append(
@@ -423,14 +514,15 @@
         "mod_bases",
         "reverse_signal",
         "base_start_justify",
         "offset",
         "model_params",
         "num_motifs",
         "model_version",
+        "pa_scaling",
         "refine_kmer_center_idx",
         "refine_do_rough_rescale",
         "refine_scale_iters",
         "refine_algo",
         "refine_half_bandwidth",
     ]:
         metadata[md_key] = model_metadata[md_key]
```

### Comparing `ont-remora-3.1.0/src/remora/parsers.py` & `ont_remora-3.2.0/src/remora/parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     subparser.set_defaults(func=lambda x: subparser.print_help())
     #  Register dataset sub commands
     register_dataset_prepare(ssubparser)
     register_dataset_inspect(ssubparser)
     register_dataset_make_config(ssubparser)
     register_dataset_merge(ssubparser)
     register_dataset_head(ssubparser)
+    register_dataset_copy(ssubparser)
 
 
 def register_dataset_prepare(parser):
     subparser = parser.add_parser(
         "prepare",
         description="Prepare a core Remora dataset",
         help="Prepare a core Remora dataset",
@@ -165,14 +166,21 @@
     data_grp.add_argument(
         "--reverse-signal",
         action="store_true",
         help="""Is nanopore signal 3' to 5' orientation? Primarily for direct
         RNA""",
     )
     data_grp.add_argument(
+        "--picoamp-scaling-basecall-model",
+        help="""Provide the path to the Dorado basecalling model directory
+        which will be linke with this modified base model. Produce dataset wtih
+        picoampere scaled signal. Note that this is incompatible with any
+        signal mapping refine arguments""",
+    )
+    data_grp.add_argument(
         "--save-every",
         default=100_000,
         type=int,
         help="""Flush dataset data and update dataset size at this interval.
         Larger values will increase RAM usage, but could increase speed.""",
     )
     data_grp.add_argument(
@@ -268,17 +276,17 @@
     )
 
     subparser.set_defaults(func=run_dataset_prepare)
 
 
 def run_dataset_prepare(args):
     from remora.io import parse_bed
-    from remora.util import Motif, prepare_out_dir
     from remora.refine_signal_map import SigMapRefiner
     from remora.prepare_train_data import extract_chunk_dataset
+    from remora.util import Motif, prepare_out_dir, parse_picoamps
 
     prepare_out_dir(args.output_path, args.overwrite)
     if args.mod_base is None and not args.mod_base_control:
         LOGGER.error("Must specify either --mod-base or --mod-base-control")
         sys.exit(1)
 
     motifs = [Motif(*mo) for mo in args.motif]
@@ -294,26 +302,30 @@
         algo=args.refine_algo,
         half_bandwidth=args.refine_half_bandwidth,
         sd_params=args.refine_short_dwell_parameters,
         do_fix_guage=True,
         rough_rescale_method=args.rough_rescale_method,
     )
     if not sig_map_refiner.is_valid:
-        raise RemoraError("Invalid signal mappnig refiner settings.")
+        raise RemoraError("Invalid signal mapping refiner settings.")
+    pa_scaling = parse_picoamps(
+        args.picoamp_scaling_basecall_model, sig_map_refiner
+    )
     extract_chunk_dataset(
         bam_path=args.bam,
         pod5_path=args.pod5,
         out_path=args.output_path,
         mod_base=args.mod_base,
         mod_base_control=args.mod_base_control,
         motifs=motifs,
         focus_ref_pos=focus_ref_pos,
         chunk_context=args.chunk_context,
         min_samps_per_base=args.min_samples_per_base,
         max_chunks_per_read=args.max_chunks_per_read,
+        pa_scaling=pa_scaling,
         sig_map_refiner=sig_map_refiner,
         kmer_context_bases=args.kmer_context_bases,
         base_start_justify=args.base_start_justify,
         offset=args.offset,
         num_reads=args.num_reads,
         num_extract_alignment_threads=args.num_extract_alignment_workers,
         num_extract_chunks_threads=args.num_extract_chunks_workers,
@@ -321,14 +333,53 @@
         rev_sig=args.reverse_signal,
         save_every=args.save_every,
         skip_shuffle=args.skip_shuffle,
     )
     LOGGER.info("Done")
 
 
+def register_dataset_inspect(parser):
+    subparser = parser.add_parser(
+        "inspect",
+        description="Inspect Remora dataset",
+        help="Inspect Remora dataset",
+        formatter_class=SubcommandHelpFormatter,
+    )
+    subparser.add_argument(
+        "remora_dataset_path",
+        help="Remora training dataset",
+    )
+    subparser.add_argument(
+        "--out-path",
+        help="Path to save new config with hierarchical datasets expanded "
+        "and dataset hash values included.",
+    )
+    subparser.set_defaults(func=run_dataset_inspect)
+
+
+def run_dataset_inspect(args):
+    import json
+
+    from remora.data_chunks import (
+        load_dataset,
+        CoreRemoraDataset,
+        RemoraDataset,
+    )
+
+    paths, props, hashes = load_dataset(args.remora_dataset_path)
+    datasets = [
+        CoreRemoraDataset(path, do_check_super_batches=True) for path in paths
+    ]
+    dataset = RemoraDataset(datasets, props, hashes)
+    print(f"Dataset summary:\n{dataset.summary}")
+    if args.out_path is not None:
+        with open(args.out_path, "w") as fh:
+            json.dump(dataset.get_config(), fh)
+
+
 def register_dataset_make_config(parser):
     subparser = parser.add_parser(
         "make_config",
         description="""Create Remora dataset from core datasets. This will not
         copy data. The config file points to the core datasets and generates
         batches with specified proportions from each core dataset.""",
         help="Create Remora dataset from core datasets",
@@ -423,26 +474,32 @@
     subparser.add_argument(
         "dataset_paths",
         nargs="+",
         help="""Remora training dataset. May be either a core Remora dataset or
         another config""",
     )
     subparser.add_argument(
+        "--max-size",
+        type=int,
+        help="""Maximum size of output dataset""",
+    )
+    subparser.add_argument(
         "--overwrite",
         action="store_true",
         help="Overwrite existing output directory if existing.",
     )
     subparser.set_defaults(func=run_dataset_merge)
 
 
 def run_dataset_merge(args):
     import numpy as np
     from tqdm import tqdm
 
     from remora.data_chunks import (
+        compute_best_split,
         load_dataset,
         CoreRemoraDataset,
         RemoraDataset,
     )
     from remora.util import prepare_out_dir
 
     prepare_out_dir(args.out_path, args.overwrite)
@@ -458,55 +515,73 @@
             )
             for path in all_paths
         ],
         np.ones(len(all_paths)),
     )
     LOGGER.info(f"Loaded dataset:\n{dataset.summary}")
     merged_metadata = dataset.metadata.copy()
-    merged_metadata.allocate_size = sum(ds.size for ds in dataset.datasets)
+    ds_out_sizes = np.array([ds.size for ds in dataset.datasets])
+    if args.max_size is not None and ds_out_sizes.sum() > args.max_size:
+        ds_out_sizes = compute_best_split(
+            args.max_size, ds_out_sizes / ds_out_sizes.sum()
+        )
+    merged_metadata.allocate_size = ds_out_sizes.sum()
     merged_metadata.max_seq_len = max(
         ds.metadata.max_seq_len for ds in dataset.datasets
     )
     merged_metadata.dataset_start = 0
     merged_metadata.dataset_end = 0
 
     merged_dataset = CoreRemoraDataset(
         data_path=args.out_path,
         mode="w",
         metadata=merged_metadata,
     )
     merged_dataset.write_metadata()
     LOGGER.info("Copying datasets")
-    for ds in tqdm(dataset.datasets, smoothing=0, desc="Datasets"):
+    for ds, ds_out_size in tqdm(
+        zip(dataset.datasets, ds_out_sizes),
+        smoothing=0,
+        desc="Datasets",
+        total=ds_out_sizes.size,
+    ):
+        if ds.metadata.dataset_end != ds_out_size:
+            LOGGER.debug(
+                f"Reducing dataset size from {ds.metadata.dataset_end:,} to "
+                f"{ds_out_size:,}"
+            )
+            ds.metadata.dataset_end = ds_out_size
         chunks_per_sb, _ = ds.adjust_batch_params()
         total_sbs = ds.size // chunks_per_sb
         LOGGER.debug(f"Adding dataset from {ds.data_path}")
         for sb_idx, sb in tqdm(
             enumerate(ds.iter_super_batches()),
             smoothing=0,
             total=total_sbs,
             leave=False,
             position=1,
             desc="Batches",
         ):
             merged_dataset.write_batch(sb)
             merged_dataset.flush()
             merged_dataset.write_metadata()
-            LOGGER.debug(f"{sb_idx + 1}/{total_sbs} super batches complete")
+            if sb_idx % 10 == 9:
+                # update every 10 batches
+                LOGGER.debug(f"{sb_idx + 1}/{total_sbs} super batches complete")
     LOGGER.info("Shuffling dataset")
     merged_dataset.shuffle(show_prog=True)
     LOGGER.info(f"Saved core dataset:\n{merged_dataset.summary}")
 
 
 def register_dataset_head(parser):
     subparser = parser.add_parser(
         "head",
-        description="""Create new dataset with a selection of the first reads
-        from another dataset.""",
-        help="Create new dataset from beginning of another",
+        description="""Create new core dataset with a selection of the first
+        reads from another core dataset.""",
+        help="Create new core dataset from beginning of another",
         formatter_class=SubcommandHelpFormatter,
     )
     subparser.add_argument(
         "out_path",
         help="Path to save new dataset.",
     )
     subparser.add_argument(
@@ -576,51 +651,84 @@
         LOGGER.debug(f"{sb_idx + 1} super batches complete")
 
     LOGGER.info("Shuffling dataset")
     head_dataset.shuffle(show_prog=True)
     LOGGER.info(f"Saved core dataset:\n{head_dataset.summary}")
 
 
-def register_dataset_inspect(parser):
+def register_dataset_copy(parser):
     subparser = parser.add_parser(
-        "inspect",
-        description="Inspect Remora dataset",
-        help="Inspect Remora dataset",
+        "copy",
+        description="""Copy dataset to a new location. Useful for moving
+        multi-part datasets to faster disk access locations. New config will be
+        at [out_path]/dataset.cfg and core datasets will be sub-directories
+        [out_path]/dataset_001, [out_path]/dataset_002, etc.""",
+        help="Move dataset to new location",
         formatter_class=SubcommandHelpFormatter,
     )
     subparser.add_argument(
-        "remora_dataset_path",
-        help="Remora training dataset",
+        "in_path",
+        help="""Input core Remora dataset (config or core dataset).""",
     )
     subparser.add_argument(
-        "--out-path",
-        help="Path to save new config with hierarchical datasets expanded "
-        "and dataset hash values included.",
+        "out_path",
+        help="Path to save new datasets.",
     )
-    subparser.set_defaults(func=run_dataset_inspect)
+    subparser.add_argument(
+        "--overwrite",
+        action="store_true",
+        help="Overwrite existing output directory if existing.",
+    )
+    subparser.set_defaults(func=run_dataset_copy)
 
 
-def run_dataset_inspect(args):
+def run_dataset_copy(args):
     import json
+    import shutil
 
+    from remora.util import prepare_out_dir
     from remora.data_chunks import (
         load_dataset,
         CoreRemoraDataset,
         RemoraDataset,
     )
 
-    paths, props, hashes = load_dataset(args.remora_dataset_path)
-    datasets = [
-        CoreRemoraDataset(path, do_check_super_batches=True) for path in paths
-    ]
-    dataset = RemoraDataset(datasets, props, hashes)
-    print(f"Dataset summary:\n{dataset.summary}")
-    if args.out_path is not None:
-        with open(args.out_path, "w") as fh:
-            json.dump(dataset.get_config(), fh)
+    out_dir = Path(args.out_path)
+    prepare_out_dir(args.out_path, args.overwrite)
+    paths, props, hashes = load_dataset(args.in_path)
+    src_fh = open(out_dir / "sources.txt", "w")
+    ds_out_dirs = []
+    for ds_idx, src_path in enumerate(paths):
+        for item in os.listdir(src_path):
+            if os.path.isdir(os.path.join(src_path, item)):
+                raise RemoraError(
+                    f"Source dataset has nested directory: {item}"
+                )
+        ds_out_dir = out_dir / f"dataset_{ds_idx:03}"
+        ds_out_dirs.append(ds_out_dir)
+        src_fh.write(f"{src_path}\t{ds_out_dir}\n")
+        try:
+            shutil.copytree(src_path, ds_out_dir)
+            LOGGER.info(f"'{src_path}' copied to '{ds_out_dir}' successfully.")
+        except FileExistsError:
+            raise RemoraError(f"Destination '{ds_out_dir}' already exists.")
+        except FileNotFoundError:
+            raise RemoraError(f"Source '{src_path}' does not exist.")
+        except PermissionError:
+            raise RemoraError("Permission denied.")
+        except Exception as e:
+            RemoraError(f"Error: {e}")
+    dataset = RemoraDataset(
+        [CoreRemoraDataset(ds_out_dir) for ds_out_dir in ds_out_dirs],
+        props,
+        hashes,
+    )
+    with open(out_dir / "dataset.cfg", "w") as fh:
+        json.dump(dataset.get_config(), fh)
+    LOGGER.info(dataset.summary)
 
 
 ################
 # remora model #
 ################
 
 
@@ -632,20 +740,26 @@
         formatter_class=SubcommandHelpFormatter,
     )
     ssubparser = subparser.add_subparsers(title="model commands")
     #  Since `model` has several sub-commands, print help as default
     subparser.set_defaults(func=lambda x: subparser.print_help())
     #  Register model sub commands
     register_model_train(ssubparser)
+    register_model_inspect(ssubparser)
     register_model_export(ssubparser)
     register_model_list_pretrained(ssubparser)
     register_model_download(ssubparser)
 
 
 def register_model_train(parser):
+    def none_or_float(x):
+        if x == "None":
+            return
+        return float(x)
+
     subparser = parser.add_parser(
         "train",
         description="Train Remora model",
         help="Train Remora model",
         formatter_class=SubcommandHelpFormatter,
     )
 
@@ -752,63 +866,88 @@
         "--epochs",
         default=constants.DEFAULT_EPOCHS,
         type=int,
         help="Number of training epochs.",
     )
     train_grp.add_argument(
         "--optimizer",
-        default=constants.OPTIMIZERS[0],
-        choices=constants.OPTIMIZERS,
-        help="Optimizer setting.",
+        default=constants.DEFAULT_OPTIMIZER,
+        help="Optimizer. Select from torch.optim",
     )
     train_grp.add_argument(
-        "--scheduler",
-        default=None,
-        help="Scheduler setting.",
+        "--optimizer-kwargs",
+        nargs=3,
+        action="append",
+        default=constants.DEFAULT_OPT_VALUES,
+        metavar=("NAME", "VALUE", "TYPE"),
+        help="Arguments to torch optimizer. TYPE should be str, int or float",
     )
     train_grp.add_argument(
         "--lr",
         default=constants.DEFAULT_LR,
         type=float,
-        help="Learning rate setting.",
+        help="Learning rate",
     )
     train_grp.add_argument(
-        "--weight-decay",
-        default=constants.DEFAULT_WEIGHT_DECAY,
-        type=float,
-        help="Weight decay setting.",
+        "--lr-scheduler",
+        default=constants.DEFAULT_SCHEDULER,
+        help="""Torch learning rate scheduler. Select from
+        torch.optim.lr_scheduler""",
+    )
+    train_grp.add_argument(
+        "--lr-scheduler-kwargs",
+        nargs=3,
+        action="append",
+        default=constants.DEFAULT_SCH_VALUES,
+        metavar=("NAME", "VALUE", "TYPE"),
+        help="Arguments to torch scheduler. TYPE should be str, int or float",
+    )
+    train_grp.add_argument(
+        "--lr-cool-down-epochs",
+        type=int,
+        default=constants.DEFAULT_SCH_COOL_DOWN_EPOCHS,
+        help="Number of cool down epochs at the end of training",
+    )
+    train_grp.add_argument(
+        "--lr-cool-down-learning-rate",
+        type=int,
+        default=constants.DEFAULT_SCH_COOL_DOWN_LR,
+        help="Cool down learning rate at the end of training",
     )
     train_grp.add_argument(
         "--early-stopping",
-        default=10,
+        default=constants.DEFAULT_EARLY_STOPPING,
         type=int,
         help="""Stops training after a number of epochs without improvement.
         If set to 0 no stopping is done.""",
     )
     train_grp.add_argument(
         "--seed",
         type=int,
         help="Seed value.",
     )
     train_grp.add_argument(
-        "--lr-sched-kwargs",
-        nargs=3,
-        action="append",
-        metavar=("NAME", "VALUE", "TYPE"),
-    )
-    train_grp.add_argument(
         "--high-conf-incorrect-thr-frac",
         nargs=2,
         type=float,
         metavar=("THRESHOLD", "FRACTION"),
         help="""Filter highly confident but incorrect chunks from training each
         iteration. First value sets the threshold for high confidence
         predictions and second value sets the maximum fraction of chunks to
         filter per batch.""",
     )
+    train_grp.add_argument(
+        "--gradient-clip-num-mads",
+        default=0,
+        type=none_or_float,
+        help="""Clip gradients (by value) at num_MADs above the median of
+        the last 1000 parameter gradient maximums. Gradient threshold
+        values are computed for each parameter group independently. Use
+        "--gradient-clip-num-mads None" for no clipping.""",
+    )
 
     comp_grp = subparser.add_argument_group("Compute Arguments")
     comp_grp.add_argument(
         "--device",
         help="Device for neural network processing. See torch.device.",
     )
     comp_grp.add_argument(
@@ -833,14 +972,15 @@
         reduce RAM usage.""",
     )
 
     subparser.set_defaults(func=run_model_train)
 
 
 def run_model_train(args):
+    from remora.model_util import TrainOpts
     from remora.train_model import train_model
     from remora.util import parse_device, prepare_out_dir
 
     prepare_out_dir(args.output_path, args.overwrite)
     PROF_TRAIN_FN = os.getenv("REMORA_TRAIN_PROFILE_FILE")
     if PROF_TRAIN_FN is not None:
         from torch.profiler import profile, ProfilerActivity
@@ -850,44 +990,121 @@
         def train_model(*args):
             with profile(
                 activities=[ProfilerActivity.CPU, ProfilerActivity.CUDA]
             ) as prof:
                 train_model_wrapper(*args)
             prof.export_chrome_trace(PROF_TRAIN_FN)
 
+    train_opts = TrainOpts(
+        epochs=args.epochs,
+        early_stopping=args.early_stopping,
+        optimizer_str=args.optimizer,
+        opt_kwargs=args.optimizer_kwargs,
+        learning_rate=args.lr,
+        lr_scheduler_str=args.lr_scheduler,
+        lr_scheduler_kwargs=args.lr_scheduler_kwargs,
+        lr_cool_down_epochs=args.lr_cool_down_epochs,
+        lr_cool_down_lr=args.lr_cool_down_learning_rate,
+    )
     train_model(
         args.seed,
         parse_device(args.device),
         Path(args.output_path),
         args.remora_dataset_path,
         args.chunk_context,
         args.kmer_context_bases,
         args.batch_size,
         args.model,
         args.size,
-        args.optimizer,
-        args.lr,
-        args.scheduler,
-        args.weight_decay,
-        args.epochs,
+        train_opts,
         args.chunks_per_epoch,
         args.num_test_chunks,
         args.save_freq,
-        args.early_stopping,
         args.filter_fraction,
         args.ext_val,
         args.ext_val_names,
-        args.lr_sched_kwargs,
         args.high_conf_incorrect_thr_frac,
         args.finetune_path,
         args.freeze_num_layers,
         args.super_batch_size,
         args.super_batch_sample_fraction,
         args.read_batches_from_disk,
+        args.gradient_clip_num_mads,
+    )
+    LOGGER.info("Done")
+
+
+def register_model_inspect(parser):
+    subparser = parser.add_parser(
+        "inspect",
+        description="Inspect a Remora model",
+        help="Inspect a Remora model",
+        formatter_class=SubcommandHelpFormatter,
+    )
+    subparser.add_argument(
+        "checkpoint_path",
+        help="Path to a pretrained model checkpoint.",
+    )
+    subparser.add_argument(
+        "--model-path",
+        help="Path to a model architecture. Default: Use path from checkpoint.",
+    )
+
+    subparser.set_defaults(func=run_model_inspect)
+
+
+def run_model_inspect(args):
+    from remora.model_util import (
+        continue_from_checkpoint,
+        load_torchscript_model,
+        repr_model_metadata,
     )
+    from remora.refine_signal_map import SigMapRefiner
+
+    LOGGER.info("Loading model")
+    try:
+        model, model_metadata = load_torchscript_model(args.checkpoint_path)
+        LOGGER.info("Loaded a torchscript model")
+    except RuntimeError:
+        model_metadata, model = continue_from_checkpoint(
+            args.checkpoint_path, args.model_path
+        )
+        # TODO add function in model_util for this simmilar to
+        # add_derived_metadata for .pt models
+        if (
+            "refine_kmer_levels" in model_metadata
+            and model_metadata["refine_kmer_levels"] is not None
+        ):
+            # load sig_map_refiner
+            model_metadata["sig_map_refiner"] = SigMapRefiner(
+                _levels_array=model_metadata["refine_kmer_levels"],
+                center_idx=int(model_metadata["refine_kmer_center_idx"]),
+                do_rough_rescale=model_metadata["refine_do_rough_rescale"],
+                scale_iters=int(model_metadata["refine_scale_iters"]),
+                algo=model_metadata["refine_algo"],
+                half_bandwidth=int(model_metadata["refine_half_bandwidth"]),
+                sd_arr=model_metadata["refine_sd_arr"],
+            )
+        else:
+            # handle original models without sig_map_refiner
+            model_metadata["sig_map_refiner"] = SigMapRefiner()
+            model_metadata["base_start_justify"] = False
+            model_metadata["offset"] = 0
+        for md_name in [
+            md_name
+            for md_name in model_metadata.keys()
+            if md_name.startswith("refine_")
+        ]:
+            del model_metadata[md_name]
+        for md_name in ["state_dict", "opt"]:
+            del model_metadata[md_name]
+        LOGGER.info("Loaded model from checkpoint")
+
+    md_str = repr_model_metadata(model_metadata)
+    LOGGER.info(f"Loaded Remora model attrs\n{md_str}\n")
     LOGGER.info("Done")
 
 
 def register_model_export(parser):
     subparser = parser.add_parser(
         "export",
         description="Export a model to TorchScript format for inference",
@@ -1093,18 +1310,25 @@
     out_grp = subparser.add_argument_group("Output Arguments")
     out_grp.add_argument("--out-bam", help="Output BAM path.", required=True)
     out_grp.add_argument(
         "--log-filename",
         help="Log filename. Default: Don't output log file.",
     )
 
-    mdl_grp = subparser.add_argument_group("Model Arguments")
+    mdl_grp = subparser.add_argument_group(
+        "Model Arguments",
+        """Specify model. --model can be specified multiple times, but only
+        one model can be specified per canonical base. Additional arguments
+        will select a default model given sufficient specificty (pore and
+        modified base).""",
+    )
     mdl_grp.add_argument(
         "--model",
-        help="Path to a pretrained model in torchscript format.",
+        action="append",
+        help="Path(s) to a pretrained model in torchscript format.",
     )
     mdl_grp.add_argument(
         "--pore",
         help="Choose the type of pore the Remora model has been trained on "
         "(e.g. dna_r10.4_e8.1)",
     )
     mdl_grp.add_argument(
@@ -1239,15 +1463,16 @@
         "--log-filename",
         help="Log filename. Default: Don't output log file.",
     )
 
     mdl_grp = subparser.add_argument_group("Model Arguments")
     mdl_grp.add_argument(
         "--model",
-        help="Path to a pretrained model in torchscript format.",
+        action="append",
+        help="Path(s) to a pretrained model in torchscript format.",
     )
     mdl_grp.add_argument(
         "--pore",
         help="""Choose the type of pore the Remora model has been trained on
         (e.g. dna_r10.4_e8.1)""",
     )
     mdl_grp.add_argument(
@@ -1306,52 +1531,78 @@
         help="""Number of chunk extraction workers. If performing signal
         refinement this should be increased.""",
     )
 
     subparser.set_defaults(func=run_infer_from_pod5_and_bam_duplex)
 
 
-def _unpack_model_kw_args(args) -> dict:
+def _unpack_models_kw_args(args) -> dict:
     from remora.util import parse_device
 
-    if args.model and not os.path.exists(args.model):
-        raise ValueError(f"didn't find model file at {args.model}")
+    device = parse_device(args.device)
+    if args.model is None:
+        return [
+            {
+                "pore": args.pore,
+                "basecall_model_type": args.basecall_model_type,
+                "basecall_model_version": args.basecall_model_version,
+                "modified_bases": args.modified_bases,
+                "remora_model_type": args.remora_model_type,
+                "remora_model_version": args.remora_model_version,
+                "device": device,
+            },
+        ]
+    if any(not os.path.exists(mdl_path) for mdl_path in args.model):
+        invalid_paths = [
+            mdl_path for mdl_path in args.model if not os.path.exists(mdl_path)
+        ]
+        raise ValueError(f"Model path(s) do not exist {invalid_paths}")
+    return [
+        {
+            "model_filename": mdl_path,
+            "device": device,
+        }
+        for mdl_path in args.model
+    ]
+
 
-    model_kwargs = {
-        "model_filename": args.model,
-        "pore": args.pore,
-        "basecall_model_type": args.basecall_model_type,
-        "basecall_model_version": args.basecall_model_version,
-        "modified_bases": args.modified_bases,
-        "remora_model_type": args.remora_model_type,
-        "remora_model_version": args.remora_model_version,
-        "device": parse_device(args.device),
-    }
-    return model_kwargs
+def check_models(models):
+    if any(
+        mdl[1]["reverse_signal"] != models[0][1]["reverse_signal"]
+        for mdl in models[1:]
+    ):
+        raise RemoraError("All models must be the same signal direction")
+    if any(
+        mdl[1]["pa_scaling"] != models[0][1]["pa_scaling"] for mdl in models[1:]
+    ):
+        raise RemoraError("All models must use the same signal normalization")
+    if len(models) != len(set(metadata["can_base"] for _, metadata in models)):
+        raise RemoraError("Only one model per canonical base allowed.")
 
 
 def run_infer_from_pod5_and_bam(args):
     import torch
 
     from remora.model_util import load_model
     from remora.inference import infer_from_pod5_and_bam
 
     if args.log_filename is not None:
         log.init_logger(args.log_filename)
     # test that model can be loaded in parent process
-    model_kwargs = _unpack_model_kw_args(args)
-    model, model_metadata = load_model(
-        **model_kwargs, quiet=False, eval_only=True
-    )
+    models_kwargs = _unpack_models_kw_args(args)
+    models = [
+        load_model(**model_kwargs, quiet=False, eval_only=True)
+        for model_kwargs in models_kwargs
+    ]
+    check_models(models)
     torch.set_grad_enabled(False)
     infer_from_pod5_and_bam(
         pod5_path=args.pod5,
         in_bam_path=args.in_bam,
-        model=model,
-        model_metadata=model_metadata,
+        models=models,
         out_bam_path=args.out_bam,
         num_reads=args.num_reads,
         queue_max=args.queue_max,
         num_extract_alignment_workers=args.num_extract_alignment_workers,
         num_prep_read_workers=args.num_prepare_read_workers,
         num_prep_nn_input_workers=args.num_prepare_nn_input_workers,
         num_post_process_workers=args.num_post_process_workers,
@@ -1365,18 +1616,26 @@
     import torch
 
     from remora.model_util import load_model
     from remora.inference import infer_duplex
 
     if args.log_filename is not None:
         log.init_logger(args.log_filename)
-    model_kwargs = _unpack_model_kw_args(args)
-    model, model_metadata = load_model(
-        **model_kwargs, quiet=False, eval_only=True
-    )
+    models_kwargs = _unpack_models_kw_args(args)
+    models = [
+        load_model(**model_kwargs, quiet=False, eval_only=True)
+        for model_kwargs in models_kwargs
+    ]
+    if len(models) > 1:
+        raise NotImplementedError(
+            "Duplex infer does not currently implement running of "
+            "multiple models"
+        )
+    # check_models(models)
+    model, model_metadata = models[0]
     torch.set_grad_enabled(False)
 
     if not os.path.exists(args.pod5):
         raise ValueError(f"didn't find pod5 at {args.pod5}")
     if not os.path.exists(args.simplex_bam):
         raise ValueError(f"didn't find simplex bam at {args.simplex_bam}")
     if not os.path.exists(args.duplex_bam):
@@ -1496,14 +1755,18 @@
 
     subparser.set_defaults(func=run_validate_modbams)
 
 
 def run_validate_modbams(args):
     from remora.validate import validate_modbams
 
+    LOGGER.warning(
+        """This cmomand is deprecated and will be removed from a future version
+        of Remora. Please use the `modkit validate` command."""
+    )
     if args.explicit_mod_tag_used:
         LOGGER.warning(
             """
             If implict modified tag types are included (from all-context
             modified base models) results from this command will be inavlid.
             Please see pysam issue here:
             https://github.com/pysam-developers/pysam/issues/1123"""
```

### Comparing `ont-remora-3.1.0/src/remora/prepare_train_data.py` & `ont_remora-3.2.0/src/remora/prepare_train_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from pathlib import Path
 from collections import defaultdict
 
 import pod5
 import numpy as np
 from tqdm import tqdm
 
@@ -127,28 +128,32 @@
     mod_base,
     mod_base_control,
     motifs,
     focus_ref_pos,
     chunk_context,
     min_samps_per_base,
     max_chunks_per_read,
+    pa_scaling,
     sig_map_refiner,
     kmer_context_bases,
     base_start_justify,
     offset,
     num_reads,
     num_extract_alignment_threads,
     num_extract_chunks_threads,
     skip_non_primary=True,
     basecall_anchor=False,
     rev_sig=False,
     save_every=100_000,
     skip_shuffle=False,
 ):
     bam_idx = ReadIndexedBam(bam_path, skip_non_primary)
+    if bam_idx.num_records == 0:
+        LOGGER.info("No records found in BAM file.")
+        sys.exit()
     with pod5.DatasetReader(Path(pod5_path)) as pod5_dr:
         read_ids, num_reads = get_read_ids(
             bam_idx, pod5_dr, num_reads, return_num_bam_reads=True
         )
     if num_reads == 0:
         return
 
@@ -175,39 +180,43 @@
                     "int64",
                     "Position within read training sequence",
                 ),
             },
             chunk_context=chunk_context,
             kmer_context_bases=kmer_context_bases,
             reverse_signal=rev_sig,
+            pa_scaling=pa_scaling,
             sig_map_refiner=sig_map_refiner,
             base_start_justify=base_start_justify,
             offset=offset,
         ),
     )
 
     LOGGER.info("Processing reads")
     signals = BackgroundIter(
         iter_signal,
         args=(pod5_path,),
         kwargs={
             "num_reads": num_reads,
             "read_ids": read_ids,
             "rev_sig": rev_sig,
+            "pa_scaling": pa_scaling,
         },
         name="ExtractSignal",
         use_process=True,
+        q_maxsize=1000,
     )
     reads = MultitaskMap(
         extract_alignments,
         signals,
         num_workers=num_extract_alignment_threads,
         args=(bam_idx, rev_sig),
         name="AddAlignments",
         use_process=True,
+        q_maxsize=1000,
     )
     chunks = MultitaskMap(
         extract_chunks,
         reads,
         num_workers=num_extract_chunks_threads,
         args=[
             0 if mod_base_control else 1,
@@ -219,14 +228,15 @@
             kmer_context_bases,
             base_start_justify,
             offset,
             basecall_anchor,
         ],
         name="ExtractChunks",
         use_process=True,
+        q_maxsize=1000,
     )
 
     errs = defaultdict(int)
     for read_chunks in tqdm(
         chunks,
         total=len(read_ids),
         smoothing=0,
```

### Comparing `ont-remora-3.1.0/src/remora/refine_signal_map.py` & `ont_remora-3.2.0/src/remora/refine_signal_map.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/refine_signal_map_core.pyx` & `ont_remora-3.2.0/src/remora/refine_signal_map_core.pyx`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/src/remora/train_model.py` & `ont_remora-3.2.0/src/remora/train_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,62 +6,133 @@
 
 import torch
 import numpy as np
 from tqdm import tqdm
 from thop import profile
 from torch.utils.data import DataLoader
 
-from remora.data_chunks import RemoraDataset, dataloader_worker_init
+from remora.data_chunks import (
+    RemoraDataset,
+    CoreRemoraDataset,
+    load_dataset,
+    dataloader_worker_init,
+)
 from remora import (
     constants,
     util,
     log,
     RemoraError,
     model_util,
     validate,
 )
 
 LOGGER = log.get_logger()
 BREACH_THRESHOLD = 0.8
 REGRESSION_THRESHOLD = 0.7
 
 
-def load_optimizer(optimizer, model, lr, weight_decay, momentum=0.9):
-    if optimizer == constants.SGD_OPT:
-        return torch.optim.SGD(
-            model.parameters(),
-            lr=lr,
-            weight_decay=weight_decay,
-            momentum=momentum,
-            nesterov=True,
-        )
-    elif optimizer == constants.ADAM_OPT:
-        return torch.optim.Adam(
-            model.parameters(),
-            lr=lr,
-            weight_decay=weight_decay,
-        )
-    elif optimizer == constants.ADAMW_OPT:
-        return torch.optim.AdamW(
-            model.parameters(),
-            lr=lr,
-            weight_decay=weight_decay,
-        )
-    raise RemoraError(f"Invalid optimizer specified ({optimizer})")
+def med_mad(
+    data, factor=constants.PA_TO_NORM_SCALING_FACTOR, axis=None, keepdims=False
+):
+    """Compute the Median Absolute Deviation, i.e., the median
+    of the absolute deviations from the median, and the median
 
+    Args:
+        data (:class:`ndarray`): Data from which to determine med/mad
+        factor (float): Factor to scale MAD by. Default (None) is to be
+            consistent with the standard deviation of a normal distribution
+            (i.e. mad( N(0,sigma^2) ) = sigma).
+        axis (int): For multidimensional arrays, which axis to calculate over
+        keepdims (bool): If True, axis is kept as dimension of length 1
+
+    :returns: a tuple containing the median and MAD of the data
+    """
+    dmed = np.median(data, axis=axis, keepdims=True)
+    dmad = factor * np.median(abs(data - dmed), axis=axis, keepdims=True)
+    if axis is None:
+        dmed = dmed.flatten()[0]
+        dmad = dmad.flatten()[0]
+    elif not keepdims:
+        dmed = dmed.squeeze(axis)
+        dmad = dmad.squeeze(axis)
+    return dmed, dmad
+
+
+class RollingMAD:
+    """Calculate rolling meadian absolute deviation cap over a specified
+    window for a vector of values
+
+    For example compute gradient maxima by:
+
+        parameters = [p for p in network.parameters() if p.requires_grad]
+        rolling_mads = RollingMAD(len(parameters))
+        grad_maxs = [
+            float(torch.max(torch.abs(layer_params.grad.detach())))
+            for layer_params in parameters]
+        grad_max_threshs = rolling_mads.update(grad_maxs)
+    """
+
+    def __init__(self, nparams, n_mads=0, window=1000, default_to=None):
+        """Set up rolling MAD calculator.
+
+        Args:
+            nparams : Number of parameter arrays to track independently
+            n_mads : Number of MADs above the median to return
+            window : calculation is done over the last <window> data points
+            default_to : Return this value before window values have been added
+        """
+        self.n_mads = n_mads
+        self.default_to = default_to
+        self._window_data = np.empty((nparams, window), dtype="f4")
+        self._curr_iter = 0
+
+    @property
+    def nparams(self):
+        return self._window_data.shape[0]
+
+    @property
+    def window(self):
+        return self._window_data.shape[1]
+
+    def update(self, vals):
+        """Update with time series values and return MAD thresholds.
+
+        Returns:
+            List of `median + (nmods * mad)` of the current window of data.
+                Before window number of values have been added via update the
+                `default_to` value is returned.
+        """
+        assert len(vals) == self.nparams, (
+            f"Number of values ({len(vals)}) provided does not match number of "
+            f"parameters ({self.nparams})."
+        )
 
-def select_scheduler(scheduler, opt, lr_sched_kwargs):
-    lr_sched_dict = {}
-    if lr_sched_kwargs is None and scheduler is None:
-        scheduler = constants.DEFAULT_SCHEDULER
-        lr_sched_dict = constants.DEFAULT_SCH_VALUES
-    else:
-        for lr_key, lr_val, lr_type in lr_sched_kwargs:
-            lr_sched_dict[lr_key] = constants.TYPE_CONVERTERS[lr_type](lr_val)
-    return getattr(torch.optim.lr_scheduler, scheduler)(opt, **lr_sched_dict)
+        self._window_data[:, self._curr_iter % self.window] = vals
+        self._curr_iter += 1
+        if self._curr_iter < self.window:
+            return self.default_to
+
+        med, mad = med_mad(self._window_data, axis=1)
+        return med + (mad * self.n_mads)
+
+
+def apply_clipping(model, grad_max_threshs):
+    parameters = [p for p in model.parameters() if p.requires_grad]
+    grad_maxs = [
+        float(torch.max(torch.abs(param_group.grad.detach())))
+        for param_group in parameters
+    ]
+    if grad_max_threshs is not None:
+        for grp_gm, grp_gmt, grp_params in zip(
+            grad_maxs, grad_max_threshs, parameters
+        ):
+            if grp_gm > grp_gmt:
+                # clip norm by value
+                grp_params.grad.data.clamp_(min=-grp_gmt, max=grp_gmt)
+    return grad_maxs
 
 
 def save_model(
     model,
     ckpt_save_data,
     out_path,
     epoch,
@@ -96,33 +167,28 @@
     out_path,
     remora_dataset_path,
     chunk_context,
     kmer_context_bases,
     batch_size,
     model_path,
     size,
-    optimizer,
-    lr,
-    scheduler_name,
-    weight_decay,
-    epochs,
+    train_opts,
     chunks_per_epoch,
     num_test_chunks,
     save_freq,
-    early_stopping,
     filt_frac,
     ext_val,
     ext_val_names,
-    lr_sched_kwargs,
     high_conf_incorrect_thr_frac,
     finetune_path,
     freeze_num_layers,
     super_batch_size,
     super_batch_sample_frac,
     read_batches_from_disk,
+    gradient_clip_num_mads,
 ):
     seed = (
         np.random.randint(0, np.iinfo(np.uint32).max, dtype=np.uint32)
         if seed is None
         else seed
     )
     LOGGER.info(f"Seed selected is {seed}")
@@ -136,17 +202,25 @@
     LOGGER.info("Loading dataset from Remora dataset config")
     # don't load extra arrays for training
     override_metadata = {"extra_arrays": {}}
     if kmer_context_bases is not None:
         override_metadata["kmer_context_bases"] = kmer_context_bases
     if chunk_context is not None:
         override_metadata["chunk_context"] = chunk_context
-    dataset = RemoraDataset.from_config(
-        remora_dataset_path,
-        override_metadata=override_metadata,
+    paths, props, hashes = load_dataset(remora_dataset_path)
+    dataset = RemoraDataset(
+        [
+            CoreRemoraDataset(
+                path,
+                override_metadata=override_metadata,
+            )
+            for path in paths
+        ],
+        props,
+        hashes,
         batch_size=batch_size,
         super_batch_size=super_batch_size,
         super_batch_sample_frac=super_batch_sample_frac,
     )
     # TODO move hash computation into background worker and write this from
     # that worker as well. This command stalls startup too much
     with open(os.path.join(out_path, "dataset_config.jsn"), "w") as ds_cfg_fh:
@@ -172,14 +246,33 @@
         "size": size,
         "kmer_len": dataset.metadata.kmer_len,
         "num_out": dataset.metadata.num_labels,
     }
     model = model_util._load_python_model(copy_model_path, **model_params)
     LOGGER.info(f"Model structure:\n{model}")
 
+    grad_max_threshs = None
+    # TODO add to batch log
+    # grad_max_thresh_str = "NaN"
+    if gradient_clip_num_mads is None:
+        LOGGER.debug("No gradient clipping")
+        rolling_mads = None
+    else:
+        nparams = len([p for p in model.parameters() if p.requires_grad])
+        if nparams == 0:
+            rolling_mads = None
+            LOGGER.warning("No gradient clipping due to missing parameters")
+        else:
+            rolling_mads = RollingMAD(nparams, gradient_clip_num_mads)
+            LOGGER.info(
+                "Gradients will be clipped (by value) at "
+                f"{rolling_mads.n_mads:3.2f} MADs above the median of the "
+                f"last {rolling_mads.window} gradient maximums."
+            )
+
     if finetune_path is not None:
         ckpt, model = model_util.continue_from_checkpoint(
             finetune_path, copy_model_path
         )
         if freeze_num_layers:
             for freeze_iter, (p_name, param) in enumerate(
                 model.named_parameters()
@@ -206,29 +299,35 @@
         if dataset.metadata.kmer_context_bases != ckpt["kmer_context_bases"]:
             raise RemoraError(
                 "The kmer context bases of the pre-trained model and "
                 "the dataset do not match."
             )
 
     if ext_val is not None:
-        LOGGER.debug("Loading external test data")
+        LOGGER.info("Loading external validation data")
         if ext_val_names is None:
             ext_val_names = [f"e_val_{idx}" for idx in range(len(ext_val))]
         else:
             assert len(ext_val_names) == len(ext_val)
         ext_datasets = []
         for e_name, e_path in zip(ext_val_names, ext_val):
-            ext_val_ds = RemoraDataset.from_config(
-                e_path.strip(),
-                ds_kwargs={
-                    "infinite_iter": False,
-                    "do_check_super_batches": True,
-                },
+            paths, props, hashes = load_dataset(e_path.strip())
+            ext_val_ds = RemoraDataset(
+                [
+                    CoreRemoraDataset(
+                        path,
+                        override_metadata=override_metadata,
+                        infinite_iter=False,
+                        do_check_super_batches=True,
+                    )
+                    for path in paths
+                ],
+                props,
+                hashes,
                 batch_size=batch_size,
-                super_batch_size=super_batch_size,
             )
             ext_val_ds.update_metadata(dataset)
             if not read_batches_from_disk:
                 ext_val_ds.load_all_batches()
             ext_datasets.append((e_name, ext_val_ds))
 
     kmer_dim = int(dataset.metadata.kmer_len * 4)
@@ -245,17 +344,17 @@
         f"Params (k) {params / (1000):.2f} | MACs (M) {macs / (1000 ** 2):.2f}"
     )
 
     LOGGER.info("Preparing training settings")
     criterion = torch.nn.CrossEntropyLoss()
     model = model.to(device)
     criterion = criterion.to(device)
-    opt = load_optimizer(optimizer, model, lr, weight_decay)
-
-    scheduler = select_scheduler(scheduler_name, opt, lr_sched_kwargs)
+    LOGGER.info(f"Training optimizer and scheduler settings: {train_opts}")
+    opt = train_opts.load_optimizer(model)
+    scheduler = train_opts.load_scheduler(opt)
 
     LOGGER.debug("Splitting dataset")
     trn_ds, val_ds = dataset.train_test_split(
         num_test_chunks,
         override_metadata=override_metadata,
     )
     val_ds.super_batch_sample_frac = None
@@ -313,15 +412,15 @@
                 ext_ds,
                 filt_frac,
                 ext_name,
             )
 
     LOGGER.info("Start training")
     ebar = tqdm(
-        total=epochs,
+        total=train_opts.epochs,
         smoothing=0,
         desc="Epochs",
         dynamic_ncols=True,
         position=0,
         leave=True,
         disable=os.environ.get("LOG_SAFE", False),
     )
@@ -357,20 +456,21 @@
         "reverse_signal": dataset.metadata.reverse_signal,
         "mod_bases": dataset.metadata.mod_bases,
         "mod_long_names": dataset.metadata.mod_long_names,
         "modified_base_labels": dataset.metadata.modified_base_labels,
         "kmer_context_bases": dataset.metadata.kmer_context_bases,
         "base_start_justify": dataset.metadata.base_start_justify,
         "offset": dataset.metadata.offset,
+        "pa_scaling": dataset.metadata.pa_scaling,
         **dataset.metadata.sig_map_refiner.asdict(),
     }
     best_val_acc = 0
     early_stop_epochs = 0
     breached = False
-    for epoch in range(epochs):
+    for epoch in range(train_opts.epochs):
         model.train()
         pbar.n = 0
         pbar.refresh()
         for epoch_i, (enc_kmers, sigs, labels) in enumerate(
             islice(trn_loader, batches_per_epoch)
         ):
             outputs = model(sigs.to(device), enc_kmers.to(device))
@@ -394,15 +494,19 @@
                     conf_thresh = max(conf_thresh, mm_preds[max_nr_skip])
                 mask = cl_match.logical_or(highest_preds < conf_thresh)
                 # avoid sending labels to device until after above computations
                 loss = criterion(outputs[mask], labels[mask].to(device))
 
             opt.zero_grad()
             loss.backward()
+            grad_maxs = apply_clipping(model, grad_max_threshs)
             opt.step()
+            if rolling_mads is not None:
+                grad_max_threshs = rolling_mads.update(grad_maxs)
+
             batch_fp.write(
                 f"{(epoch * batches_per_epoch) + epoch_i}\t"
                 f"{loss.detach().cpu():.6f}"
             )
             if high_conf_incorrect_thr_frac is None:
                 batch_fp.write("\n")
             else:
@@ -508,22 +612,28 @@
         ebar.set_postfix(
             acc_val=f"{val_metrics.acc:.4f}",
             acc_train=f"{trn_metrics.acc:.4f}",
             loss_val=f"{val_metrics.loss:.6f}",
             loss_train=f"{trn_metrics.loss:.6f}",
         )
         ebar.update()
-        if early_stopping and early_stop_epochs >= early_stopping:
+        if (
+            train_opts.early_stopping
+            and early_stop_epochs >= train_opts.early_stopping
+        ):
             break
     ebar.close()
     pbar.close()
-    if early_stopping and early_stop_epochs >= early_stopping:
+    if (
+        train_opts.early_stopping
+        and early_stop_epochs >= train_opts.early_stopping
+    ):
         LOGGER.info(
-            f"No validation accuracy improvement after {early_stopping} "
-            "epochs. Training stopped early."
+            "No validation accuracy improvement after "
+            f"{train_opts.early_stopping} epochs. Training stopped early."
         )
     LOGGER.info("Saving final model checkpoint")
     save_model(
         model,
         ckpt_save_data,
         out_path,
         epoch,
```

### Comparing `ont-remora-3.1.0/src/remora/util.py` & `ont_remora-3.2.0/src/remora/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import toml
 import array
 import queue
 import platform
 import traceback
 from abc import ABC
 from time import sleep
 from pathlib import Path
@@ -43,15 +44,15 @@
 BASES_TO_CODES = dict((v, k) for k, v in SINGLE_LETTER_CODE.items())
 SEQ_MIN = np.array(["A"], dtype="S1").view(np.uint8)[0]
 SEQ_TO_INT_ARR = np.full(26, -1, dtype=int)
 SEQ_TO_INT_ARR[0] = 0
 SEQ_TO_INT_ARR[2] = 1
 SEQ_TO_INT_ARR[6] = 2
 SEQ_TO_INT_ARR[19] = 3
-COMP_BASES = dict(zip(map(ord, "ACGT"), map(ord, "TGCA")))
+COMP_BASES = dict(zip(map(ord, "ACGTBVDHKMRY"), map(ord, "TGCAVBHDMKYR")))
 NP_COMP_BASES = np.array([3, 2, 1, 0], dtype=np.uintp)
 U_TO_T_BASES = {ord("U"): ord("T")}
 T_TO_U_BASES = {ord("T"): ord("U")}
 
 DEFAULT_QUEUE_SIZE = 10_000
 
 
@@ -88,26 +89,38 @@
     device = torch.device(device)
     if device.type == "cuda" and not torch.cuda.is_available():
         LOGGER.warning("Device option specified, but CUDA not available.")
     return device
 
 
 def comp(seq):
+    """Convert seq to its complement sequence.
+    Handles IUPAC ambiguous bases.
+    """
     return seq.translate(COMP_BASES)
 
 
 def revcomp(seq):
+    """Convert seq to its complement sequence and reverse the sequence.
+    Handles IUPAC ambiguous bases.
+    """
     return seq.upper().translate(COMP_BASES)[::-1]
 
 
 def comp_np(np_seq):
+    """Convert numpy seq to its complement sequence.
+    Does NOT handles IUPAC ambiguous bases.
+    """
     return NP_COMP_BASES[np_seq]
 
 
 def revcomp_np(np_seq):
+    """Convert numpy seq to its complement sequence and reverse the sequence.
+    Does NOT handles IUPAC ambiguous bases.
+    """
     return NP_COMP_BASES[np_seq][::-1]
 
 
 def u_to_t(seq):
     return seq.translate(U_TO_T_BASES)
 
 
@@ -474,15 +487,15 @@
     https://samtools.github.io/hts-specs/SAMtags.pdf for format details.
 
     Args:
         seq (str): read-centric read sequence. For reference-anchored calls
             this should be the reverse complement sequence.
         poss (list): positions relative to seq
         probs (np.array): probabilities for modified bases
-        mod_bases (str): modified base single letter codes
+        mod_bases (list): modified base single letter codes
         can_base (str): canonical base
         strand (bool): should be '+' for SEQ-oriented strand and '-' if
             complement strand
 
     Returns:
         MM string tag and ML array tag
     """
@@ -520,14 +533,37 @@
         # last interval includes prob=1
         scaled_probs[scaled_probs == 256] = 255
         ml_tag.extend(scaled_probs.astype(np.uint8))
 
     return mm_tag, ml_tag
 
 
+def parse_picoamps(bc_model, sig_map_refiner):
+    if bc_model is None:
+        return
+    if sig_map_refiner.do_rough_rescale or sig_map_refiner.scale_iters > -1:
+        raise RemoraError(
+            "Cannot specify signal scaling/mapping refinement and "
+            "picoamp scaling options."
+        )
+    bc_cfg = Path(bc_model) / "config.toml"
+    if not bc_cfg.exists():
+        raise RemoraError(f"Basecalling model config does not exist: {bc_cfg}")
+    cfg = toml.load(bc_cfg)
+    try:
+        std_cfg = cfg["standardisation"]
+        do_std = std_cfg["standardise"]
+        pa_scaling = (std_cfg["mean"], std_cfg["stdev"])
+    except KeyError:
+        raise RemoraError("Basecalling model is not picoamp scaling model")
+    if do_std != 1:
+        raise RemoraError("Basecalling model is not picoamp scaling model")
+    return pa_scaling
+
+
 def profile(prof_path):
     if prof_path is not None:
         import cProfile
 
     def inner(func):
         def wrapper(*args, **kwargs):
             if prof_path is None:
```

### Comparing `ont-remora-3.1.0/src/remora/validate.py` & `ont_remora-3.2.0/src/remora/validate.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/tests/test_coding_standards.py` & `ont_remora-3.2.0/tests/test_coding_standards.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/tests/test_duplex.py` & `ont_remora-3.2.0/tests/test_duplex.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/tests/test_main.py` & `ont_remora-3.2.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ont-remora-3.1.0/tests/test_notebooks.py` & `ont_remora-3.2.0/tests/test_notebooks.py`

 * *Files identical despite different names*

