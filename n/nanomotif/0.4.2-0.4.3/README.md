# Comparing `tmp/nanomotif-0.4.2.tar.gz` & `tmp/nanomotif-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomotif-0.4.2.tar", last modified: Mon May 13 12:28:48 2024, max compression
+gzip compressed data, was "nanomotif-0.4.3.tar", last modified: Tue May 21 09:42:41 2024, max compression
```

## Comparing `nanomotif-0.4.2.tar` & `nanomotif-0.4.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:48.376263 nanomotif-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 12:28:40.000000 nanomotif-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-13 12:28:48.376263 nanomotif-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-05-13 12:28:40.000000 nanomotif-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:48.336264 nanomotif-0.4.2/nanomotif/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/bin_consensus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:48.340264 nanomotif-0.4.2/nanomotif/binnary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/binnary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/binnary/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/binnary/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/binnary/detect_contamination.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/binnary/include_contigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/binnary/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/binnary/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/binnary/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/dataload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:48.340264 nanomotif-0.4.2/nanomotif/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/datasets/geobacillus-contig-bin.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   176247 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
--rw-r--r--   0 runner    (1001) docker     (127) 26479844 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/datasets/geobacillus-plasmids.pileup.bed
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    28603 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:48.372264 nanomotif-0.4.2/nanomotif/mtase_linker/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/mtase_linker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/mtase_linker/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/mtase_linker/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/old_search_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/scoremotifs.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-13 12:28:40.000000 nanomotif-0.4.2/nanomotif/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:48.376263 nanomotif-0.4.2/nanomotif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-13 12:28:48.000000 nanomotif-0.4.2/nanomotif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-13 12:28:48.000000 nanomotif-0.4.2/nanomotif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:28:48.000000 nanomotif-0.4.2/nanomotif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 12:28:48.000000 nanomotif-0.4.2/nanomotif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:28:48.000000 nanomotif-0.4.2/nanomotif.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 12:28:48.000000 nanomotif-0.4.2/nanomotif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 12:28:48.000000 nanomotif-0.4.2/nanomotif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:28:48.376263 nanomotif-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-13 12:28:40.000000 nanomotif-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:48.372264 nanomotif-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:48.376263 nanomotif-0.4.2/tests/binnary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/test_arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/test_cli_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/test_data_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/test_detect_contamination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/test_generate_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/test_include_contigs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/test_scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/binnary/test_write_bins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/test_candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/test_dataload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/test_motif_find.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:28:40.000000 nanomotif-0.4.2/tests/test_motif_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.719247 nanomotif-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-21 09:42:37.000000 nanomotif-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-21 09:42:41.719247 nanomotif-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-21 09:42:37.000000 nanomotif-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.683247 nanomotif-0.4.3/nanomotif/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/bin_consensus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.683247 nanomotif-0.4.3/nanomotif/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/dataload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.683247 nanomotif-0.4.3/nanomotif/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/datasets/geobacillus-contig-bin.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   176247 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
+-rw-r--r--   0 runner    (1001) docker     (127) 26479844 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/datasets/geobacillus-plasmids.pileup.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28633 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20030 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.715247 nanomotif-0.4.3/nanomotif/mtase_linker/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/mtase_linker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/mtase_linker/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/mtase_linker/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/old_search_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/scoremotifs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.719247 nanomotif-0.4.3/nanomotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:42:41.719247 nanomotif-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-21 09:42:37.000000 nanomotif-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.719247 nanomotif-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.719247 nanomotif-0.4.3/tests/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_data_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_generate_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_write_bins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/test_candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/test_dataload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/test_motif_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/test_motif_score.py
```

### Comparing `nanomotif-0.4.2/LICENSE` & `nanomotif-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/PKG-INFO` & `nanomotif-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.4.2
+Version: 0.4.3
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -17,14 +17,16 @@
 Requires-Dist: pyarrow>=15.0.2
 Requires-Dist: Bio>=1.6.2
 Requires-Dist: snakemake>=7.32.4
 Requires-Dist: progressbar2>=3.53.1
 
 # Nanomotif
 
+#### *OBS: Bioconda is currently down for pushing new versions, we therefore recommend using pip for installing Nanomotif, see [here](https://nanomotif.readthedocs.io/en/latest/installation.html#local-environment)*
+
 Nanomotif is a Python package designed to explore methylation in prokaryotic genomes using Nanopore sequencing. Nanomotif is a fast, scalable, and sensitive tool for identification and utilization of methylation motifs in monocultures and metagenomic samples.
   - [Overview](#nanomotif-offers)
   - [Documentation](#documentation)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Citation](#citation)
```

### Comparing `nanomotif-0.4.2/README.md` & `nanomotif-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Nanomotif
 
+#### *OBS: Bioconda is currently down for pushing new versions, we therefore recommend using pip for installing Nanomotif, see [here](https://nanomotif.readthedocs.io/en/latest/installation.html#local-environment)*
+
 Nanomotif is a Python package designed to explore methylation in prokaryotic genomes using Nanopore sequencing. Nanomotif is a fast, scalable, and sensitive tool for identification and utilization of methylation motifs in monocultures and metagenomic samples.
   - [Overview](#nanomotif-offers)
   - [Documentation](#documentation)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Citation](#citation)
```

### Comparing `nanomotif-0.4.2/nanomotif/argparser.py` & `nanomotif-0.4.3/nanomotif/argparser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/bin_consensus.py` & `nanomotif-0.4.3/nanomotif/bin_consensus.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,78 +49,63 @@
     bin_motifs = contig_motifs.groupby("bin", "motif", "mod_position", "mod_type") \
         .agg(
             pl.col("n_mod").sum().alias("n_mod_bin"),
             pl.col("n_nomod").sum().alias("n_nomod_bin"),
             pl.col("contig").count().alias("contig_count")
         ).with_columns( 
             pl.col("motif").apply(lambda x: nm.utils.motif_type(x)).alias("motif_type"),
-            (pl.col("n_mod_bin") / (pl.col("n_mod_bin") + pl.col("n_nomod_bin"))).alias("mean_sum")
+            (pl.col("n_mod_bin") / (pl.col("n_mod_bin") + pl.col("n_nomod_bin"))).alias("mean_methylation")
         )
     return bin_motifs
 
+def merge_bin_motifs(bin_motifs, bins, pileup, assembly):
+    assert list(bin_motifs.schema.keys()) == ['bin', 'motif', 'mod_position', 'mod_type', 'n_mod_bin', 'n_nomod_bin', 'contig_count', 'motif_type', 'mean_methylation']
 
-
-def merge_motifs_in_df(motif_df, pileup, assembly, mean_shift_threshold = -0.25):
-    # DEPRECATED CURRENTLY
-    new_df = []
-    for (contig, mod_type), df in motif_df.groupby("contig", "mod_type"):
+    for (bin, mod_type), df in bin_motifs.groupby("bin", "mod_type"):
+        contig_count = df.get_column("contig_count").max()
+        
         # Get list of motifs
         motif_seq = df["motif"].to_list()
         motif_pos = df["mod_position"].to_list()
-        motifs = [nm.candidate.Motif(seq, pos) for seq, pos in zip(motif_seq, motif_pos)]
-
-        # Merge motifs
+        motifs = [nm.candidate.Motif(nm.candidate.iupac_to_regex(seq), pos) for seq, pos in zip(motif_seq, motif_pos)]
+        
         merged_motifs = nm.candidate.merge_motifs(motifs)
-        all_merged_motifs = []
-        all_premerge_motifs = []
-        # Check mean shift of premerge motifs to merged motif is high enough
         for cluster, motifs in merged_motifs.items():
             merged_motif = motifs[0]
             premerge_motifs = motifs[1]
-            merge_mean = nm.evaluate.motif_model_contig(
-                pileup.filter((col("contig") == contig) & (col("mod_type") == mod_type)), 
-                assembly.assembly[contig].sequence,
-                merged_motif
-            ).mean()
-            pre_merge_means = []
-            for pre_merge_motif in premerge_motifs:
-                pre_merge_means.append(nm.evaluate.motif_model_contig(
-                    pileup.filter((col("contig") == contig) & (col("mod_type") == mod_type)), 
-                    assembly.assembly[contig].sequence,
-                    pre_merge_motif
-                ).mean())
-            
-            pre_merge_mean = sum(np.array(pre_merge_means)) / len(pre_merge_means)
-            mean_shift = merge_mean - pre_merge_mean
-            if mean_shift < mean_shift_threshold:
-                log.info(f"Mean shift of merged motif {merged_motif} is {mean_shift}, keeping original motifs")
-            
-            else:
-                log.info(f"Mean shift of merged motif {merged_motif} is {mean_shift}")
-                all_merged_motifs.append(merged_motif)
-                all_premerge_motifs.extend(premerge_motifs)
 
-        # Create a new dataframe with the non merged motifs
-        if  len(all_premerge_motifs) == 0:
-            # No motifs were merged
-            new_df.append(df)
-            continue
-        single_df = df.filter(col("motif").is_in(all_premerge_motifs).not_())
-        new_df.append(single_df)
-        merged_df = []
-        for motif in all_merged_motifs:
-            merged_model = nm.evaluate.motif_model_contig(
-                pileup.filter((col("contig") == contig) & (col("mod_type") == mod_type)), 
-                assembly.assembly[contig].sequence,
-                motif
-            )
-            merged_df.append(pl.DataFrame({
-                "contig": contig,
-                "mod_type": mod_type,
-                "n_mod": merged_model._alpha,
-                "n_nomod": merged_model._beta - 1,
-                "motif": nm.candidate.regex_to_iupac(motif.string),
-                "mod_position": motif.mod_position
-            }))
-        new_df.append(pl.concat(merged_df))
-    new_df = pl.concat(new_df)
-    return new_df
+            premerge_motifs_iupac = [motif.iupac() for motif in premerge_motifs]
+            previous_motif_mean_max = bin_motifs.filter(pl.col("motif").is_in(premerge_motifs_iupac)).get_column("mean_methylation").max()
+
+            merge_motif_n_mod = 0
+            merge_motif_n_nomod = 0
+            for contig in bins.filter(pl.col("bin") == bin).get_column("contig").unique():
+                merge_motif_model = nm.evaluate.motif_model_contig(
+                            pileup.pileup.filter((pl.col("contig") == contig) & (pl.col("mod_type") == mod_type)), 
+                            assembly.assembly[contig].sequence,
+                            merged_motif
+                        )
+                
+                merge_motif_n_mod += merge_motif_model._alpha
+                merge_motif_n_nomod += merge_motif_model._beta
+            merge_motif_mean = merge_motif_n_mod / (merge_motif_n_mod + merge_motif_n_nomod)
+
+            if merge_motif_mean - previous_motif_mean_max > -0.1:
+                bin_motifs = bin_motifs.filter(pl.col("motif").is_in(premerge_motifs_iupac).not_())
+                bin_motifs = pl.concat(
+                    [bin_motifs,
+                    pl.DataFrame(
+                        {
+                            "bin": bin,
+                            "motif": merged_motif.iupac(),
+                            "mod_position": merged_motif.mod_position,
+                            "mod_type": mod_type,
+                            "n_mod_bin": merge_motif_n_mod,
+                            "n_nomod_bin": merge_motif_n_nomod,
+                            "contig_count": contig_count,
+                            "motif_type": nm.utils.motif_type(merged_motif.iupac()),
+                            "mean_methylation": merge_motif_mean
+                        },
+                        schema=bin_motifs.schema
+                    )]
+                )
+    return bin_motifs
```

### Comparing `nanomotif-0.4.2/nanomotif/binnary/analysis.py` & `nanomotif-0.4.3/nanomotif/binnary/analysis.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/binnary/data_processing.py` & `nanomotif-0.4.3/nanomotif/binnary/data_processing.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/binnary/detect_contamination.py` & `nanomotif-0.4.3/nanomotif/binnary/detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/binnary/include_contigs.py` & `nanomotif-0.4.3/nanomotif/binnary/include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/binnary/logging.py` & `nanomotif-0.4.3/nanomotif/binnary/logging.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/binnary/scoring.py` & `nanomotif-0.4.3/nanomotif/binnary/scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/binnary/utils.py` & `nanomotif-0.4.3/nanomotif/binnary/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/candidate.py` & `nanomotif-0.4.3/nanomotif/candidate.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 class Motif(str):
     def __new__(cls, motif_string, *args, **kwargs):
         return str.__new__(cls, motif_string)
     
     def __init__(self, _, mod_position):
         self.mod_position = mod_position
         self.string = self.__str__()
-
-    def from_iupac(iupac_motif):
+    def from_iupac(self):
         """
-        Generate Motif from IUPAC seqeunce
+        Create a motif from an IUPAC string.
         """
+        regex = iupac_to_regex(self.string)
+        return Motif(regex, self.mod_position)
     def iupac(self):
         """
         Get IUPAC sequence of motif
         """
         return regex_to_iupac(self.string)
     def identical(self, other_motif):
         """
@@ -219,23 +220,24 @@
 
         # Split the motifs into lists of bases
         motif_split = self.split()
         other_split = other.split()
 
         motif_right = len(motif_split) - mod_pos 
         other_right = len(other_split) - mod_pos_other
+
         # Pad the shorter motif with '.' to ensure equal lengths for merging
         if mod_pos < mod_pos_other:
             motif_split = ['.'] * abs(offset) + motif_split
-        else:
+        elif mod_pos > mod_pos_other:
             other_split = ['.'] * abs(offset) + other_split
 
         if motif_right < other_right:
             motif_split = motif_split + ['.'] * (other_right - motif_right)
-        else:
+        elif motif_right > other_right:
             other_split = other_split + ['.'] * (motif_right - other_right)
         # Merge the motifs base by base, keeping the modification position aligned
         merged_motif_string = ''.join([self.merge_bases(base, base_other) for base, base_other in zip(motif_split, other_split)])
 
         # The modification position in the merged motif is the same as in the original motifs
         merged_mod_position = mod_pos + abs(offset)
```

### Comparing `nanomotif-0.4.2/nanomotif/constants.py` & `nanomotif-0.4.3/nanomotif/constants.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/dataload.py` & `nanomotif-0.4.3/nanomotif/dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/datasets/geobacillus-plasmids.assembly.fasta` & `nanomotif-0.4.3/nanomotif/datasets/geobacillus-plasmids.assembly.fasta`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/datasets/geobacillus-plasmids.pileup.bed` & `nanomotif-0.4.3/nanomotif/datasets/geobacillus-plasmids.pileup.bed`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/datasets.py` & `nanomotif-0.4.3/nanomotif/datasets.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/evaluate.py` & `nanomotif-0.4.3/nanomotif/evaluate.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
     pool.join()
 
     # Close the progress bar
     progress_bar_process.join()
 
     if len(results) == 0:
         return None
-    motifs = pl.concat(results)
+    motifs = pl.concat(results, rechunk=True, parallel=False)
 
     model_col = []
     for a, b in zip(motifs.get_column("alpha").to_list(), motifs.get_column("beta").to_list()):
         model_col.append(BetaBernoulliModel(a, b))
 
     motifs = motifs.with_columns([
             pl.Series(model_col).alias("model"),
```

### Comparing `nanomotif-0.4.2/nanomotif/feature.py` & `nanomotif-0.4.3/nanomotif/feature.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/main.py` & `nanomotif-0.4.3/nanomotif/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 import shutil
 from pathlib import Path
 import json
 os.environ["POLARS_MAX_THREADS"] = "1"
 import polars as pl
+from polars import col
 import numpy as np
 import random
 import warnings
 from nanomotif._version import __version__
 
 
 def shared_setup(args, working_dir):
@@ -83,32 +84,37 @@
             threshold_methylation_general = args.threshold_methylation_general,
             threshold_valid_coverage = args.threshold_valid_coverage,
             minimum_kl_divergence = args.minimum_kl_divergence,
             verbose = args.verbose,
             log_dir = args.out + "/logs",
             seed = args.seed
         )
-
+    motifs = pl.DataFrame(motifs)
     if motifs is None:
         log.info("No motifs found")
         return
 
     log.info("Writing motifs")
-
+    pl.show_versions()
     def format_motif_df(df):
         if "model" in df.columns:
-            df = df.with_columns(
-                pl.col("model").apply(lambda x: x._alpha).alias("n_mod"),
-                pl.col("model").apply(lambda x: x._beta).alias("n_nomod")
-            )
+            n_mod = [x._alpha for x in df["model"]]
+            n_nomod = [x._beta for x in df["model"]]
+        motif_iupac = [nm.seq.regex_to_iupac(x) for x in df["motif"]]
+        motif_type = [nm.utils.motif_type(x) for x in motif_iupac]
+
         df_out = df.with_columns([
-            pl.col("motif").apply(lambda x: nm.seq.regex_to_iupac(x)).alias("motif")
-        ]).with_columns([
-            pl.col("motif").apply(lambda x: nm.utils.motif_type(x)).alias("motif_type")
-        ]).unique(["motif", "contig", "mod_type", "mod_position"])
+            pl.Series("motif", motif_iupac),
+            pl.Series("motif_type", motif_type)
+        ])
+        if "model" in df.columns:
+            df_out = df_out.with_columns([
+                pl.Series("n_mod", n_mod),
+                pl.Series("n_nomod", n_nomod)
+            ])
         try:
             df_out = df_out.select([
                 "contig", "motif", "mod_position", "mod_type", "n_mod", "n_nomod", "motif_type",
                 "motif_complement", "mod_position_complement", "n_mod_complement", "n_nomod_complement"
             ])
         except:
             df_out = df_out.select([
@@ -122,15 +128,15 @@
     os.makedirs(args.out + "/precleanup-motifs/", exist_ok=True)
     save_motif_df(motifs, "precleanup-motifs/motifs-raw")
 
     log.info("Postprocessing motifs")
     motifs_file_name = "precleanup-motifs/motifs"
 
     log.info(" - Writing motifs")
-    motifs = motifs.filter(pl.col("score") > 0.1)
+    motifs = motifs.filter(col("score") > 0.1)
     if len(motifs) == 0:
         log.info("No motifs found")
         return
     
     motifs_file_name = motifs_file_name + "-score"
     save_motif_df(motifs, motifs_file_name)
 
@@ -265,14 +271,16 @@
             .select(pl.all().name.map(lambda col_name: col_name.replace('_complement', ''))) \
             .select(motifs_fwd.columns) \
             .filter(pl.col("motif").is_not_null())
         motifs = pl.concat([motifs_fwd, motifs_rev]).unique(["motif", "contig", "mod_type", "mod_position"])
 
 
     output = nm.bin_consensus.within_bin_motifs_consensus(pileup.pileup, assembly, motifs, motifs_scored, bins)
+    output = nm.bin_consensus.merge_bin_motifs(output, bins, pileup, assembly)
+
     output = output.rename({"bin":"contig", "n_mod_bin":"n_mod", "n_nomod_bin":"n_nomod"})
 
     output = nm.postprocess.join_motif_complements(output)
 
     output = output.rename({"contig":"bin", "n_mod":"n_mod_bin", "n_nomod":"n_nomod_bin"})
     output = output.sort(["bin", "mod_type", "motif"])
     output.write_csv(args.out + "/bin-motifs.tsv", separator="\t")
```

### Comparing `nanomotif-0.4.2/nanomotif/model.py` & `nanomotif-0.4.3/nanomotif/model.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/mtase_linker/command.py` & `nanomotif-0.4.3/nanomotif/mtase_linker/command.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/mtase_linker/dependencies.py` & `nanomotif-0.4.3/nanomotif/mtase_linker/dependencies.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/old_search_method.py` & `nanomotif-0.4.3/nanomotif/old_search_method.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/parallel.py` & `nanomotif-0.4.3/nanomotif/parallel.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/postprocess.py` & `nanomotif-0.4.3/nanomotif/postprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,18 +109,22 @@
             }))
         new_df.append(pl.concat(merged_df))
     new_df = pl.concat(new_df)
     return new_df
 
 def join_motif_complements(motif_df):
     if "model" in motif_df.columns:
-        motif_df = motif_df.with_columns(
-            pl.col("model").map_elements(lambda x: x._alpha).alias("n_mod"),
-            pl.col("model").map_elements(lambda x: x._beta).alias("n_nomod")
-        ).drop("model")
+        if "model" in motif_df.columns:
+            n_mod = [x._alpha for x in motif_df["model"]]
+            n_nomod = [x._beta for x in motif_df["model"]]
+
+            motif_df = motif_df.with_columns([
+                pl.Series("n_mod", n_mod),
+                pl.Series("n_nomod", n_nomod)
+            ]).drop(["model"])
     motif_df = motif_df.select([
         "contig", "mod_type", "motif", "mod_position", "n_mod", "n_nomod"
     ])
     motif_df = motif_df.with_columns([
         pl.col("motif").apply(lambda x: nm.candidate.regex_to_iupac(x)).alias("motif")
     ]).with_columns([
         pl.col("motif").apply(lambda x: nm.utils.motif_type(x)).alias("motif_type")
```

### Comparing `nanomotif-0.4.2/nanomotif/scoremotifs.py` & `nanomotif-0.4.3/nanomotif/scoremotifs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/seq.py` & `nanomotif-0.4.3/nanomotif/seq.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif/utils.py` & `nanomotif-0.4.3/nanomotif/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/nanomotif.egg-info/PKG-INFO` & `nanomotif-0.4.3/nanomotif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.4.2
+Version: 0.4.3
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -17,14 +17,16 @@
 Requires-Dist: pyarrow>=15.0.2
 Requires-Dist: Bio>=1.6.2
 Requires-Dist: snakemake>=7.32.4
 Requires-Dist: progressbar2>=3.53.1
 
 # Nanomotif
 
+#### *OBS: Bioconda is currently down for pushing new versions, we therefore recommend using pip for installing Nanomotif, see [here](https://nanomotif.readthedocs.io/en/latest/installation.html#local-environment)*
+
 Nanomotif is a Python package designed to explore methylation in prokaryotic genomes using Nanopore sequencing. Nanomotif is a fast, scalable, and sensitive tool for identification and utilization of methylation motifs in monocultures and metagenomic samples.
   - [Overview](#nanomotif-offers)
   - [Documentation](#documentation)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Citation](#citation)
```

### Comparing `nanomotif-0.4.2/nanomotif.egg-info/SOURCES.txt` & `nanomotif-0.4.3/nanomotif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/setup.py` & `nanomotif-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/conftest.py` & `nanomotif-0.4.3/tests/binnary/conftest.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/test_arg_parser.py` & `nanomotif-0.4.3/tests/binnary/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/test_cli_commands.py` & `nanomotif-0.4.3/tests/binnary/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/test_data_processing_functions.py` & `nanomotif-0.4.3/tests/binnary/test_data_processing_functions.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/test_detect_contamination.py` & `nanomotif-0.4.3/tests/binnary/test_detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/test_generate_output.py` & `nanomotif-0.4.3/tests/binnary/test_generate_output.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/test_include_contigs.py` & `nanomotif-0.4.3/tests/binnary/test_include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/test_scoring.py` & `nanomotif-0.4.3/tests/binnary/test_scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/test_utils.py` & `nanomotif-0.4.3/tests/binnary/test_utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/binnary/test_write_bins.py` & `nanomotif-0.4.3/tests/binnary/test_write_bins.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/test_candidate.py` & `nanomotif-0.4.3/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/test_dataload.py` & `nanomotif-0.4.3/tests/test_dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.2/tests/test_motif_find.py` & `nanomotif-0.4.3/tests/test_motif_find.py`

 * *Files identical despite different names*

