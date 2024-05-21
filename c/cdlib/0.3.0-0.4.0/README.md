# Comparing `tmp/cdlib-0.3.0.tar.gz` & `tmp/cdlib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdlib-0.3.0.tar", last modified: Thu Jun  8 09:23:51 2023, max compression
+gzip compressed data, was "cdlib-0.4.0.tar", last modified: Tue May 21 09:37:56 2024, max compression
```

## Comparing `cdlib-0.3.0.tar` & `cdlib-0.4.0.tar`

### file list

```diff
@@ -1,122 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 09:23:40.000000 cdlib-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 09:23:40.000000 cdlib-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-08 09:23:51.870546 cdlib-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-08 09:23:40.000000 cdlib-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.858546 cdlib-0.3.0/cdlib/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.862546 cdlib-0.3.0/cdlib/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/attribute_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/bipartite_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)   104945 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/crisp_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/edge_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.866546 cdlib-0.3.0/cdlib/algorithms/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/AGDL.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/BIGCLAM.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/COACH.py
--rw-r--r--   0 runner    (1001) docker     (123)    22041 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/CONGA.py
--rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/CONGO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/DCS.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/DER.py
--rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/DPCLUS.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/EBGC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/EnDNTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/FuzzyCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/GDMP2_nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/HLC.py
--rw-r--r--   0 runner    (1001) docker     (123)    17301 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/ILouvain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/IPCA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/Kcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LAIS2_nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LEMON.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LPAM.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LPANNI.py
--rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LSWL.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/MCODE.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/Markov.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/NodePerception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/OSSE.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/PercoMCV.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/RSC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/SLPA_nx.py
--rw-r--r--   0 runner    (1001) docker     (123)    29121 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/SiblinarityAntichain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/UMSTMO.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/belief_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/core_exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/ga.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/graph_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/headtail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/lfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/modularity_m.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/modularity_r.py
--rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/multicom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/paris.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/principled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/pycondor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/spectralCD.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/walkscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/weightedCommunity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.866546 cdlib-0.3.0/cdlib/algorithms/internal_dcd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal_dcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13960 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal_dcd/eTILES.py
--rw-r--r--   0 runner    (1001) docker     (123)    70332 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/overlapping_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/temporal_partition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.866546 cdlib-0.3.0/cdlib/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/dynamic_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.866546 cdlib-0.3.0/cdlib/benchmark/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/internal/rdyn.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/internal/xmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/static_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/attr_node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/bipartite_node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/edge_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/fuzzy_node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/named_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    38635 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/temporal_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/datasets/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/ensemble/bunch_executions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/comparisonranking.py
--rw-r--r--   0 runner    (1001) docker     (123)    43486 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/fitnessranking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/evaluation/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/TOPSIS.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/link_modularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/omega.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/onmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/statistical_ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/prompt_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/readwrite/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/readwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/readwrite/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/viz/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/viz/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/viz/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.862546 cdlib-0.3.0/cdlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 09:23:40.000000 cdlib-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 09:23:51.870546 cdlib-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-08 09:23:40.000000 cdlib-0.3.0/setup.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.359856 cdlib-0.4.0/
+-rw-r--r--   0 rossetti   (501) staff       (20)     1298 2022-12-07 16:48:08.000000 cdlib-0.4.0/LICENSE
+-rw-r--r--   0 rossetti   (501) staff       (20)       58 2022-12-07 16:48:08.000000 cdlib-0.4.0/MANIFEST.in
+-rw-r--r--   0 rossetti   (501) staff       (20)     7487 2024-05-21 09:37:56.360213 cdlib-0.4.0/PKG-INFO
+-rw-r--r--   0 rossetti   (501) staff       (20)     6692 2023-06-08 09:30:02.000000 cdlib-0.4.0/README.md
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.321903 cdlib-0.4.0/cdlib/
+-rw-r--r--   0 rossetti   (501) staff       (20)      518 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/__init__.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.326322 cdlib-0.4.0/cdlib/algorithms/
+-rw-r--r--   0 rossetti   (501) staff       (20)      205 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     5380 2023-06-08 07:56:19.000000 cdlib-0.4.0/cdlib/algorithms/attribute_clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    11030 2023-09-03 07:36:01.000000 cdlib-0.4.0/cdlib/algorithms/bipartite_clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)   106290 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/algorithms/crisp_partition.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     1812 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/edge_clustering.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.343289 cdlib-0.4.0/cdlib/algorithms/internal/
+-rw-r--r--   0 rossetti   (501) staff       (20)     7058 2023-06-06 11:21:17.000000 cdlib-0.4.0/cdlib/algorithms/internal/AGDL.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     2675 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/BIGCLAM.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     5562 2023-06-06 19:22:34.000000 cdlib-0.4.0/cdlib/algorithms/internal/COACH.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    22041 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/CONGA.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    23967 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/CONGO.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    14836 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/DCS.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     8951 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/DER.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    15849 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/DPCLUS.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     5501 2023-06-06 19:25:31.000000 cdlib-0.4.0/cdlib/algorithms/internal/EBGC.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     2317 2023-06-06 19:25:31.000000 cdlib-0.4.0/cdlib/algorithms/internal/EnDNTM.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3674 2023-06-06 11:21:17.000000 cdlib-0.4.0/cdlib/algorithms/internal/FuzzyCom.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     5398 2023-06-07 02:03:23.000000 cdlib-0.4.0/cdlib/algorithms/internal/GDMP2_nx.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     8289 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/HLC.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    17301 2022-12-09 09:16:15.000000 cdlib-0.4.0/cdlib/algorithms/internal/ILouvain.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4335 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/IPCA.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3718 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/Kcut.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4182 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/LAIS2_nx.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     7446 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/LEMON.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     5774 2023-06-06 19:20:15.000000 cdlib-0.4.0/cdlib/algorithms/internal/LPAM.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     6237 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/LPANNI.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    22712 2023-06-06 19:25:31.000000 cdlib-0.4.0/cdlib/algorithms/internal/LSWL.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4921 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/MCODE.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3198 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/Markov.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    13034 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/NodePerception.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     6727 2022-12-09 09:16:15.000000 cdlib-0.4.0/cdlib/algorithms/internal/OSSE.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3580 2023-06-06 19:25:36.000000 cdlib-0.4.0/cdlib/algorithms/internal/PercoMCV.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     7307 2024-05-13 09:01:30.000000 cdlib-0.4.0/cdlib/algorithms/internal/RSC.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     2335 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/SLPA_nx.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    29121 2023-06-07 02:09:16.000000 cdlib-0.4.0/cdlib/algorithms/internal/SiblinarityAntichain.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4581 2023-06-06 19:25:31.000000 cdlib-0.4.0/cdlib/algorithms/internal/UMSTMO.py
+-rw-r--r--   0 rossetti   (501) staff       (20)        0 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     8421 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/belief_prop.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    10362 2023-06-06 19:22:59.000000 cdlib-0.4.0/cdlib/algorithms/internal/core_exp.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     2838 2024-05-13 06:58:27.000000 cdlib-0.4.0/cdlib/algorithms/internal/em.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4889 2023-06-06 11:21:17.000000 cdlib-0.4.0/cdlib/algorithms/internal/ga.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4609 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/graph_entropy.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     1626 2023-06-06 19:25:31.000000 cdlib-0.4.0/cdlib/algorithms/internal/headtail.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3961 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/lfm.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     6898 2024-05-13 09:01:30.000000 cdlib-0.4.0/cdlib/algorithms/internal/markov_clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     5707 2023-06-06 19:25:31.000000 cdlib-0.4.0/cdlib/algorithms/internal/modularity_m.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4451 2023-06-06 19:25:31.000000 cdlib-0.4.0/cdlib/algorithms/internal/modularity_r.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     9827 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/multicom.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4358 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/paris.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     1421 2023-06-06 19:14:09.000000 cdlib-0.4.0/cdlib/algorithms/internal/principled.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     7147 2024-05-13 06:58:27.000000 cdlib-0.4.0/cdlib/algorithms/internal/pycondor.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3210 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/scan.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3098 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/spectralCD.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3523 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/walkscan.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     7785 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal/weightedCommunity.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.343711 cdlib-0.4.0/cdlib/algorithms/internal_dcd/
+-rw-r--r--   0 rossetti   (501) staff       (20)        0 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal_dcd/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    13960 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/algorithms/internal_dcd/eTILES.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    70332 2023-06-07 01:38:12.000000 cdlib-0.4.0/cdlib/algorithms/overlapping_partition.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     2810 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/algorithms/temporal_partition.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.344313 cdlib-0.4.0/cdlib/benchmark/
+-rw-r--r--   0 rossetti   (501) staff       (20)       65 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/benchmark/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3537 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/benchmark/dynamic_benchmark.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.344998 cdlib-0.4.0/cdlib/benchmark/internal/
+-rw-r--r--   0 rossetti   (501) staff       (20)        0 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/benchmark/internal/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    19426 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/benchmark/internal/rdyn.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    12369 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/benchmark/internal/xmark.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    15939 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/benchmark/static_benchmark.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.347389 cdlib-0.4.0/cdlib/classes/
+-rw-r--r--   0 rossetti   (501) staff       (20)      350 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/classes/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     1309 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/classes/attr_node_clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     1053 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/classes/bipartite_node_clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3875 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/classes/clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     1776 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/classes/edge_clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     1494 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/classes/fuzzy_node_clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)      835 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/classes/named_clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    57685 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/classes/node_clustering.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     5248 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/classes/temporal_clustering.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.347912 cdlib-0.4.0/cdlib/datasets/
+-rw-r--r--   0 rossetti   (501) staff       (20)       22 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/datasets/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    15225 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/datasets/remote.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.348417 cdlib-0.4.0/cdlib/ensemble/
+-rw-r--r--   0 rossetti   (501) staff       (20)       32 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/ensemble/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    11122 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/ensemble/bunch_executions.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.350465 cdlib-0.4.0/cdlib/evaluation/
+-rw-r--r--   0 rossetti   (501) staff       (20)      112 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/evaluation/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    42349 2024-05-14 11:49:21.000000 cdlib-0.4.0/cdlib/evaluation/comparison.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     9237 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/evaluation/comparisonranking.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    43500 2024-05-14 11:50:08.000000 cdlib-0.4.0/cdlib/evaluation/fitness.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     9387 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/evaluation/fitnessranking.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.352573 cdlib-0.4.0/cdlib/evaluation/internal/
+-rw-r--r--   0 rossetti   (501) staff       (20)     4859 2024-05-13 06:58:27.000000 cdlib-0.4.0/cdlib/evaluation/internal/NF1.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3041 2022-12-09 09:16:15.000000 cdlib-0.4.0/cdlib/evaluation/internal/TOPSIS.py
+-rw-r--r--   0 rossetti   (501) staff       (20)        0 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/evaluation/internal/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4057 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/evaluation/internal/link_modularity.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     2816 2022-12-09 09:16:15.000000 cdlib-0.4.0/cdlib/evaluation/internal/omega.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     4971 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/evaluation/internal/onmi.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     3999 2022-12-09 09:16:15.000000 cdlib-0.4.0/cdlib/evaluation/internal/statistical_ranking.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.352764 cdlib-0.4.0/cdlib/lifecycles/
+-rw-r--r--   0 rossetti   (501) staff       (20)       73 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/__init__.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.354580 cdlib-0.4.0/cdlib/lifecycles/algorithms/
+-rw-r--r--   0 rossetti   (501) staff       (20)      109 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/algorithms/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     9505 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/algorithms/classic_match.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     8108 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/algorithms/event_analysis.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     6209 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/algorithms/measures.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     5635 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/algorithms/null_model.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.356060 cdlib-0.4.0/cdlib/lifecycles/classes/
+-rw-r--r--   0 rossetti   (501) staff       (20)       45 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/classes/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    32917 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/classes/event.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     9770 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/classes/matching.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.356755 cdlib-0.4.0/cdlib/lifecycles/utils/
+-rw-r--r--   0 rossetti   (501) staff       (20)       21 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/utils/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     1876 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/lifecycles/utils/utils.py
+-rw-r--r--   0 rossetti   (501) staff       (20)      471 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/prompt_utils.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.357366 cdlib-0.4.0/cdlib/readwrite/
+-rw-r--r--   0 rossetti   (501) staff       (20)       18 2022-12-07 16:48:08.000000 cdlib-0.4.0/cdlib/readwrite/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     8977 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/readwrite/io.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     7578 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/utils.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.359345 cdlib-0.4.0/cdlib/viz/
+-rw-r--r--   0 rossetti   (501) staff       (20)       77 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/viz/__init__.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    15803 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/viz/community_events.py
+-rw-r--r--   0 rossetti   (501) staff       (20)    21305 2024-05-21 08:34:29.000000 cdlib-0.4.0/cdlib/viz/networks.py
+-rw-r--r--   0 rossetti   (501) staff       (20)     6306 2023-06-06 12:27:53.000000 cdlib-0.4.0/cdlib/viz/plots.py
+drwxr-xr-x   0 rossetti   (501) staff       (20)        0 2024-05-21 09:37:56.323130 cdlib-0.4.0/cdlib.egg-info/
+-rw-r--r--   0 rossetti   (501) staff       (20)     7487 2024-05-21 09:37:56.000000 cdlib-0.4.0/cdlib.egg-info/PKG-INFO
+-rw-r--r--   0 rossetti   (501) staff       (20)     4050 2024-05-21 09:37:56.000000 cdlib-0.4.0/cdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 rossetti   (501) staff       (20)        1 2024-05-21 09:37:56.000000 cdlib-0.4.0/cdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 rossetti   (501) staff       (20)      442 2024-05-21 09:37:56.000000 cdlib-0.4.0/cdlib.egg-info/requires.txt
+-rw-r--r--   0 rossetti   (501) staff       (20)        6 2024-05-21 09:37:56.000000 cdlib-0.4.0/cdlib.egg-info/top_level.txt
+-rw-r--r--   0 rossetti   (501) staff       (20)      206 2024-05-21 08:34:29.000000 cdlib-0.4.0/requirements.txt
+-rw-r--r--   0 rossetti   (501) staff       (20)       53 2024-05-21 09:37:56.360583 cdlib-0.4.0/setup.cfg
+-rw-r--r--   0 rossetti   (501) staff       (20)     2426 2024-05-21 09:34:42.000000 cdlib-0.4.0/setup.py
```

### Comparing `cdlib-0.3.0/LICENSE` & `cdlib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/PKG-INFO` & `cdlib-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdlib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Community Discovery Library
 Home-page: https://github.com/GiulioRossetti/cdlib
 Author: Giulio Rossetti
 Author-email: giulio.rossetti@gmail.com
 License: BSD-Clause-2
 Keywords: community-discovery node-clustering edge-clustering complex-networks
 Classifier: Development Status :: 4 - Beta
@@ -86,27 +86,27 @@
 conda install cdlib
 ```
 
 ### Optional Dependencies (pip package)
 To simplify the installation process, the default installation does not include optional dependencies (e.g., ``graph-tool``). If you need them, you can install them manually or run the following command:
 
 ```bash
-pip install cdlib[C]
+pip install 'cdlib[C]'
 ```
 
 This option, safe for *nix users, will install all those optional dependencies that require C code compilation.
 
 ```bash
-pip install cdlib[pypi]
+pip install 'cdlib[pypi]'
 ```
 
 This option will install all those optional dependencies that are not available on conda/conda-forge.
 
 ```bash
-pip install cdlib[all]
+pip install 'cdlib[all]'
 ```
 
 This option will install all optional dependencies accessible with the flag ``C`` and ``pypi``.
 
 #### (Advanced) 
 
 Due to some strict requirements, the installation of a subset of optional dependencies is left outside the previous procedures.
```

### Comparing `cdlib-0.3.0/README.md` & `cdlib-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -63,27 +63,27 @@
 conda install cdlib
 ```
 
 ### Optional Dependencies (pip package)
 To simplify the installation process, the default installation does not include optional dependencies (e.g., ``graph-tool``). If you need them, you can install them manually or run the following command:
 
 ```bash
-pip install cdlib[C]
+pip install 'cdlib[C]'
 ```
 
 This option, safe for *nix users, will install all those optional dependencies that require C code compilation.
 
 ```bash
-pip install cdlib[pypi]
+pip install 'cdlib[pypi]'
 ```
 
 This option will install all those optional dependencies that are not available on conda/conda-forge.
 
 ```bash
-pip install cdlib[all]
+pip install 'cdlib[all]'
 ```
 
 This option will install all optional dependencies accessible with the flag ``C`` and ``pypi``.
 
 #### (Advanced) 
 
 Due to some strict requirements, the installation of a subset of optional dependencies is left outside the previous procedures.
```

### Comparing `cdlib-0.3.0/cdlib/algorithms/attribute_clustering.py` & `cdlib-0.4.0/cdlib/algorithms/attribute_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/bipartite_clustering.py` & `cdlib-0.4.0/cdlib/algorithms/bipartite_clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 __all__ = ["bimlpa", "CPM_Bipartite", "infomap_bipartite", "condor"]
 
 
 def bimlpa(g_original: object, theta: float = 0.3, lambd: int = 7) -> BiNodeClustering:
     """
     BiMLPA is designed to detect the many-to-many correspondence community in bipartite networks using multi-label propagation algorithm.
 
+    This method works for the connected graph. If the graph is not connected, the method will be applied to each connected component of the graph and the results will be merged.
 
     **Supported Graph Types**
 
     ========== ======== ======== =========
     Undirected Directed Weighted Bipartite
     ========== ======== ======== =========
     Yes        No       No       Yes
@@ -56,15 +57,15 @@
     :return: BiNodeClustering object
 
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
-    >>> G = nx.algorithms.bipartite.generators.random_graph(100, 20, 0.1)
+    >>> G = nx.algorithms.bipartite.random_graph(50, 50, 0.25)
     >>> coms = algorithms.bimlpa(G)
 
     :References:
 
     Taguchi, Hibiki, Tsuyoshi Murata, and Xin Liu. "BiMLPA: Community Detection in Bipartite Networks by Multi-Label Propagation." International Conference on Network Science. Springer, Cham, 2020.
 
     .. note:: Reference implementation: https://github.com/hbkt/BiMLPA
@@ -119,15 +120,15 @@
     :return: BiNodeClustering object
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
     >>> G = nx.algorithms.bipartite.generators.random_graph(100, 20, 0.5)
-    >>> coms = algorithms.CPM_Bipartite(G, 1)
+    >>> coms = algorithms.CPM_Bipartite(G, 0.5)
 
     :References:
 
     Barber, M. J. (2007). Modularity and community detection in bipartite networks. Physical Review E, 76(6), 066102. 10.1103/PhysRevE.76.066102
 
     .. note:: Reference implementation: https://leidenalg.readthedocs.io/en/stable/multiplex.html?highlight=bipartite#bipartite
     """
@@ -197,15 +198,15 @@
     :param flags: str flags for Infomap
     :return: BiNodeClustering object
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
+    >>> G = nx.algorithms.bipartite.generators.random_graph(100, 20, 0.5)
     >>> coms = algorithms.infomap_bipartite(G)
 
     :References:
 
     Rosvall M, Bergstrom CT (2008) `Maps of random walks on complex networks reveal community structure. <https://www.pnas.org/content/105/4/1118/>`_ Proc Natl Acad SciUSA 105(4):1118–1123
 
     .. note:: Reference implementation: https://pypi.org/project/infomap/
@@ -284,25 +285,25 @@
 
 
     **Supported Graph Types**
 
     ========== ======== ======== =========
     Undirected Directed Weighted Bipartite
     ========== ======== ======== =========
-    Yes        No       No       Yes
+    Yes        No       Yes      Yes
     ========== ======== ======== =========
 
     :param g_original: a networkx/igraph object
     :return: BiNodeClustering object
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
+    >>> G = nx.algorithms.bipartite.random_graph(50, 50, 0.25)
     >>> coms = algorithms.condor(G)
 
     :References:
 
     Platig, J., Castaldi, P. J., DeMeo, D., & Quackenbush, J. (2016). Bipartite community structure of eQTLs. PLoS computational biology, 12(9), e1005033.
 
     .. note:: Reference implementation: https://github.com/genisott/pycondor
```

### Comparing `cdlib-0.3.0/cdlib/algorithms/crisp_partition.py` & `cdlib-0.4.0/cdlib/algorithms/crisp_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,18 @@
 from cdlib.algorithms.internal.headtail import HeadTail
 from cdlib.algorithms.internal.Kcut import kcut_exec
 from cdlib.algorithms.internal.paris import paris as paris_alg, paris_best_clustering
 from cdlib.algorithms.internal.principled import principled
 from cdlib.algorithms.internal.MCODE import m_code
 from cdlib.algorithms.internal.RSC import rsc_evaluate_graph
 from cdlib.prompt_utils import report_missing_packages, prompt_import_failure
+import cdlib.algorithms.internal.markov_clustering as mc
 
 import warnings
 
-import markov_clustering as mc
-
 # from chinese_whispers import chinese_whispers as cw
 # from chinese_whispers import aggregate_clusters
 from thresholdclustering.thresholdclustering import best_partition as th_best_partition
 import networkx as nx
 
 from cdlib.utils import (
     convert_graph_formats,
@@ -87,14 +86,15 @@
 
 try:
     import bayanpy as by
 except ModuleNotFoundError:
     missing_packages.add("bayanpy")
     by = None
 
+
 # try:
 #    import karateclub
 # except ModuleNotFoundError:
 #    missing_packages.add("karateclub")
 
 
 report_missing_packages(missing_packages)
@@ -489,14 +489,15 @@
         "AGDL",
         method_parameters={"number_communities": number_communities, "kc": kc},
     )
 
 
 def louvain(
     g_original: object,
+    partition: NodeClustering = None,
     weight: str = "weight",
     resolution: float = 1.0,
     randomize: int = None,
 ) -> NodeClustering:
     """
     Louvain  maximizes a modularity score for each community.
     The algorithm optimises the modularity in two elementary phases:
@@ -508,42 +509,54 @@
 
 
     **Supported Graph Types**
 
     ========== ======== ========
     Undirected Directed Weighted
     ========== ======== ========
-    Yes        No       No
+    Yes        No       Yes
     ========== ======== ========
 
     :param g_original: a networkx/igraph object
-    :param weight: str, optional the key in graph to use as weight. Default to 'weight'
+    :param partition: NodeClustering object, optional the algorithm will start using this partition of the nodes
+    :param weight: str, optional the key in graph to use as weight. Default to "weight"
     :param resolution: double, optional  Will change the size of the communities, default to 1.
-    :param randomize: int, RandomState instance or None, optional (default=None). If int, random_state is the seed used by the random number generator; If RandomState instance, random_state is the random number generator; If None, the random number generator is the RandomState instance used by `np.random`.
+    :param randomize: int, RandomState instance or None, optional (default=None).
     :return: NodeClustering object
 
-
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
     >>> G = nx.karate_club_graph()
     >>> coms = algorithms.louvain(G, weight='weight', resolution=1.)
 
     :References:
 
     Blondel, Vincent D., et al. `Fast unfolding of communities in large networks. <https://iopscience.iop.org/article/10.1088/1742-5468/2008/10/P10008/meta/>`_ Journal of statistical mechanics: theory and experiment 2008.10 (2008): P10008.
 
     .. note:: Reference implementation: https://github.com/taynaud/python-louvain
+
     """
 
     g = convert_graph_formats(g_original, nx.Graph)
 
+    if partition is not None:
+        communities = {}
+        for idc, com in enumerate(partition.communities):
+            for n in com:
+                communities[n] = idc
+        partition = communities
+
     coms = community_louvain.best_partition(
-        g, weight=weight, resolution=resolution, randomize=randomize
+        g,
+        partition=partition,
+        weight=weight,
+        resolution=resolution,
+        randomize=randomize,
     )
 
     # Reshaping the results
     coms_to_node = defaultdict(list)
     for n, c in coms.items():
         coms_to_node[c].append(n)
 
@@ -572,15 +585,15 @@
 
 
     **Supported Graph Types**
 
     ========== ======== ========
     Undirected Directed Weighted
     ========== ======== ========
-    Yes        No       No
+    Yes        No       Yes
     ========== ======== ========
 
     :param g_original: a networkx/igraph object
     :param initial_membership:  list of int Initial membership for the partition. If :obj:`None` then defaults to a singleton partition. Deafault None
     :param weights: list of double, or edge attribute Weights of edges. Can be either an iterable or an edge attribute. Deafault None
     :return: NodeClustering object
 
@@ -673,18 +686,23 @@
 
     Reichardt, J., & Bornholdt, S. (2006).  `Statistical mechanics of community detection. <https://journals.aps.org/pre/abstract/10.1103/PhysRevE.74.016110/>`_  Physical Review E, 74(1), 016110. 10.1103/PhysRevE.74.016110
 
     Leicht, E. A., & Newman, M. E. J. (2008).  `Community Structure in Directed Networks. <https://www.ncbi.nlm.nih.gov/pubmed/18517839/>`_  Physical Review Letters, 100(11), 118703. 10.1103/PhysRevLett.100.118703
 
     """
 
-    if ig is None:
-        raise ModuleNotFoundError(
-            "Optional dependency not satisfied: install igraph to use the selected feature."
-        )
+    global leidenalg
+    if ig is None or leidenalg is None:
+        try:
+            import leidenalg
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "Optional dependency not satisfied: install igraph and leidenalg to use the "
+                "selected feature."
+            )
 
     g = convert_graph_formats(g_original, ig.Graph)
 
     part = leidenalg.find_partition(
         g,
         leidenalg.RBConfigurationVertexPartition,
         resolution_parameter=resolution_parameter,
@@ -747,18 +765,23 @@
     Reichardt, J., & Bornholdt, S. (2006).  `Statistical mechanics of community detection. <https://journals.aps.org/pre/abstract/10.1103/PhysRevE.74.016110/>`_  Physical Review E, 74(1), 016110. 10.1103/PhysRevE.74.016110
 
 
     .. note:: Reference implementation: https://github.com/vtraag/leidenalg
 
     """
 
-    if ig is None:
-        raise ModuleNotFoundError(
-            "Optional dependency not satisfied: install igraph to use the selected feature."
-        )
+    global leidenalg
+    if ig is None or leidenalg is None:
+        try:
+            import leidenalg
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "Optional dependency not satisfied: install igraph and leidenalg to use the "
+                "selected feature."
+            )
 
     g = convert_graph_formats(g_original, ig.Graph)
 
     part = leidenalg.find_partition(
         g,
         leidenalg.RBERVertexPartition,
         resolution_parameter=resolution_parameter,
@@ -833,18 +856,23 @@
     Traag, V. A., Van Dooren, P., & Nesterov, Y. (2011).  `Narrow scope for resolution-limit-free community detection. <https://journals.aps.org/pre/abstract/10.1103/PhysRevE.84.016114/>`_ Physical Review E, 84(1), 016114. 10.1103/PhysRevE.84.016114
 
 
     .. note:: Reference implementation: https://github.com/vtraag/leidenalg
 
     """
 
-    if ig is None:
-        raise ModuleNotFoundError(
-            "Optional dependency not satisfied: install igraph to use the selected feature."
-        )
+    global leidenalg
+    if ig is None or leidenalg is None:
+        try:
+            import leidenalg
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "Optional dependency not satisfied: install igraph and leidenalg to use the "
+                "selected feature."
+            )
 
     g = convert_graph_formats(g_original, ig.Graph)
 
     part = leidenalg.find_partition(
         g,
         leidenalg.CPMVertexPartition,
         resolution_parameter=resolution_parameter,
@@ -905,18 +933,23 @@
 
     Traag, V. A., Krings, G., & Van Dooren, P. (2013). `Significant scales in community structure. <https://www.nature.com/articles/srep02930/>`_  Scientific Reports, 3, 2930. `10.1038/srep02930 <http://doi.org/10.1038/srep02930>`
 
     .. note:: Reference implementation: https://github.com/vtraag/leidenalg
 
     """
 
-    if ig is None:
-        raise ModuleNotFoundError(
-            "Optional dependency not satisfied: install igraph to use the selected feature."
-        )
+    global leidenalg
+    if ig is None or leidenalg is None:
+        try:
+            import leidenalg
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "Optional dependency not satisfied: install igraph and leidenalg to use the "
+                "selected feature."
+            )
 
     g = convert_graph_formats(g_original, ig.Graph)
 
     part = leidenalg.find_partition(
         g,
         leidenalg.SignificanceVertexPartition,
         initial_membership=initial_membership,
@@ -979,18 +1012,23 @@
 
     Traag, V. A., Aldecoa, R., & Delvenne, J.-C. (2015).  `Detecting communities using asymptotical surprise. <https://journals.aps.org/pre/abstract/10.1103/PhysRevE.92.022816/>`_ Physical Review E, 92(2), 022816. 10.1103/PhysRevE.92.022816
 
     .. note:: Reference implementation: https://github.com/vtraag/leidenalg
 
     """
 
-    if ig is None:
-        raise ModuleNotFoundError(
-            "Optional dependency not satisfied: install igraph to use the selected feature."
-        )
+    global leidenalg
+    if ig is None or leidenalg is None:
+        try:
+            import leidenalg
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "Optional dependency not satisfied: install igraph and leidenalg to use the "
+                "selected feature."
+            )
 
     g = convert_graph_formats(g_original, ig.Graph)
 
     part = leidenalg.find_partition(
         g,
         leidenalg.SurpriseVertexPartition,
         initial_membership=initial_membership,
@@ -2647,17 +2685,29 @@
 
     :References:
 
     Bonald, T., Charpentier, B., Galland, A., & Hollocou, A. (2018). Hierarchical graph clustering using node pair sampling. arXiv preprint arXiv:1806.01664.
 
     .. note:: Reference implementation: https://github.com/tbonald/paris
     """
+
     g = convert_graph_formats(g_original, nx.Graph)
-    D = paris_alg(g)
-    clustering = paris_best_clustering(D)
+
+    dmap = {n: i for i, n in enumerate(g.nodes)}
+    reverse_map = {i: n for n, i in dmap.items()}
+    nx.relabel_nodes(g_original, dmap, False)
+
+    D = paris_alg(g_original)
+    coms = paris_best_clustering(D)
+
+    clustering = []
+
+    for com in coms:
+        com = [reverse_map[c] for c in com]
+        clustering.append(com)
 
     return NodeClustering(
         clustering, g_original, "Paris", method_parameters={}, overlap=False
     )
 
 
 def ricci_community(
@@ -2723,15 +2773,15 @@
         method_parameters={"alpha": alpha, "method": method},
         overlap=False,
     )
 
 
 def spectral(
     g_original: object,
-    kmax: int,
+    kmax: int = 2,
     projection_on_smaller_class: bool = True,
     scaler: Callable = None,
 ) -> NodeClustering:
     """
     SCD implements a Spectral Clustering algorithm for Communities Discovery.
     It is based on Fielder’s vector (obtained from the eigenvector related to the second eigenvalue of the normalized Laplacian) that are leveraged to extract the communities using Kmeans clustering.
     SCD a hierarchical graph clustering algorithm inspired by modularity-based clustering techniques.
@@ -2739,30 +2789,30 @@
 
 
     **Supported Graph Types**
 
     ========== ======== ======== =========
     Undirected Directed Weighted Bipartite
     ========== ======== ======== =========
-    Yes        No       No       Yes
+    Yes        No       No       No
     ========== ======== ======== =========
 
     :param g_original: a networkx/igraph object
-    :param kmax: maximum number of desired communities
+    :param kmax: maximum number of desired communities (mandatory). Default 2.
     :param projection_on_smaller_class: a boolean value that if True then it project a bipartite network in the smallest class of node. (default is True)
     :param scaler: the function to scale the fielder’s vector to apply KMeans
     :return: NodeClustering object
 
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
     >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.spectral(G)
+    >>> coms = algorithms.spectral(G, kmax=2)
 
     :References:
 
     Higham, Desmond J., Gabriela Kalna, and Milla Kibble. "Spectral clustering and its use in bioinformatics." Journal of computational and applied mathematics 204.1 (2007): 25-37.
 
     .. note:: Implementation provided by Gianmarco Pepi <g.pepi2@unipi.it>,  Monia Bennici <m.bennici4@studenti.unipi.it>,  Khashayar Abtin <k.abtin@studenti.unipi.it> and Kamran Mehravar <k.mehravar@studenti.unipi.it> (Computer Science Dept., University of Pisa, Italy)
     """
```

### Comparing `cdlib-0.3.0/cdlib/algorithms/edge_clustering.py` & `cdlib-0.4.0/cdlib/algorithms/edge_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/AGDL.py` & `cdlib-0.4.0/cdlib/algorithms/internal/AGDL.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/BIGCLAM.py` & `cdlib-0.4.0/cdlib/algorithms/internal/BIGCLAM.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/COACH.py` & `cdlib-0.4.0/cdlib/algorithms/internal/COACH.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/CONGA.py` & `cdlib-0.4.0/cdlib/algorithms/internal/CONGA.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/CONGO.py` & `cdlib-0.4.0/cdlib/algorithms/internal/CONGO.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/DCS.py` & `cdlib-0.4.0/cdlib/algorithms/internal/DCS.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/DER.py` & `cdlib-0.4.0/cdlib/algorithms/internal/DER.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/DPCLUS.py` & `cdlib-0.4.0/cdlib/algorithms/internal/DPCLUS.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/EBGC.py` & `cdlib-0.4.0/cdlib/algorithms/internal/EBGC.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/EnDNTM.py` & `cdlib-0.4.0/cdlib/algorithms/internal/EnDNTM.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/FuzzyCom.py` & `cdlib-0.4.0/cdlib/algorithms/internal/FuzzyCom.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/GDMP2_nx.py` & `cdlib-0.4.0/cdlib/algorithms/internal/GDMP2_nx.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/HLC.py` & `cdlib-0.4.0/cdlib/algorithms/internal/HLC.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/ILouvain.py` & `cdlib-0.4.0/cdlib/algorithms/internal/ILouvain.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/IPCA.py` & `cdlib-0.4.0/cdlib/algorithms/internal/IPCA.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/Kcut.py` & `cdlib-0.4.0/cdlib/algorithms/internal/Kcut.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/LAIS2_nx.py` & `cdlib-0.4.0/cdlib/algorithms/internal/LAIS2_nx.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/LEMON.py` & `cdlib-0.4.0/cdlib/algorithms/internal/LEMON.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/LPAM.py` & `cdlib-0.4.0/cdlib/algorithms/internal/LPAM.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/LPANNI.py` & `cdlib-0.4.0/cdlib/algorithms/internal/LPANNI.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/LSWL.py` & `cdlib-0.4.0/cdlib/algorithms/internal/LSWL.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/MCODE.py` & `cdlib-0.4.0/cdlib/algorithms/internal/MCODE.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/Markov.py` & `cdlib-0.4.0/cdlib/algorithms/internal/Markov.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/NodePerception.py` & `cdlib-0.4.0/cdlib/algorithms/internal/NodePerception.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/OSSE.py` & `cdlib-0.4.0/cdlib/algorithms/internal/OSSE.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/PercoMCV.py` & `cdlib-0.4.0/cdlib/algorithms/internal/PercoMCV.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/RSC.py` & `cdlib-0.4.0/cdlib/algorithms/internal/RSC.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,31 @@
     [2]Kamalika Chaudhuri, Fan Chung, and Alexander Tsiatas 2018.
         Spectral clustering of graphs with general degrees in the extended planted partition model.
     L = I - D^-1/2 * A * D ^-1/2
     :param adj_matrix: adjacency matrix representation of graph where [m][n] >0 if there is edge and [m][n] = weight
     :param tau: the regularisation constant
     :return: the first K eigenvector
     """
-    import scipy.sparse
+    import scipy.sparse as sp
+    import scipy
 
     # Code inspired from nx.normalized_laplacian_matrix, with changes to allow regularisation
     n, m = adj_matrix.shape
     I = np.eye(n, m)
     diags = adj_matrix.sum(axis=1).flatten()
     # add tau to the diags to produce a regularised diags
     if tau != 0:
         diags = np.add(diags, tau)
 
     # diags will be zero at points where there is no edge and/or the node you are at
     #  ignore the error and make it zero later
-    with scipy.errstate(divide="ignore"):
-        diags_sqrt = 1.0 / scipy.sqrt(diags)
-    diags_sqrt[scipy.isinf(diags_sqrt)] = 0
-    D = scipy.sparse.spdiags(diags_sqrt, [0], m, n, format="csr")
+    # with scipy.errstate(divide="ignore"):
+    diags_sqrt = 1.0 / np.sqrt(diags)
+    diags_sqrt[np.isinf(diags_sqrt)] = 0
+    D = sp.spdiags(diags_sqrt, [0], m, n, format="csr")
 
     L = I - (D.dot(adj_matrix.dot(D)))
     return L
 
 
 def __eigen_solver(laplacian, n_clusters):
     """
```

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/SLPA_nx.py` & `cdlib-0.4.0/cdlib/algorithms/internal/SLPA_nx.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/SiblinarityAntichain.py` & `cdlib-0.4.0/cdlib/algorithms/internal/SiblinarityAntichain.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/UMSTMO.py` & `cdlib-0.4.0/cdlib/algorithms/internal/UMSTMO.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/belief_prop.py` & `cdlib-0.4.0/cdlib/algorithms/internal/belief_prop.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/core_exp.py` & `cdlib-0.4.0/cdlib/algorithms/internal/core_exp.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/em.py` & `cdlib-0.4.0/cdlib/algorithms/internal/em.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             for g in range(self.k):
                 x = self.pi[g]
                 for j in self.g.neighbors(i):
                     x *= self.theta[g][j]
                 q[i].append(x)
                 norm += x
             for g in range(self.k):
-                q[i][g] /= (norm + 1e-10)  # tolerance adjustment
+                q[i][g] /= norm + 1e-10  # tolerance adjustment
 
     def m_step(self, q):
         for g in range(self.k):
             sum1 = 0.0
             sum3 = 0.0
             for i in range(self.n):
                 sum1 += q[i][g]
```

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/ga.py` & `cdlib-0.4.0/cdlib/algorithms/internal/ga.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/graph_entropy.py` & `cdlib-0.4.0/cdlib/algorithms/internal/graph_entropy.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/headtail.py` & `cdlib-0.4.0/cdlib/algorithms/internal/headtail.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/lfm.py` & `cdlib-0.4.0/cdlib/algorithms/internal/lfm.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/modularity_m.py` & `cdlib-0.4.0/cdlib/algorithms/internal/modularity_m.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/modularity_r.py` & `cdlib-0.4.0/cdlib/algorithms/internal/modularity_r.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/multicom.py` & `cdlib-0.4.0/cdlib/algorithms/internal/multicom.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/paris.py` & `cdlib-0.4.0/cdlib/algorithms/internal/paris.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/principled.py` & `cdlib-0.4.0/cdlib/algorithms/internal/principled.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/pycondor.py` & `cdlib-0.4.0/cdlib/algorithms/internal/pycondor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import numpy as np
 import pandas as pd
-from igraph import *
+
+try:
+    from igraph import Graph
+except ModuleNotFoundError:
+    raise (
+        "This module requires the igraph package. Please install it with pip install python-igraph."
+    )
 
 
 def condor_object(net):
     """Initialization of the condor object. The function gets a network in edgelist format encoded in a pandas
     dataframe. Returns a dictionary with an igraph network, names of the targets and regulators, list of edges,
     modularity, and vertex memberships.
     """
```

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/scan.py` & `cdlib-0.4.0/cdlib/algorithms/internal/scan.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/spectralCD.py` & `cdlib-0.4.0/cdlib/algorithms/internal/spectralCD.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/walkscan.py` & `cdlib-0.4.0/cdlib/algorithms/internal/walkscan.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal/weightedCommunity.py` & `cdlib-0.4.0/cdlib/algorithms/internal/weightedCommunity.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/internal_dcd/eTILES.py` & `cdlib-0.4.0/cdlib/algorithms/internal_dcd/eTILES.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/overlapping_partition.py` & `cdlib-0.4.0/cdlib/algorithms/overlapping_partition.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/algorithms/temporal_partition.py` & `cdlib-0.4.0/cdlib/algorithms/temporal_partition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from cdlib import TemporalClustering, NamedClustering
 from cdlib.algorithms.internal_dcd.eTILES import eTILES
+import networkx as nx
 
 __all__ = ["tiles"]
 
 
 def tiles(dg: object, obs: int = 1) -> TemporalClustering:
     """
     TILES is designed to incrementally identify and update communities in stream graphs.
@@ -30,15 +31,15 @@
     >>> for x in range(10):
     >>>     g = nx.erdos_renyi_graph(200, 0.05)
     >>>     dg.add_interactions_from(list(g.edges()), t=x)
     >>> coms = algorithms.tiles(dg, 2)
 
     :References:
 
-    Rossetti, Giulio; Pappalardo, Luca; Pedreschi, Dino, and Giannotti, Fosca. `Tiles: an online algorithm for community discovery in dynamic social networks.<https://link.springer.com/article/10.1007/s10994-016-5582-8>`_ Machine Learning (2016), 106(8), 1213-1241.
+    Rossetti, Giulio; Pappalardo, Luca; Pedreschi, Dino, and Giannotti, Fosca. Tiles: an online algorithm for community discovery in dynamic social networks. Machine Learning (2016), 106(8), 1213-1241.
     """
     alg = eTILES(dg=dg, obs=obs)
     tc = TemporalClustering()
     t = obs
     for c in alg.execute():
         communities = {}
         for k, v in c.items():
@@ -53,16 +54,18 @@
         else:
             break
 
     # add community matches (can contain communities not present in the observations)
     mtc = alg.get_matches()
     tc.add_matching(mtc)
 
+    ### polytree
+
     # cleaning & updating community matching
-    dg = tc.lifecycle_polytree(None, False)
+    dg = __lifecycle_polytree(tc)
     community_ids = list(dg.nodes())
 
     tids = tc.get_observation_ids()
     ndss = []
     for tid in tids:
         c = tc.get_clustering_at(tid)
         comunity_ids_m = c.named_communities.keys()
@@ -73,7 +76,26 @@
         if tid not in ndss:
             dg.remove_node(tid)
 
     mtc = list(dg.edges())
     tc.add_matching(mtc)
 
     return tc
+
+
+def __lifecycle_polytree(tc) -> nx.DiGraph:
+    """
+    Reconstruct the poly-tree representing communities lifecycles using a provided similarity function.
+    """
+
+    lifecycle = tc.matching
+
+    pt = nx.DiGraph()
+    if len(lifecycle[0]) == 3:
+        for u, v, w in lifecycle:
+            pt.add_edge(u, v, weight=w)
+    else:
+        # implicit matching
+        for u, v in lifecycle:
+            pt.add_edge(u, v)
+
+    return pt
```

### Comparing `cdlib-0.3.0/cdlib/benchmark/dynamic_benchmark.py` & `cdlib-0.4.0/cdlib/benchmark/dynamic_benchmark.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/benchmark/internal/rdyn.py` & `cdlib-0.4.0/cdlib/benchmark/internal/rdyn.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/benchmark/internal/xmark.py` & `cdlib-0.4.0/cdlib/benchmark/internal/xmark.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/benchmark/static_benchmark.py` & `cdlib-0.4.0/cdlib/benchmark/static_benchmark.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/classes/attr_node_clustering.py` & `cdlib-0.4.0/cdlib/classes/attr_node_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/classes/bipartite_node_clustering.py` & `cdlib-0.4.0/cdlib/classes/bipartite_node_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/classes/clustering.py` & `cdlib-0.4.0/cdlib/classes/clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/classes/edge_clustering.py` & `cdlib-0.4.0/cdlib/classes/edge_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/classes/fuzzy_node_clustering.py` & `cdlib-0.4.0/cdlib/classes/fuzzy_node_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/classes/named_clustering.py` & `cdlib-0.4.0/cdlib/classes/named_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/classes/node_clustering.py` & `cdlib-0.4.0/cdlib/evaluation/fitness.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,956 +1,1232 @@
-from cdlib.classes.clustering import Clustering
-from cdlib import evaluation
 import networkx as nx
-
-try:
-    import igraph as ig
-except ModuleNotFoundError:
-    ig = None
-
+from cdlib.utils import convert_graph_formats
+from collections import namedtuple
+import numpy as np
+import scipy
+from cdlib.evaluation.internal.link_modularity import cal_modularity
+import Eva
+from typing import Callable
 from collections import defaultdict
 
+__all__ = [
+    "FitnessResult",
+    "link_modularity",
+    "normalized_cut",
+    "internal_edge_density",
+    "average_internal_degree",
+    "fraction_over_median_degree",
+    "expansion",
+    "cut_ratio",
+    "edges_inside",
+    "flake_odf",
+    "avg_odf",
+    "max_odf",
+    "triangle_participation_ratio",
+    "modularity_density",
+    "z_modularity",
+    "erdos_renyi_modularity",
+    "newman_girvan_modularity",
+    "significance",
+    "surprise",
+    "conductance",
+    "size",
+    "avg_embeddedness",
+    "scaled_density",
+    "avg_distance",
+    "hub_dominance",
+    "avg_transitivity",
+    "purity",
+    "modularity_overlap",
+]
+
+FitnessResult = namedtuple("FitnessResult", "min max score std")
+FitnessResult.__new__.__defaults__ = (None,) * len(FitnessResult._fields)
+
+
+def __median(lst: list) -> int:
+    return np.median(np.array(lst))
+
+
+def __out_degree_fraction(g: nx.Graph, coms: list) -> list:
+    nds = []
+    for n in coms:
+        nds.append(g.degree(n) - coms.degree(n))
+    return nds
+
+
+def __quality_indexes(
+    graph: nx.Graph,
+    communities: object,
+    scoring_function: Callable[[object, object], float],
+    summary: bool = True,
+) -> object:
+    """
 
-class NodeClustering(Clustering):
-    """Node Communities representation.
-
-    :param communities: list of communities
-    :param graph: a networkx/igraph object
-    :param method_name: community discovery algorithm name
-    :param method_parameters: configuration for the community discovery algorithm used
-    :param overlap: boolean, whether the partition is overlapping or not
-    """
-
-    def __init__(
-        self,
-        communities: list,
-        graph: object,
-        method_name: str = "",
-        method_parameters: dict = None,
-        overlap: bool = False,
-    ):
-        super().__init__(communities, graph, method_name, method_parameters, overlap)
-
-        if graph is not None:
-            node_count = len(
-                {nid: None for community in communities for nid in community}
-            )
-            if isinstance(graph, nx.Graph):
-                self.node_coverage = node_count / graph.number_of_nodes()
-            elif ig is not None and isinstance(graph, ig.Graph):
-                self.node_coverage = node_count / graph.vcount()
-            else:
-                raise ValueError("Unsupported Graph type.")
-
-    def __check_graph(self) -> bool:
-        return self.graph is not None
-
-    def to_node_community_map(self) -> dict:
-        """
-        Generate a <node, list(communities)> representation of the current clustering
-
-        :return: dict of the form <node, list(communities)>
-        """
-
-        node_to_communities = defaultdict(list)
-        for cid, community in enumerate(self.communities):
-            for node in community:
-                node_to_communities[node].append(cid)
-
-        return node_to_communities
-
-    def link_modularity(self) -> evaluation.FitnessResult:
-        """
-        Quality function designed for directed graphs with overlapping communities.
-
-        :return: the link modularity score
-
-        :Example:
-
-        >>> from cdlib import evaluation
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.link_modularity()
-
-        """
-        if self.__check_graph():
-            return evaluation.link_modularity(self.graph, self)
-        else:
-            raise ValueError("Graph instance not specified")
-
-    def normalized_cut(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Normalized variant of the Cut-Ratio
-
-        .. math:: : f(S) = \\frac{c_S}{2m_S+c_S} + \\frac{c_S}{2(m−m_S )+c_S}
-
-        where :math:`m` is the number of graph edges, :math:`m_S` is the number of algorithms internal edges and :math:`c_S` is the number of algorithms nodes.
-
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
-
-        :Example:
+    :param graph: NetworkX/igraph graph
+    :param communities: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-communitys ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.normalized_cut()
+    """
 
-        """
-        if self.__check_graph():
-            return evaluation.normalized_cut(self.graph, self, **kwargs)
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in communities.communities:
+        community = nx.subgraph(graph, com)
+        try:
+            values.append(scoring_function(graph, community))
+        except:
+            values.append(None)
+
+    if summary:
+        values = [v for v in values if v is not None]
+
+        if len(values) > 0:
+            return FitnessResult(
+                min=min(values),
+                max=max(values),
+                score=np.mean(values),
+                std=np.std(values),
+            )
         else:
-            raise ValueError("Graph instance not specified")
+            return FitnessResult(min=None, max=None, score=None, std=None)
+    return values
 
-    def internal_edge_density(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        The internal density of the algorithms set.
 
-        .. math:: f(S) = \\frac{m_S}{n_S(n_S−1)/2}
+def size(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """Size is the number of nodes in the community
 
-        where :math:`m_S` is the number of algorithms internal edges and :math:`n_S` is the number of algorithms nodes.
-
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+
+    Example:
+
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> sz = evaluation.size(g,communities)
+    """
 
-        :Example:
+    return __quality_indexes(graph, communities, lambda g, com: len(com), **kwargs)
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.internal_edge_density()
 
-        """
-        if self.__check_graph():
-            return evaluation.internal_edge_density(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+def scaled_density(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """Scaled density.
 
-    def average_internal_degree(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        The average internal degree of the algorithms set.
+    The scaled density of a community is defined as the ratio of the community density w.r.t. the complete graph density.
 
-        .. math:: f(S) = \\frac{2m_S}{n_S}
-
-        where :math:`m_S` is the number of algorithms internal edges and :math:`n_S` is the number of algorithms nodes.
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+
+    Example:
+
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> scd = evaluation.scaled_density(g,communities)
+    """
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+    return __quality_indexes(
+        graph,
+        communities,
+        lambda graph, coms: nx.density(nx.subgraph(graph, coms)) / nx.density(graph),
+        **kwargs
+    )
 
-        :Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.average_internal_degree()
+def avg_distance(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """Average distance.
 
+    The average distance of a community is defined average path length across all possible pair of nodes composing it.
 
-        """
-        if self.__check_graph():
-            return evaluation.average_internal_degree(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+
+    Example:
+
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> scd = evaluation.avg_distance(g,communities)
+    """
 
-    def fraction_over_median_degree(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Fraction of algorithms nodes of having internal degree higher than the median degree value.
+    return __quality_indexes(
+        graph,
+        communities,
+        lambda graph, coms: nx.average_shortest_path_length(nx.subgraph(graph, coms)),
+        **kwargs
+    )
 
-        .. math:: f(S) = \\frac{|\{u: u \\in S,| \{(u,v): v \\in S\}| > d_m\}| }{n_S}
 
+def hub_dominance(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """Hub dominance.
 
-        where :math:`d_m` is the internal degree median value
+    The hub dominance of a community is defined as the ratio of the degree of its most connected node w.r.t. the theoretically maximal degree within the community.
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+
+    Example:
+
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> scd = evaluation.hub_dominance(g,communities)
+    """
 
-        :Example:
+    return __quality_indexes(
+        graph,
+        communities,
+        lambda graph, coms: max(
+            [x[1] for x in list(nx.degree(nx.subgraph(graph, coms)))]
+        )
+        / (len(coms) - 1),
+        **kwargs
+    )
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.fraction_over_median_degree()
 
-        """
-        if self.__check_graph():
-            return evaluation.fraction_over_median_degree(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+def avg_transitivity(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """Average transitivity.
 
-    def expansion(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Number of edges per algorithms node that point outside the cluster.
+    The average transitivity of a community is defined the as the average clustering coefficient of its nodes w.r.t. their connection within the community itself.
 
-        .. math:: f(S) = \\frac{c_S}{n_S}
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+
+    Example:
+
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> scd = evaluation.avg_transitivity(g,communities)
+    """
 
-        where :math:`n_S` is the number of edges on the algorithms boundary, :math:`c_S` is the number of algorithms nodes.
+    return __quality_indexes(
+        graph,
+        communities,
+        lambda graph, coms: nx.average_clustering(nx.subgraph(graph, coms)),
+        **kwargs
+    )
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
 
-        :Example:
+def avg_embeddedness(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """Average embeddedness of nodes within the community.
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.expansion()
+    The embeddedness of a node n w.r.t. a community C is the ratio of its degree within the community and its overall degree.
 
-        """
-        if self.__check_graph():
-            return evaluation.expansion(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    .. math:: emb(n,C) = \\frac{k_n^C}{k_n}
 
-    def cut_ratio(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Fraction of existing edges (out of all possible edges) leaving the algorithms.
+    The average embeddedness of a community C is:
 
-        ..math:: f(S) = \\frac{c_S}{n_S (n − n_S)}
+    .. math:: avg_embd(c) = \\frac{1}{|C|} \sum_{i \in C} \\frac{k_n^C}{k_n}
 
-        where :math:`c_S` is the number of algorithms nodes and, :math:`n_S` is the number of edges on the algorithms boundary
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+
+    Example:
+
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> ave = evaluation.avg_embeddedness(g,communities)
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+    :References:
 
-        :Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.cut_ratio()
+    """
 
-        """
-        if self.__check_graph():
-            return evaluation.cut_ratio(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    return __quality_indexes(
+        graph,
+        communities,
+        lambda g, com: np.mean(
+            [float(nx.degree(nx.subgraph(g, com))[n]) / nx.degree(g)[n] for n in com]
+        ),
+        **kwargs
+    )
 
-    def edges_inside(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Number of edges internal to the algorithms.
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+def normalized_cut(graph: nx.Graph, community: object, summary: bool = True) -> object:
+    """Normalized variant of the Cut-Ratio
 
-        :Example:
+    .. math:: f(S) = \\frac{c_S}{2m_S+c_S} + \\frac{c_S}{2(m−m_S )+c_S}
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.edges_inside()
+    where :math:`m` is the number of graph edges, :math:`m_S` is the number of community internal edges and :math:`c_S` is the number of community nodes.
 
-        """
-        if self.__check_graph():
-            return evaluation.edges_inside(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-    def conductance(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Fraction of total edge volume that points outside the algorithms.
 
-        .. math:: f(S) = \\frac{c_S}{2 m_S+c_S}
+    Example:
 
-        where :math:`c_S` is the number of algorithms nodes and, :math:`m_S` is the number of algorithms edges
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.normalized_cut(g,communities)
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+    :References:
 
-        :Example:
+    1.Shi, J., Malik, J.: Normalized cuts and image segmentation. Departmental Papers (CIS), 107 (2000)
+    """
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.conductance()
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+
+        ms = len(coms.edges())
+        edges_outside = 0
+        for n in coms.nodes():
+            neighbors = graph.neighbors(n)
+            for n1 in neighbors:
+                if n1 not in coms:
+                    edges_outside += 1
+        try:
+            ratio = (float(edges_outside) / ((2 * ms) + edges_outside)) + float(
+                edges_outside
+            ) / (2 * (len(graph.edges()) - ms) + edges_outside)
+        except:
+            ratio = 0
+        values.append(ratio)
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-        """
-        if self.__check_graph():
-            return evaluation.conductance(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
 
-    def max_odf(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Maximum fraction of edges of a node of a algorithms that point outside the algorithms itself.
+def internal_edge_density(
+    graph: nx.Graph, community: object, summary: bool = True
+) -> object:
+    """The internal density of the community set.
 
-        .. math:: max_{u \\in S} \\frac{|\{(u,v)\\in E: v \\not\\in S\}|}{d(u)}
+     .. math:: f(S) = \\frac{m_S}{n_S(n_S−1)/2}
 
-        where :math:`E` is the graph edge set, :math:`v` is a node in :math:`S` and :math:`d(u)` is the degree of :math:`u`
+     where :math:`m_S` is the number of community internal edges and :math:`n_S` is the number of community nodes.
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        :Example:
+    Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.max_odf()
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.internal_edge_density(g,communities)
 
-        """
-        if self.__check_graph():
-            return evaluation.max_odf(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
 
-    def avg_odf(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Average fraction of edges of a node of a algorithms that point outside the algorithms itself.
+    :References:
 
-        .. math:: \\frac{1}{n_S} \\sum_{u \\in S} \\frac{|\{(u,v)\\in E: v \\not\\in S\}|}{d(u)}
+    1. Radicchi, F., Castellano, C., Cecconi, F., Loreto, V., & Parisi, D. (2004). Defining and identifying communities in networks. Proceedings of the National Academy of Sciences, 101(9), 2658-2663.
+    """
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+
+        ms = len(coms.edges())
+        ns = len(coms.nodes())
+        try:
+            internal_density = float(ms) / (float(ns * (ns - 1)) / 2)
+        except:
+            internal_density = 0
+        values.append(internal_density)
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-        where :math:`E` is the graph edge set, :math:`v` is a node in :math:`S`, :math:`d(u)` is the degree of :math:`u` and :math:`n_S` is the set of algorithms nodes.
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
-        :Example:
+def average_internal_degree(
+    graph: nx.Graph, community: object, summary: bool = True
+) -> object:
+    """The average internal degree of the community set.
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.avg_odf()
+     .. math:: f(S) = \\frac{2m_S}{n_S}
 
-        """
-        if self.__check_graph():
-            return evaluation.avg_odf(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
 
-    def flake_odf(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Fraction of nodes in S that have fewer edges pointing inside than to the outside of the algorithms.
 
-        .. math:: f(S) = \\frac{| \{ u:u \in S,| \{(u,v) \in E: v \in S \}| < d(u)/2 \}|}{n_S}
+     where :math:`m_S` is the number of community internal edges and :math:`n_S` is the number of community nodes.
 
-        where :math:`E` is the graph edge set, :math:`v` is a node in :math:`S`, :math:`d(u)` is the degree of :math:`u` and :math:`n_S` is the set of algorithms nodes.
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+    Example:
 
-        :Example:
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.average_internal_degree(g,communities)
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.flake_odf()
+    :References:
 
-        """
-        if self.__check_graph():
-            return evaluation.flake_odf(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    1. Radicchi, F., Castellano, C., Cecconi, F., Loreto, V., & Parisi, D. (2004). Defining and identifying communities in networks. Proceedings of the National Academy of Sciences, 101(9), 2658-2663.
+    """
 
-    def triangle_participation_ratio(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """
-        Fraction of algorithms nodes that belong to a triad.
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+
+        ms = len(coms.edges())
+        ns = len(coms.nodes())
+        try:
+            avg_id = float(2 * ms) / ns
+        except:
+            avg_id = 0
+        values.append(avg_id)
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-        .. math:: f(S) = \\frac{ | \{ u: u \in S,\{(v,w):v, w \in S,(u,v) \in E,(u,w) \in E,(v,w) \in E \} \\not = \\emptyset \} |}{n_S}
 
-        where :math:`n_S` is the set of algorithms nodes.
+def fraction_over_median_degree(
+    graph: nx.Graph, community: object, summary: bool = True
+) -> object:
+    """Fraction of community nodes of having internal degree higher than the median degree value.
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+    .. math:: f(S) = \\frac{|\{u: u \\in S,| \{(u,v): v \\in S\}| > d_m\}| }{n_S}
 
-        :Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.triangle_participation_ratio()
+    where :math:`d_m` is the internal degree median value
 
-        """
-        if self.__check_graph():
-            return evaluation.triangle_participation_ratio(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-    def size(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """Size is the number of nodes in the community
+    Example:
 
-        :param summary: (optional, default True) if **True**, an overall summary is returned for the partition (min, max, avg, std); if **False** a list of community-wise score
-        :return: a FitnessResult object/a list of community-wise score
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.fraction_over_median_degree(g,communities)
 
-        Example:
+    :References:
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.size()
-        """
+    1. Yang, J., Leskovec, J.: Defining and evaluating network communities based on ground-truth. Knowledge and Information Systems 42(1), 181–213 (2015)
+    """
 
-        return evaluation.size(self.graph, self, **kwargs)
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+
+        ns = coms.number_of_nodes()
+        degs = coms.degree()
+
+        med = __median([d[1] for d in degs])
+        above_med = len([d[0] for d in degs if d[1] > med])
+        try:
+            ratio = float(above_med) / ns
+        except:
+            ratio = 0
+        values.append(ratio)
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-    def newman_girvan_modularity(self) -> evaluation.FitnessResult:
-        """
-        Difference the fraction of intra algorithms edges of a partition with the expected number of such edges if distributed according to a null model.
 
-        In the standard version of modularity, the null model preserves the expected degree sequence of the graph under consideration. In other words, the modularity compares the real network structure with a corresponding one where nodes are connected without any preference about their neighbors.
+def expansion(graph: nx.Graph, community: object, summary: bool = True) -> object:
+    """Number of edges per community node that point outside the cluster.
 
-        .. math:: Q(S) = \\frac{1}{m}\\sum_{c \\in S}(m_S - \\frac{(2 m_S + l_S)^2}{4m})
+    .. math:: f(S) = \\frac{c_S}{n_S}
 
-        where :math:`m` is the number of graph edges, :math:`m_S` is the number of algorithms edges, :math:`l_S` is the number of edges from nodes in S to nodes outside S.
+    where :math:`c_S` is the number of edges on the community boundary, :math:`n_S` is the number of community nodes.
 
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        :return: the Newman-Girvan modularity score
+    Example:
 
-        :Example:
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.expansion(g,communities)
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.newman_girvan_modularity()
+    :References:
 
-        :References:
+    1. Radicchi, F., Castellano, C., Cecconi, F., Loreto, V., & Parisi, D. (2004). Defining and identifying communities in networks. Proceedings of the National Academy of Sciences, 101(9), 2658-2663.
+    """
 
-        Newman, M.E.J. & Girvan, M. **Finding and evaluating algorithms structure in networks.** Physical Review E 69, 26113(2004).
-        """
-        if self.__check_graph():
-            return evaluation.newman_girvan_modularity(self.graph, self)
-        else:
-            raise ValueError("Graph instance not specified")
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+
+        ns = len(coms.nodes())
+        edges_outside = 0
+        for n in coms.nodes():
+            neighbors = graph.neighbors(n)
+            for n1 in neighbors:
+                if n1 not in coms:
+                    edges_outside += 1
+        try:
+            exp = float(edges_outside) / ns
+        except:
+            exp = 0
+        values.append(exp)
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-    def erdos_renyi_modularity(self) -> evaluation.FitnessResult:
-        """
 
-        Erdos-Renyi modularity is a variation of the Newman-Girvan one.
-        It assumes that vertices in a network are connected randomly with a constant probability :math:`p`.
+def cut_ratio(graph: nx.Graph, community: object, summary: bool = True) -> object:
+    """Fraction of existing edges (out of all possible edges) leaving the community.
 
-        .. math:: Q(S) = \\frac{1}{m}\\sum_{c \\in S} (m_S − \\frac{mn_S(n_S −1)}{n(n−1)})
+    .. math:: f(S) = \\frac{c_S}{n_S (n − n_S)}
 
-        where :math:`m` is the number of graph edges, :math:`m_S` is the number of algorithms edges, :math:`l_S` is the number of edges from nodes in S to nodes outside S.
+    where :math:`c_S` is the cut size (number of edges on the community boundary) and :math:`n_S` is the number of community nodes
 
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        :return: the Erdos-Renyi modularity score
+    Example:
 
-        :Example:
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.cut_ratio(g,communities)
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.erdos_renyi_modularity()
+    :References:
 
-        :References:
+    1. Fortunato, S.: Community detection in graphs. Physics reports 486(3-5), 75–174 (2010)
+    """
 
-        Erdos, P., & Renyi, A. (1959). **On random graphs I.** Publ. Math. Debrecen, 6, 290-297.
-        """
-        if self.__check_graph():
-            return evaluation.erdos_renyi_modularity(self.graph, self)
-        else:
-            raise ValueError("Graph instance not specified")
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+
+        ns = len(coms.nodes())
+        edges_outside = 0
+        for n in coms.nodes():
+            neighbors = graph.neighbors(n)
+            for n1 in neighbors:
+                if n1 not in coms:
+                    edges_outside += 1
+        try:
+            ratio = float(edges_outside) / (ns * (len(graph.nodes()) - ns))
+        except:
+            ratio = 0
+        values.append(ratio)
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-    def modularity_density(self) -> evaluation.FitnessResult:
-        """
-        The modularity density is one of several propositions that envisioned to palliate the resolution limit issue of modularity based measures.
-        The idea of this metric is to include the information about algorithms size into the expected density of algorithms to avoid the negligence of small and dense communities.
-        For each algorithms :math:`C` in partition :math:`S`, it uses the average modularity degree calculated by :math:`d(C) = d^{int(C)} − d^{ext(C)}` where :math:`d^{int(C)}` and :math:`d^{ext(C)}` are the average internal and external degrees of :math:`C` respectively to evaluate the fitness of :math:`C` in its network.
-        Finally, the modularity density can be calculated as follows:
 
-        .. math:: Q(S) = \\sum_{C \\in S} \\frac{1}{n_C} ( \\sum_{i \\in C} k^{int}_{iC} - \\sum_{i \\in C} k^{out}_{iC})
+def edges_inside(graph: nx.Graph, community: object, summary: bool = True) -> object:
+    """Number of edges internal to the community.
 
-        where :math:`n_C` is the number of nodes in C, :math:`k^{int}_{iC}` is the degree of node i within :math:`C` and :math:`k^{out}_{iC}` is the deree of node i outside :math:`C`.
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
+    Example:
 
-        :return: the modularity density score
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.edges_inside(g,communities)
 
-        :Example:
+    :References:
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.modularity_density()
+    1. Radicchi, F., Castellano, C., Cecconi, F., Loreto, V., & Parisi, D. (2004). Defining and identifying communities in networks. Proceedings of the National Academy of Sciences, 101(9), 2658-2663.
+    """
 
-        :References:
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+        values.append(coms.number_of_edges())
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-        Li, Z., Zhang, S., Wang, R. S., Zhang, X. S., & Chen, L. (2008). **Quantitative function for algorithms detection.** Physical review E, 77(3), 036109.
 
-        """
+def conductance(graph: nx.Graph, community: object, summary: bool = True) -> object:
+    """Fraction of total edge volume that points outside the community.
 
-        if self.__check_graph():
-            return evaluation.modularity_density(self.graph, self)
-        else:
-            raise ValueError("Graph instance not specified")
+    .. math:: f(S) = \\frac{c_S}{2 m_S+c_S}
 
-    def z_modularity(self) -> evaluation.FitnessResult:
-        """
-        Z-modularity is another variant of the standard modularity proposed to avoid the resolution limit.
-        The concept of this version is based on an observation that the difference between the fraction of edges inside communities and the expected number of such edges in a null model should not be considered as the only contribution to the final quality of algorithms structure.
+    where :math:`c_S` is the number of community nodes and, :math:`m_S` is the number of community edges
 
-        :return: the z-modularity score
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        :Example:
+    Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.z_modularity()
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.conductance(g,communities)
 
+    :References:
 
-        :References:
+    1.Shi, J., Malik, J.: Normalized cuts and image segmentation. Departmental Papers (CIS), 107 (2000)
+    """
 
-        Miyauchi, Atsushi, and Yasushi Kawase. **Z-score-based modularity for algorithms detection in networks.** PloS one 11.1 (2016): e0147805.
-        """
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+
+        ms = len(coms.edges())
+        edges_outside = 0
+        for n in coms.nodes():
+            neighbors = graph.neighbors(n)
+            for n1 in neighbors:
+                if n1 not in coms:
+                    edges_outside += 1
+        try:
+            ratio = float(edges_outside) / ((2 * ms) + edges_outside)
+        except:
+            ratio = 0
+        values.append(ratio)
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-        if self.__check_graph():
-            return evaluation.z_modularity(self.graph, self)
-        else:
-            raise ValueError("Graph instance not specified")
 
-    def modularity_overlap(self, weight: str = None) -> evaluation.FitnessResult:
-        """Determines the Overlapping Modularity of a partition C on a graph G.
+def max_odf(graph: nx.Graph, community: object, summary: bool = True) -> object:
+    """Maximum fraction of edges of a node of a community that point outside the community itself.
 
-        Overlapping Modularity is defined as
+    .. math:: max_{u \\in S} \\frac{|\{(u,v)\\in E: v \\not\\in S\}|}{d(u)}
 
-        .. math:: M_{c_{r}}^{ov} = \\sum_{i \\in c_{r}} \\frac{\\sum_{j \\in c_{r}, i \\neq j}a_{ij} - \\sum_{j \\not \\in c_{r}}a_{ij}}{d_{i} \\cdot s_{i}} \\cdot \\frac{n_{c_{r}}^{e}}{n_{c_{r}} \\cdot \\binom{n_{c_{r}}}{2}}
+    where :math:`E` is the graph edge set, :math:`v` is a node in :math:`S` and :math:`d(u)` is the degree of :math:`u`
 
-        :param weight: label identifying the edge weight parameter name (if present), default None
-        :return: FitnessResult object
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        Example:
+    Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> from cdlib import evaluation
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.modularity_overlap()
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.max_odf(g,communities)
 
-        :References:
+    :References:
 
-        1. A. Lazar, D. Abel and T. Vicsek, "Modularity measure of networks with overlapping communities"  EPL, 90 (2010) 18001 doi: 10.1209/0295-5075/90/18001
-        """
+    1. Flake, G.W., Lawrence, S., Giles, C.L., et al.: Efficient identification of web communities. In: KDD, vol. 2000, pp. 150–160 (2000)
+    """
 
-        if self.__check_graph():
-            return evaluation.modularity_overlap(self.graph, self, weight)
-        else:
-            raise ValueError("Graph instance not specified")
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+        values.append(max(__out_degree_fraction(graph, coms)))
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-    def surprise(self) -> evaluation.FitnessResult:
-        """
-        Surprise is statistical approach proposes a quality metric assuming that edges between vertices emerge randomly according to a hyper-geometric distribution.
 
-        According to the Surprise metric, the higher the score of a partition, the less likely it is resulted from a random realization, the better the quality of the algorithms structure.
+def avg_odf(graph: nx.Graph, community: object, summary: bool = True) -> object:
+    """Average fraction of edges of a node of a community that point outside the community itself.
 
-        :return: the surprise score
+    .. math:: \\frac{1}{n_S} \\sum_{u \\in S} \\frac{|\{(u,v)\\in E: v \\not\\in S\}|}{d(u)}
 
-        :Example:
+    where :math:`E` is the graph edge set, :math:`v` is a node in :math:`S`, :math:`d(u)` is the degree of :math:`u` and :math:`n_S` is the set of community nodes.
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.surprise()
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        :References:
+    Example:
 
-        Traag, V. A., Aldecoa, R., & Delvenne, J. C. (2015). **Detecting communities using asymptotical surprise.** Physical Review E, 92(2), 022816.
-        """
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.avg_odf(g,communities)
 
-        if self.__check_graph():
-            return evaluation.surprise(self.graph, self)
-        else:
-            raise ValueError("Graph instance not specified")
+    :References:
 
-    def significance(self) -> evaluation.FitnessResult:
-        """
-        Significance estimates how likely a partition of dense communities appear in a random graph.
+    1. Flake, G.W., Lawrence, S., Giles, C.L., et al.: Efficient identification of web communities. In: KDD, vol. 2000, pp. 150–160 (2000)
+    """
 
-        :return: the significance score
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+        values.append(float(sum(__out_degree_fraction(graph, coms))) / len(coms))
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-        :Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> mod = communities.significance()
+def flake_odf(graph: nx.Graph, community: object, summary: bool = True) -> object:
+    """Fraction of nodes in S that have fewer edges pointing inside than to the outside of the community.
 
+    .. math:: f(S) = \\frac{| \{ u:u \in S,| \{(u,v) \in E: v \in S \}| < d(u)/2 \}|}{n_S}
 
-        :References:
+    where :math:`E` is the graph edge set, :math:`v` is a node in :math:`S`, :math:`d(u)` is the degree of :math:`u` and :math:`n_S` is the set of community nodes.
 
-        Traag, V. A., Aldecoa, R., & Delvenne, J. C. (2015). **Detecting communities using asymptotical surprise.** Physical Review E, 92(2), 022816.
-        """
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        if self.__check_graph():
-            return evaluation.significance(self.graph, self)
-        else:
-            raise ValueError("Graph instance not specified")
+    Example:
 
-    def scaled_density(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """Scaled density.
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.flake_odf(g,communities)
 
-        The scaled density of a community is defined as the ratio of the community density w.r.t. the complete graph density.
+    :References:
 
-        :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
-        :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+    1. Flake, G.W., Lawrence, S., Giles, C.L., et al.: Efficient identification of web communities. In: KDD, vol. 2000, pp. 150–160 (2000)
+    """
 
-        Example:
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+        df = 0
+        for n in coms:
+            fr = coms.degree(n) - (graph.degree(n) - coms.degree(n))
+            if fr < 0:
+                df += 1
+        score = float(df) / len(coms)
+        values.append(score)
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-        >>> from cdlib.algorithms import louvain
-        >>> from cdlib import evaluation
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> scd = communities.scaled_density()
-        """
 
-        if self.__check_graph():
-            return evaluation.scaled_density(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+def triangle_participation_ratio(
+    graph: nx.Graph, community: object, summary: bool = True
+) -> object:
+    """Fraction of community nodes that belong to a triad.
 
-    def avg_distance(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """Average distance.
+    .. math:: f(S) = \\frac{ | \{ u: u \in S,\{(v,w):v, w \in S,(u,v) \in E,(u,w) \in E,(v,w) \in E \} \\not = \\emptyset \} |}{n_S}
 
-        The average distance of a community is defined average path length across all possible pair of nodes composing it.
+    where :math:`n_S` is the set of community nodes.
 
-        :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
-        :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+    :param graph: a networkx/igraph object
+    :param community: NodeClustering object
+    :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
+    :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        Example:
+    Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> from cdlib import evaluation
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> scd = communities.avg_distance()
-        """
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.triangle_participation_ratio(g,communities)
 
-        if self.__check_graph():
-            return evaluation.avg_distance(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    :References:
 
-    def hub_dominance(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """Hub dominance.
+    1. Yang, J., Leskovec, J.: Defining and evaluating network communities based on ground-truth. Knowledge and Information Systems 42(1), 181–213 (2015)
+    """
 
-        The hub dominance of a community is defined as the ratio of the degree of its most connected node w.r.t. the theoretically maximal degree within the community.
+    graph = convert_graph_formats(graph, nx.Graph)
+    values = []
+    for com in community.communities:
+        coms = nx.subgraph(graph, com)
+        cls = nx.triangles(coms)
+        nc = [n for n in cls if cls[n] > 0]
+        score = float(len(nc)) / len(coms)
+        values.append(score)
+
+    if summary:
+        return FitnessResult(
+            min=min(values), max=max(values), score=np.mean(values), std=np.std(values)
+        )
+    return values
 
-        :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
-        :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
 
-        Example:
+def link_modularity(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """
+    Quality function designed for directed graphs with overlapping communities.
 
-        >>> from cdlib.algorithms import louvain
-        >>> from cdlib import evaluation
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> scd = communities.hub_dominance()
-        """
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :return: FitnessResult object
 
-        if self.__check_graph():
-            return evaluation.hub_dominance(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    Example:
 
-    def avg_transitivity(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """Average transitivity.
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.link_modularity(g,communities)
 
-        The average transitivity of a community is defined the as the average clustering coefficient of its nodes w.r.t. their connection within the community itself.
+    :References:
 
-        :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
-        :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+    1. Nicosia, V., Mangioni, G., Carchiolo, V., Malgeri, M.: Extending the definition of modularity to directed graphs with overlapping communities. Journal of Statistical Mechanics: Theory and Experiment 2009(03), 03024 (2009)
 
-        Example:
+    """
 
-        >>> from cdlib.algorithms import louvain
-        >>> from cdlib import evaluation
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> scd = communities.avg_transitivity()
-        """
+    graph = convert_graph_formats(graph, nx.Graph)
 
-        if self.__check_graph():
-            return evaluation.avg_transitivity(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    return FitnessResult(score=cal_modularity(graph, communities.communities))
 
-    def avg_embeddedness(self, **kwargs: dict) -> evaluation.FitnessResult:
-        """Average embeddedness of nodes within the community.
 
-        The embeddedness of a node n w.r.t. a community C is the ratio of its degree within the community and its overall degree.
+def newman_girvan_modularity(
+    graph: nx.Graph, communities: object, **kwargs: dict
+) -> object:
+    """Difference the fraction of intra community edges of a partition with the expected number of such edges if distributed according to a null model.
 
-        .. math:: emb(n,C) = \\frac{k_n^C}{k_n}
+    In the standard version of modularity, the null model preserves the expected degree sequence of the graph under consideration. In other words, the modularity compares the real network structure with a corresponding one where nodes are connected without any preference about their neighbors.
 
-        The average embeddedness of a community C is:
+    .. math:: Q(S) = \\frac{1}{m}\\sum_{c \\in S}(m_S - \\frac{(2 m_S + l_S)^2}{4m})
 
-        .. math:: avg_embd(c) = \\frac{1}{|C|} \sum_{i \in C} \\frac{k_n^C}{k_n}
+    where :math:`m` is the number of graph edges, :math:`m_S` is the number of community edges, :math:`l_S` is the number of edges from nodes in S to nodes outside S.
 
-        :param summary: boolean. If **True** it is returned an aggregated score for the partition is returned, otherwise individual-community ones. Default **True**.
-        :return: If **summary==True** a FitnessResult object, otherwise a list of floats.
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :return: FitnessResult object
 
-        Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> from cdlib import evaluation
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> ave = communities.avg_embeddedness()
+    Example:
 
-        """
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.newman_girvan_modularity(g,communities)
 
-        if self.__check_graph():
-            return evaluation.avg_embeddedness(self.graph, self, **kwargs)
-        else:
-            raise ValueError("Graph instance not specified")
+    :References:
 
-    def normalized_mutual_information(
-        self, clustering: Clustering
-    ) -> evaluation.MatchingResult:
-        """
-        Normalized Mutual Information between two clusterings.
+    1. Newman, M.E.J. & Girvan, M. `Finding and evaluating community structure in networks. <https://www.ncbi.nlm.nih.gov/pubmed/14995526/>`_ Physical Review E 69, 26113(2004).
+    """
 
-        Normalized Mutual Information (NMI) is an normalization of the Mutual
-        Information (MI) score to scale the results between 0 (no mutual
-        information) and 1 (perfect correlation). In this function, mutual
-        information is normalized by ``sqrt(H(labels_true) * H(labels_pred))``
+    graph = convert_graph_formats(graph, nx.Graph)
+    coms = {}
+    for cid, com in enumerate(communities.communities):
+        for node in com:
+            coms[node] = cid
+
+    inc = dict([])
+    deg = dict([])
+    links = graph.size(weight="weight")
+    if links == 0:
+        raise ValueError("A graph without link has an undefined modularity")
+
+    for node in graph:
+        try:
+            com = coms[node]
+            deg[com] = deg.get(com, 0.0) + graph.degree(node, weight="weight")
+            for neighbor, dt in graph[node].items():
+                weight = dt.get("weight", 1)
+                if coms[neighbor] == com:
+                    if neighbor == node:
+                        inc[com] = inc.get(com, 0.0) + float(weight)
+                    else:
+                        inc[com] = inc.get(com, 0.0) + float(weight) / 2.0
+        except:
+            pass
+
+    res = 0.0
+    for com in set(coms.values()):
+        res += (inc.get(com, 0.0) / links) - (deg.get(com, 0.0) / (2.0 * links)) ** 2
+
+    return FitnessResult(score=res)
+
+
+def erdos_renyi_modularity(
+    graph: nx.Graph, communities: object, **kwargs: dict
+) -> object:
+    """Erdos-Renyi modularity is a variation of the Newman-Girvan one.
+    It assumes that vertices in a network are connected randomly with a constant probability :math:`p`.
 
-        :param clustering: NodeClustering object
-        :return: normalized mutual information score
+    .. math:: Q(S) = \\frac{1}{m}\\sum_{c \\in S} (m_S − \\frac{mn_S(n_S −1)}{n(n−1)})
 
-        :Example:
+    where :math:`m` is the number of graph edges, :math:`m_S` is the number of community edges, :math:`l_S` is the number of edges from nodes in S to nodes outside S.
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> leiden_communities = algorithms.leiden(g)
-        >>> mod = communities.normalized_mutual_information(leiden_communities)
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :return: FitnessResult object
 
-        """
+    Example:
 
-        return evaluation.normalized_mutual_information(self, clustering)
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.erdos_renyi_modularity(g,communities)
 
-    def overlapping_normalized_mutual_information_LFK(
-        self, clustering: Clustering
-    ) -> evaluation.MatchingResult:
-        """
-        Overlapping Normalized Mutual Information between two clusterings.
+    :References:
 
-        Extension of the Normalized Mutual Information (NMI) score to cope with overlapping partitions.
-        This is the version proposed by Lancichinetti et al.
+    1. Erdos, P., & Renyi, A. (1959). `On random graphs I. <https://gnunet.org/sites/default/files/Erd%C5%91s%20%26%20R%C3%A9nyi%20-%20On%20Random%20Graphs.pdf/>`_ Publ. Math. Debrecen, 6, 290-297.
+    """
+    graph = convert_graph_formats(graph, nx.Graph)
+    m = graph.number_of_edges()
+    n = graph.number_of_nodes()
+    q = 0
+
+    for community in communities.communities:
+        c = nx.subgraph(graph, community)
+        mc = c.number_of_edges()
+        nc = c.number_of_nodes()
+        q += mc - (m * nc * (nc - 1)) / (n * (n - 1))
+
+    return FitnessResult(score=(1 / m) * q)
+
+
+def modularity_density(
+    graph: nx.Graph, communities: object, lmbd: float = 0.5, **kwargs: dict
+) -> object:
+    """The modularity density is one of several propositions that envisioned to palliate the resolution limit issue of modularity based measures.
+    The idea of this metric is to include the information about community size into the expected density of community to avoid the negligence of small and dense communities.
+    For each community :math:`C` in partition :math:`S`, it uses the average modularity degree calculated by :math:`d(C) = d^{int(C)} − d^{ext(C)}` where :math:`d^{int(C)}` and :math:`d^{ext(C)}` are the average internal and external degrees of :math:`C` respectively to evaluate the fitness of :math:`C` in its network.
+    Finally, the modularity density can be calculated as follows:
 
-        :param clustering: NodeClustering object
-        :return: onmi score
+    .. math:: Q(S) = \\sum_{C \\in S} \\frac{1}{n_C} ( \\sum_{i \\in C} 2 * \lambda * k^{int}_{iC} - \\sum_{i \\in C} 2 * (1 - \lambda) * k^{out}_{iC})
 
-        :Example:
+    where :math:`n_C` is the number of nodes in C, :math:`k^{int}_{iC}` is the degree of node i within :math:`C`, :math:`k^{out}_{iC}` is the deree of node i outside :math:`C` and :math:`\lambda` is a paramter that allows for tuning the measure resolution (its default value, 0.5, computes the standard modularity density score).
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> leiden_communities = algorithms.leiden(g)
-        >>> mod = communities.overlapping_normalized_mutual_information_LFK(leiden_communities)
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :param lmbd: resolution parameter, float in [0,1]. Default 0.5.
+    :return: FitnessResult object
 
-        :Reference:
 
-        1. Lancichinetti, A., Fortunato, S., & Kertesz, J. (2009). Detecting the overlapping and hierarchical community structure in complex networks. New Journal of Physics, 11(3), 033015.
+    Example:
 
-        """
-        return evaluation.overlapping_normalized_mutual_information_LFK(
-            self, clustering
-        )
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.modularity_density(g,communities)
 
-    def overlapping_normalized_mutual_information_MGH(
-        self, clustering: Clustering, normalization: str = "max"
-    ) -> evaluation.MatchingResult:
-        """
-        Overlapping Normalized Mutual Information between two clusterings.
+    :References:
 
-        Extension of the Normalized Mutual Information (NMI) score to cope with overlapping partitions.
-        This is the version proposed by McDaid et al. using a different normalization than the original LFR one. See ref.
-        for more details.
+    1. Zhang, S., Ning, XM., Ding, C. et al. Determining modular organization of protein interaction networks by maximizing modularity density. <https://doi.org/10.1186/1752-0509-4-S2-S10>`_ BMC Syst Biol 4, S10 (2010).
+    """
+    graph = convert_graph_formats(graph, nx.Graph)
+    q = 0
 
-        :param clustering: NodeClustering object
-        :param normalization: one of "max" or "LFK". Default "max" (corresponds to the main method described in the article)
-        :return: onmi score
+    for community in communities.communities:
+        c = nx.subgraph(graph, community)
 
-        :Example:
+        nc = c.number_of_nodes()
+        dint = []
+        dext = []
+        for node in c:
+            dint.append(c.degree(node))
+            dext.append(graph.degree(node) - c.degree(node))
+
+        try:
+            q += (1 / nc) * (
+                (2 * lmbd * np.sum(dint)) - (2 * (1 - lmbd) * np.sum(dext))
+            )
+        except ZeroDivisionError:
+            pass
 
-        >>> from cdlib import evaluation, algorithms
-        >>> g = nx.karate_club_graph()
-        >>> louvain_communities = algorithms.louvain(g)
-        >>> leiden_communities = algorithms.leiden(g)
-        >>> evaluation.overlapping_normalized_mutual_information_MGH(louvain_communities,leiden_communities)
-        :Reference:
+    return FitnessResult(score=q)
 
-        1. McDaid, A. F., Greene, D., & Hurley, N. (2011). Normalized mutual information to evaluate overlapping community finding algorithms. arXiv preprint arXiv:1110.2515. Chicago
-        """
-        return evaluation.overlapping_normalized_mutual_information_MGH(
-            self, clustering, normalization=normalization
-        )
 
-    def omega(self, clustering: Clustering) -> evaluation.MatchingResult:
-        """
+def z_modularity(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """Z-modularity is another variant of the standard modularity proposed to avoid the resolution limit.
+    The concept of this version is based on an observation that the difference between the fraction of edges inside communities and the expected number of such edges in a null model should not be considered as the only contribution to the final quality of community structure.
 
-        Index of resemblance for overlapping, complete coverage, network clusterings.
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :return: FitnessResult object
 
-        :param clustering: NodeClustering object
-        :return: omega index
+    Example:
 
-        :Example:
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.z_modularity(g,communities)
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> leiden_communities = algorithms.leiden(g)
-        >>> mod = communities.omega(leiden_communities)
 
+    :References:
 
-        :Reference:
+    1. Miyauchi, Atsushi, and Yasushi Kawase. `Z-score-based modularity for community detection in networks. <https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0147805/>`_ PloS one 11.1 (2016): e0147805.
+    """
+    graph = convert_graph_formats(graph, nx.Graph)
+    m = graph.number_of_edges()
 
-        1. Gabriel Murray, Giuseppe Carenini, and Raymond Ng. 2012. **Using the omega index for evaluating abstractive algorithms detection.** In Proceedings of Workshop on Evaluation Metrics and System Comparison for Automatic Summarization. Association for Computational Linguistics, Stroudsburg, PA, USA, 10-18.
-        """
-        return evaluation.omega(self, clustering)
+    mmc = 0
+    dc2m = 0
 
-    def f1(self, clustering: Clustering) -> evaluation.MatchingResult:
-        """
-        Compute the average F1 score of the optimal algorithms matches among the partitions in input.
-        Works on overlapping/non-overlapping complete/partial coverage partitions.
+    for community in communities.communities:
+        c = nx.subgraph(graph, community)
+        mc = c.number_of_edges()
+        dc = 0
 
-        :param clustering: NodeClustering object
-        :return: F1 score (harmonic mean of precision and recall)
+        for node in c:
+            dc += graph.degree(node)
 
-        :Example:
+        mmc += mc / m
+        dc2m += (dc / (2 * m)) ** 2
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> leiden_communities = algorithms.leiden(g)
-        >>> mod = communities.f1(leiden_communities)
+    res = 0
+    try:
+        res = (mmc - dc2m) / np.sqrt(dc2m * (1 - dc2m))
+    except ZeroDivisionError:
+        pass
 
+    return FitnessResult(score=res)
 
-        :Reference:
 
-        1. Rossetti, G., Pappalardo, L., & Rinzivillo, S. (2016). **A novel approach to evaluate algorithms detection internal on ground truth.** In Complex Networks VII (pp. 133-144). Springer, Cham.
-        """
-        return evaluation.f1(self, clustering)
+def surprise(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """Surprise is statistical approach proposes a quality metric assuming that edges between vertices emerge randomly according to a hyper-geometric distribution.
 
-    def nf1(self, clustering: Clustering) -> evaluation.MatchingResult:
-        """
-        Compute the Normalized F1 score of the optimal algorithms matches among the partitions in input.
-        Works on overlapping/non-overlapping complete/partial coverage partitions.
+    According to the Surprise metric, the higher the score of a partition, the less likely it is resulted from a random realization, the better the quality of the community structure.
 
-        :param clustering: NodeClustering object
-        :return: MatchingResult instance
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :return: FitnessResult object
 
-        :Example:
+    Example:
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> leiden_communities = algorithms.leiden(g)
-        >>> mod = communities.nf1(leiden_communities)
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.surprise(g,communities)
 
+    :References:
 
-        :Reference:
+    1. Traag, V. A., Aldecoa, R., & Delvenne, J. C. (2015). `Detecting communities using asymptotical surprise. <https://link.aps.org/doi/10.1103/PhysRevE.92.022816/>`_ Physical Review E, 92(2), 022816.
+    """
+    graph = convert_graph_formats(graph, nx.Graph)
+    m = graph.number_of_edges()
+    n = graph.number_of_nodes()
+
+    q = 0
+    qa = 0
+    sp = 0
+
+    for community in communities.communities:
+        c = nx.subgraph(graph, community)
+        mc = c.number_of_edges()
+        nc = c.number_of_nodes()
+
+        q += mc
+        qa += scipy.special.comb(nc, 2, exact=True)
+    try:
+        q = q / m
+        qa = qa / scipy.special.comb(n, 2, exact=True)
+
+        sp = m * (q * np.log(q / qa) + (1 - q) * np.log((1 - q) / (1 - qa)))
+    except ZeroDivisionError:
+        pass
 
-        1. Rossetti, G., Pappalardo, L., & Rinzivillo, S. (2016). **A novel approach to evaluate algorithms detection internal on ground truth.**
+    return FitnessResult(score=sp)
 
-        2. Rossetti, G. (2017). : **RDyn: graph benchmark handling algorithms dynamics. Journal of Complex Networks.** 5(6), 893-912.
-        """
-        return evaluation.nf1(self, clustering)
 
-    def adjusted_rand_index(self, clustering: Clustering) -> evaluation.MatchingResult:
-        """
-        Rand index adjusted for chance.
+def significance(graph: nx.Graph, communities: object, **kwargs: dict) -> object:
+    """Significance estimates how likely a partition of dense communities appear in a random graph.
 
-        The Rand Index computes a similarity measure between two clusterings
-        by considering all pairs of samples and counting pairs that are
-        assigned in the same or different clusters in the predicted and
-        true clusterings.
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :return: FitnessResult object
 
-        The raw RI score is then "adjusted for chance" into the ARI score
-        using the following scheme::
+    Example:
 
-            ARI = (RI - Expected_RI) / (max(RI) - Expected_RI)
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.significance(g,communities)
 
-        The adjusted Rand index is thus ensured to have a value close to
-        0.0 for random labeling independently of the number of clusters and
-        samples and exactly 1.0 when the clusterings are identical (up to
-        a permutation).
+    :References:
 
-        ARI is a symmetric measure::
+    1. Traag, V. A., Aldecoa, R., & Delvenne, J. C. (2015). `Detecting communities using asymptotical surprise. <https://link.aps.org/doi/10.1103/PhysRevE.92.022816/>`_ Physical Review E, 92(2), 022816.
+    """
+    graph = convert_graph_formats(graph, nx.Graph)
+    m = graph.number_of_edges()
 
-            adjusted_rand_index(a, b) == adjusted_rand_index(b, a)
+    binom = scipy.special.comb(m, 2, exact=True)
+    p = m / binom
 
-        :param clustering: NodeClustering object
-        :return: ARI score
+    q = 0
 
-        :Example:
+    for community in communities.communities:
+        try:
+            c = nx.subgraph(graph, community)
+            nc = c.number_of_nodes()
+            mc = c.number_of_edges()
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> leiden_communities = algorithms.leiden(g)
-        >>> mod = communities.adjusted_rand_index(leiden_communities)
+            binom_c = scipy.special.comb(nc, 2, exact=True)
+            pc = mc / binom_c
 
+            q += binom_c * (pc * np.log(pc / p) + (1 - pc) * np.log((1 - pc) / (1 - p)))
+        except ZeroDivisionError:
+            pass
+    return FitnessResult(score=q)
 
-        :Reference:
 
-        1. Hubert, L., & Arabie, P. (1985). **Comparing partitions**. Journal of classification, 2(1), 193-218.
-        """
-        return evaluation.adjusted_rand_index(self, clustering)
+def purity(communities: object) -> FitnessResult:
+    """Purity is the product of the frequencies of the most frequent labels carried by the nodes within the communities
 
-    def adjusted_mutual_information(
-        self, clustering: Clustering
-    ) -> evaluation.MatchingResult:
-        """
-        Adjusted Mutual Information between two clusterings.
+    :param communities: AttrNodeClustering object
+    :return: FitnessResult object
 
-        Adjusted Mutual Information (AMI) is an adjustment of the Mutual
-        Information (MI) score to account for chance. It accounts for the fact that
-        the MI is generally higher for two clusterings with a larger number of
-        clusters, regardless of whether there is actually more information shared.
-        For two clusterings :math:`U` and :math:`V`, the AMI is given as::
+    Example:
 
-            AMI(U, V) = [MI(U, V) - E(MI(U, V))] / [max(H(U), H(V)) - E(MI(U, V))]
+    >>> from cdlib.algorithms import eva
+    >>> from cdlib import evaluation
+    >>> import random
+    >>> l1 = ['A', 'B', 'C', 'D']
+    >>> l2 = ["E", "F", "G"]
+    >>> g = nx.barabasi_albert_graph(100, 5)
+    >>> labels=dict()
+    >>> for node in g.nodes():
+    >>>    labels[node]={"l1":random.choice(l1), "l2":random.choice(l2)}
+    >>> communities = eva(g_attr, labels, alpha=0.5)
+    >>> pur = evaluation.purity(communities)
 
-        This metric is independent of the absolute values of the labels:
-        a permutation of the class or cluster label values won't change the
-        score value in any way.
+    :References:
 
-        This metric is furthermore symmetric: switching ``label_true`` with
-        ``label_pred`` will return the same score value. This can be useful to
-        measure the agreement of two independent label assignments strategies
-        on the same dataset when the real ground truth is not known.
+    1. Citraro, Salvatore, and Giulio Rossetti. "Eva: Attribute-Aware Network Segmentation." International Conference on Complex Networks and Their Applications. Springer, Cham, 2019.
+    """
 
-        Be mindful that this function is an order of magnitude slower than other
-        metrics, such as the Adjusted Rand Index.
+    pur = Eva.purity(communities.coms_labels)
+    return FitnessResult(score=pur)
 
-        :param clustering: NodeClustering object
-        :return: AMI score
 
-        :Example:
+def modularity_overlap(
+    graph: nx.Graph, communities: object, weight: str = None
+) -> FitnessResult:
+    """Determines the Overlapping Modularity of a partition C on a graph G.
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> leiden_communities = algorithms.leiden(g)
-        >>> mod = communities.adjusted_mutual_information(leiden_communities)
+    Overlapping Modularity is defined as
 
-        :Reference:
+     .. math:: M_{c_{r}}^{ov} = \\sum_{i \\in c_{r}} \\frac{\\sum_{j \\in c_{r}, i \\neq j}a_{ij} - \\sum_{j \\not \\in c_{r}}a_{ij}}{d_{i} \\cdot s_{i}} \\cdot \\frac{n_{c_{r}}^{e}}{n_{c_{r}} \\cdot \\binom{n_{c_{r}}}{2}}
 
-        1. Vinh, N. X., Epps, J., & Bailey, J. (2010). **Information theoretic measures for clusterings comparison: Variants, properties, normalization and correction for chance.** Journal of Machine Learning Research, 11(Oct), 2837-2854.
-        """
-        return evaluation.adjusted_mutual_information(self, clustering)
+    :param graph: a networkx/igraph object
+    :param communities: NodeClustering object
+    :param weight: label identifying the edge weight parameter name (if present), default None
+    :return: FitnessResult object
 
-    def variation_of_information(
-        self, clustering: Clustering
-    ) -> evaluation.MatchingResult:
-        """
-        Variation of Information among two nodes partitions.
 
-        $$ H(p)+H(q)-2MI(p, q) $$
+    Example:
 
-        where MI is the mutual information, H the partition entropy and p,q are the algorithms sets
+    >>> from cdlib.algorithms import louvain
+    >>> from cdlib import evaluation
+    >>> g = nx.karate_club_graph()
+    >>> communities = louvain(g)
+    >>> mod = evaluation.modularity_overlap(g, communities)
 
-        :param clustering: NodeClustering object
-        :return: VI score
+    :References:
 
-        :Example:
+    1. A. Lazar, D. Abel and T. Vicsek, "Modularity measure of networks with overlapping communities"  EPL, 90 (2010) 18001 doi: 10.1209/0295-5075/90/18001
 
-        >>> from cdlib.algorithms import louvain
-        >>> g = nx.karate_club_graph()
-        >>> communities = louvain(g)
-        >>> leiden_communities = algorithms.leiden(g)
-        >>> mod = communities.variation_of_information(leiden_communities)
+    .. note:: Reference implementation: https://github.com/aonghus/nxtools/blob/master/nxtools/algorithms/community/quality.py
+    """
 
+    graph = convert_graph_formats(graph, nx.Graph)
 
-        :Reference:
+    affiliation_dict = defaultdict(list)
+    for cid, coms in enumerate(communities.communities):
+        for n in coms:
+            affiliation_dict[n].append(cid)
+
+    mOvTotal = 0
+
+    for nodes in communities.communities:
+        nCommNodes = len(nodes)
+
+        # the contribution of communities with 1 node is 0
+        if nCommNodes <= 1:
+            continue
+
+        nInwardEdges = 0
+        commStrength = 0
+
+        for node in nodes:
+            degree, inwardEdges, outwardEdges = 0, 0, 0
+            for u, v, data in graph.edges(node, data=True):
+                w = data.get(weight, 1)
+                degree += w
+                if v in nodes:
+                    inwardEdges += w
+                    nInwardEdges += 1
+                else:
+                    outwardEdges += w
+
+            affiliationCount = len(affiliation_dict[node])
+            denom = degree * affiliationCount
+            if denom > 0:
+                commStrength += (inwardEdges - outwardEdges) / denom
+
+        binomC = nCommNodes * (nCommNodes - 1)
+        v1 = commStrength / nCommNodes
+        v2 = nInwardEdges / binomC
+        mOv = v1 * v2
+        mOvTotal += mOv
 
-        1. Meila, M. (2007). **Comparing clusterings - an information based distance.** Journal of Multivariate Analysis, 98, 873-895. doi:10.1016/j.jmva.2006.11.013
-        """
-        return evaluation.variation_of_information(self, clustering)
+    score = mOvTotal / len(communities.communities)
+    return FitnessResult(score=score)
```

### Comparing `cdlib-0.3.0/cdlib/datasets/remote.py` & `cdlib-0.4.0/cdlib/datasets/remote.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/ensemble/bunch_executions.py` & `cdlib-0.4.0/cdlib/ensemble/bunch_executions.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/evaluation/comparisonranking.py` & `cdlib-0.4.0/cdlib/evaluation/comparisonranking.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/evaluation/fitnessranking.py` & `cdlib-0.4.0/cdlib/evaluation/fitnessranking.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/evaluation/internal/TOPSIS.py` & `cdlib-0.4.0/cdlib/evaluation/internal/TOPSIS.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/evaluation/internal/link_modularity.py` & `cdlib-0.4.0/cdlib/evaluation/internal/link_modularity.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/evaluation/internal/omega.py` & `cdlib-0.4.0/cdlib/evaluation/internal/omega.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/evaluation/internal/onmi.py` & `cdlib-0.4.0/cdlib/evaluation/internal/onmi.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/evaluation/internal/statistical_ranking.py` & `cdlib-0.4.0/cdlib/evaluation/internal/statistical_ranking.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib/utils.py` & `cdlib-0.4.0/cdlib/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     tp.add_edges_from([(int(e.source()), int(e.target())) for e in graph.edges()])
     if node_map:
         nx.relabel_nodes(tp, node_map, copy=False)
 
     return tp
 
 
-def __from_nx_to_igraph(g: object, directed: bool = None) -> ig.Graph:
+def __from_nx_to_igraph(g: object, directed: bool = None) -> object:
     """
     :param g:
     :param directed:
     :return:
     """
     from networkx.algorithms import bipartite
 
@@ -94,20 +94,24 @@
 
     if directed is None:
         directed = g.is_directed()
 
     gi = ig.Graph(directed=directed)
 
     a_r = {}
+    skip_bipartite = False
     if bipartite.is_bipartite(g):
-        A, B = bipartite.sets(g)
-        for a in A:
-            a_r[a] = 0
-        for b in B:
-            a_r[b] = 1
+        try:
+            A, B = bipartite.sets(g)
+            for a in A:
+                a_r[a] = 0
+            for b in B:
+                a_r[b] = 1
+        except nx.exception.AmbiguousSolution:
+            skip_bipartite = True
 
     ## Two problems to handle:
     # 1)in igraph, names have to be str.
     # 2)since we can ask to compute metrics with found communities and the the original graph, we need to keep
     # the original nodes types in communities. Therefore we need to handle some transparent conversion for non-str nodes
     if type(list(g.nodes)[0]) is str:  # if nodes are string, no problem
         gi.add_vertices([n for n in g.nodes()])
@@ -123,28 +127,28 @@
             gi.vs["name"] = ["\\" + str(n) for n in g.nodes()]
         else:  # if names are not well formed ints, convert to string and use the identifier to remember
             # converting back to int
             # convert = {str(x):x for x in g.nodes()}
             gi.add_vertices(["\\" + str(n) for n in g.nodes()])
             gi.add_edges([("\\" + str(u), "\\" + str(v)) for (u, v) in g.edges()])
 
-    if bipartite.is_bipartite(g):
+    if bipartite.is_bipartite(g) and not skip_bipartite:
         gi.vs["type"] = [
             a_r[name] if type(name) == int else a_r[int(name.replace("\\", ""))]
             for name in gi.vs["name"]
         ]
 
     edgelist = nx.to_pandas_edgelist(g)
     for attr in edgelist.columns[2:]:
         gi.es[attr] = edgelist[attr]
 
     return gi
 
 
-def __from_igraph_to_nx(gi: ig.Graph, directed: bool = None) -> object:
+def __from_igraph_to_nx(gi: object, directed: bool = None) -> object:
     """
 
     :param gi:
     :param directed:
     :return:
     """
 
@@ -217,15 +221,15 @@
         else:
             raise ValueError("graph must be a networkx Graph object")
 
     return graph, None
 
 
 def remap_node_communities(communities: object, node_map: dict) -> list:
-    """Apply a map to the obtained communities to retreive the original node labels
+    """Apply a map to the obtained communities to retrive the original node labels
 
     :param communities: NodeClustering object
     :param node_map: dictionary <numeric_id, node_label>
     :return: remapped communities
     """
 
     cms = []
```

### Comparing `cdlib-0.3.0/cdlib/viz/plots.py` & `cdlib-0.4.0/cdlib/viz/plots.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.3.0/cdlib.egg-info/PKG-INFO` & `cdlib-0.4.0/cdlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdlib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Community Discovery Library
 Home-page: https://github.com/GiulioRossetti/cdlib
 Author: Giulio Rossetti
 Author-email: giulio.rossetti@gmail.com
 License: BSD-Clause-2
 Keywords: community-discovery node-clustering edge-clustering complex-networks
 Classifier: Development Status :: 4 - Beta
@@ -86,27 +86,27 @@
 conda install cdlib
 ```
 
 ### Optional Dependencies (pip package)
 To simplify the installation process, the default installation does not include optional dependencies (e.g., ``graph-tool``). If you need them, you can install them manually or run the following command:
 
 ```bash
-pip install cdlib[C]
+pip install 'cdlib[C]'
 ```
 
 This option, safe for *nix users, will install all those optional dependencies that require C code compilation.
 
 ```bash
-pip install cdlib[pypi]
+pip install 'cdlib[pypi]'
 ```
 
 This option will install all those optional dependencies that are not available on conda/conda-forge.
 
 ```bash
-pip install cdlib[all]
+pip install 'cdlib[all]'
 ```
 
 This option will install all optional dependencies accessible with the flag ``C`` and ``pypi``.
 
 #### (Advanced) 
 
 Due to some strict requirements, the installation of a subset of optional dependencies is left outside the previous procedures.
```

### Comparing `cdlib-0.3.0/cdlib.egg-info/SOURCES.txt` & `cdlib-0.4.0/cdlib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 cdlib/algorithms/internal/belief_prop.py
 cdlib/algorithms/internal/core_exp.py
 cdlib/algorithms/internal/em.py
 cdlib/algorithms/internal/ga.py
 cdlib/algorithms/internal/graph_entropy.py
 cdlib/algorithms/internal/headtail.py
 cdlib/algorithms/internal/lfm.py
+cdlib/algorithms/internal/markov_clustering.py
 cdlib/algorithms/internal/modularity_m.py
 cdlib/algorithms/internal/modularity_r.py
 cdlib/algorithms/internal/multicom.py
 cdlib/algorithms/internal/paris.py
 cdlib/algorithms/internal/principled.py
 cdlib/algorithms/internal/pycondor.py
 cdlib/algorithms/internal/scan.py
@@ -89,18 +90,31 @@
 cdlib/ensemble/__init__.py
 cdlib/ensemble/bunch_executions.py
 cdlib/evaluation/__init__.py
 cdlib/evaluation/comparison.py
 cdlib/evaluation/comparisonranking.py
 cdlib/evaluation/fitness.py
 cdlib/evaluation/fitnessranking.py
+cdlib/evaluation/internal/NF1.py
 cdlib/evaluation/internal/TOPSIS.py
 cdlib/evaluation/internal/__init__.py
 cdlib/evaluation/internal/link_modularity.py
 cdlib/evaluation/internal/omega.py
 cdlib/evaluation/internal/onmi.py
 cdlib/evaluation/internal/statistical_ranking.py
+cdlib/lifecycles/__init__.py
+cdlib/lifecycles/algorithms/__init__.py
+cdlib/lifecycles/algorithms/classic_match.py
+cdlib/lifecycles/algorithms/event_analysis.py
+cdlib/lifecycles/algorithms/measures.py
+cdlib/lifecycles/algorithms/null_model.py
+cdlib/lifecycles/classes/__init__.py
+cdlib/lifecycles/classes/event.py
+cdlib/lifecycles/classes/matching.py
+cdlib/lifecycles/utils/__init__.py
+cdlib/lifecycles/utils/utils.py
 cdlib/readwrite/__init__.py
 cdlib/readwrite/io.py
 cdlib/viz/__init__.py
+cdlib/viz/community_events.py
 cdlib/viz/networks.py
 cdlib/viz/plots.py
```

### Comparing `cdlib-0.3.0/setup.py` & `cdlib-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
+
 __author__ = "Giulio Rossetti"
 __license__ = "BSD-2-Clause"
 __email__ = "giulio.rossetti@gmail.com"
 
 
 here = path.abspath(path.dirname(__file__))
 
@@ -15,15 +16,15 @@
 
 with open(path.join(here, "requirements.txt"), encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="cdlib",
-    version="0.3.0",
+    version="0.4.0",
     license="BSD-Clause-2",
     description="Community Discovery Library",
     url="https://github.com/GiulioRossetti/cdlib",
     author="Giulio Rossetti",
     author_email="giulio.rossetti@gmail.com",
     classifiers=[
         # How mature is this project? Common values are
@@ -50,28 +51,26 @@
     extras_require={
         "C": [
             "infomap>=1.3.0",
             "wurlitzer>=1.0.2",
             "GraphRicciCurvature",
             "networkit",
             "pycombo",
-            "leidenalg"
-        ],
-        "pypi": [
-            "bayanpy",
-            "pyclustering"
+            "leidenalg",
         ],
+        "pypi": ["bayanpy", "pyclustering", "clusim"],
         "all": [
             "infomap>=1.3.0",
             "wurlitzer>=1.0.2",
             "GraphRicciCurvature",
             "networkit",
             "pycombo",
             "leidenalg",
             "bayanpy",
-            "pyclustering"
-        ]
+            "pyclustering",
+            "clusim",
+        ],
     },
     packages=find_packages(
         exclude=["*.test", "*.test.*", "test.*", "test", "cdlib.test", "cdlib.test.*"]
     ),
 )
```

