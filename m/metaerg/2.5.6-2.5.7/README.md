# Comparing `tmp/metaerg-2.5.6.tar.gz` & `tmp/metaerg-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaerg-2.5.6.tar", last modified: Wed Apr 17 21:36:31 2024, max compression
+gzip compressed data, was "metaerg-2.5.7.tar", last modified: Tue May 21 17:44:26 2024, max compression
```

## Comparing `metaerg-2.5.6.tar` & `metaerg-2.5.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 21:36:31.203657 metaerg-2.5.6/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    27706 2024-04-17 21:36:31.203657 metaerg-2.5.6/PKG-INFO
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    26558 2024-04-17 21:36:24.000000 metaerg-2.5.6/README.md
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)      103 2023-05-24 19:12:00.000000 metaerg-2.5.6/pyproject.toml
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)       78 2024-04-17 21:36:31.203657 metaerg-2.5.6/setup.cfg
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1630 2024-04-17 21:36:24.000000 metaerg-2.5.6/setup.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 21:36:31.200324 metaerg-2.5.6/src/
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 21:36:31.200324 metaerg-2.5.6/src/metaerg/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.6/src/metaerg/__init__.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 21:36:31.200324 metaerg-2.5.6/src/metaerg/calculations/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.6/src/metaerg/calculations/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3444 2023-08-30 16:15:59.000000 metaerg-2.5.6/src/metaerg/calculations/cluster_database.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    14431 2024-02-16 15:24:10.000000 metaerg-2.5.6/src/metaerg/calculations/codon_usage_bias.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    22700 2024-04-17 21:36:24.000000 metaerg-2.5.6/src/metaerg/context.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 21:36:31.200324 metaerg-2.5.6/src/metaerg/datatypes/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.6/src/metaerg/datatypes/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7085 2024-02-08 17:31:28.000000 metaerg-2.5.6/src/metaerg/datatypes/blast.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2996 2024-04-17 21:28:57.000000 metaerg-2.5.6/src/metaerg/datatypes/excel.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     8709 2023-08-18 21:22:31.000000 metaerg-2.5.6/src/metaerg/datatypes/fasta.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7143 2024-04-11 15:56:34.000000 metaerg-2.5.6/src/metaerg/datatypes/functional_genes.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4997 2024-02-21 20:53:57.000000 metaerg-2.5.6/src/metaerg/datatypes/gbk.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5628 2024-02-13 17:36:57.000000 metaerg-2.5.6/src/metaerg/datatypes/gff.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4951 2023-08-16 16:12:04.000000 metaerg-2.5.6/src/metaerg/datatypes/ncbi_ftp.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    17721 2024-04-17 17:29:54.000000 metaerg-2.5.6/src/metaerg/datatypes/sqlite.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 21:36:31.203657 metaerg-2.5.6/src/metaerg/html/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)       97 2023-05-24 19:12:00.000000 metaerg-2.5.6/src/metaerg/html/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3656 2023-05-24 19:12:00.000000 metaerg-2.5.6/src/metaerg/html/html_all_genomes.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6882 2024-02-16 22:08:40.000000 metaerg-2.5.6/src/metaerg/html/html_feature_details.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     9850 2024-02-16 22:08:40.000000 metaerg-2.5.6/src/metaerg/html/html_feature_table.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3307 2023-05-24 19:12:00.000000 metaerg-2.5.6/src/metaerg/html/html_genome_properties_and_subsystems.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    17193 2024-02-23 16:22:10.000000 metaerg-2.5.6/src/metaerg/installation.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    15175 2024-04-17 21:28:57.000000 metaerg-2.5.6/src/metaerg/main.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)      109 2023-05-24 19:12:00.000000 metaerg-2.5.6/src/metaerg/registry.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 21:36:31.203657 metaerg-2.5.6/src/metaerg/run_and_read/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)      197 2023-12-07 19:43:19.000000 metaerg-2.5.6/src/metaerg/run_and_read/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7290 2024-04-17 17:36:43.000000 metaerg-2.5.6/src/metaerg/run_and_read/antismash.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5507 2024-04-17 17:36:40.000000 metaerg-2.5.6/src/metaerg/run_and_read/aragorn.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6460 2024-04-17 17:37:11.000000 metaerg-2.5.6/src/metaerg/run_and_read/cdd.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2387 2024-04-17 17:37:10.000000 metaerg-2.5.6/src/metaerg/run_and_read/checkm.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6360 2024-04-17 17:37:31.000000 metaerg-2.5.6/src/metaerg/run_and_read/cmscan.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    37930 2024-04-17 18:06:00.000000 metaerg-2.5.6/src/metaerg/run_and_read/comparative_genomics.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2213 2024-04-17 17:37:53.000000 metaerg-2.5.6/src/metaerg/run_and_read/crispr_detect.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 21:36:31.203657 metaerg-2.5.6/src/metaerg/run_and_read/data/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.6/src/metaerg/run_and_read/data/__init__.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    75923 2024-04-11 15:35:57.000000 metaerg-2.5.6/src/metaerg/run_and_read/data/functional_gene_data
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5800 2024-04-17 17:38:44.000000 metaerg-2.5.6/src/metaerg/run_and_read/deepsig.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    26068 2024-04-17 17:38:44.000000 metaerg-2.5.6/src/metaerg/run_and_read/diamond_and_blastn.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    14194 2024-04-17 20:21:43.000000 metaerg-2.5.6/src/metaerg/run_and_read/functional_genes.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3644 2024-04-17 17:38:42.000000 metaerg-2.5.6/src/metaerg/run_and_read/gene_writer.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1683 2024-04-17 17:38:59.000000 metaerg-2.5.6/src/metaerg/run_and_read/ltr_harvest.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1445 2024-04-17 17:39:10.000000 metaerg-2.5.6/src/metaerg/run_and_read/minced.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6214 2024-04-17 17:39:24.000000 metaerg-2.5.6/src/metaerg/run_and_read/padloc.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4676 2024-04-17 17:50:21.000000 metaerg-2.5.6/src/metaerg/run_and_read/prodigal.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6452 2024-04-17 17:41:08.000000 metaerg-2.5.6/src/metaerg/run_and_read/pureseqtm.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5688 2024-04-17 18:01:07.000000 metaerg-2.5.6/src/metaerg/run_and_read/repeat_masker.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1825 2024-04-17 17:40:12.000000 metaerg-2.5.6/src/metaerg/run_and_read/signalp.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2644 2024-04-17 17:40:42.000000 metaerg-2.5.6/src/metaerg/run_and_read/tmhmm.py
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2368 2024-04-17 18:01:07.000000 metaerg-2.5.6/src/metaerg/run_and_read/trf.py
-drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-04-17 21:36:31.203657 metaerg-2.5.6/src/metaerg.egg-info/
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)    27706 2024-04-17 21:36:31.000000 metaerg-2.5.6/src/metaerg.egg-info/PKG-INFO
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1892 2024-04-17 21:36:31.000000 metaerg-2.5.6/src/metaerg.egg-info/SOURCES.txt
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        1 2024-04-17 21:36:31.000000 metaerg-2.5.6/src/metaerg.egg-info/dependency_links.txt
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)       46 2024-04-17 21:36:31.000000 metaerg-2.5.6/src/metaerg.egg-info/entry_points.txt
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)      148 2024-04-17 21:36:31.000000 metaerg-2.5.6/src/metaerg.egg-info/requires.txt
--rw-r--r--   0 mstrous   (1000) mstrous   (1000)        8 2024-04-17 21:36:31.000000 metaerg-2.5.6/src/metaerg.egg-info/top_level.txt
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-05-21 17:44:26.301784 metaerg-2.5.7/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    27706 2024-05-21 17:44:26.301784 metaerg-2.5.7/PKG-INFO
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    26558 2024-05-21 17:24:57.000000 metaerg-2.5.7/README.md
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      103 2023-05-24 19:12:00.000000 metaerg-2.5.7/pyproject.toml
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       78 2024-05-21 17:44:26.305117 metaerg-2.5.7/setup.cfg
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1630 2024-05-21 17:25:10.000000 metaerg-2.5.7/setup.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-05-21 17:44:26.295117 metaerg-2.5.7/src/
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-05-21 17:44:26.298451 metaerg-2.5.7/src/metaerg/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.7/src/metaerg/__init__.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-05-21 17:44:26.298451 metaerg-2.5.7/src/metaerg/calculations/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.7/src/metaerg/calculations/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3444 2023-08-30 16:15:59.000000 metaerg-2.5.7/src/metaerg/calculations/cluster_database.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    14431 2024-02-16 15:24:10.000000 metaerg-2.5.7/src/metaerg/calculations/codon_usage_bias.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    22700 2024-05-21 17:24:57.000000 metaerg-2.5.7/src/metaerg/context.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-05-21 17:44:26.298451 metaerg-2.5.7/src/metaerg/datatypes/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.7/src/metaerg/datatypes/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7085 2024-02-08 17:31:28.000000 metaerg-2.5.7/src/metaerg/datatypes/blast.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3034 2024-04-17 21:42:45.000000 metaerg-2.5.7/src/metaerg/datatypes/excel.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     8709 2023-08-18 21:22:31.000000 metaerg-2.5.7/src/metaerg/datatypes/fasta.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7143 2024-04-11 15:56:34.000000 metaerg-2.5.7/src/metaerg/datatypes/functional_genes.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4997 2024-02-21 20:53:57.000000 metaerg-2.5.7/src/metaerg/datatypes/gbk.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5628 2024-02-13 17:36:57.000000 metaerg-2.5.7/src/metaerg/datatypes/gff.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4951 2023-08-16 16:12:04.000000 metaerg-2.5.7/src/metaerg/datatypes/ncbi_ftp.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    17721 2024-04-17 17:29:54.000000 metaerg-2.5.7/src/metaerg/datatypes/sqlite.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-05-21 17:44:26.301784 metaerg-2.5.7/src/metaerg/html/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       97 2023-05-24 19:12:00.000000 metaerg-2.5.7/src/metaerg/html/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3656 2023-05-24 19:12:00.000000 metaerg-2.5.7/src/metaerg/html/html_all_genomes.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6882 2024-02-16 22:08:40.000000 metaerg-2.5.7/src/metaerg/html/html_feature_details.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     9850 2024-02-16 22:08:40.000000 metaerg-2.5.7/src/metaerg/html/html_feature_table.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3307 2023-05-24 19:12:00.000000 metaerg-2.5.7/src/metaerg/html/html_genome_properties_and_subsystems.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    17193 2024-02-23 16:22:10.000000 metaerg-2.5.7/src/metaerg/installation.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    15175 2024-04-17 21:28:57.000000 metaerg-2.5.7/src/metaerg/main.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      109 2023-05-24 19:12:00.000000 metaerg-2.5.7/src/metaerg/registry.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-05-21 17:44:26.301784 metaerg-2.5.7/src/metaerg/run_and_read/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      197 2023-12-07 19:43:19.000000 metaerg-2.5.7/src/metaerg/run_and_read/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7290 2024-04-17 17:36:43.000000 metaerg-2.5.7/src/metaerg/run_and_read/antismash.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5507 2024-04-17 17:36:40.000000 metaerg-2.5.7/src/metaerg/run_and_read/aragorn.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6460 2024-04-17 17:37:11.000000 metaerg-2.5.7/src/metaerg/run_and_read/cdd.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2387 2024-04-17 17:37:10.000000 metaerg-2.5.7/src/metaerg/run_and_read/checkm.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6360 2024-04-17 17:37:31.000000 metaerg-2.5.7/src/metaerg/run_and_read/cmscan.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    38442 2024-05-21 17:23:54.000000 metaerg-2.5.7/src/metaerg/run_and_read/comparative_genomics.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2213 2024-04-17 17:37:53.000000 metaerg-2.5.7/src/metaerg/run_and_read/crispr_detect.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-05-21 17:44:26.301784 metaerg-2.5.7/src/metaerg/run_and_read/data/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2023-05-24 19:12:00.000000 metaerg-2.5.7/src/metaerg/run_and_read/data/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    75924 2024-04-19 14:49:47.000000 metaerg-2.5.7/src/metaerg/run_and_read/data/functional_gene_data
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5800 2024-04-17 17:38:44.000000 metaerg-2.5.7/src/metaerg/run_and_read/deepsig.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    26068 2024-04-17 17:38:44.000000 metaerg-2.5.7/src/metaerg/run_and_read/diamond_and_blastn.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    14194 2024-04-17 20:21:43.000000 metaerg-2.5.7/src/metaerg/run_and_read/functional_genes.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3644 2024-04-17 17:38:42.000000 metaerg-2.5.7/src/metaerg/run_and_read/gene_writer.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1683 2024-04-17 17:38:59.000000 metaerg-2.5.7/src/metaerg/run_and_read/ltr_harvest.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1445 2024-04-17 17:39:10.000000 metaerg-2.5.7/src/metaerg/run_and_read/minced.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6214 2024-04-17 17:39:24.000000 metaerg-2.5.7/src/metaerg/run_and_read/padloc.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4676 2024-04-17 17:50:21.000000 metaerg-2.5.7/src/metaerg/run_and_read/prodigal.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6452 2024-04-17 17:41:08.000000 metaerg-2.5.7/src/metaerg/run_and_read/pureseqtm.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5688 2024-04-17 18:01:07.000000 metaerg-2.5.7/src/metaerg/run_and_read/repeat_masker.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1825 2024-04-17 17:40:12.000000 metaerg-2.5.7/src/metaerg/run_and_read/signalp.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2644 2024-04-17 17:40:42.000000 metaerg-2.5.7/src/metaerg/run_and_read/tmhmm.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2368 2024-04-17 18:01:07.000000 metaerg-2.5.7/src/metaerg/run_and_read/trf.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2024-05-21 17:44:26.301784 metaerg-2.5.7/src/metaerg.egg-info/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    27706 2024-05-21 17:44:26.000000 metaerg-2.5.7/src/metaerg.egg-info/PKG-INFO
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1892 2024-05-21 17:44:26.000000 metaerg-2.5.7/src/metaerg.egg-info/SOURCES.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        1 2024-05-21 17:44:26.000000 metaerg-2.5.7/src/metaerg.egg-info/dependency_links.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       46 2024-05-21 17:44:26.000000 metaerg-2.5.7/src/metaerg.egg-info/entry_points.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      148 2024-05-21 17:44:26.000000 metaerg-2.5.7/src/metaerg.egg-info/requires.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        8 2024-05-21 17:44:26.000000 metaerg-2.5.7/src/metaerg.egg-info/top_level.txt
```

### Comparing `metaerg-2.5.6/PKG-INFO` & `metaerg-2.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaerg
-Version: 2.5.6
+Version: 2.5.7
 Summary: Annotation of genomes and contigs
 Home-page: https://github.com/kinestetika/MetaErg
 Author: Marc Strous
 Author-email: mstrous@ucalgary.ca
 License: MIT
 Project-URL: Source, https://github.com/kinestetika/MetaErg
 Keywords: repeat-regions genes functions taxonomy
@@ -30,15 +30,15 @@
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 
-## metaerg.py, version 2.5.6
+## metaerg.py, version 2.5.7
 
 Metaerg.py annotates genomes or sets of mags/bins from microbial ecosystems (bacteria, archaea, viruses). Input data 
 consists of nucleotide fasta files, one per genome or mag, each with one or more contigs. Output files with annotations 
 are in common formats such as .gff, .gbk, .fasta and .html with predicted genes, their functions and taxonomic 
 classifications.
 
 Metaerg 2.5 can annotate a group of related genomes and apply a suite of comparative genomics analyses. To do this, put
```

### Comparing `metaerg-2.5.6/README.md` & `metaerg-2.5.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## metaerg.py, version 2.5.6
+## metaerg.py, version 2.5.7
 
 Metaerg.py annotates genomes or sets of mags/bins from microbial ecosystems (bacteria, archaea, viruses). Input data 
 consists of nucleotide fasta files, one per genome or mag, each with one or more contigs. Output files with annotations 
 are in common formats such as .gff, .gbk, .fasta and .html with predicted genes, their functions and taxonomic 
 classifications.
 
 Metaerg 2.5 can annotate a group of related genomes and apply a suite of comparative genomics analyses. To do this, put
```

### Comparing `metaerg-2.5.6/setup.py` & `metaerg-2.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='metaerg',
-    version='2.5.6',
+    version='2.5.7',
     packages=setuptools.find_packages(where='src'),
     url='https://github.com/kinestetika/MetaErg',
     license='MIT',
     author='Marc Strous',
     author_email='mstrous@ucalgary.ca',
     description='Annotation of genomes and contigs',
     long_description=long_description,
```

### Comparing `metaerg-2.5.6/src/metaerg/calculations/cluster_database.py` & `metaerg-2.5.7/src/metaerg/calculations/cluster_database.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/calculations/codon_usage_bias.py` & `metaerg-2.5.7/src/metaerg/calculations/codon_usage_bias.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/context.py` & `metaerg-2.5.7/src/metaerg/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from time import sleep
 
 import httpx
 
 from metaerg import registry
 from metaerg.datatypes import sqlite
 
-VERSION = "2.5.6"
+VERSION = "2.5.7"
 
 BASE_DIR = Path()
 TEMP_DIR = Path()
 HTML_DIR = Path()
 DATABASE_DIR = Path()
 CHECKM_DIR:None | Path = None
 GTDBTK_DIR:None | Path = None
```

### Comparing `metaerg-2.5.6/src/metaerg/datatypes/blast.py` & `metaerg-2.5.7/src/metaerg/datatypes/blast.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/datatypes/excel.py` & `metaerg-2.5.7/src/metaerg/datatypes/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,12 +65,13 @@
         for subsystem, genes in genome.subsystems.items():
             first_row = True
             for gene, feature_ids in genes.items():
                 if first_row:
                     e_sheet.cell(row=row, column=1).value = subsystem
                 else:
                     e_sheet.cell(row=row, column=1).value = ''
+                    first_row = False
                 e_sheet.cell(row=row, column=2).value = gene
                 e_sheet.cell(row=row, column=e_column).value = ', '.join(feature_ids)
                 row += 1
         e_column += 1
     e_workbook.save(excel_file)
```

### Comparing `metaerg-2.5.6/src/metaerg/datatypes/fasta.py` & `metaerg-2.5.7/src/metaerg/datatypes/fasta.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/datatypes/functional_genes.py` & `metaerg-2.5.7/src/metaerg/datatypes/functional_genes.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/datatypes/gbk.py` & `metaerg-2.5.7/src/metaerg/datatypes/gbk.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/datatypes/gff.py` & `metaerg-2.5.7/src/metaerg/datatypes/gff.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/datatypes/ncbi_ftp.py` & `metaerg-2.5.7/src/metaerg/datatypes/ncbi_ftp.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/datatypes/sqlite.py` & `metaerg-2.5.7/src/metaerg/datatypes/sqlite.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/html/html_all_genomes.py` & `metaerg-2.5.7/src/metaerg/html/html_all_genomes.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/html/html_feature_details.py` & `metaerg-2.5.7/src/metaerg/html/html_feature_details.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/html/html_feature_table.py` & `metaerg-2.5.7/src/metaerg/html/html_feature_table.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/html/html_genome_properties_and_subsystems.py` & `metaerg-2.5.7/src/metaerg/html/html_genome_properties_and_subsystems.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/installation.py` & `metaerg-2.5.7/src/metaerg/installation.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/main.py` & `metaerg-2.5.7/src/metaerg/main.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/antismash.py` & `metaerg-2.5.7/src/metaerg/run_and_read/antismash.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/aragorn.py` & `metaerg-2.5.7/src/metaerg/run_and_read/aragorn.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/cdd.py` & `metaerg-2.5.7/src/metaerg/run_and_read/cdd.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/checkm.py` & `metaerg-2.5.7/src/metaerg/run_and_read/checkm.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/cmscan.py` & `metaerg-2.5.7/src/metaerg/run_and_read/cmscan.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/comparative_genomics.py` & `metaerg-2.5.7/src/metaerg/run_and_read/comparative_genomics.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             yield Cluster(current_cluster_seq_id_list, self.taxa_by_orf_id, self.blast_scores)
 
 
 def cluster(seq_id_2_taxon: list, cluster_list: list,
             input_fasta_file:Path, tmp_dir: Path, fasta_output_dir: Path,
             fraction_id:float=0.5, fraction_overlap:float=0.8,
             min_fraction_orthologues:float=0.0,
-            min_fraction_of_taxa_represented:float=0.1, min_taxa_represented:float=3,
+            min_fraction_of_taxa_represented:float=0.0, min_taxa_represented:float=3,
             include_paralogues_in_fasta_output=True, file_extension:str='.faa'):
     unique_taxa = {taxon for taxon in seq_id_2_taxon}
     context.log(f'Now clustering sequences in {input_fasta_file}...')
     context.log(f'Working with {len(unique_taxa)} unique taxa.')
     # prep files
     tmp_dir.mkdir(exist_ok=True)
     cluster_file_base = input_fasta_file.parent / f'{input_fasta_file.stem}.clustering'
@@ -144,27 +144,27 @@
     coded_seq_id_2_cluster_rejected = {}
     rejected_cluster_count = 0
     error_count = 0
     percent_id = 0
     accepted_cluster_count = 0
     sequences_clustered_count = 0
     taxon_representaton = Counter()
-    final_min_taxpon_threshold = max(min_taxa_represented, min_fraction_of_taxa_represented * len(unique_taxa))
+    final_min_taxon_threshold = max(min_taxa_represented, min_fraction_of_taxa_represented * len(unique_taxa))
     with MMSeqsClusterParser(cluster_file_tsv, seq_id_2_taxon, blast_scores) as reader:
         for cluster in reader:
             cluster.seq_type = file_extension
             cluster.members = []  # list of tuples (id, taxon, is_paralogue]
             cluster.annotation = ''
             cluster.lengths = []
             cluster.links = []  # links to other clusters based on gene-context, list of tuples (other cluster, score)
             cluster.codon_bias_quantile = -1  # quantile of median codon usage bias (orthologous members only), 0 = low expression, 9 = high expression
             cluster.selection_omega = -1  # w = ka / ks (orthologous members only)
             cluster.selection_omega_quantile = -1  # quantile of median w, 0 = purifying, 9 = diversifying
             if cluster.fraction_orthologues < min_fraction_orthologues \
-                    or len(cluster.taxa) < final_min_taxpon_threshold\
+                    or len(cluster.taxa) < final_min_taxon_threshold\
                     or cluster.error:
                 error_count += cluster.error
                 for seq_id in cluster.seq_ids:
                     coded_seq_id_2_cluster_rejected[seq_id] = cluster
                 cluster.id = f'rejected_{rejected_cluster_count}'
                 cluster.fasta_file = rejected_fasta_output_dir /  f'{cluster.id}{file_extension}'
                 rejected_cluster_count += 1
@@ -176,15 +176,20 @@
                     coded_seq_id_2_cluster[seq_id] = cluster
                 taxon_representaton.update(cluster.taxa)
                 cluster.fasta_file = fasta_output_dir / f'{cluster.id}{file_extension}'
                 accepted_cluster_count += 1
                 sequences_clustered_count += len(cluster.seq_ids)
             cluster.taxa = set()  # reset taxa, recoded numbers will be replaced with original filenames
 
-    context.log(f'Accepted {accepted_cluster_count} clusters in total, rejected {rejected_cluster_count} because <{final_min_taxpon_threshold} taxa represented or too many ({(1-min_fraction_orthologues):.1%}) paralogues, {error_count} due to lacking mmseqs alignments.')
+    context.log(f'Accepted {accepted_cluster_count} clusters in total, rejected {rejected_cluster_count} because <{final_min_taxon_threshold} taxa represented or too many ({(1-min_fraction_orthologues):.1%}) paralogues, {error_count} due to lacking mmseqs alignments.')
+    if accepted_cluster_count == 0 or not cluster_list:
+        context.log(f'Fatal problem in comparative genomics analysis of {file_extension} files - no sets of homologous '
+                    f'genes were acceptable. This happens when too few genomes or MAGs were included in the analysis or '
+                    f'data quality is very poor.')
+        return
     context.log(f'Average percent id among all clusters: {percent_id/accepted_cluster_count:.1%}')
     # filter out taxa with poor representaton
     poorly_represented_taxa = {t for t in unique_taxa if taxon_representaton[t] < 0.2 * len(cluster_list)}
     for t in poorly_represented_taxa:
         context.log(f'WARNING: taxon {t}; represented in only {taxon_representaton[t]/len(cluster_list):.1%} of clusters.')
 
     taxonomy_pattern = re.compile(r'\s\(Bacteria;.+?\)$|\s\(Archaea;.+?\)$|\s\(Viruses;.+?\)$|\s\(Eukaryota;.+?\)$') # |(\s\(Archaea;.+?\)$)|(\s\(Viruses;.+?\)$)
@@ -592,14 +597,18 @@
             file_extension = '.faa')
     cluster(seq_id_2_taxon=seq_id_2_taxon, cluster_list=cluster_list,
             input_fasta_file=rna_merged_fasta_file,
             tmp_dir=comparative_genomics_dir / 'tmp',
             fasta_output_dir=rna_clusters_dir,
             fraction_id=0.5,
             file_extension='.fna')
+    if not cluster_list:
+        context.log('No acceptable sets of homologous genes found. Aborting comparative genomics analysis.')
+        return
+
     align_aa_clusters(cluster_list, cds_clusters_alignment_dir)
     save_clusters_as_nt_fasta_and_compute_codon_bias(cluster_list, taxa, cds_clusters_nt_dir)
     estimate_selection_pressure(cluster_list, cds_clusters_alignment_dir, cds_clusters_nt_dir)
     write_homologue_info_to_sql(cluster_list, taxa)
     cluster_context_links = analyse_gene_context(cluster_list, taxa, cluster_window_size, min_match_score)
     write_overview_tsv_file(comparative_genomics_dir, cluster_list, taxa)
     write_remaining_results_to_sql(cluster_list, cluster_context_links, taxa, cluster_window_size)
```

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/crispr_detect.py` & `metaerg-2.5.7/src/metaerg/run_and_read/crispr_detect.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/data/functional_gene_data` & `metaerg-2.5.7/src/metaerg/run_and_read/data/functional_gene_data`

 * *Files 1% similar despite different names*

```diff
@@ -692,15 +692,15 @@
 10 PRK05557|PRK05565|PRK05786|PRK06077|PRK06463|PRK06550|PRK07666|PRK07792|PRK08217|PRK08261|PRK08642|PRK12825 3-Oxoacyl-acyl-carrier protein reductase FabG
 11 PRK08063 Enoyl-acyl-carrier-protein reductase FabL
 12 PRK13656 Enoyl-acyl-carrier-protein reductase FabV
 
 >Metabolism, Phosphonate Biosynthesis
 1 TIGR02320 Phosphoenolpyruvate mutase, PepM
 2 TIGR03297 Phosphonopyruvate decarboxylase, Ppd/AepY
-3 cd08182 Hydroxyethylphosphoate dehydrogenase HepD/PhpC
+3 cd08182 Hydroxyethylphosphoate dehydrogenase, HepD/PhpC
 4 TIGR03405 Phosphonate-associated iron-containing alcohol dehydrogenase
 
 >Metabolism, Phosphonate Degradation, Generic Pathway
 1 cl01456|COG3626|pfam05861 Alpha-D-ribose 1-methylphosphonate 5-triphosphate synthase, PhnI
 2 COG3454|PRK15446|TIGR02318 Alpha-D-ribose 1-methylphosphonate 5-triphosphate diphosphatase, PhnM
 3 COG3627 Alpha-D-ribose 1-methylphosphonate 5-phosphate C-P lyase, PhnJ
```

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/deepsig.py` & `metaerg-2.5.7/src/metaerg/run_and_read/deepsig.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/diamond_and_blastn.py` & `metaerg-2.5.7/src/metaerg/run_and_read/diamond_and_blastn.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/functional_genes.py` & `metaerg-2.5.7/src/metaerg/run_and_read/functional_genes.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/gene_writer.py` & `metaerg-2.5.7/src/metaerg/run_and_read/gene_writer.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/ltr_harvest.py` & `metaerg-2.5.7/src/metaerg/run_and_read/ltr_harvest.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/minced.py` & `metaerg-2.5.7/src/metaerg/run_and_read/minced.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/padloc.py` & `metaerg-2.5.7/src/metaerg/run_and_read/padloc.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/prodigal.py` & `metaerg-2.5.7/src/metaerg/run_and_read/prodigal.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/pureseqtm.py` & `metaerg-2.5.7/src/metaerg/run_and_read/pureseqtm.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/repeat_masker.py` & `metaerg-2.5.7/src/metaerg/run_and_read/repeat_masker.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/signalp.py` & `metaerg-2.5.7/src/metaerg/run_and_read/signalp.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/tmhmm.py` & `metaerg-2.5.7/src/metaerg/run_and_read/tmhmm.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg/run_and_read/trf.py` & `metaerg-2.5.7/src/metaerg/run_and_read/trf.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.5.6/src/metaerg.egg-info/PKG-INFO` & `metaerg-2.5.7/src/metaerg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaerg
-Version: 2.5.6
+Version: 2.5.7
 Summary: Annotation of genomes and contigs
 Home-page: https://github.com/kinestetika/MetaErg
 Author: Marc Strous
 Author-email: mstrous@ucalgary.ca
 License: MIT
 Project-URL: Source, https://github.com/kinestetika/MetaErg
 Keywords: repeat-regions genes functions taxonomy
@@ -30,15 +30,15 @@
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 
-## metaerg.py, version 2.5.6
+## metaerg.py, version 2.5.7
 
 Metaerg.py annotates genomes or sets of mags/bins from microbial ecosystems (bacteria, archaea, viruses). Input data 
 consists of nucleotide fasta files, one per genome or mag, each with one or more contigs. Output files with annotations 
 are in common formats such as .gff, .gbk, .fasta and .html with predicted genes, their functions and taxonomic 
 classifications.
 
 Metaerg 2.5 can annotate a group of related genomes and apply a suite of comparative genomics analyses. To do this, put
```

### Comparing `metaerg-2.5.6/src/metaerg.egg-info/SOURCES.txt` & `metaerg-2.5.7/src/metaerg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

