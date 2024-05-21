# Comparing `tmp/wgse_ng-1.0.0a5.tar.gz` & `tmp/wgse_ng-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-1.0.0a5.tar", last modified: Sat May 18 06:50:03 2024, max compression
+gzip compressed data, was "wgse_ng-1.0.0a7.tar", last modified: Tue May 21 06:02:43 2024, max compression
```

## Comparing `wgse_ng-1.0.0a5.tar` & `wgse_ng-1.0.0a7.tar`

### file list

```diff
@@ -1,134 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.143529 wgse_ng-1.0.0a5/
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-18 06:50:03.143529 wgse_ng-1.0.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.143529 wgse_ng-1.0.0a5/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-18 06:50:03.000000 wgse_ng-1.0.0a5/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-18 06:50:03.000000 wgse_ng-1.0.0a5/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 06:50:03.000000 wgse_ng-1.0.0a5/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-18 06:50:03.000000 wgse_ng-1.0.0a5/WGSE_NG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-18 06:50:03.000000 wgse_ng-1.0.0a5/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 06:50:03.000000 wgse_ng-1.0.0a5/WGSE_NG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 06:50:03.143529 wgse_ng-1.0.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.111529 wgse_ng-1.0.0a5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/test/test_raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/test/test_unknown_bases_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.111529 wgse_ng-1.0.0a5/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.111529 wgse_ng-1.0.0a5/wgse/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/adapters/alignment_map_file_info_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/adapters/alignment_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/adapters/header_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/adapters/index_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/adapters/reference_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.111529 wgse_ng-1.0.0a5/wgse/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/alignment_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/alignment_map/alignment_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/alignment_map/alignment_map_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/alignment_map/alignment_map_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/alignment_map/alignment_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/alignment_map/depth_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/alignment_map/index_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.115529 wgse_ng-1.0.0a5/wgse/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/alignment_map_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/alignment_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/chromosome_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/genome.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/mitochondrial_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/mitochondrial_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/mitochondrial_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/read_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/data/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.115529 wgse_ng-1.0.0a5/wgse/fasta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/fasta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/fasta/fasta_letter_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/fasta/fasta_stats_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/fasta/letter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/fasta/letter_run_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/fasta/letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/fasta/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.119529 wgse_ng-1.0.0a5/wgse/fastq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/fastq/fastq_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.119529 wgse_ng-1.0.0a5/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/gui/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/gui/microarray_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/gui/ui_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/gui/ui_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.123529 wgse_ng-1.0.0a5/wgse/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.135529 wgse_ng-1.0.0a5/wgse/metadata/bed_templates/
--rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/metadata/bed_templates/19_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/metadata/bed_templates/19_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/metadata/bed_templates/38_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/metadata/bed_templates/38_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/metadata/bed_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:58.000000 wgse_ng-1.0.0a5/wgse/metadata/builds.json
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/mtdna.json
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/ploidy.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4213156 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/references.json
--rw-r--r--   0 runner    (1001) docker     (127)    17094 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/references_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.139529 wgse_ng-1.0.0a5/wgse/metadata/report_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/report_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/report_templates/table_macro.html
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/report_templates/table_simple.html
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/report_templates/table_tab.html
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/sequencers.json
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/metadata/sources.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.139529 wgse_ng-1.0.0a5/wgse/microarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/microarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/microarray/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/microarray/microarray_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/microarray/raw_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.139529 wgse_ng-1.0.0a5/wgse/mtDNA/
--rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/mtDNA/CRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/mtDNA/RSRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/mtDNA/Yoruba.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/mtDNA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/mtDNA/rCRS.fasta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.139529 wgse_ng-1.0.0a5/wgse/reference_genome/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/reference_genome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/reference_genome/bgzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/reference_genome/decompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/reference_genome/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/reference_genome/genome_metadata_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/reference_genome/repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.139529 wgse_ng-1.0.0a5/wgse/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/renderers/csv_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/renderers/html_aligned_file_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/renderers/html_simple_table_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:50:03.143529 wgse_ng-1.0.0a5/wgse/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/check_prerequisites.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/file_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/mt_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/sequence_orderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/sequencers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/unit_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/utility/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-18 06:49:59.000000 wgse_ng-1.0.0a5/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.879788 wgse_ng-1.0.0a7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.887788 wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/add-a-new-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.887788 wgse_ng-1.0.0a7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/workflows/python-pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.887788 wgse_ng-1.0.0a7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.891788 wgse_ng-1.0.0a7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/basic-usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/reference-genome.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/wgse-library.md
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/main.spec
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.891788 wgse_ng-1.0.0a7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116407 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/fake_genome.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_unknown_bases_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.891788 wgse_ng-1.0.0a7/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/fake_reference_genome_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/import_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/last_file_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/reference_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.891788 wgse_ng-1.0.0a7/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/wgse/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.895788 wgse_ng-1.0.0a7/wgse/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/alignment_map_file_info_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/alignment_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/header_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/index_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/reference_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.895788 wgse_ng-1.0.0a7/wgse/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/alignment_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/depth_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/index_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.899788 wgse_ng-1.0.0a7/wgse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/alignment_map_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/alignment_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/chromosome_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/mitochondrial_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/mitochondrial_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/mitochondrial_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/read_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.899788 wgse_ng-1.0.0a7/wgse/fasta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/fasta_letter_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/fasta_stats_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/letter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/letter_run_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.899788 wgse_ng-1.0.0a7/wgse/fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fastq/fastq_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.903788 wgse_ng-1.0.0a7/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/WGSE-NG.pyproject
+-rw-r--r--   0 runner    (1001) docker     (127)    11778 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/WGSE-NG.pyproject.user
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.903788 wgse_ng-1.0.0a7/wgse/gui/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/extract/extract_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/extract/format_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/extract/microarray_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/extract/sequence_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/form.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/reference.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.903788 wgse_ng-1.0.0a7/wgse/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67343 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/resources/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   327118 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/resources/logo_nXP_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/resources.qrc
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/ui_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.911788 wgse_ng-1.0.0a7/wgse/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/19_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/19_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/38_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/38_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/builds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/mtdna.json
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/ploidy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4213157 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/references.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/references_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/metadata/report_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/report_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_macro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/sequencers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/microarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/microarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/microarray/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/microarray/microarray_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/microarray/raw_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/mtDNA/
+-rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/CRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/RSRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/Yoruba.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/rCRS.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/reference_genome/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/bgzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/genome_metadata_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/wgse/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/renderers/csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/renderers/html_aligned_file_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/renderers/html_simple_table_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/wgse/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/check_prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/file_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/mt_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/process_io_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/sequence_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/sequencers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/simple_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/unit_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/variant_caller.py
```

### Comparing `wgse_ng-1.0.0a5/WGSE_NG.egg-info/SOURCES.txt` & `wgse_ng-1.0.0a7/WGSE_NG.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,53 @@
+.gitignore
+.pre-commit-config.yaml
+.readthedocs.yaml
+LICENSE
 README.md
-setup.py
+main.spec
+pyproject.toml
+.github/ISSUE_TEMPLATE/add-a-new-reference.md
+.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/python-app.yml
+.github/workflows/python-publish.yml
+.github/workflows/python-pyinstaller.yml
+.vscode/launch.json
+.vscode/settings.json
+.vscode/tasks.json
 WGSE_NG.egg-info/PKG-INFO
 WGSE_NG.egg-info/SOURCES.txt
 WGSE_NG.egg-info/dependency_links.txt
 WGSE_NG.egg-info/entry_points.txt
 WGSE_NG.egg-info/requires.txt
 WGSE_NG.egg-info/top_level.txt
+docs/Makefile
+docs/basic-usage.md
+docs/conf.py
+docs/index.rst
+docs/make.bat
+docs/reference-genome.md
+docs/requirements.in
+docs/requirements.txt
+docs/wgse-library.md
+test/__init__.py
+test/fake_genome.fasta
 test/test_buckets.py
 test/test_fasta.py
 test/test_fasta_dictionary.py
 test/test_microarray_converter.py
 test/test_raw_file.py
 test/test_sequence.py
 test/test_unknown_bases_stats.py
+test/utility.py
+tools/__init__.py
+tools/fake_reference_genome_generator.py
+tools/import_scanner.py
+tools/last_file_export.py
+tools/reference_stats.py
 wgse/VERSION.py
 wgse/__init__.py
 wgse/configuration.py
 wgse/main.py
 wgse/variant_caller.py
 wgse/adapters/__init__.py
 wgse/adapters/alignment_map_file_info_adapter.py
@@ -54,21 +85,29 @@
 wgse/fasta/fasta_stats_files.py
 wgse/fasta/letter_run.py
 wgse/fasta/letter_run_buckets.py
 wgse/fasta/letter_run_collection.py
 wgse/fasta/reference.py
 wgse/fastq/__init__.py
 wgse/fastq/fastq_file.py
+wgse/gui/WGSE-NG.pyproject
+wgse/gui/WGSE-NG.pyproject.user
 wgse/gui/__init__.py
-wgse/gui/extract.py
+wgse/gui/form.ui
 wgse/gui/main.py
-wgse/gui/microarray_format.py
+wgse/gui/reference.ui
+wgse/gui/resources.qrc
 wgse/gui/table_dialog.py
-wgse/gui/ui_extract.py
 wgse/gui/ui_form.py
+wgse/gui/extract/extract_wizard.py
+wgse/gui/extract/format_selection.py
+wgse/gui/extract/microarray_selection.py
+wgse/gui/extract/sequence_selection.py
+wgse/gui/resources/logo.jpg
+wgse/gui/resources/logo_nXP_icon.ico
 wgse/metadata/__init__.py
 wgse/metadata/builds.json
 wgse/metadata/mtdna.json
 wgse/metadata/ploidy.txt
 wgse/metadata/references.json
 wgse/metadata/references_template.json
 wgse/metadata/sequencers.json
@@ -103,12 +142,15 @@
 wgse/renderers/html_simple_table_report.py
 wgse/utility/__init__.py
 wgse/utility/check_prerequisites.py
 wgse/utility/external.py
 wgse/utility/file_type_checker.py
 wgse/utility/installer.py
 wgse/utility/mt_dna.py
+wgse/utility/process_io_monitor.py
 wgse/utility/regions.py
 wgse/utility/sequence_orderer.py
 wgse/utility/sequencers.py
+wgse/utility/shortcut.py
+wgse/utility/simple_worker.py
 wgse/utility/unit_prefix.py
 wgse/utility/updater.py
```

### Comparing `wgse_ng-1.0.0a5/test/test_buckets.py` & `wgse_ng-1.0.0a7/test/test_buckets.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,58 +12,62 @@
     # Act
     # 1000/10 = 100 -> 10 buckets with length of 100
     sut = LetterRunBuckets(sequence, 10, 0).buckets
     # Assert
     assert 0 in sut
     assert len(sut) == 1
     assert sut[0] == 99
-    
+
+
 def test_more_run_in_single_bucket():
     # Arrange
     sequence = LetterRunCollection("Foo", 1000)
     sequence.open_run(0)
     sequence.close_run(50)
-    
+
     sequence.open_run(51)
     sequence.close_run(60)
     # Act
     # 1000/10 = 100 -> 10 buckets with length of 100
     sut = LetterRunBuckets(sequence, 10, 0).buckets
     # Assert
     assert 0 in sut
     assert len(sut) == 1
     assert sut[0] == 59
-    
+
+
 def test_run_in_multiple_buckets():
     # Arrange
     sequence = LetterRunCollection("Foo", 1000)
     sequence.open_run(0)
     sequence.close_run(150)
     # Act
     # 1000/10 = 100 -> 10 buckets with length of 100
     sut = LetterRunBuckets(sequence, 10, 0).buckets
     # Assert
     assert 0 in sut
     assert 1 in sut
     assert len(sut) == 2
-    assert sut[0] == 99 # 0 -> 99
-    assert sut[1] == 50 # 99 -> 151
-    
+    assert sut[0] == 99  # 0 -> 99
+    assert sut[1] == 50  # 99 -> 151
+
+
 def test_too_many_buckets():
     sequence = LetterRunCollection("Foo", 1000)
 
     sequence.open_run(0)
     sequence.close_run(99)
 
     sequence.open_run(100)
     sequence.close_run(201)
 
     sut = LetterRunBuckets(sequence, 1001, 0).buckets
     assert len(sut) == 0
-    
+
+
 def test_run_end_to_end_divisible():
     sequence = LetterRunCollection("Foo", 1000)
 
     sequence.open_run(0)
     sequence.close_run(1000)
     sut = LetterRunBuckets(sequence, 10, 0).buckets
     for index in range(10):
@@ -75,15 +79,15 @@
     sequence = LetterRunCollection("Foo", 1000)
 
     sequence.open_run(0)
     sequence.close_run(1000)
     sut = LetterRunBuckets(sequence, 3, 0).buckets
     assert 0 in sut
     assert 1 in sut
-    assert 2 in sut    
+    assert 2 in sut
     assert 3 in sut
-    
+
     assert len(sut) == 4
     assert sut[0] == 332
     assert sut[1] == 332
     assert sut[2] == 332
-    assert sut[3] == 1
+    assert sut[3] == 1
```

### Comparing `wgse_ng-1.0.0a5/test/test_fasta.py` & `wgse_ng-1.0.0a7/test/test_fasta.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,83 +22,83 @@
         f"{'N'*5}\n",
         ">2 irrelevant\n",
     ]
     dict_lines = [
         "@HD\tVN:1.0\tSO:unsorted",
         "@SQ\tSN:1\tLN:10\tM5:dummy\tUR:file://c:/foo.fa.gz",
     ]
-   
+
     with pytest.raises(RuntimeError) as e:
-        genome = MockGenome(MockPath(fa_lines), MockPath(None,False))
+        genome = MockGenome(MockPath(fa_lines), MockPath(None, False))
         sut = FASTALetterCounter(genome)
     assert "Unable to find dictionary" in str(e.value)
 
+
 def test_sequence_not_in_dictionary():
     fa_lines = [
         ">1 irrelevant\n",
         f"{'N'*5}\n",
         f"{'N'*5}\n",
         ">2 irrelevant\n",
     ]
     dict_lines = [
         "@HD\tVN:1.0\tSO:unsorted",
         "@SQ\tSN:1\tLN:10\tM5:dummy\tUR:file://c:/foo.fa.gz",
     ]
     pytest.MonkeyPatch().setattr("gzip.open", gzip_open)
-   
+
     with pytest.raises(ValueError) as e:
         genome = MockGenome(MockPath(fa_lines), MockPath(dict_lines))
         FASTALetterCounter(genome).count_letters()
     assert "not present in dictionary" in str(e.value)
-    
+
+
 def test_fastq():
     fa_lines = [
         ">1 irrelevant\n",
         f"{'N'*5}\n",
         f"{'N'*5}\n",
         "+2 irrelevant\n",
     ]
     dict_lines = [
         "@HD\tVN:1.0\tSO:unsorted",
         "@SQ\tSN:1\tLN:10\tM5:dummy\tUR:file://c:/foo.fa.gz",
     ]
     pytest.MonkeyPatch().setattr("gzip.open", gzip_open)
-   
+
     with pytest.raises(RuntimeError) as e:
         genome = MockGenome(MockPath(fa_lines), MockPath(dict_lines))
         FASTALetterCounter(genome).count_letters()
     assert "Expected a FASTA" in str(e.value)
-    
+
+
 def test_duplicate_sequence():
     fa_lines = [
         ">1 irrelevant\n",
         f"{'N'*5}\n",
         f"{'N'*5}\n",
         ">1 irrelevant\n",
     ]
     dict_lines = [
         "@HD\tVN:1.0\tSO:unsorted",
         "@SQ\tSN:1\tLN:10\tM5:dummy\tUR:file://c:/foo.fa.gz",
     ]
     pytest.MonkeyPatch().setattr("gzip.open", gzip_open)
-   
+
     with pytest.raises(RuntimeError) as e:
         genome = MockGenome(MockPath(fa_lines), MockPath(dict_lines))
         FASTALetterCounter(genome).count_letters()
     assert "duplicated sequence" in str(e.value)
-    
-    
+
+
 def test_only_comments():
-    fa_lines = [
-        "#Hello\n",
-        f"#Foo\n"
-    ]
+    fa_lines = ["#Hello\n", f"#Foo\n"]
     dict_lines = [
         "@HD\tVN:1.0\tSO:unsorted",
         "@SQ\tSN:1\tLN:10\tM5:dummy\tUR:file://c:/foo.fa.gz",
     ]
     pytest.MonkeyPatch().setattr("gzip.open", gzip_open)
-   
+
     with pytest.raises(RuntimeError) as e:
         genome = MockGenome(MockPath(fa_lines), MockPath(dict_lines))
         FASTALetterCounter(genome).count_letters()
-    assert "no sequences" in str(e.value)
+    assert "no sequences" in str(e.value)
```

### Comparing `wgse_ng-1.0.0a5/test/test_fasta_dictionary.py` & `wgse_ng-1.0.0a7/test/test_fasta_dictionary.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,36 +7,37 @@
         "@HD\tVN:1.0\tSO:coordinate",
     ]
     sut = AlignmentMapHeader(lines)
     assert len(sut.sequences) == 0
     assert sut.metadata.sorted == Sorting.Coordinate
     assert sut.metadata.version == "1.0"
 
+
 def test_unsorted_parsed_correctly():
     lines = [
         "@HD\tVN:1.0\tSO:unsorted",
     ]
     sut = AlignmentMapHeader(lines)
     assert len(sut.sequences) == 0
     assert sut.metadata.sorted == Sorting.Unsorted
     assert sut.metadata.version == "1.0"
-    
+
+
 def test_unsorted_parsed_correctly():
     lines = [
         "@HD\tVN:1.0\tSO:unknown",
     ]
     sut = AlignmentMapHeader(lines)
     assert len(sut.sequences) == 0
     assert sut.metadata.sorted == Sorting.Unknown
     assert sut.metadata.version == "1.0"
 
+
 def test_sequences_parsed_correctly():
-    lines = [
-        "@SQ\tSN:Seq1\tLN:123\tM5:abcdefabcdef123123\tUR:/directory/genome.fasta"
-    ]
+    lines = ["@SQ\tSN:Seq1\tLN:123\tM5:abcdefabcdef123123\tUR:/directory/genome.fasta"]
     sut = AlignmentMapHeader(lines)
     assert sut.metadata is None
     assert len(sut.sequences) == 1
     assert "Seq1" in sut.sequences
     assert sut.sequences["Seq1"].length == 123
     assert sut.sequences["Seq1"].md5 == "abcdefabcdef123123"
     assert sut.sequences["Seq1"].uri == "/directory/genome.fasta"
```

### Comparing `wgse_ng-1.0.0a5/test/test_microarray_converter.py` & `wgse_ng-1.0.0a7/test/test_microarray_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,56 @@
-
 from pathlib import Path
 from test.test_fasta import MockPath
 from test.utility import MockFile
 from unittest.mock import patch
 
 import pytest
 
 from wgse.configuration import RepositoryConfig
 from wgse.data.microarray_converter import MicroarrayConverterTarget
 from wgse.microarray.microarray_converter import MicroarrayConverter
 from wgse.microarray.microarray_line_formatter import TARGET_FORMATTER_MAP
 
-
 # def test_every_target_has_formatter():
 #     assert all(x in TARGET_FORMATTER_MAP for x in MicroarrayConverterTarget)
-    
+
+
 def test_inexistent_head_folder_raise():
     config = RepositoryConfig()
     config.metadata = MockPath(exists=False)
     microarray_templates = MockPath(exists=False, name="microarray_templates")
-    microarray_templates.joinpath = lambda x: MockPath([], False if x=="body" else True, x)
+    microarray_templates.joinpath = lambda x: MockPath(
+        [], False if x == "body" else True, x
+    )
     config.metadata.joinpath = lambda _: microarray_templates
     with pytest.raises(FileNotFoundError) as e:
         MicroarrayConverter(config)
     assert "template body"
-    
+
+
 def test_inexistent_head_folder_raise():
     config = RepositoryConfig()
     config.metadata = MockPath(exists=False)
     microarray_templates = MockPath(exists=False, name="microarray_templates")
-    microarray_templates.joinpath = lambda x: MockPath([], False if x=="head" else True, x)
+    microarray_templates.joinpath = lambda x: MockPath(
+        [], False if x == "head" else True, x
+    )
     config.metadata.joinpath = lambda _: microarray_templates
     with pytest.raises(FileNotFoundError) as e:
         MicroarrayConverter(config)
     assert "template head"
 
+
 def test_inexistent_head_folder_raise():
     config = RepositoryConfig()
     config.metadata = MockPath(exists=False)
     microarray_templates = MockPath(exists=False, name="microarray_templates")
-    microarray_templates.joinpath = lambda x: MockPath([], False if x=="body" else True, x)
+    microarray_templates.joinpath = lambda x: MockPath(
+        [], False if x == "body" else True, x
+    )
     config.metadata.joinpath = lambda _: microarray_templates
     with pytest.raises(FileNotFoundError) as e:
         MicroarrayConverter(config)
     assert "template body"
 
 
 # @patch('pathlib.Path.exists')
@@ -52,17 +59,17 @@
 # @patch('shutil.copy')
 # def test_missing_path(mock_copy, mock_gzip_open, mock_open, mock_exists):
 #     output_lines = []
 #     template_body = MockFile(["rs1\t1\t1"])
 #     input_file = MockFile(["rs1\t1\t1\tAA"])
 #     output_file = MockFile([])
 #     output_file.write = lambda x: output_lines.append(x)
-    
+
 #     mock_open.side_effect = [input_file, output_file]
 #     mock_exists.side_effect = [True, True, True, True]
 #     mock_gzip_open.side_effect = [template_body]
 
 #     config = RepositoryConfig()
 #     config.metadata = Path("blah")
 #     sut = MicroarrayConverter(config)
 #     sut.convert(Path("foo"), MicroarrayConverterTarget.Ancestry_v1)
-#     pass
+#     pass
```

### Comparing `wgse_ng-1.0.0a5/test/test_raw_file.py` & `wgse_ng-1.0.0a7/test/test_raw_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,56 +5,60 @@
 from wgse.microarray.raw_file import RawEntry, RawFile
 
 
 def test_raw_entry():
     sut = RawEntry("rs1", "1", 1, "AA")
     assert sut.template_entry == "rs1\t1\t1\n"
 
-@patch('gzip.open')
-@patch('pathlib.Path.open')
+
+@patch("gzip.open")
+@patch("pathlib.Path.open")
 def test_compressed_raw_file(mock_open, mock_gzopen):
     lines = []
     file = Mock()
     file.write = lambda x: lines.append(x)
-    
-    mock_gzopen.side_effect = [MockFile(["#FOO", " rs1 \t 1 \t 1 \t AA \n", "rs2\tX\t123\tBB"])]
+
+    mock_gzopen.side_effect = [
+        MockFile(["#FOO", " rs1 \t 1 \t 1 \t AA \n", "rs2\tX\t123\tBB"])
+    ]
     mock_open.side_effect = [file]
-    
-    elements : list[RawEntry] = []
-    
+
+    elements: list[RawEntry] = []
+
     for item in RawFile(Path("test.txt.gz")):
         elements.append(item)
-        
+
     assert len(elements) == 2
     assert elements[0].id == "rs1"
     assert elements[0].chromosome == "1"
     assert elements[0].position == 1
     assert elements[0].result == "AA"
     assert elements[1].id == "rs2"
     assert elements[1].chromosome == "X"
     assert elements[1].position == 123
     assert elements[1].result == "BB"
-    
+
+
 # @patch('builtins.open')
 # @patch('pathlib.Path.open')
 # def test_compressed_raw_file(mock_open, mock_gzopen):
 #     lines = []
 #     file = Mock()
 #     file.write = lambda x: lines.append(x)
-    
+
 #     mock_gzopen.side_effect = [MockFile(["#FOO", " rs1 \t 1 \t 1 \t AA \n", "rs2\tX\t123\tBB"])]
 #     mock_open.side_effect = [file]
-    
+
 #     elements : list[RawEntry] = []
-    
+
 #     for item in RawFile(Path("test.txt")):
 #         elements.append(item)
-    
+
 #     assert len(elements) == 2
 #     assert elements[0].id == "rs1"
 #     assert elements[0].chromosome == "1"
 #     assert elements[0].position == 1
 #     assert elements[0].result == "AA"
 #     assert elements[1].id == "rs2"
 #     assert elements[1].chromosome == "X"
 #     assert elements[1].position == 123
-#     assert elements[1].result == "BB"
+#     assert elements[1].result == "BB"
```

### Comparing `wgse_ng-1.0.0a5/test/test_sequence.py` & `wgse_ng-1.0.0a7/test/test_sequence.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,95 +4,106 @@
 
 
 def test_sequence_with_invalid_length():
     with pytest.raises(IndexError) as e:
         LetterRunCollection("Foo", 0)
     assert "greater than" in str(e.value)
 
+
 def test_end_incomplete_sequence():
     with pytest.raises(ValueError) as e:
         sut = LetterRunCollection("Foo", 100)
         sut.end(99)
     assert "but processed" in str(e.value)
-    
+
+
 def test_open_run_on_ended_sequence():
     with pytest.raises(RuntimeError) as e:
         sut = LetterRunCollection("Foo", 100)
         sut.end(100)
         sut.open_run(101)
     assert "ended" in str(e.value)
 
+
 def test_double_open_run():
     with pytest.raises(RuntimeError) as e:
         sut = LetterRunCollection("Foo", 10)
         sut.open_run(0)
         sut.open_run(0)
     assert "already opened" in str(e.value)
 
+
 def test_negative_open():
     with pytest.raises(IndexError) as e:
         sut = LetterRunCollection("Foo", 10)
         sut.open_run(-10)
     assert "negative" in str(e.value)
 
+
 def test_close_run_less_equal_than_open():
     with pytest.raises(RuntimeError) as e:
         sut = LetterRunCollection("Foo", 10)
         sut.open_run(0)
         sut.close_run(0)
     assert "greater" in str(e.value)
 
+
 def test_only_close_run():
     with pytest.raises(RuntimeError) as e:
         sut = LetterRunCollection("Foo", 10)
         sut.close_run(0)
     assert "already closed" in str(e.value)
 
+
 def test_double_close_run():
     with pytest.raises(RuntimeError) as e:
         sut = LetterRunCollection("Foo", 1)
         sut.open_run(0)
         sut.close_run(1)
         sut.close_run(1)
     assert "already closed" in str(e.value)
 
+
 def test_close_run_greater_than_open():
     # Arrange
     sut = LetterRunCollection("Foo", 10)
-    # Act    
+    # Act
     sut.open_run(0)
     sut.close_run(1)
     # Assert
     assert len(sut.runs) == 1
     assert sut.runs[0].start == 0
     assert sut.runs[0].length == 1
 
+
 def test_overlapping_runs():
     with pytest.raises(ValueError) as e:
         sut = LetterRunCollection("Foo", 19)
         sut.open_run(0)
         sut.close_run(15)
 
         sut.open_run(15)
         sut.close_run(19)
     assert "overlapping" in str(e.value)
 
+
 def test_filter():
     # Arrange
     sequence = LetterRunCollection("Foo", 449)
     # Act
     sequence.open_run(0)
     sequence.close_run(150)
     sequence.open_run(300)
     sequence.close_run(449)
     sut = sequence.filter(lambda x: x.length > 149)
     # Assert
     assert len(sut) == 1
     assert sut[0].start == 0
     assert sut[0].length == 150
-    
+
+
 def test_is_run_open():
     sut = LetterRunCollection("Foo", 150)
     sut.open_run(0)
     assert sut.is_run_open() == True
     sut.close_run(150)
-    assert sut.is_run_open() == False
+    assert sut.is_run_open() == False
```

### Comparing `wgse_ng-1.0.0a5/test/test_unknown_bases_stats.py` & `wgse_ng-1.0.0a7/test/test_unknown_bases_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a5/wgse/__init__.py` & `wgse_ng-1.0.0a7/wgse/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pkgutil shenanigans to make python load wgse.third_party from site-packages
 #
 # tl;dr wgse.third_party contains some executables for windows and is installed
 # from another pypi package (wgse-ng-3rd-party).
 # When importing wgse.third_party from any files inside WGSE, python will expect
-# to find wgse.third_party INSIDE this package and not in site-packages. Code 
-# below will make this package a "Native Namespace Package" (PEP 420) and will 
-# make it possible to have different packages contributing to the same namespace 
+# to find wgse.third_party INSIDE this package and not in site-packages. Code
+# below will make this package a "Native Namespace Package" (PEP 420) and will
+# make it possible to have different packages contributing to the same namespace
 # (wgse). Only downside is the the IDE won't recognize wgse.third_party, which is
 # not a big deal as it doesn't contain any python code.
 
 from pkgutil import extend_path
-__path__ = extend_path(__path__, __name__)
+
+__path__ = extend_path(__path__, __name__)
```

### Comparing `wgse_ng-1.0.0a5/wgse/adapters/alignment_map_file_info_adapter.py` & `wgse_ng-1.0.0a7/wgse/adapters/alignment_map_file_info_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from wgse.data.alignment_map_file_info import AlignmentMapFileInfo
 from wgse.data.tabular_data import TabularData, TabularDataRow
 
 
 class AlignmentMapFileInfoAdapter:
-    def adapt(stats: AlignmentMapFileInfo):    
+    def adapt(stats: AlignmentMapFileInfo):
         label_map = {
             "path": "Path",
             "sorted": "Sorted",
             "indexed": "Indexed",
             "file_type": "File type",
             "reference_genome": "Reference genome",
             "content": "Content",
@@ -31,8 +31,8 @@
         data["File type"] = [stats.file_type.name]
         data["Path"] = [str(stats.path)]
         data["Size"] = [size]
         for key, value in label_map.items():
             if value not in data or data[value] is None:
                 data[value] = [str(stats.__dict__[key])]
         data = TabularData(None, [TabularDataRow(x[0], x[1]) for x in data.items()])
-        return data
+        return data
```

### Comparing `wgse_ng-1.0.0a5/wgse/adapters/alignment_stats_adapter.py` & `wgse_ng-1.0.0a7/wgse/adapters/alignment_stats_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+
 from wgse.data.alignment_stats import AlignmentStats
 from wgse.data.tabular_data import TabularData, TabularDataRow
 
 
 class AlignmentStatsAdapter:
     def adapt(input_data: AlignmentStats):
         name_map = {
@@ -24,8 +25,8 @@
 
         rows = []
         for key, value in name_map.items():
             data = input_data.__dict__[key]
             if isinstance(data, enum.Enum):
                 data = str(data.name)
             rows.append(TabularDataRow(value, [str(data)]))
-        return TabularData(None, rows)
+        return TabularData(None, rows)
```

### Comparing `wgse_ng-1.0.0a5/wgse/adapters/header_adapter.py` & `wgse_ng-1.0.0a7/wgse/adapters/header_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a5/wgse/adapters/index_stats_adapter.py` & `wgse_ng-1.0.0a7/wgse/adapters/index_stats_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,15 @@
             "Unmapped length",
         ]
         grouped_stats = []
         grouped_others = TabularDataRow(
             "Others",
             [
                 "Others",
-                sum(
-                    x.reference_length for x in stats if x.type == SequenceType.Other
-                ),
+                sum(x.reference_length for x in stats if x.type == SequenceType.Other),
                 sum(x.mapped for x in stats if x.type == SequenceType.Other),
                 sum(x.unmapped for x in stats if x.type == SequenceType.Other),
             ],
         )
 
         percentage_mapped = ""
         percentage_unmapped = ""
@@ -60,8 +58,8 @@
                         f"{stat.mapped}{percentage_mapped}",
                         f"{stat.unmapped}{percentage_unmapped}",
                     ],
                 )
             )
         grouped_stats.append(grouped_others)
 
-        return TabularData(header, grouped_stats)
+        return TabularData(header, grouped_stats)
```

### Comparing `wgse_ng-1.0.0a5/wgse/adapters/reference_adapter.py` & `wgse_ng-1.0.0a7/wgse/adapters/reference_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
             ref_map = stats.reference_map
         max_columns = max([len(x) for x in ref_map.values()])
         genome_index_map = {}
         headers = ["Loaded file"]
         max_index = 0
         rows = []
         for key, value in ref_map.items():
-            row = [None for x in range(max_columns+1)]
+            row = [None for x in range(max_columns + 1)]
             row[0] = key
             for sequence in value:
                 if sequence.parent not in genome_index_map:
                     genome_index_map[sequence.parent] = max_index
                     headers.append(str(sequence.parent))
                     max_index += 1
-                row[genome_index_map[sequence.parent]+1] = sequence
+                row[genome_index_map[sequence.parent] + 1] = sequence
             rows.append([str(x) for x in row])
-        return TabularData(headers, [TabularDataRow(None, x) for x in rows])
+        return TabularData(headers, [TabularDataRow(None, x) for x in rows])
```

### Comparing `wgse_ng-1.0.0a5/wgse/alignment_map/alignment_map_file.py` & `wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 from wgse.alignment_map.alignment_map_header import AlignmentMapHeader
 from wgse.alignment_map.alignment_stats_calculator import AlignmentStatsCalculator
 from wgse.alignment_map.index_stats_calculator import (
     IndexStatsCalculator,
     SequenceStatistics,
 )
 from wgse.configuration import MANAGER_CFG
+from wgse.data.alignment_map_file_info import AlignmentMapFileInfo
 from wgse.data.file_type import FileType
+from wgse.data.gender import Gender
 from wgse.data.mitochondrial_model_type import MitochondrialModelType
-from wgse.data.alignment_map_file_info import (
-    AlignmentMapFileInfo,
-)
 from wgse.data.sequence_type import SequenceType
-from wgse.data.gender import Gender
 from wgse.data.sorting import Sorting
-from wgse.utility.external import External
 from wgse.fasta.reference import Reference
 from wgse.reference_genome.repository_manager import RepositoryManager
+from wgse.utility.external import External
 from wgse.utility.mt_dna import MtDNA
 from wgse.utility.sequence_orderer import SequenceOrderer
 
 logger = logging.getLogger(__name__)
 
 
 class AlignmentMapFile:
@@ -92,78 +90,90 @@
     def _load_header(self) -> AlignmentMapHeader:
         lines = self._external.samtools(
             ["view", "-H", "--no-PG", self.path], stdout=subprocess.PIPE, wait=True
         )
         lines = lines.decode().split("\n")
         return AlignmentMapHeader(lines)
 
-    def _to_fastq(self):
+    def _to_fastq(self, io):
         pass
 
-    def _to_fasta(self, regions=""):
-        input = None
-        output = None
+    def _to_fasta(self, regions="", io=None):
+        input = self.path
+        suffixes = self.path.suffixes.copy()
+        suffixes[-1] = ".fasta"
+        output = self.path.with_name(self.path.stem + "".join(suffixes))
         reference = str(self.file_info.reference_genome.ready_reference.fasta)
-        faidx_opt = f"faidx {reference} {regions}"
-        consensus_opt = f"consensus {input} -o {output}"
+        faidx_opt = f'faidx "{reference}" {regions}'
+        consensus_opt = f'consensus "{input}" -o "{output}"'
+        # if io is not None:
+        #     io = lambda r,w: io(r,w)
 
-        faidx = self._external.samtools(faidx_opt, stdout=subprocess.PIPE)
+        faidx = self._external.samtools(faidx_opt, stdout=subprocess.PIPE)  # io=io)
         consensus = self._external.samtools(
             shlex.split(consensus_opt), stdin=faidx.stdout
         )
         consensus.communicate()
         return output
 
-    def _to_alignment_map(self, target: FileType, region):
+    def _to_alignment_map(self, target: FileType, region, io):
         suffixes = self.path.suffixes.copy()
         if len(suffixes) == 0:
             suffixes = [None]
         format_dependent_opt = ""
+        target_opt = ""
         if target == FileType.BAM:
             suffixes[-1] = ".bam"
             target_opt = "-b"
         elif target == FileType.CRAM:
             suffixes[-1] = ".cram"
             target_opt = "-C"
             if self.file_info.reference_genome.ready_reference is None:
-                raise RuntimeError("Reference genome was not found but is mandatory for CRAM files.")
+                raise RuntimeError(
+                    "Reference genome was not found but is mandatory for CRAM files."
+                )
             reference = self.file_info.reference_genome.ready_reference.fasta
             format_dependent_opt = f'-T "{reference}"'
         elif target == FileType.SAM:
             suffixes[-1] = ".sam"
             target_opt = ""
         output = self.path.with_name(self.path.stem + "".join(suffixes))
-        
+
         view_opt = f'view {target_opt} {format_dependent_opt} "{self.path!s}" {region} -o "{output}"'
         view_opt = shlex.split(view_opt)
-        self._external.samtools(view_opt, wait=True)
+        progress = None
+        if io is not None:
+            progress = lambda r, w: io(self.path.stat().st_size, r)
+        return self._external.samtools(view_opt, io=progress)
 
-    def convert(self, target: FileType, regions = ""):
+    def convert(self, target: FileType, regions="", io=None):
         if self.file_info.file_type == target:
             raise ValueError("Target and source file type for conversion are identical")
         if target == FileType.FASTA:
-            self._to_fasta()
+            self._to_fasta(io=io)
         if target == FileType.FASTQ:
-            self._to_fastq()
-        self._to_alignment_map(target, regions)
+            self._to_fastq(io=io)
+        return self._to_alignment_map(target, regions, io=io)
 
     def _initialize_file_info(self):
         file_info = AlignmentMapFileInfo()
         file_info.path = self.path
         file_info.file_type = AlignmentMapFile.SUPPORTED_FILES[self.path.suffix.lower()]
         file_info.sorted = self.header.metadata.sorted
         file_info.name_type_mtdna = self.header.mtdna_name_type()
         file_info.name_type_chromosomes = self.header.chromosome_name_type()
         file_info.sequence_count = self.header.sequence_count()
         file_info.indexed = self._indexed(file_info.file_type)
         file_info.gender = Gender.Unknown
         file_info.reference_genome = self._repo.find(
             list(self.header.sequences.values())
         )
-        file_info.mitochondrial_dna_model = self.get_mitochondrial_dna_type(file_info.reference_genome)
+        file_info.mitochondrial_dna_model = self.get_mitochondrial_dna_type(
+            file_info.reference_genome
+        )
 
         # Compute IndexStats automatically only if it's inexpensive to do so.
         # Otherwise, let the caller explicitly request them.
         inexpensive_index_stats = file_info.indexed and file_info.file_type not in [
             FileType.CRAM,
             FileType.SAM,
         ]
@@ -172,15 +182,15 @@
             indexed_stats = IndexStatsCalculator(self.path)
             file_info.index_stats = indexed_stats.get_stats()
             file_info.gender = self.get_gender(file_info.index_stats)
 
         # If file is not sorted computing AlignmentStats is expensive.
         # Let the caller request them.
         if file_info.sorted == Sorting.Coordinate:
-            is_cram = file_info.file_type == FileType.CRAM 
+            is_cram = file_info.file_type == FileType.CRAM
             has_reference = file_info.reference_genome.ready_reference is not None
             if is_cram and has_reference or not is_cram:
                 calculator = AlignmentStatsCalculator(file_info)
                 file_info.alignment_stats = calculator.get_stats()
         return file_info
 
     def get_mitochondrial_dna_type(self, reference: Reference):
@@ -189,15 +199,15 @@
         sequences = {
             SequenceOrderer.canonicalize(x.name): x
             for x in self.header.sequences.values()
         }
         if "M" not in sequences:
             return MitochondrialModelType.Unknown
         mito_md5 = None
-        # If the sequence does not have MD5, we still have 
+        # If the sequence does not have MD5, we still have
         # the chance to get it from the reference genome.
         # TODO: finish this thing
         # if sequences["M"].md5 is None:
         #     ref_sequences = [x.sequences for x in reference.matching]
         #     for sequence in ref_sequences:
         #         names = [x.name for x in SequenceOrderer(sequence) if names]
```

### Comparing `wgse_ng-1.0.0a5/wgse/alignment_map/alignment_map_header.py` & `wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_header.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,104 +83,104 @@
         }
         self._load(lines)
 
     def _program_process(self, parts: list[str]):
         program = AlignmentMapHeaderProgram()
         for part in parts:
             if part.startswith("ID"):
-                program.id = part.split(":",1)[1]
+                program.id = part.split(":", 1)[1]
             elif part.startswith("PN"):
-                program.id = part.split(":",1)[1]
+                program.id = part.split(":", 1)[1]
             elif part.startswith("CL"):
-                program.id = part.split(":",1)[1]
+                program.id = part.split(":", 1)[1]
             elif part.startswith("PP"):
-                program.previous = part.split(":",1)[1]
+                program.previous = part.split(":", 1)[1]
                 if program.previous in [x.id for x in self.programs]:
                     prev = [x for x in self.programs if x.id == program.previous]
                     program.previous = prev[0]
             elif part.startswith("DS"):
-                program.description = part.split(":",1)[1]
+                program.description = part.split(":", 1)[1]
             elif part.startswith("VN"):
-                program.program_version = part.split(":",1)[1]
+                program.program_version = part.split(":", 1)[1]
         self.programs.append(program)
 
     def _read_group_process(self, parts: list[str]):
         read_group = AlignmentMapHeaderReadGroup()
         for part in parts:
             if part.startswith("ID"):
-                read_group.id = part.split(":",1)[1]
+                read_group.id = part.split(":", 1)[1]
             elif part.startswith("BC"):
-                read_group.barcode = part.split(":",1)[1]
+                read_group.barcode = part.split(":", 1)[1]
             elif part.startswith("CN"):
-                read_group.sequencing_center = part.split(":",1)[1]
+                read_group.sequencing_center = part.split(":", 1)[1]
             elif part.startswith("DS"):
-                read_group.description = part.split(":",1)[1]
+                read_group.description = part.split(":", 1)[1]
             elif part.startswith("DT"):
-                read_group.date = part.split(":",1)[1]
+                read_group.date = part.split(":", 1)[1]
             elif part.startswith("FO"):
-                read_group.flow_order = part.split(":",1)[1]
+                read_group.flow_order = part.split(":", 1)[1]
             elif part.startswith("KS"):
-                read_group.key_sequence = part.split(":",1)[1]
+                read_group.key_sequence = part.split(":", 1)[1]
             elif part.startswith("LB"):
-                read_group.library = part.split(":",1)[1]
+                read_group.library = part.split(":", 1)[1]
             elif part.startswith("PG"):
-                read_group.programs = part.split(":",1)[1]
+                read_group.programs = part.split(":", 1)[1]
             elif part.startswith("PI"):
-                read_group.predicted_median_insert_size = part.split(":",1)[1]
+                read_group.predicted_median_insert_size = part.split(":", 1)[1]
             elif part.startswith("PL"):
-                read_group.platform = part.split(":",1)[1]
+                read_group.platform = part.split(":", 1)[1]
             elif part.startswith("PM"):
-                read_group.platform_model = part.split(":",1)[1]
+                read_group.platform_model = part.split(":", 1)[1]
             elif part.startswith("PU"):
-                read_group.platform_unit = part.split(":",1)[1]
+                read_group.platform_unit = part.split(":", 1)[1]
             elif part.startswith("SM"):
-                read_group.sample = part.split(":",1)[1]
+                read_group.sample = part.split(":", 1)[1]
         self.read_groups.append(read_group)
 
     def _comment_process(self, parts: list[str]):
         self.comments.append(" ".join(parts))
         return
 
     def _metadata_process(self, parts: list[str]):
         metadata = AlignmentMapHeaderMetadata()
         for part in parts:
             if part.startswith("VN"):
-                metadata.version = part.split(":",1)[1]
+                metadata.version = part.split(":", 1)[1]
             elif part.startswith("SO:"):
                 metadata.sorted = self._sorted(part)
             elif part.startswith("GO:"):
-                metadata.grouping = part.split(":",1)[1]
+                metadata.grouping = part.split(":", 1)[1]
             elif part.startswith("SS:"):
-                metadata.subsorting = part.split(":",1)[1]
+                metadata.subsorting = part.split(":", 1)[1]
         self.metadata = metadata
 
     def _sequence_process(self, parts: typing.List[str]):
         entry = AlignmentMapHeaderSequence()
 
         for part in parts:
             if part.startswith("SN"):
-                entry.name = part.split(":",1)[1]
+                entry.name = part.split(":", 1)[1]
             elif part.startswith("LN"):
-                entry.length = int(part.split(":",1)[1])
+                entry.length = int(part.split(":", 1)[1])
             elif part.startswith("M5"):
-                entry.md5 = part.split(":",1)[1]
+                entry.md5 = part.split(":", 1)[1]
             elif part.startswith("UR"):
-                entry.uri = part.split(":",1)[1]
+                entry.uri = part.split(":", 1)[1]
             elif part.startswith("AH"):
-                entry.alternate_locus = part.split(":",1)[1]
+                entry.alternate_locus = part.split(":", 1)[1]
             elif part.startswith("AN"):
-                entry.alternative_names = part.split(":",1)[1].split(",")
+                entry.alternative_names = part.split(":", 1)[1].split(",")
             elif part.startswith("AS"):
-                entry.genome_assembly_identifier = part.split(":",1)[1]
+                entry.genome_assembly_identifier = part.split(":", 1)[1]
             elif part.startswith("DS"):
-                entry.description = part.split(":",1)[1]
+                entry.description = part.split(":", 1)[1]
             elif part.startswith("SP"):
-                entry.species = part.split(":",1)[1]
+                entry.species = part.split(":", 1)[1]
             elif part.startswith("TP"):
-                entry.molecule_topology = part.split(":",1)[1]
+                entry.molecule_topology = part.split(":", 1)[1]
         if entry.name == None:
             raise RuntimeError("Unable to find the name of the sequence.")
         if entry.length == None:
             raise RuntimeError("Unable to find the length of the sequence.")
 
         self.sequences[entry.name] = entry
```

### Comparing `wgse_ng-1.0.0a5/wgse/alignment_map/alignment_map_row.py` & `wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_row.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a5/wgse/alignment_map/alignment_stats_calculator.py` & `wgse_ng-1.0.0a7/wgse/alignment_map/alignment_stats_calculator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+import logging
 import subprocess
 from math import sqrt
 
-from wgse.alignment_map.alignment_map_row import (AlignmentMapFlag,
-                                                  AlignmentMapRow)
+from wgse.alignment_map.alignment_map_row import AlignmentMapFlag, AlignmentMapRow
 from wgse.configuration import MANAGER_CFG
-from wgse.data.file_type import FileType
 from wgse.data.alignment_map_file_info import AlignmentMapFileInfo
 from wgse.data.alignment_stats import AlignmentStats
+from wgse.data.file_type import FileType
 from wgse.data.read_type import ReadType
 from wgse.utility.external import External
 from wgse.utility.sequencers import Sequencers
 
+logger = logging.getLogger(__name__)
+
 
 class AlignmentStatsCalculator:
     def __init__(
         self,
         path: AlignmentMapFileInfo,
-        config = MANAGER_CFG.ALIGNMENT_STATS,
+        config=MANAGER_CFG.ALIGNMENT_STATS,
         external: External = External(),
         sequencers: Sequencers = Sequencers(),
     ) -> None:
         self.aligned_file = path
         self._config = config
         self._external = external
         self._sequencers = sequencers
@@ -31,16 +33,18 @@
         # TODO: handle long reads
         return stats
 
     def _read_samples(self, skip, samples_count):
         options = []
         if self.aligned_file.file_type == FileType.CRAM:
             ready_reference = self.aligned_file.reference_genome.ready_reference
-            if  ready_reference is None:
-                raise RuntimeError("Unable to compute stats because there is no reference available for a CRAM file")
+            if ready_reference is None:
+                raise RuntimeError(
+                    "Unable to compute stats because there is no reference available for a CRAM file"
+                )
             options.extend(["-T", ready_reference.fasta])
         options.append(self.aligned_file.path)
 
         process: subprocess.Popen = self._external.samtools(
             ["view", *options], stdout=subprocess.PIPE
         )
         samples = []
@@ -64,15 +68,16 @@
             AlignmentMapFlag.DUPLICATE,
             AlignmentMapFlag.SUPPLEMENTARY_ALIGNMENT,
         ]
         read_type_count = 0
         considered_samples = 0
 
         if len(samples) == 0:
-            raise RuntimeError("Cannot compute stats as the file is empty")
+            logger.error("Cannot compute alignment stats as the file is empty")
+            return
 
         # Process the template name for 1st sample to determine the sequencer
         # as it should not give a different result on the other samples.
         sequencer = self._sequencers.determine_sequencer(samples[0].query_template_name)
 
         # Used to compute stats for read length
         count_length = 0
@@ -137,29 +142,33 @@
         read_type = ReadType.Unknown
         if read_type_count > majority:
             read_type = ReadType.Paired
         elif read_type_count < -majority:
             read_type = ReadType.Single
 
         if count_length <= 2:
-            raise RuntimeError(
+            logger.error(
                 "Unable to compute read length stats as the number of valid samples is less than 2."
             )
+            return None
         if count_insert_size <= 2 and read_type == ReadType.Paired:
-            raise RuntimeError(
+            logger.error(
                 "Unable to compute insert size stats as the number of valid samples is less than 2."
             )
+            return None
         if count_quality <= 2:
-            raise RuntimeError(
+            logger.error(
                 "Unable to compute alignment quality stats as the number of valid samples is less than 2."
             )
+            return None
         if read_type == ReadType.Unknown:
-            raise RuntimeError(
+            logger.error(
                 "Unable to determine read type as there's a similar number of single vs paired reads."
             )
+            return None
 
         stats = AlignmentStats()
         stats.samples_count = self._config.samples
         stats.skipped_samples = self._config.skip
         stats.read_type = read_type
         stats.duplicate = duplicate_count
         stats.sequencer = sequencer
```

### Comparing `wgse_ng-1.0.0a5/wgse/alignment_map/depth_analyzer.py` & `wgse_ng-1.0.0a7/wgse/alignment_map/depth_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,39 @@
         self._external = external
         pass
 
     def analyze_aligned_file(self, path: Path):
         file = AlignmentMapFile(path, self._external)
 
         process = self._external.samtools(
-            ["depth", "-a", "-b", "C:\\Users\\Marco\\Documents\\Bioinformatics\\WGSExtractv4-dev\\reference\\xgen_plus_spikein.GRCh38.bed", str(path)], stdout=subprocess.PIPE
+            [
+                "depth",
+                "-a",
+                "-b",
+                "C:\\Users\\Marco\\Documents\\Bioinformatics\\WGSExtractv4-dev\\reference\\xgen_plus_spikein.GRCh38.bed",
+                str(path),
+            ],
+            stdout=subprocess.PIPE,
         )
         self.analyze_depth_lines(iter(process.stdout.readline, b""), file)
 
     def analyze_depth_lines(self, lines, file: AlignmentMapFile):
-        progress = tqdm.tqdm(
-            lines, total=39009164, smoothing=0)
-        
+        progress = tqdm.tqdm(lines, total=39009164, smoothing=0)
+
         stats = DepthStats()
         stats_by_name = {}
         sums_by_name = {}
 
-        stats_by_name = {bytes(x, "utf-8"): [0] * 4 for x in file.header.sequences.keys()}
-        sums_by_name = {bytes(x, "utf-8"): [0] * 4 for x in file.header.sequences.keys()}
-        
+        stats_by_name = {
+            bytes(x, "utf-8"): [0] * 4 for x in file.header.sequences.keys()
+        }
+        sums_by_name = {
+            bytes(x, "utf-8"): [0] * 4 for x in file.header.sequences.keys()
+        }
+
         for line in lines:
             line = line.split()
             name = line[0]
             position = int(line[1])
             reads = int(line[2])
             progress.update(1)
```

### Comparing `wgse_ng-1.0.0a5/wgse/alignment_map/index_stats_calculator.py` & `wgse_ng-1.0.0a7/wgse/alignment_map/index_stats_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,12 +54,14 @@
             elif name_normalized == "Y":
                 chromosome_type = SequenceType.Y
             elif name_normalized == "*":
                 chromosome_type = SequenceType.Unmapped
             else:
                 chromosome_type = SequenceType.Other
 
-            stats.append(SequenceStatistics(
-                chromosome_type, name, reference_length, mapped, unmapped
-            ))
+            stats.append(
+                SequenceStatistics(
+                    chromosome_type, name, reference_length, mapped, unmapped
+                )
+            )
 
         return stats
```

### Comparing `wgse_ng-1.0.0a5/wgse/configuration.py` & `wgse_ng-1.0.0a7/wgse/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import configparser
 import logging
 import multiprocessing
 from pathlib import Path
 
+import wgse
+
 # Why third_party is not recognized by the IDE?
 # See wgse/__init__.py
-from wgse import third_party
-from wgse import mtDNA
-from wgse import metadata
-import wgse
+from wgse import metadata, mtDNA, third_party
 
 logger = logging.getLogger("configuration")
 logging.getLogger().setLevel(logging.DEBUG)
 
 
 class WGSEDefaults:
     """Specify some directory where to find configuration files."""
@@ -77,15 +76,15 @@
         metadata (Path): Root folder for metadata.
         mtdna (Path): Root folder for mtDNA files.
     """
 
     def __init__(self) -> None:
         self.genomes: Path = Path(WGSEDefaults.LOCAL_FOLDER, "genomes")
         self.temporary: Path = Path(WGSEDefaults.LOCAL_FOLDER, "temp")
-        self.log_path: Path = Path(WGSEDefaults.LOCAL_FOLDER,"logs")
+        self.log_path: Path = Path(WGSEDefaults.LOCAL_FOLDER, "logs")
         self.metadata: Path = Path(metadata.__file__).parent
         self.mtdna: Path = Path(mtDNA.__file__).parent
 
 
 class AlignmentStatsConfig:
     """Configuration for alignment stats calculation.
```

### Comparing `wgse_ng-1.0.0a5/wgse/data/alignment_map_file_info.py` & `wgse_ng-1.0.0a7/wgse/data/alignment_map_file_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from pathlib import Path
 
 from wgse.alignment_map.index_stats_calculator import SequenceStatistics
+from wgse.data.alignment_stats import AlignmentStats
 from wgse.data.chromosome_name_type import ChromosomeNameType
 from wgse.data.file_type import FileType
-from wgse.data.mitochondrial_name_type import MitochondrialNameType
+from wgse.data.gender import Gender
 from wgse.data.mitochondrial_model_type import MitochondrialModelType
-from wgse.data.alignment_stats import AlignmentStats
+from wgse.data.mitochondrial_name_type import MitochondrialNameType
 from wgse.data.sequence_type import SequenceType
-from wgse.data.gender import Gender
 from wgse.data.sorting import Sorting
 from wgse.fasta.reference import Reference
 
 
 class AlignmentMapFileInfo:
     def __init__(self) -> None:
         self.path: Path = None
         self.sorted: Sorting = None
         self.indexed: bool = None
         self.file_type: FileType = None
         self.reference_genome: Reference = None
-        self.content : SequenceType = None
+        self.content: SequenceType = None
         self.primary: bool = None
         self.mitochondrial_dna_model: MitochondrialModelType = None
         self.build: int = None
         self.name_type_chromosomes: ChromosomeNameType = None
         self.name_type_mtdna: MitochondrialNameType = None
         self.sequence_count: int = None
         self.alignment_stats: AlignmentStats = None
-        self.index_stats: dict[SequenceType, list[SequenceStatistics]] = None
+        self.index_stats: list[SequenceStatistics] = None
         self.gender: Gender = None
```

### Comparing `wgse_ng-1.0.0a5/wgse/data/alignment_stats.py` & `wgse_ng-1.0.0a7/wgse/data/alignment_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from wgse.data.read_type import ReadType
 
 
 class AlignmentStats:
     def __init__(self) -> None:
         self.skipped_samples: int = None
         self.samples_count: int = None
@@ -13,8 +12,8 @@
         self.standard_dev_length: float = None
         self.count_insert_size: int = None
         self.average_insert_size: float = None
         self.standard_dev_insert_size: float = None
         self.count_quality: int = None
         self.average_quality: float = None
         self.standard_dev_quality: float = None
-        self.read_type: ReadType = None
+        self.read_type: ReadType = None
```

### Comparing `wgse_ng-1.0.0a5/wgse/data/genome.py` & `wgse_ng-1.0.0a7/wgse/data/genome.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.bgzip_size = bgzip_size
         self.downloaded_md5 = downloaded_md5
         self.decompressed_md5 = decompressed_md5
         self.bgzip_md5 = bgzip_md5
         # Not serialized as it depends on the config
         self.__parent_folder = parent_folder
         # Not serialized as it's populated at runtime
-        self.__parent : Build = None
+        self.__parent: Build = None
 
     @property
     def parent_folder(self):
         return self.__parent_folder
 
     @parent_folder.setter
     def parent_folder(self, parent: Path):
@@ -124,8 +124,7 @@
         return Path(str(self.no_extensions) + ".dict")
 
     def __repr__(self) -> str:
         return str(self.no_extensions.name)
 
     def __str__(self) -> str:
         return self.__repr__()
-
```

### Comparing `wgse_ng-1.0.0a5/wgse/data/microarray_converter.py` & `wgse_ng-1.0.0a7/wgse/data/microarray_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum, auto
 
 
 class MicroarrayConverterExtensions(Enum):
     CSV = ".csv"
     TXT = ".txt"
 
+
 class MicroarrayConverterTarget(Enum):
     All = auto()
     Ancestry_v1 = auto()
     Ancestry_v2 = auto()
     FTDNA_v1 = auto()
     FTDNA_v2 = auto()
     FTDNA_v3 = auto()
@@ -21,8 +22,8 @@
     ReichLab_HumanOrigins_v1 = auto()
     SelfDecode = auto()
     TellMeGen = auto()
     TwentyThreeAndMe_v3 = auto()
     TwentyThreeAndMe_v35 = auto()
     TwentyThreeAndMe_v4 = auto()
     TwentyThreeAndMe_v5 = auto()
-    TwentyThreeAndMe_SNPs_API = auto()
+    TwentyThreeAndMe_SNPs_API = auto()
```

### Comparing `wgse_ng-1.0.0a5/wgse/data/mitochondrial_model.py` & `wgse_ng-1.0.0a7/wgse/data/mitochondrial_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from wgse.configuration import MANAGER_CFG
 from wgse.data.mitochondrial_model_type import MitochondrialModelType
 from wgse.data.sequence import Sequence
-from wgse.configuration import MANAGER_CFG
+
 
 class MitochondrialModel:
     def __init__(self, sequence, url, type, config=MANAGER_CFG.REPOSITORY) -> None:
         self.sequence: Sequence = sequence
         self.url = url
         self.type: MitochondrialModelType = type
         self.path = config.mtdna.joinpath(self.type.name + ".fasta")
@@ -13,8 +14,8 @@
         with self.path.open("r") as f:
             return f.read()
 
     def __str__(self) -> str:
         return f"{self.type.name}"
 
     def __repr__(self) -> str:
-        return f"{self.type.name}"
+        return f"{self.type.name}"
```

### Comparing `wgse_ng-1.0.0a5/wgse/data/sequence.py` & `wgse_ng-1.0.0a7/wgse/data/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-
 class Sequence:
-    def __init__(
-        self, name: str, length: int, md5: str = None
-    ) -> None:
+    def __init__(self, name: str, length: int, md5: str = None) -> None:
         self.name = name
         self.length = length
         self.md5 = md5
         self.__parent = None
 
     @property
     def parent(self):
@@ -16,8 +13,8 @@
     def parent(self, value):
         self.__parent = value
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
-        return f"{self.name}: Length: {self.length}bp, MD5: {self.md5}"
+        return f"{self.name}: Length: {self.length}bp, MD5: {self.md5}"
```

### Comparing `wgse_ng-1.0.0a5/wgse/fasta/fasta_letter_counter.py` & `wgse_ng-1.0.0a7/wgse/fasta/fasta_letter_counter.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,39 +13,45 @@
 except:
     tqdm = None
 
 from wgse.reference_genome.genome_metadata_loader import Genome
 
 
 class FASTALetterCounter:
-    """Represent a collection of sequences"""
-
     def __init__(self, genome: Genome):
         self._bases_progressbar = None
         self.genome = genome
         self._sequences_progressbar = None
         self._bases_progressbar = None
         if not self.genome.dict.exists():
             raise RuntimeError(f"Unable to find dictionary in {self.genome.dict.name}.")
-        self._dict :AlignmentMapHeader = AlignmentMapHeader.load_from_file(self.genome.dict)
-        self._support_multiline_progress = "win" not in sys.platform
+        self._dict: AlignmentMapHeader = AlignmentMapHeader.load_from_file(
+            self.genome.dict
+        )
+        self._support_multiline_progress = "win32" == sys.platform
 
     @property
     def model_name(self):
         return self.genome.fasta
 
-    def _progress(self, name, current_sequence, total_sequences, current_position, total_position):
+    def _progress(
+        self, name, current_sequence, total_sequences, current_position, total_position
+    ):
         if tqdm is not None:
             # Windows Prompt does not support nested progress bar and there's nothing
             # that can be done about that. On Windows, just keep only one progress bar.
             if self._sequences_progressbar is None and self._support_multiline_progress:
-                self._sequences_progressbar = tqdm.tqdm(total=total_sequences, desc=f"Sequences")
+                self._sequences_progressbar = tqdm.tqdm(
+                    total=total_sequences, desc=f"Sequences"
+                )
             if self._bases_progressbar is None:
-                self._bases_progressbar = tqdm.tqdm(total=total_position, desc=f"{name}")
-            
+                self._bases_progressbar = tqdm.tqdm(
+                    total=total_position, desc=f"{name}"
+                )
+
             if current_sequence != 0 and self._support_multiline_progress:
                 self._sequences_progressbar.update(current_sequence)
             if current_position != 0:
                 self._bases_progressbar.update(current_position)
 
     def _sequence_from_line(self, line: str) -> LetterRunCollection:
         # Processing the opening of a new sequence in a FASTA file.
@@ -96,15 +102,21 @@
                         f"Found a duplicated sequence: {current_sequence.name}"
                     )
                 logging.debug(
                     f"{self.genome.fasta.name}: Processing sequence {current_sequence.name}"
                 )
                 sequences[current_sequence.name] = current_sequence
                 if progress is not None:
-                    progress(current_sequence.name, 1, len(self._dict.sequences), 0, current_sequence.length)
+                    progress(
+                        current_sequence.name,
+                        1,
+                        len(self._dict.sequences),
+                        0,
+                        current_sequence.length,
+                    )
                 position = 0
                 continue
 
             matches = list(pattern.finditer(line))
 
             # No Ns found in this line: close the open run (if any).
             if len(matches) == 0:
@@ -126,26 +138,32 @@
                     current_sequence.open_run(match.start() + position)
 
                 # The run is ending before the end of the line. Close the open run (if any).
                 if match.end() < len(line):
                     current_sequence.close_run(match.end() + position)
             position += len(line)
             if progress is not None:
-                progress(current_sequence.name, 0,len(self._dict.sequences), len(line), current_sequence.length)
+                progress(
+                    current_sequence.name,
+                    0,
+                    len(self._dict.sequences),
+                    len(line),
+                    current_sequence.length,
+                )
 
         # File is terminated: close the current sequence and the open run (if any).
         if current_sequence is None:
             raise RuntimeError("Found the end of the file but no sequences found.")
         current_sequence.end(position)
         return list(sequences.values())
 
     def count_letters(
         self,
         letter: str = "N",
         progress: typing.Callable[[str, int, int, int, int], None] = False,
     ) -> typing.List[LetterRunCollection]:
         if progress is False:
             progress = self._progress
-        
+
         with gzip.open(self.genome.fasta, "rt") as f:
             sequences = self._process_file(f, letter, progress)
         return sequences
```

### Comparing `wgse_ng-1.0.0a5/wgse/fasta/fasta_stats_files.py` & `wgse_ng-1.0.0a7/wgse/fasta/fasta_stats_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class FASTAStatsFiles:
     """Manage the creation of statistics files for Ns."""
 
     def __init__(
         self,
         fasta_file: FASTALetterCounter,
         long_run_threshold: int = 300,
-        buckets_number: int = 1000
+        buckets_number: int = 1000,
     ) -> None:
         self._long_run_threshold = long_run_threshold
         self._buckets_number = buckets_number
         self._fasta_file = fasta_file
 
     def save_nbin(self, sequences: typing.List[LetterRunCollection]):
         lines = [
@@ -34,15 +34,15 @@
         for sequence in sequences:
             for index, run in enumerate(
                 sequence.filter(lambda x: x.length > self._long_run_threshold)
             ):
                 row = f"{sequence.name}\t{index+1}\t{run.start:,}\t{run.length:,}\n"
                 lines.append(row)
         return lines
-    
+
     def load_bed(self):
         pass
 
     def save_bed(self, sequences: typing.List[LetterRunCollection]):
         lines = [
             "#WGS Extract runs of N: BED file of bin definitions\n",
             f"#Processing Ref Model: {self._fasta_file.model_name} with >{self._long_run_threshold}bp of N runs\n",
@@ -50,29 +50,29 @@
         ]
 
         for sequence in sequences:
             for run in sequence.filter(lambda x: x.length > self._long_run_threshold):
                 row = f"{sequence.name}\t{run.start}\t{run.start+run.length}\n"
                 lines.append(row)
         return lines
-    
+
     def load_nbuc(self):
         entries = list()
         with open(self._fasta_file.genome.nbuc, "r") as f:
             reader = csv.DictReader(f, delimiter="\t")
             for row in reader:
                 entries.append
                 sequence = LetterRunCollection(row[0], row[1])
-                
-                n_count= row[0]
-                NumNreg= row[0]
-                NregSizeMean= row[0]
-                NregSizeStdDev= row[0]
-                SmlNreg= row[0]
-                BuckSize= row[0]
+
+                n_count = row[0]
+                NumNreg = row[0]
+                NregSizeMean = row[0]
+                NregSizeStdDev = row[0]
+                SmlNreg = row[0]
+                BuckSize = row[0]
 
     def save_nbuc(self, sequences: typing.List[LetterRunCollection]):
         lines = [
             "#WGS Extract generated Sequence of N summary file\n",
             f"#Model {self._fasta_file.model_name} with >{self._long_run_threshold}bp Sequence of N and {self._buckets_number} buckets per sequence\n",
             "#Seq\tNumBP\tNumNs\tNumNreg\tNregSizeMean\tNregSizeStdDev\tSmlNreg\tBuckSize\tBucket Sparse List (bp start, ln value) when nonzero\n",
         ]
@@ -110,20 +110,24 @@
             lines.append(row)
         return lines
 
     def _generate_file(self, path: Path, lines: typing.List[str]):
         with path.open("wt", encoding="utf8") as f:
             f.writelines(lines)
 
-    def _generate_files(self, sequences: typing.Dict[str, typing.List[LetterRunCollection]]):
+    def _generate_files(
+        self, sequences: typing.Dict[str, typing.List[LetterRunCollection]]
+    ):
         self._generate_file(self._fasta_file.genome.nbuc, self.save_nbuc(sequences))
         self._generate_file(self._fasta_file.genome.bed, self.save_bed(sequences))
         self._generate_file(self._fasta_file.genome.nbin, self.save_nbin(sequences))
-        
+
     def _load_files(self):
         pass
 
     def generate_stats(self):
         logging.info(f"{self._fasta_file.genome.final_name.name}: Counting Ns.")
         sequences = self._fasta_file.count_letters("N")
-        logging.info(f"{self._fasta_file.genome.final_name.name}: Finished counting Ns.")
-        self._generate_files(sequences)
+        logging.info(
+            f"{self._fasta_file.genome.final_name.name}: Finished counting Ns."
+        )
+        self._generate_files(sequences)
```

### Comparing `wgse_ng-1.0.0a5/wgse/fasta/letter_run_buckets.py` & `wgse_ng-1.0.0a7/wgse/fasta/letter_run_buckets.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         long_run_threshold: int,
         items: typing.OrderedDict[int, int] = None,
     ) -> None:
         self._buckets_number = buckets_number
         self._long_run_threshold: int = long_run_threshold
         self._sequence: LetterRunCollection = sequence
         self.buckets = items
-        
+
         if self.buckets is None:
             self.buckets = self._make_buckets()
 
     def _make_buckets(self) -> typing.OrderedDict[int, int]:
         if self._buckets_number > self._sequence.length:
             # Can't have less than 1 N per bucket.
             # This can happen in short sequence (i.e., decoy).
@@ -37,19 +37,19 @@
         ):
             # Determine how many buckets this run is spanning
             start = run.start
             end = run.start + run.length
             index_bucket_start = int(math.floor(start / bucket_size))
             index_bucket_end = int(math.floor(end / bucket_size))
 
-            # Iterate over each bucket determining how many elements are in 
+            # Iterate over each bucket determining how many elements are in
             # each bucket.
             for bucket in range(index_bucket_start, index_bucket_end + 1):
                 start_bucket_offset = max(bucket * bucket_size, start)
                 end_bucket_offset = min(bucket * bucket_size + bucket_size - 1, end)
                 runs_count = end_bucket_offset - start_bucket_offset
                 if runs_count < 1:
                     continue
                 if bucket not in buckets:
                     buckets[bucket] = 0
                 buckets[bucket] += runs_count
-        return buckets
+        return buckets
```

### Comparing `wgse_ng-1.0.0a5/wgse/fasta/letter_run_collection.py` & `wgse_ng-1.0.0a7/wgse/fasta/letter_run_collection.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,8 @@
         if self.is_run_open():
             self.close_run(position)
         self._is_ended = True
 
         if position != self.length:
             raise ValueError(
                 f"Expected {self.length} base pairs in this sequence but processed {position}."
-            )
+            )
```

### Comparing `wgse_ng-1.0.0a5/wgse/fasta/reference.py` & `wgse_ng-1.0.0a7/wgse/fasta/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from collections import OrderedDict
 import enum
 import logging
+from collections import OrderedDict
 
 from wgse.data.genome import Genome
 from wgse.data.sequence import Sequence
 
-
 logger = logging.getLogger(__name__)
 
+
 class ReferenceStatus(enum.Enum):
     Available = enum.auto()
     Downloadable = enum.auto()
     Buildable = enum.auto()
     Unknown = enum.auto()
 
 
@@ -107,13 +107,13 @@
                 if query_sequence.length != query_sequence.length:
                     matching = False
                     break
             if matching:
                 logger.info(f"{genome!s} is a perfect match.")
                 match_list.append(genome)
         return match_list
-    
+
     def __str__(self) -> str:
         return f"{self.build} ({self.status.name})"
-    
+
     def __repr__(self) -> str:
-        return self.__str__()
+        return self.__str__()
```

### Comparing `wgse_ng-1.0.0a5/wgse/fastq/fastq_file.py` & `wgse_ng-1.0.0a7/wgse/fastq/fastq_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 from math import sqrt
 from pathlib import Path
 
 from wgse.utility.sequencers import Sequencers
 
 
 class FASTQFile:
-    def __init__(
-        self, path: Path, sequencers: Sequencers = Sequencers()
-    ) -> None:
+    def __init__(self, path: Path, sequencers: Sequencers = Sequencers()) -> None:
         self.path = path
         self._sequencers = sequencers
 
     def process_FASTQ(self, paired=True):
         line_count = 0
         char_count = 0
         sequencer_id = ""
```

### Comparing `wgse_ng-1.0.0a5/wgse/gui/main.py` & `wgse_ng-1.0.0a7/wgse/gui/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import os
-import signal
-from subprocess import Popen
 import sys
 import webbrowser
 from pathlib import Path
 
-from PyQt6.QtCore import QObject, QThread
-from PyQt6.QtWidgets import QApplication, QMainWindow
-from PySide6.QtCore import QModelIndex, SignalInstance, Signal
+from PySide6.QtCore import QModelIndex
 from PySide6.QtWidgets import (
     QApplication,
     QFileDialog,
     QMainWindow,
     QMessageBox,
     QTableWidgetItem,
 )
@@ -22,39 +18,25 @@
     HeaderProgramsAdapter,
     HeaderReadGroupAdapter,
     HeaderSequenceAdapter,
 )
 from wgse.adapters.index_stats_adapter import IndexStatsAdapter
 from wgse.adapters.reference_adapter import ReferenceAdapter
 from wgse.alignment_map.alignment_map_file import AlignmentMapFile
+from wgse.alignment_map.index_stats_calculator import IndexStatsCalculator
 from wgse.configuration import MANAGER_CFG
 from wgse.data.gender import Gender
 from wgse.data.sorting import Sorting
-from wgse.gui.extract import ExtractDialog
+from wgse.gui.extract.extract_wizard import ExtractWizard
 from wgse.gui.table_dialog import ListTableDialog, TableDialog
 from wgse.gui.ui_form import Ui_MainWindow
 from wgse.utility.external import External
-
-
-class SimpleWorker(QThread):
-    def __init__(self, function, parent=None) -> None:
-        super().__init__(parent)
-        self.progress = Signal(int)
-        self.function = function
-        self.process: Popen = None
-
-    def run(self):
-        self.process = self.function()
-        self.process.wait()
-
-    def kill(self):
-        if hasattr(os.sys, "winver"):
-            self.process.kill()
-        else:
-            self.process.send_signal(signal.SIGTERM)
+from wgse.utility.shortcut import Shortcut
+from wgse.utility.simple_worker import SimpleWorker
+from wgse.variant_caller import VariantCaller
 
 
 class WGSEWindow(QMainWindow):
     def launch():
         app = QApplication(sys.argv)
         widget = WGSEWindow()
         widget.show()
@@ -65,41 +47,67 @@
         parent=None,
         config=MANAGER_CFG.GENERAL,
         external: External = External(),
     ):
         super().__init__(parent)
         self._external = external
         self.config = config
+        self.current_file = None
+
         self.switch_to_main()
-        return
+        self.ui.actionDocumentation.triggered.connect(self.on_doc)
+        self.ui.actionOpen.triggered.connect(self.on_open)
+        self.ui.actionExit.triggered.connect(self.on_close)
+        self.ui.actionSettings.triggered.connect(self.on_settings)
+        self.ui.actionCreate_launcher_on_desktop.triggered.connect(self.create_launcher)
+
+    def create_launcher(self):
+        path = Shortcut().create()
+        message_box = QMessageBox()
+        message_box.setWindowTitle("Created")
+        message_box.setText(f"A link to WGSE-NG was created at {path}")
+        message_box.setStandardButtons(QMessageBox.StandardButton.Ok)
+        message_box.exec()
 
     def switch_to_main(self):
         self.ui = Ui_MainWindow()
         self.ui.setupUi(self)
 
         self.ui.fileInformationTable.setAlternatingRowColors(True)
 
-        self.ui.actionDocumentation.triggered.connect(self.on_doc)
-        self.ui.actionOpen.triggered.connect(self.on_open)
-        self.ui.actionExit.triggered.connect(self.on_close)
-        self.ui.actionSettings.triggered.connect(self.on_settings)
         self.ui.fileInformationTable.doubleClicked.connect(self.file_item_clicked)
         self.ui.extract.clicked.connect(self.export)
-        self.ui.progress.hide()
-        self.ui.stop.hide()
-        self.ui.stop.clicked.connect(self.stop)
+        self.ui.variant.clicked.connect(self.variant_calling)
 
         self._long_operation: SimpleWorker = None
-        if self.config.last_path != None:
-            self.on_open(self.config.last_path)
+        self._prepare_ready(self.config.last_path)
+
+    def variant_calling(self):
+        if self.current_file is None:
+            return
+        self._prepare_long_operation(f"Variant calling.")
+        self._long_operation = VariantCaller(progress=self._set_calling_progress)
+        self._worker = SimpleWorker(
+            self._long_operation.call,
+            self.current_file,
+        )
+
+    def _set_calling_progress(self, sub_operation, total, current):
+        if current is None:
+            self._prepare_ready()
+            return
+        if total is None or total == 0:
+            return
+        self.ui.statusbar.showMessage(f"Variant calling, {sub_operation}")
+        self.ui.progress.setValue((current / total) * 100)
 
     def stop(self):
-        self.ui.stop.setDisabled(True)
         if self._long_operation is not None:
             self._long_operation.kill()
+        self._prepare_ready()
 
     def dragEnterEvent(self, event):
         if event.mimeData().hasUrls():
             event.accept()
         else:
             event.ignore()
 
@@ -108,17 +116,26 @@
             file_path = url.toLocalFile()
             print("Dropped file:", file_path)
             # Do something with the dropped file
 
     def export(self):
         if self.current_file is None:
             return
-        dialog = ExtractDialog(self.current_file, self)
+        self._prepare_long_operation("Exporting")
+        dialog = ExtractWizard(self.current_file, progress=self._set_export_progress)
         dialog.exec()
 
+    def _set_export_progress(self, total, current):
+        if current is None:
+            self._prepare_ready()
+            return
+        if total is None or total == 0:
+            return
+        self.ui.progress.setValue((current / total) * 100)
+
     def on_close(self):
         MANAGER_CFG.save()
         self.close()
 
     def closeEvent(self, event=False):
         MANAGER_CFG.save()
         event.accept()
@@ -176,15 +193,18 @@
         size = f"{size:.1f} GB"
 
         rows = [
             ("Directory", str(self.current_file.path.parent)),
             ("Filename", str(self.current_file.path.name)),
             ("Size", size),
             ("File Type", info.file_type.name),
-            ("Reference", f"{info.reference_genome.build} ({info.reference_genome.status.name})"),
+            (
+                "Reference",
+                f"{info.reference_genome.build} ({info.reference_genome.status.name})",
+            ),
             ("Gender", gender_string),
             ("Sorted", sorted_string),
             ("Indexed", indexed_string),
             ("Mitochondrial DNA Model", info.mitochondrial_dna_model.name),
             ("Header", click_to_open),
             ("Alignment stats", click_to_open),
             ("Index stats", click_to_open),
@@ -255,88 +275,127 @@
             prompt.setStandardButtons(
                 QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No
             )
             prompt.setDefaultButton(QMessageBox.StandardButton.No)
             choice = QMessageBox.StandardButton(prompt.exec())
             if choice == QMessageBox.StandardButton.No:
                 return
+        self._prepare_long_operation("Indexing")
+        self._long_operation = SimpleWorker(
+            self._external.index, self.current_file.path, io=self._set_index_progress
+        )
 
-        self.ui.progress.setMaximum(0)
+    def _prepare_long_operation(self, message):
+        self.ui.progress.setMaximum(100)
         self.ui.progress.setMinimum(0)
         self.ui.progress.setValue(0)
         self.ui.progress.show()
         self.ui.stop.setEnabled(True)
         self.ui.stop.show()
-        self._long_operation = SimpleWorker(
-            lambda: self._external.index(self.current_file.path, wait=False)
-        )
-        self._long_operation.finished.connect(self.reload)
-        self._long_operation.start()
+        self.ui.statusbar.showMessage(message)
 
-    def reload(self):
+    def _prepare_ready(self, path=None):
+        self._long_operation = None
         self.ui.progress.hide()
+        self.ui.stop.setEnabled(False)
         self.ui.stop.hide()
-        self._long_operation.deleteLater()
-        self.on_open(self.current_file.path)
+        if self.current_file is not None:
+            self.on_open(self.current_file.path)
+        elif path is not None:
+            self.on_open(path)
+        self.ui.statusbar.showMessage("Ready.")
+
+    def _set_index_progress(self, read_bytes, _):
+        if read_bytes is None:
+            self._prepare_ready()
+            return
+        percentage = read_bytes / self.current_file.path.stat().st_size
+        print(int(percentage * 100))
+        self.ui.progress.setValue(int(percentage * 100))
+
+    def _yn_message_box(self, title, text, info):
+        prompt = QMessageBox()
+        prompt.setWindowTitle(title)
+        prompt.setText(text)
+        if info is not None:
+            prompt.setInformativeText(info)
+
+        buttons = QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No
+        prompt.setStandardButtons(buttons)
+        prompt.setDefaultButton(QMessageBox.StandardButton.Yes)
+        return QMessageBox.StandardButton(prompt.exec())
 
     def _show_index_stats(self):
         if self.current_file is None:
             return
+
         if not self.current_file.file_info.indexed:
-            prompt = QMessageBox()
-            prompt.setWindowTitle("File is not indexed")
-            prompt.setText("Index stats are not available if the file is not indexed.")
-            prompt.setInformativeText(
-                "Do you want to index the file? This may take a while."
+            choice = self._yn_message_box(
+                "File is not indexed",
+                "Index stats are not available if the file is not indexed.",
+                "Do you want to index the file? This may take a while.",
             )
-            prompt.setStandardButtons(
-                QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No
-            )
-            prompt.setDefaultButton(QMessageBox.StandardButton.No)
-            choice = QMessageBox.StandardButton(prompt.exec())
             if choice == QMessageBox.StandardButton.No:
                 return
             self._do_indexing(user_informed=True)
+
+        if self.current_file.file_info.index_stats is None:
+            choice = self._yn_message_box(
+                "Index stats not available",
+                "Index stats needs to be calculated for this file.",
+                "Do you want to calculate the stats? This may take a while.",
+            )
+            if choice == QMessageBox.StandardButton.No:
+                return
+
+            indexed_stats = IndexStatsCalculator(self.current_file.path)
+            self.current_file.file_info.index_stats = indexed_stats.get_stats()
+            self.current_file.file_info.gender = self.current_file.get_gender(
+                self.current_file.file_info.index_stats
+            )
+
+        index_stats = self.current_file.file_info.index_stats
         dialog = TableDialog("Index Statistics", self)
-        dialog.set_data(
-            IndexStatsAdapter.adapt(self.current_file.file_info.index_stats)
-        )
+        dialog.set_data(IndexStatsAdapter.adapt(index_stats))
         dialog.exec()
 
     def _show_coverage_stats(self):
         return
 
     def _show_reference(self):
-        adapted = ReferenceAdapter.adapt(self.current_file.file_info.reference_genome)
+        if self.current_file is None:
+            return
+        reference = self.current_file.file_info.reference_genome
         dialog = TableDialog("Reference genome", self)
-        dialog.set_data(adapted)
+        dialog.set_data(ReferenceAdapter.adapt(reference))
         dialog.exec()
 
     def _show_alignment_stats(self):
         if self.current_file is None:
             return
+        alignment_stats = self.current_file.file_info.alignment_stats
         dialog = TableDialog("Alignment statistics", self)
-        dialog.set_data(
-            AlignmentStatsAdapter.adapt(self.current_file.file_info.alignment_stats)
-        )
+        dialog.set_data(AlignmentStatsAdapter.adapt(alignment_stats))
         dialog.exec()
 
     def _show_header(self):
         if self.current_file is None:
             return
 
+        sequences = self.current_file.header.sequences.values()
+        programs = self.current_file.header.programs
+        read_groups = self.current_file.header.read_groups
+        comments = self.current_file.header.comments
+
         dialog = ListTableDialog("Header", self)
-        data = {
-            "Sequences": HeaderSequenceAdapter.adapt(
-                self.current_file.header.sequences.values()
-            ),
-            "Programs": HeaderProgramsAdapter.adapt(self.current_file.header.programs),
-            "Read groups": HeaderReadGroupAdapter.adapt(
-                self.current_file.header.read_groups
-            ),
-            "Comments": HeaderCommentsAdapter.adapt(self.current_file.header.comments),
-        }
-        dialog.set_data(data)
+        dialog.set_data(
+            {
+                "Sequences": HeaderSequenceAdapter.adapt(sequences),
+                "Programs": HeaderProgramsAdapter.adapt(programs),
+                "Read groups": HeaderReadGroupAdapter.adapt(read_groups),
+                "Comments": HeaderCommentsAdapter.adapt(comments),
+            }
+        )
         dialog.exec()
 
     def _gender_determined(self, gender: Gender):
         pass
```

### Comparing `wgse_ng-1.0.0a5/wgse/gui/microarray_format.py` & `wgse_ng-1.0.0a7/wgse/gui/extract/microarray_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-from PySide6.QtCore import QCoreApplication, QMetaObject
 from PySide6.QtGui import QFont
 from PySide6.QtWidgets import (
     QCheckBox,
     QGridLayout,
     QGroupBox,
     QLabel,
     QSizePolicy,
     QSpacerItem,
     QVBoxLayout,
     QWidget,
 )
+
 from wgse.microarray.microarray_converter import MicroarrayConverterTarget
 
 
-class MicroarrayFormatWidget(QWidget):
+class MicroarraySelection(QWidget):
     def __init__(self, parent):
         super().__init__(parent)
-        self.setObjectName("microarrayFormatSelection")
+        self.setObjectName(MicroarraySelection.__name__)
         self.main_group_box = QGroupBox("Select microarray format", parent)
-        self.group_box_layout = QVBoxLayout(self.main_group_box)
+        self.inner_layout = QVBoxLayout(self.main_group_box)
+        self.main_layout = QVBoxLayout()
 
         self.main_group_box.setObjectName("mainGroupBox")
-        self.group_box_layout.setObjectName("mainLayout")
+        self.inner_layout.setObjectName("innerLayout")
 
         self.combined_checkboxes = None
         self.genealogy_checkboxes = None
         self.health_checkboxes = None
         self.ancient_dna_checkboxes = None
 
         self.combined_group = self._create_combined_group_box(self.main_group_box)
         self.genealogy_group = self._create_genealogy_group_box(self.main_group_box)
         self.health_group = self._create_health_group_box(self.main_group_box)
         self.ancient_group = self._create_ancient_dna_group_box(self.main_group_box)
 
-        self.group_box_layout.addWidget(self.combined_group)
-        self.group_box_layout.addWidget(self.genealogy_group)
-        self.group_box_layout.addWidget(self.health_group)
-        self.group_box_layout.addWidget(self.ancient_group)
+        self.checkboxes = [
+            *self.combined_checkboxes,
+            *self.genealogy_checkboxes,
+            *self.health_checkboxes,
+            *self.ancient_dna_checkboxes,
+        ]
+
+        self.inner_layout.addWidget(self.combined_group)
+        self.inner_layout.addWidget(self.genealogy_group)
+        self.inner_layout.addWidget(self.health_group)
+        self.inner_layout.addWidget(self.ancient_group)
 
-        self.main_layout = QVBoxLayout()
         self.main_layout.addWidget(self.main_group_box)
         self.setLayout(self.main_layout)
         self.hide()
 
     def _create_combined_group_box(self, parent):
         boldFont = QFont()
         boldFont.setBold(True)
```

### Comparing `wgse_ng-1.0.0a5/wgse/gui/table_dialog.py` & `wgse_ng-1.0.0a7/wgse/gui/table_dialog.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 from PySide6.QtCore import QMetaObject, Qt
-from PySide6.QtWidgets import (QAbstractItemView, QComboBox, QDialog,
-                               QTableWidget, QTableWidgetItem, QVBoxLayout)
+from PySide6.QtWidgets import (
+    QAbstractItemView,
+    QComboBox,
+    QDialog,
+    QTableWidget,
+    QTableWidgetItem,
+    QVBoxLayout,
+)
 
 from wgse.data.tabular_data import TabularData
 
 
 class TableDialog(QDialog):
-    def __init__(
-        self, title="Dialog", parent=None, f=Qt.WindowType.Dialog
-    ) -> None:
+    def __init__(self, title="Dialog", parent=None, f=Qt.WindowType.Dialog) -> None:
         super().__init__(parent, f)
         self.setObjectName(title)
         self.setWindowTitle(title)
         self.resize(640, 480)
-        
+
         self.tableWidget = QTableWidget(self)
         self.tableWidget.setEditTriggers(QAbstractItemView.NoEditTriggers)
-        
+
         self.verticalLayout = QVBoxLayout(self)
         self.verticalLayout.addWidget(self.tableWidget)
-        
-        self.setWindowModality(Qt.WindowModality.ApplicationModal)        
+
+        self.setWindowModality(Qt.WindowModality.ApplicationModal)
         QMetaObject.connectSlotsByName(self)
 
     def set_data(self, data: TabularData):
         self.tableWidget.setRowCount(len(data.rows))
         self.tableWidget.setColumnCount(max(len(x.columns) for x in data.rows))
         self.tableWidget.horizontalHeader().setStretchLastSection(True)
         if data.horizontal_header:
             for index, header in enumerate(data.horizontal_header):
-                self.tableWidget.setHorizontalHeaderItem(index, QTableWidgetItem(header))
+                self.tableWidget.setHorizontalHeaderItem(
+                    index, QTableWidgetItem(header)
+                )
         else:
             self.tableWidget.horizontalHeader().hide()
-            
+
         vertical_header = False
         for row_index, row in enumerate(data.rows):
             if row.vertical_header is not None:
-                self.tableWidget.setVerticalHeaderItem(row_index, QTableWidgetItem(row.vertical_header))
+                self.tableWidget.setVerticalHeaderItem(
+                    row_index, QTableWidgetItem(row.vertical_header)
+                )
                 vertical_header = True
             for col_index, text in enumerate(row.columns):
                 self.tableWidget.setItem(row_index, col_index, QTableWidgetItem(text))
         if not vertical_header:
             self.tableWidget.verticalHeader().hide()
-                
+
+
 class ListTableDialog(TableDialog):
     def __init__(self, title="Dialog", parent=None, f=Qt.WindowType.Dialog) -> None:
         super().__init__(title, parent, f)
         self.itemList = QComboBox(self)
         self.verticalLayout.insertWidget(0, self.itemList)
         self.data = None
         self.itemList.currentIndexChanged.connect(self.index_changed)
-        
+
     def set_data(self, data: dict[str, TabularData]):
         self.itemList.addItems(list(data.keys()))
         self.data = data
         self.index_changed(0)
-    
+
     def index_changed(self, index):
         if self.data is None:
             return
         text = self.itemList.itemText(index)
-        super().set_data(self.data[text])
+        super().set_data(self.data[text])
```

### Comparing `wgse_ng-1.0.0a5/wgse/gui/ui_form.py` & `wgse_ng-1.0.0a7/wgse/gui/ui_form.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,59 +4,105 @@
 ## Form generated from reading UI file 'form.ui'
 ##
 ## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
-    QMetaObject, QObject, QPoint, QRect,
-    QSize, QTime, QUrl, Qt)
-from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
-    QCursor, QFont, QFontDatabase, QGradient,
-    QIcon, QImage, QKeySequence, QLinearGradient,
-    QPainter, QPalette, QPixmap, QRadialGradient,
-    QTransform)
-from PySide6.QtWidgets import (QAbstractItemView, QApplication, QGridLayout, QHeaderView,
-    QMainWindow, QMenu, QMenuBar, QProgressBar,
-    QPushButton, QSizePolicy, QStatusBar, QTableWidget,
-    QTableWidgetItem, QWidget)
+from PySide6.QtCore import (
+    QCoreApplication,
+    QDate,
+    QDateTime,
+    QLocale,
+    QMetaObject,
+    QObject,
+    QPoint,
+    QRect,
+    QSize,
+    Qt,
+    QTime,
+    QUrl,
+)
+from PySide6.QtGui import (
+    QAction,
+    QBrush,
+    QColor,
+    QConicalGradient,
+    QCursor,
+    QFont,
+    QFontDatabase,
+    QGradient,
+    QIcon,
+    QImage,
+    QKeySequence,
+    QLinearGradient,
+    QPainter,
+    QPalette,
+    QPixmap,
+    QRadialGradient,
+    QTransform,
+)
+from PySide6.QtWidgets import (
+    QAbstractItemView,
+    QApplication,
+    QGridLayout,
+    QHeaderView,
+    QMainWindow,
+    QMenu,
+    QMenuBar,
+    QProgressBar,
+    QPushButton,
+    QSizePolicy,
+    QStatusBar,
+    QTableWidget,
+    QTableWidgetItem,
+    QWidget,
+)
+
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
-            MainWindow.setObjectName(u"MainWindow")
+            MainWindow.setObjectName("MainWindow")
         MainWindow.resize(724, 562)
         MainWindow.setMinimumSize(QSize(0, 20))
         self.actionSettings = QAction(MainWindow)
-        self.actionSettings.setObjectName(u"actionSettings")
+        self.actionSettings.setObjectName("actionSettings")
         self.actionOpen = QAction(MainWindow)
-        self.actionOpen.setObjectName(u"actionOpen")
+        self.actionOpen.setObjectName("actionOpen")
         self.actionExit = QAction(MainWindow)
-        self.actionExit.setObjectName(u"actionExit")
+        self.actionExit.setObjectName("actionExit")
         self.actionDocumentation = QAction(MainWindow)
-        self.actionDocumentation.setObjectName(u"actionDocumentation")
+        self.actionDocumentation.setObjectName("actionDocumentation")
         self.actionAbout = QAction(MainWindow)
-        self.actionAbout.setObjectName(u"actionAbout")
+        self.actionAbout.setObjectName("actionAbout")
         self.actionLog_viewer = QAction(MainWindow)
-        self.actionLog_viewer.setObjectName(u"actionLog_viewer")
+        self.actionLog_viewer.setObjectName("actionLog_viewer")
         self.actionGenomes = QAction(MainWindow)
-        self.actionGenomes.setObjectName(u"actionGenomes")
+        self.actionGenomes.setObjectName("actionGenomes")
+        self.actionCreate_launcher_on_desktop = QAction(MainWindow)
+        self.actionCreate_launcher_on_desktop.setObjectName(
+            "actionCreate_launcher_on_desktop"
+        )
         self.centralwidget = QWidget(MainWindow)
-        self.centralwidget.setObjectName(u"centralwidget")
+        self.centralwidget.setObjectName("centralwidget")
         self.gridLayout = QGridLayout(self.centralwidget)
-        self.gridLayout.setObjectName(u"gridLayout")
+        self.gridLayout.setObjectName("gridLayout")
         self.fileInformationTable = QTableWidget(self.centralwidget)
-        self.fileInformationTable.setObjectName(u"fileInformationTable")
-        sizePolicy = QSizePolicy(QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.MinimumExpanding)
+        self.fileInformationTable.setObjectName("fileInformationTable")
+        sizePolicy = QSizePolicy(
+            QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.MinimumExpanding
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.fileInformationTable.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.fileInformationTable.sizePolicy().hasHeightForWidth()
+        )
         self.fileInformationTable.setSizePolicy(sizePolicy)
-        self.fileInformationTable.setStyleSheet(u"")
+        self.fileInformationTable.setStyleSheet("")
         self.fileInformationTable.setEditTriggers(QAbstractItemView.NoEditTriggers)
         self.fileInformationTable.setAlternatingRowColors(True)
         self.fileInformationTable.setShowGrid(True)
         self.fileInformationTable.setGridStyle(Qt.DotLine)
         self.fileInformationTable.setSortingEnabled(False)
         self.fileInformationTable.setColumnCount(0)
         self.fileInformationTable.horizontalHeader().setVisible(False)
@@ -68,106 +114,136 @@
         self.fileInformationTable.verticalHeader().setDefaultSectionSize(30)
         self.fileInformationTable.verticalHeader().setHighlightSections(False)
         self.fileInformationTable.verticalHeader().setStretchLastSection(False)
 
         self.gridLayout.addWidget(self.fileInformationTable, 0, 0, 1, 4)
 
         self.extract = QPushButton(self.centralwidget)
-        self.extract.setObjectName(u"extract")
+        self.extract.setObjectName("extract")
 
         self.gridLayout.addWidget(self.extract, 1, 0, 1, 1)
 
         self.haplotype = QPushButton(self.centralwidget)
-        self.haplotype.setObjectName(u"haplotype")
+        self.haplotype.setObjectName("haplotype")
 
         self.gridLayout.addWidget(self.haplotype, 1, 1, 1, 1)
 
         self.analysis = QPushButton(self.centralwidget)
-        self.analysis.setObjectName(u"analysis")
+        self.analysis.setObjectName("analysis")
 
         self.gridLayout.addWidget(self.analysis, 1, 2, 1, 1)
 
         self.variant = QPushButton(self.centralwidget)
-        self.variant.setObjectName(u"variant")
+        self.variant.setObjectName("variant")
 
         self.gridLayout.addWidget(self.variant, 1, 3, 1, 1)
 
         self.progress = QProgressBar(self.centralwidget)
-        self.progress.setObjectName(u"progress")
-        sizePolicy1 = QSizePolicy(QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.Fixed)
+        self.progress.setObjectName("progress")
+        sizePolicy1 = QSizePolicy(
+            QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.Fixed
+        )
         sizePolicy1.setHorizontalStretch(0)
         sizePolicy1.setVerticalStretch(0)
         sizePolicy1.setHeightForWidth(self.progress.sizePolicy().hasHeightForWidth())
         self.progress.setSizePolicy(sizePolicy1)
         self.progress.setMinimumSize(QSize(0, 0))
         self.progress.setValue(24)
 
         self.gridLayout.addWidget(self.progress, 4, 0, 1, 3)
 
         self.stop = QPushButton(self.centralwidget)
-        self.stop.setObjectName(u"stop")
+        self.stop.setObjectName("stop")
         sizePolicy2 = QSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed)
         sizePolicy2.setHorizontalStretch(0)
         sizePolicy2.setVerticalStretch(0)
         sizePolicy2.setHeightForWidth(self.stop.sizePolicy().hasHeightForWidth())
         self.stop.setSizePolicy(sizePolicy2)
         self.stop.setMinimumSize(QSize(0, 0))
 
         self.gridLayout.addWidget(self.stop, 4, 3, 1, 1)
 
         MainWindow.setCentralWidget(self.centralwidget)
         self.menubar = QMenuBar(MainWindow)
-        self.menubar.setObjectName(u"menubar")
+        self.menubar.setObjectName("menubar")
         self.menubar.setGeometry(QRect(0, 0, 724, 21))
-        sizePolicy3 = QSizePolicy(QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.Minimum)
+        sizePolicy3 = QSizePolicy(
+            QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.Minimum
+        )
         sizePolicy3.setHorizontalStretch(0)
         sizePolicy3.setVerticalStretch(0)
         sizePolicy3.setHeightForWidth(self.menubar.sizePolicy().hasHeightForWidth())
         self.menubar.setSizePolicy(sizePolicy3)
         self.menuFile = QMenu(self.menubar)
-        self.menuFile.setObjectName(u"menuFile")
+        self.menuFile.setObjectName("menuFile")
         self.menuHelp = QMenu(self.menubar)
-        self.menuHelp.setObjectName(u"menuHelp")
+        self.menuHelp.setObjectName("menuHelp")
         self.menuTools = QMenu(self.menubar)
-        self.menuTools.setObjectName(u"menuTools")
+        self.menuTools.setObjectName("menuTools")
         MainWindow.setMenuBar(self.menubar)
         self.statusbar = QStatusBar(MainWindow)
-        self.statusbar.setObjectName(u"statusbar")
+        self.statusbar.setObjectName("statusbar")
         MainWindow.setStatusBar(self.statusbar)
 
         self.menubar.addAction(self.menuFile.menuAction())
         self.menubar.addAction(self.menuTools.menuAction())
         self.menubar.addAction(self.menuHelp.menuAction())
         self.menuFile.addAction(self.actionOpen)
         self.menuFile.addAction(self.actionSettings)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionExit)
         self.menuHelp.addAction(self.actionDocumentation)
         self.menuHelp.addAction(self.actionAbout)
         self.menuTools.addAction(self.actionLog_viewer)
         self.menuTools.addAction(self.actionGenomes)
+        self.menuTools.addSeparator()
+        self.menuTools.addAction(self.actionCreate_launcher_on_desktop)
 
         self.retranslateUi(MainWindow)
         self.actionExit.triggered.connect(MainWindow.close)
 
         QMetaObject.connectSlotsByName(MainWindow)
+
     # setupUi
 
     def retranslateUi(self, MainWindow):
-        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"WGSE - Genome sequencing data manipulation tool", None))
-        self.actionSettings.setText(QCoreApplication.translate("MainWindow", u"Settings", None))
-        self.actionOpen.setText(QCoreApplication.translate("MainWindow", u"Open", None))
-        self.actionExit.setText(QCoreApplication.translate("MainWindow", u"Exit", None))
-        self.actionDocumentation.setText(QCoreApplication.translate("MainWindow", u"Documentation", None))
-        self.actionAbout.setText(QCoreApplication.translate("MainWindow", u"About", None))
-        self.actionLog_viewer.setText(QCoreApplication.translate("MainWindow", u"Log viewer", None))
-        self.actionGenomes.setText(QCoreApplication.translate("MainWindow", u"Reference genomes", None))
-        self.extract.setText(QCoreApplication.translate("MainWindow", u"Extract", None))
-        self.haplotype.setText(QCoreApplication.translate("MainWindow", u"Haplotype", None))
-        self.analysis.setText(QCoreApplication.translate("MainWindow", u"Analysis", None))
-        self.variant.setText(QCoreApplication.translate("MainWindow", u"Variant calling", None))
-        self.stop.setText(QCoreApplication.translate("MainWindow", u"Stop", None))
-        self.menuFile.setTitle(QCoreApplication.translate("MainWindow", u"File", None))
-        self.menuHelp.setTitle(QCoreApplication.translate("MainWindow", u"Help", None))
-        self.menuTools.setTitle(QCoreApplication.translate("MainWindow", u"Tools", None))
-    # retranslateUi
+        MainWindow.setWindowTitle(
+            QCoreApplication.translate(
+                "MainWindow", "WGSE - Genome sequencing data manipulation tool", None
+            )
+        )
+        self.actionSettings.setText(
+            QCoreApplication.translate("MainWindow", "Settings", None)
+        )
+        self.actionOpen.setText(QCoreApplication.translate("MainWindow", "Open", None))
+        self.actionExit.setText(QCoreApplication.translate("MainWindow", "Exit", None))
+        self.actionDocumentation.setText(
+            QCoreApplication.translate("MainWindow", "Documentation", None)
+        )
+        self.actionAbout.setText(
+            QCoreApplication.translate("MainWindow", "About", None)
+        )
+        self.actionLog_viewer.setText(
+            QCoreApplication.translate("MainWindow", "Log viewer", None)
+        )
+        self.actionGenomes.setText(
+            QCoreApplication.translate("MainWindow", "Reference genomes", None)
+        )
+        self.actionCreate_launcher_on_desktop.setText(
+            QCoreApplication.translate("MainWindow", "Create launcher on desktop", None)
+        )
+        self.extract.setText(QCoreApplication.translate("MainWindow", "Extract", None))
+        self.haplotype.setText(
+            QCoreApplication.translate("MainWindow", "Haplotype", None)
+        )
+        self.analysis.setText(
+            QCoreApplication.translate("MainWindow", "Analysis", None)
+        )
+        self.variant.setText(
+            QCoreApplication.translate("MainWindow", "Variant calling", None)
+        )
+        self.stop.setText(QCoreApplication.translate("MainWindow", "Stop", None))
+        self.menuFile.setTitle(QCoreApplication.translate("MainWindow", "File", None))
+        self.menuHelp.setTitle(QCoreApplication.translate("MainWindow", "Help", None))
+        self.menuTools.setTitle(QCoreApplication.translate("MainWindow", "Tools", None))
 
+    # retranslateUi
```

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/bed_templates/19_wes.csv` & `wgse_ng-1.0.0a7/wgse/metadata/bed_templates/19_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/bed_templates/38_wes.csv` & `wgse_ng-1.0.0a7/wgse/metadata/bed_templates/38_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/bed_templates/38_y_mt.csv` & `wgse_ng-1.0.0a7/wgse/metadata/bed_templates/38_y_mt.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/mtdna.json` & `wgse_ng-1.0.0a7/wgse/metadata/mtdna.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 00000240: 2020 226d 6435 2220 3a20 2222 2c0d 0a20    "md5" : "",.. 
 00000250: 2020 2020 2020 2022 6c65 6e67 7468 223a         "length":
 00000260: 2031 3635 3731 2c0d 0a20 2020 2020 2020   16571,..       
 00000270: 2022 7572 6c22 203a 2022 6874 7470 733a   "url" : "https:
 00000280: 2f2f 7777 772e 6e63 6269 2e6e 6c6d 2e6e  //www.ncbi.nlm.n
 00000290: 6968 2e67 6f76 2f6e 7563 6c65 6f74 6964  ih.gov/nucleotid
 000002a0: 652f 4146 3334 3730 3135 220d 0a20 2020  e/AF347015"..   
-000002b0: 207d 0d0a 5d                              }..]
+000002b0: 207d 0d0a 5d0a                            }..].
```

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/references.json` & `wgse_ng-1.0.0a7/wgse/metadata/references.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -263316,8 +263316,8 @@
 00404930: 3538 3035 2c20 2264 6f77 6e6c 6f61 6465  5805, "downloade
 00404940: 645f 6d64 3522 3a20 2235 3832 3536 3766  d_md5": "582567f
 00404950: 3339 3533 6437 3661 6662 3737 3663 3633  3953d76afb776c63
 00404960: 3932 3261 3466 6232 6622 2c20 2264 6563  922a4fb2f", "dec
 00404970: 6f6d 7072 6573 7365 645f 6d64 3522 3a20  ompressed_md5": 
 00404980: 2237 3335 3336 6338 3139 3938 3435 3066  "73536c81998450f
 00404990: 3531 6230 6534 3366 3363 3833 3033 3538  51b0e43f3c830358
-004049a0: 3322 7d5d                                3"}]
+004049a0: 3322 7d5d 0a                             3"}].
```

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/references_template.json` & `wgse_ng-1.0.0a7/wgse/metadata/references_template.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1062,8 +1062,8 @@
 00004250: 0d0a 2020 2020 7d2c 0d0a 2020 2020 7b0d  ..    },..    {.
 00004260: 0a20 2020 2020 2020 2022 6e61 6d65 223a  .        "name":
 00004270: 2022 4542 4922 2c0d 0a20 2020 2020 2020   "EBI",..       
 00004280: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
 00004290: 2246 696c 220d 0a20 2020 207d 2c0d 0a20  "Fil"..    },.. 
 000042a0: 2020 207b 0d0a 2020 2020 2020 2020 226e     {..        "n
 000042b0: 616d 6522 3a20 224e 4342 4922 0d0a 2020  ame": "NCBI"..  
-000042c0: 2020 7d0d 0a5d                             }..]
+000042c0: 2020 7d0d 0a5d 0a                          }..].
```

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/report_templates/table_macro.html` & `wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_macro.html`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
                 {% for column in row.columns %}
                 <td>{{ column }}</td>
                 {% endfor %}
             </tr>
             {% endfor %}
         </tbody>
     </table>
-{% endmacro %}
+{% endmacro %}
```

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/report_templates/table_simple.html` & `wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_simple.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/report_templates/table_tab.html` & `wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_tab.html`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             <ul class="navbar-nav">
                 <li class="nav-item">
                     <a class="nav-link" href="#file-info">File info</a>
                 </li>
                 <li class="nav-item">
                     <a class="nav-link" href="#alignment-statistics">Alignment statistics</a>
                 </li>
-                
+
                 <li class="nav-item dropdown">
                     <a class="nav-link dropdown-toggle" role="button" data-toggle="dropdown" id="navbarDropdownHeader" aria-haspopup="true" aria-expanded="false" href="javascript:void">Header</a>
                     <ul class="dropdown-menu" aria-labelledby="navbarDropdownHeader">
                         <a class="dropdown-item" href="#sequences">Sequences</a></li>
                         <a class="dropdown-item" href="#read-groups">Read groups</a></li>
                         <a class="dropdown-item" href="#programs">Programs</a></li>
                         <a class="dropdown-item" href="#comments">Comments</a></li>
@@ -59,21 +59,21 @@
                     <a class="nav-link" href="#index-statistics">Index statistics</a>
                 </li>
             </ul>
         </div>
     </nav>
 
     <div id="home" class="container page-content active">
-        
+
         <h1>WGSE - Welcome!</h1>
-        <p>This is your report made with WGSE. It contains information about your WGS file. 
+        <p>This is your report made with WGSE. It contains information about your WGS file.
             Please use the menu above to navigate through the sections.
             This file was generated on {{ general.now }} with WGSE {{ general.version }}. For more info about WGSE see <a href="https://wgse.io">here</a>.
         </p>
-        
+
     </div>
 
     <div id="file-info" class="container page-content">
         {{ build_table(file_info_data) }}
     </div>
 
     <div id="alignment-statistics" class="container page-content">
@@ -97,8 +97,8 @@
     </div>
 
     <div id="index-statistics" class="container page-content">
         {{ build_table(index_stat_data) }}
     </div>
 </body>
 
-</html>
+</html>
```

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/sequencers.json` & `wgse_ng-1.0.0a7/wgse/metadata/sequencers.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -709,8 +709,8 @@
 00002c40: 302d 3961 2d66 5d7b 3132 7d29 2422 2c0d  0-9a-f]{12})$",.
 00002c50: 0a20 2020 2020 2020 2022 636f 6f72 645f  .        "coord_
 00002c60: 7265 6765 7822 3a20 2222 2c0d 0a20 2020  regex": "",..   
 00002c70: 2020 2020 2022 636f 6f72 645f 6f72 6465       "coord_orde
 00002c80: 7222 3a20 2222 2c0d 0a20 2020 2020 2020  r": "",..       
 00002c90: 2022 7572 6c22 3a20 2268 7474 7073 3a2f   "url": "https:/
 00002ca0: 2f6e 616e 6f70 6f72 6574 6563 682e 636f  /nanoporetech.co
-00002cb0: 6d2f 220d 0a20 2020 207d 0d0a 5d         m/"..    }..]
+00002cb0: 6d2f 220d 0a20 2020 207d 0d0a 5d0a       m/"..    }..].
```

### Comparing `wgse_ng-1.0.0a5/wgse/metadata/sources.json` & `wgse_ng-1.0.0a7/wgse/metadata/sources.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -128,8 +128,8 @@
 000007f0: 7073 3a2f 2f6e 6362 692e 6e6c 6d2e 6e69  ps://ncbi.nlm.ni
 00000800: 682e 676f 762f 2922 2c0d 0a20 2020 2020  h.gov/)",..     
 00000810: 2020 2022 7572 6c73 223a 205b 0d0a 2020     "urls": [..  
 00000820: 2020 2020 2020 2020 2020 2268 7474 7073            "https
 00000830: 3a2f 2f66 7470 2e6e 6362 692e 6e6c 6d2e  ://ftp.ncbi.nlm.
 00000840: 6e69 682e 676f 762f 6765 6e6f 6d65 7322  nih.gov/genomes"
 00000850: 0d0a 2020 2020 2020 2020 5d0d 0a20 2020  ..        ]..   
-00000860: 207d 0d0a 5d                              }..]
+00000860: 207d 0d0a 5d0a                            }..].
```

### Comparing `wgse_ng-1.0.0a5/wgse/microarray/microarray_converter.py` & `wgse_ng-1.0.0a7/wgse/microarray/microarray_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from wgse.data.microarray_converter import MicroarrayConverterTarget
 from wgse.microarray.microarray_line_formatter import TARGET_FORMATTER_MAP
 from wgse.microarray.raw_file import RawEntry, RawFile
 from wgse.utility.sequence_orderer import SequenceOrderer
 
 
 class MicroarrayConverter:
-    def __init__(self, config= MANAGER_CFG.REPOSITORY) -> None:
+    def __init__(self, config=MANAGER_CFG.REPOSITORY) -> None:
         self._config = config
         self._template_folder = self._config.metadata.joinpath("microarray_templates")
         self._head_folder = self._template_folder.joinpath("head")
         self._body_folder = self._template_folder.joinpath("body")
 
         if not self._body_folder.exists():
             raise FileNotFoundError(
@@ -102,15 +102,17 @@
         lines.append("# Duplicate coordinate report\n")
         lines.append("# Duplicates,Chromosome,Position\n")
         for chromosome, positions in template.items():
             position = 0
             for position, entry in positions.items():
                 if len(entry) != 1:
                     lines.append(f"{len(entry)},{chromosome},{position}\n")
-        print(f"Target {target.name} has a total of {len(lines)-2} duplicate coordinates.")
+        print(
+            f"Target {target.name} has a total of {len(lines)-2} duplicate coordinates."
+        )
 
         with duplicate_coords.open("wt") as file:
             file.writelines(lines)
 
         lines = []
         lines.append("# Non sequential entries\n")
         lines.append("# RSID,Chromosome,Position\n")
@@ -134,16 +136,18 @@
 
             if entry.position < last_position:
                 lines.append(f"{entry.id},{entry.chromosome},{entry.position}\n")
             last_position = entry.position
 
         with non_sequential.open("wt") as file:
             file.writelines(lines)
-        
-        print(f"Target {target.name} has a total of {len(lines)-2} non sequential entries.")
+
+        print(
+            f"Target {target.name} has a total of {len(lines)-2} non sequential entries."
+        )
 
         lines = []
         lines.append("# Same RSID different coordinates\n")
         lines.append("# RSID,Chromosome,Position\n")
         same_rsids: list[list[RawEntry]] = [
             index_by_rsid[x] for x in index_by_rsid if len(index_by_rsid[x]) > 1
         ]
@@ -164,16 +168,18 @@
                 lines.append(
                     f"{broken_element.id},{broken_element.chromosome},{broken_element.position}\n"
                 )
 
         with same_rsid_different_c.open("wt") as file:
             file.writelines(lines)
 
-        print(f"Target {target.name} has a total of {len(lines)-2} entries with same rsID but different coordinates.")
-        
+        print(
+            f"Target {target.name} has a total of {len(lines)-2} entries with same rsID but different coordinates."
+        )
+
         lines = []
         lines.append("# Same coordinates different RSID\n")
         lines.append("# RSID,Chromosome,Position\n")
         same_coords: list[list[RawEntry]] = [
             index_by_coord[x] for x in index_by_coord if len(index_by_coord[x]) > 1
         ]
 
@@ -184,19 +190,21 @@
                 lines.append(
                     f"{first_element.id},{first_element.chromosome},{first_element.position}\n"
                 )
             for broken_element in broken_elements:
                 lines.append(
                     f"{broken_element.id},{broken_element.chromosome},{broken_element.position}\n"
                 )
-        
+
         with same_c_different_rsid.open("wt") as file:
             file.writelines(lines)
-        
-        print(f"Target {target.name} has a total of {len(lines)-2} entries with same coordinate but different rsIDs.")
+
+        print(
+            f"Target {target.name} has a total of {len(lines)-2} entries with same coordinate but different rsIDs."
+        )
 
     def convert(self, input: Path, target: MicroarrayConverterTarget):
         header_path = self._head_folder.joinpath(target.name).with_suffix(".txt")
         body_path = self._body_folder.joinpath(target.name).with_suffix(".txt.gz")
 
         if not header_path.exists():
             raise FileNotFoundError(
```

### Comparing `wgse_ng-1.0.0a5/wgse/microarray/microarray_line_formatter.py` & `wgse_ng-1.0.0a7/wgse/microarray/microarray_line_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from wgse.data.microarray_converter import (MicroarrayConverterExtensions,
-                                            MicroarrayConverterTarget)
+from wgse.data.microarray_converter import (
+    MicroarrayConverterExtensions,
+    MicroarrayConverterTarget,
+)
 
 TARGET_FORMATTER_MAP: dict[
     MicroarrayConverterTarget, tuple[callable, MicroarrayConverterExtensions]
 ] = dict()
 
 
 def target(
```

### Comparing `wgse_ng-1.0.0a5/wgse/microarray/raw_file.py` & `wgse_ng-1.0.0a7/wgse/microarray/raw_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-
 import gzip
 from pathlib import Path
 
 
 class RawEntry:
     def __init__(self, id=None, chromosome=None, position=None, result=None) -> None:
-        self.id : str = id
+        self.id: str = id
         self.chromosome: str = chromosome
         self.position: int = position
         self.result: str = result
-    
+
     @property
     def template_entry(self):
         return f"{self.id}\t{self.chromosome}\t{self.position}\n"
-    
+
     def __str__(self) -> str:
         return f"{self.id},{self.chromosome},{self.position},{self.result}"
-    
+
     def __repr__(self) -> str:
         return self.__str__()
 
+
 class RawFile:
     def __init__(self, path: Path) -> None:
         self.path = path
         if self.path.suffix == ".gz":
-            self.open_file = lambda:gzip.open(self.path, "rt")
+            self.open_file = lambda: gzip.open(self.path, "rt")
         else:
-            self.open_file = lambda:self.path.open("rt")
+            self.open_file = lambda: self.path.open("rt")
 
     def __iter__(self):
         with self.open_file() as file:
             for line in file:
                 if "#" in line:
                     continue
                 parts = line.split("\t")
                 id = parts[0].strip()
                 chromosome = parts[1].strip()
                 position = int(parts[2])
                 result = None
                 if len(parts) > 3:
                     result = parts[3].strip()
-                yield RawEntry(id, chromosome, position, result)
+                yield RawEntry(id, chromosome, position, result)
```

### Comparing `wgse_ng-1.0.0a5/wgse/mtDNA/CRS.fasta` & `wgse_ng-1.0.0a7/wgse/mtDNA/CRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a5/wgse/mtDNA/RSRS.fasta` & `wgse_ng-1.0.0a7/wgse/mtDNA/RSRS.fasta`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -271,8 +271,8 @@
 ACTTGACCACCTGTAGTACATAAAAACCCAATCCACATCAAAACCCTCCCCCCATGCTTA
 CAAGCAAGTACAGCAATCAACCTTCAACTGTCACACATCAACTGCAACTCCAAAGCCACC
 CCTCACCCACTAGGATATCAACAAACCTACCCACCCTTAACAGTACATAGCACATAAAGC
 CATTTACCGTACATAGCACATTACAGTCAAATCCCTTCTCGTCCCCATGGATGACCCCCC
 TCAGATAGGGGTCCCTTGACCACCATCCTCCGTGAAATCAATATCCCGCACAAGAGTGCT
 ACTCTCCTCGCTCCGGGCCCATAACACTTGGGGGTAGCTAAAGTGAACTGTATCCGACAT
 CTGGTTCCTACTTCAGGGCCATAAAGCCTAAATAGCCCACACGTTCCCCTTAAATAAGAC
-ATCACGATG
+ATCACGATG
```

### Comparing `wgse_ng-1.0.0a5/wgse/mtDNA/Yoruba.fasta` & `wgse_ng-1.0.0a7/wgse/mtDNA/Yoruba.fasta`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -231,8 +231,8 @@
 CATGGGGAAGCAGATTTGGGTACCACCCAAGTATTGACTCACCCATCAACAACCGCTATGTATTTCGTAC
 ATTACTGCCAGCCACCATGAATATTGTACGGTACCATAAATACTTGACCACCTGTAGTACATAAAAACCC
 AACCCACATCAAACCCCCCCCCCCCATGCTTACAAGCAAGTACAGCAATCAACCTTCAACTATCACACAT
 CAACTGCAACTCCAAAGCCACCCCTCACCCACTAGGATACCAACAAACCTACCCACCCTTAACAGTACAT
 AGTACATAAAGTCATTTACCGTACATAGCACATTACAGTCAAATCCCTTCTCGTCCCCATGGATGACCCC
 CCTCAGATAGGGGTCCCTTGACCACCATCCTCCGTGAAATCAATATCCCGCACAAGAGTGCTACTCTCCT
 CGCTCCGGGCCCATAACACTTGGGGGTAGCTAAAGTGAACTGTATCCGACATCTGGTTCCTACTTCAGGG
-CCATAAAGCCTAAATAGCCCACACGTTCCCCTTAAATAAGACATCACGATG
+CCATAAAGCCTAAATAGCCCACACGTTCCCCTTAAATAAGACATCACGATG
```

### Comparing `wgse_ng-1.0.0a5/wgse/mtDNA/rCRS.fasta` & `wgse_ng-1.0.0a7/wgse/mtDNA/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a5/wgse/reference_genome/bgzip_compressor.py` & `wgse_ng-1.0.0a7/wgse/reference_genome/bgzip_compressor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from pathlib import Path
 
-from wgse.utility.external import External
 from wgse.reference_genome.genome_metadata_loader import Genome
+from wgse.utility.external import External
 from wgse.utility.file_type_checker import FileType, FileTypeChecker
 
 
 class BGZIPCompressor:
-    def __init__(self, external: External = External(), file_type_checker = FileTypeChecker()) -> None:
+    def __init__(
+        self, external: External = External(), file_type_checker=FileTypeChecker()
+    ) -> None:
         self._type_checker = file_type_checker
         self._external = external
 
     def perform(self, genome: Genome, file: Path) -> Path:
         if self._type_checker.get_type(file) == FileType.BGZIP:
             if genome.fasta != file:
                 if genome.fasta.exists():
                     genome.fasta.unlink()
                 file.rename(genome.fasta)
             return genome.fasta
-        return self._external.bgzip_wrapper(file, genome.fasta)
+        return self._external.bgzip_wrapper(file, genome.fasta)
```

### Comparing `wgse_ng-1.0.0a5/wgse/reference_genome/decompressor.py` & `wgse_ng-1.0.0a7/wgse/reference_genome/decompressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import hashlib
 import logging
 import shutil
 import typing
 import zipfile
 from pathlib import Path
 
-from wgse.utility.external import BgzipAction, External
 from wgse.reference_genome.genome_metadata_loader import Genome
-from wgse.utility.file_type_checker import FileTypeChecker, FileType
+from wgse.utility.external import BgzipAction, External
+from wgse.utility.file_type_checker import FileType, FileTypeChecker
 
 
 class Decompressor:
     def __init__(
         self,
         type_checker: FileTypeChecker = FileTypeChecker(),
         external: External = External(),
@@ -83,15 +83,15 @@
             if file.stat().st_size == genome.decompressed_size:
                 return False
         return True
 
     def perform(self, genome: Genome, downloaded: Path = None):
         if not self.decompression_needed(genome, downloaded):
             return downloaded
-        
+
         target = downloaded.with_suffix(".fa")
         if not self.decompression_needed(genome, target):
             return target
 
         if not downloaded.exists():
             raise FileNotFoundError(f"Unable to find file {downloaded.name}")
 
@@ -103,15 +103,17 @@
 
         handler = self._handlers[type]
         logging.debug(
             f"Decompressing {genome.fasta.name}. {type.name} compression detected."
         )
         handler(self, downloaded, target)
         if not target.exists():
-            raise RuntimeError(f"Error during the decompression of {str(genome)}. Decompressed file is not present.")
+            raise RuntimeError(
+                f"Error during the decompression of {str(genome)}. Decompressed file is not present."
+            )
 
         if genome.decompressed_size is None:
             genome.decompressed_size = target.stat().st_size
         elif genome.decompressed_size != target.stat().st_size:
             raise RuntimeError(
                 f"Error during the decompression of {str(genome)}. Size mismatch."
             )
```

### Comparing `wgse_ng-1.0.0a5/wgse/reference_genome/downloader.py` & `wgse_ng-1.0.0a7/wgse/reference_genome/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,33 +16,38 @@
 logging.getLogger("requests").setLevel(logging.WARNING)
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 logging.getLogger("google").setLevel(logging.WARNING)
 
 HANDLERS = {}
 SIZE_HANDLERS = {}
 
+
 def uri_handler(uri):
     def decorator(f):
         global HANDLERS
         HANDLERS[uri] = f
         return f
+
     return decorator
 
+
 def size_handler(uri):
     def decorator(f):
         global SIZE_HANDLERS
         SIZE_HANDLERS[uri] = f
         return f
+
     return decorator
 
+
 class Downloader:
-    
+
     def __init__(
         self,
-        config = MANAGER_CFG.REPOSITORY,
+        config=MANAGER_CFG.REPOSITORY,
         file_type_checker: FileTypeChecker = FileTypeChecker(),
     ) -> None:
         if file_type_checker is None:
             raise RuntimeError("FileTypeChecker cannot be None.")
 
         self._config = config
         self._progressbar = None
@@ -93,40 +98,40 @@
             file = Path(file)
             if file.stat().st_size == genome.download_size:
                 return file
         return target
 
     @size_handler("https://storage.cloud.google.com")
     @size_handler("gs://")
-    def size_google(self, genome : Genome):
-        chunk_size = 1024*1024
+    def size_google(self, genome: Genome):
+        chunk_size = 1024 * 1024
         storage_client = storage.Client.create_anonymous_client()
         uri = genome.fasta_url.strip()
         if not uri.startswith("gs://"):
-            uri = 'gs://' + uri.replace('https://storage.cloud.google.com/', '')
+            uri = "gs://" + uri.replace("https://storage.cloud.google.com/", "")
 
         blob = storage.Blob.from_string(uri, client=storage_client)
         blob.reload()
         return blob.size
 
     @uri_handler("https://storage.cloud.google.com")
     @uri_handler("gs://")
-    def download_google(self, genome : Genome, callback : any):
+    def download_google(self, genome: Genome, callback: any):
         storage_client = storage.Client.create_anonymous_client()
         uri = genome.fasta_url.strip()
         if not uri.startswith("gs://"):
-            uri = 'gs://' + uri.replace('https://storage.cloud.google.com/', '')
+            uri = "gs://" + uri.replace("https://storage.cloud.google.com/", "")
 
         blob = storage.Blob.from_string(uri, client=storage_client)
         blob.reload()
         if genome.download_size is None:
             genome.download_size = blob.size
-        
+
         target = self.pre_download_action(genome)
-        
+
         if target.exists():
             if target.stat().st_size == genome.download_size:
                 return self.post_download_action(genome, target)
 
         blob.download_to_filename(target)
         return self.post_download_action(genome, target)
 
@@ -162,17 +167,17 @@
         return self.download_pycurl(genome, callback)
 
     def download_pycurl(self, genome: Genome, callback: any):
         if genome.download_size is None:
             genome.download_size = self.get_file_size(genome.fasta_url)
             if genome.download_size == None:
                 raise RuntimeError(f"Unable to download file {genome.fasta_url}")
-        
+
         target = self.pre_download_action(genome)
-        
+
         resume_from = None
         if target.exists():
             if target.stat().st_size == genome.download_size:
                 return self.post_download_action(genome, target)
             else:
                 resume_from = target.stat().st_size
```

### Comparing `wgse_ng-1.0.0a5/wgse/reference_genome/genome_metadata_loader.py` & `wgse_ng-1.0.0a7/wgse/reference_genome/genome_metadata_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,19 @@
         FileNotFoundError: _description_
         FileNotFoundError: _description_
         FileNotFoundError: _description_
 
     Returns:
         _type_: _description_
     """
-    
+
     class _CircularReferenceEncoder(json.JSONEncoder):
         """Helps with the serialization of metadata, ensuring
         that is serialized only what's really needed."""
+
         def __init__(self, **kwargs) -> None:
             self.seen = set()
             super().__init__()
 
         def default(self, obj):
             if hasattr(obj, "__dict__"):
                 obj_dict = obj.__dict__.copy()
@@ -42,23 +43,20 @@
                         # process. Let's add to the seen set an object only if it is
                         # non trivial.
                         if hasattr(value, "__dict__"):
                             self.seen.add(id(value))
                 return {k: v for k, v in obj_dict.items() if not k.startswith("_")}
             return super().default(obj)
 
-    def __init__(
-        self,
-        config= MANAGER_CFG.REPOSITORY
-    ):
+    def __init__(self, config=MANAGER_CFG.REPOSITORY):
         self._config = config
         self.genome_root = self._config.genomes
         self.references_path = self._config.metadata.joinpath("references.json")
         self.sources_path = self._config.metadata.joinpath("sources.json")
-        
+
         if not self.genome_root.is_dir():
             raise FileNotFoundError(
                 f"Unable to find {str(self.genome_root)} or is not a directory."
             )
         if not self.references_path.is_file():
             raise FileNotFoundError(
                 f"Unable to find {str(self.references_path)} or is not a file."
@@ -110,8 +108,8 @@
     def save(self, source: typing.List[Genome]):
         with self.references_path.open("wt") as f:
             json.dump(
                 source,
                 f,
                 cls=GenomeMetadataLoader._CircularReferenceEncoder,
                 default=lambda o: o.__dict__,
-            )
+            )
```

### Comparing `wgse_ng-1.0.0a5/wgse/reference_genome/repository_manager.py` & `wgse_ng-1.0.0a7/wgse/reference_genome/repository_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 from collections import OrderedDict
 
 from wgse.alignment_map.alignment_map_header import AlignmentMapHeader
 from wgse.configuration import RepositoryConfig
 from wgse.data.genome import Genome
 from wgse.data.sequence import Sequence
-from wgse.utility.external import BgzipAction, External
 from wgse.fasta.reference import Reference
 from wgse.reference_genome.bgzip_compressor import BGZIPCompressor
 from wgse.reference_genome.decompressor import Decompressor
 from wgse.reference_genome.downloader import Downloader
 from wgse.reference_genome.genome_metadata_loader import GenomeMetadataLoader
+from wgse.utility.external import BgzipAction, External
 from wgse.utility.mt_dna import MtDNA
 from wgse.utility.sequence_orderer import SequenceOrderer
 
 
 class RepositoryManager:
     def __init__(
         self,
@@ -187,8 +187,8 @@
         logging.info(f"2/4: Decompressing: {download_output.name}.")
         decompressor_output = decompressor.perform(genome, download_output)
         logging.info(f"3/4: Compressing to gzip: {decompressor_output.name}.")
         compressor_output = compressor.perform(genome, decompressor_output)
         logging.info(f"4/4: Extracting sequence data: {compressor_output.name}.")
         self._create_companion_files(genome)
         genome.sequences = self._get_sequences(genome)
-        return genome
+        return genome
```

### Comparing `wgse_ng-1.0.0a5/wgse/renderers/html_aligned_file_report.py` & `wgse_ng-1.0.0a7/wgse/renderers/html_aligned_file_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from jinja2 import Environment, FileSystemLoader
 
 from wgse.adapters.alignment_map_file_info_adapter import AlignmentMapFileInfoAdapter
 from wgse.adapters.alignment_stats_adapter import AlignmentStatsAdapter
 from wgse.adapters.header_adapter import HeaderAdapter
 from wgse.adapters.index_stats_adapter import IndexStatsAdapter
 from wgse.alignment_map.alignment_map_file import AlignmentMapFile
-from wgse.alignment_map.alignment_map_header import AlignmentMapHeader
 from wgse.configuration import MANAGER_CFG
 from wgse.data.tabular_data import TabularData
-from wgse.VERSION import VERSION
+from wgse.VERSION import version
 
 
 class HTMLAlignedFileReport:
     def __init__(self, config=MANAGER_CFG.REPOSITORY) -> None:
         self._templates_folder = config.metadata.joinpath("report_templates")
 
     def from_aligned_file(file=AlignmentMapFile):
@@ -53,9 +52,9 @@
             file_info_data=file_info_data,
             index_stat_data=index_stat_data,
             alignment_stats_data=alignment_stats_data,
             sequences_data=sequences_data,
             read_groups_data=read_groups_data,
             programs_data=programs_data,
             comments_data=comments_data,
-            general={"now": datetime.datetime.now(), "version": VERSION},
+            general={"now": datetime.datetime.now(), "version": version},
         )
```

### Comparing `wgse_ng-1.0.0a5/wgse/renderers/html_simple_table_report.py` & `wgse_ng-1.0.0a7/wgse/renderers/html_simple_table_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from jinja2 import Environment, FileSystemLoader
+
 from wgse.configuration import MANAGER_CFG
 from wgse.data.tabular_data import TabularData
 
 
 class HTMLSimpleTableReport:
     def __init__(self, name, config=MANAGER_CFG.REPOSITORY) -> None:
         self._name = name
```

### Comparing `wgse_ng-1.0.0a5/wgse/utility/check_prerequisites.py` & `wgse_ng-1.0.0a7/wgse/utility/check_prerequisites.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import enum
 import inspect
 import logging
-from logging.handlers import TimedRotatingFileHandler
 import subprocess
-import wgse.utility.external
+from logging.handlers import TimedRotatingFileHandler
 from subprocess import Popen
 
+import wgse.utility.external
 from wgse.configuration import MANAGER_CFG
 from wgse.utility.external import External
 
 logger = logging.getLogger(__name__)
 
 
 class PrerequisiteIssueSeverity(enum.Enum):
@@ -52,26 +52,28 @@
     def _config_logging(self):
         if not self._repo.log_path.exists():
             self._repo.log_path.mkdir(parents=True, exist_ok=True)
         logger = logging.getLogger()
         logger.setLevel(logging.DEBUG)
         for handler in logger.handlers:
             logger.removeHandler(handler)
-            
+
         formatter = logging.Formatter(
             "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
         )
-        
+
         console_handler = logging.StreamHandler()
         console_handler.setLevel(logging.DEBUG)
         console_handler.setFormatter(formatter)
         logger.addHandler(console_handler)
 
-        log_file = self._repo.log_path.joinpath('app.log')
-        handler = TimedRotatingFileHandler(log_file, when='midnight', interval=1, backupCount=10)
+        log_file = self._repo.log_path.joinpath("app.log")
+        handler = TimedRotatingFileHandler(
+            log_file, when="midnight", interval=1, backupCount=10
+        )
         handler.suffix = "%Y-%m-%d"
         handler.setLevel(logging.DEBUG)
         handler.setFormatter(formatter)
         logger.addHandler(handler)
 
         return logger
```

### Comparing `wgse_ng-1.0.0a5/wgse/utility/external.py` & `wgse_ng-1.0.0a7/wgse/utility/external.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import shlex
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
 from wgse.configuration import MANAGER_CFG
+from wgse.utility.process_io_monitor import ProcessIOMonitor
 
 logger = logging.getLogger(__name__)
 
-if "win" in sys.platform:
+if sys.platform == "win32":
     third_party = str(MANAGER_CFG.EXTERNAL.root)
     if third_party not in os.environ["PATH"]:
         os.environ["PATH"] += ";" + third_party
     if ".JAR" not in os.environ["PATHEXT"]:
         os.environ["PATHEXT"] += ";.JAR"
 
 
@@ -31,28 +32,38 @@
     it's decorating, passing the arguments that were received when
     the function was invoked.
 
     Args:
         f (Callable): function to decorate.
     """
 
-    def execute_binary(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def execute_binary(
+        self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None
+    ):
         args = [*interpreter, shutil.which(f.__name__), *[str(x) for x in args]]
 
         if wait:
             # Force stdout/stderr to be PIPE as we
             # need to collect the output
             stdout = subprocess.PIPE
             stderr = subprocess.PIPE
         logger.debug(f"Calling: {shlex.join(args)}")
-        si=None
-        if "win" in sys.platform:
-            si = subprocess.STARTUPINFO()
-            si.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        output = subprocess.Popen(args, stdout=stdout, stdin=stdin, stderr=stderr, startupinfo=si)
+
+        # Force windows to hide the prompt window
+        startup_info = None
+        if sys.platform == "win32":
+            startup_info = subprocess.STARTUPINFO()
+            startup_info.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+
+        output = subprocess.Popen(
+            args, stdout=stdout, stdin=stdin, stderr=stderr, startupinfo=startup_info
+        )
+        if io is not None:
+            monitor = ProcessIOMonitor(output, io)
+            monitor.start()
         if wait == True:
             out, err = output.communicate()
             if output.returncode != 0:
                 raise RuntimeError(f"Call to {f.__name__} failed: {err.decode()}")
             return out
         return output
 
@@ -128,17 +139,17 @@
     def make_dictionary(self, path: Path, output: Path = None):
         if output is None:
             output = Path(path.parent, path.name + ".dict")
         arguments = [self._samtools, "dict", str(path), "-o", str(output)]
         process = subprocess.run(arguments, check=True, capture_output=True)
         return process.stdout.decode("utf-8")
 
-    def index(self, path: Path, wait=True):
+    def index(self, path: Path, wait=True, io=None):
         return self.samtools(
-            ["index", "-@", self._config.threads, "-b", str(path)], wait=wait
+            ["index", "-@", self._config.threads, "-b", str(path)], wait=wait, io=io
         )
 
     def _gzip_filename(self, input: Path, action: BgzipAction):
         if action == BgzipAction.Compress:
             return Path(str(input) + ".gz")
         elif action == BgzipAction.Decompress:
             if len(input.suffixes) == 0:
@@ -209,15 +220,17 @@
             inferred_filename.rename(output)
             if action == BgzipAction.Compress:
                 target = Path(str(output) + ".gzi")
                 inferred_gzi_filename = Path(str(inferred_filename) + ".gzi")
                 if target.exists():
                     target.unlink()
                 if not inferred_gzi_filename.exists():
-                    raise FileNotFoundError(f"BGZIP index not found for {inferred_gzi_filename.name}")
+                    raise FileNotFoundError(
+                        f"BGZIP index not found for {inferred_gzi_filename.name}"
+                    )
                 inferred_gzi_filename.rename(target)
         return output
 
     def idxstats(self, input: Path):
         """Generate BAM index statistics"""
         arguments = [self._samtools, "idxstat", input]
         process = subprocess.run(arguments)
@@ -233,53 +246,69 @@
 
     # Starting from here all the functions are
     # just calling executables with the same name.
     # See the implementation of @exe and @jar decorator
     # for more details.
 
     @exe
-    def bgzip(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def bgzip(self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None):
         raise FileNotFoundError()
 
     @exe
-    def samtools(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def samtools(
+        self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None
+    ):
         raise FileNotFoundError()
 
     @exe
-    def bwa(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def bwa(self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None):
         raise FileNotFoundError()
 
     @exe
-    def bwamem2(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def bwamem2(
+        self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None
+    ):
         raise FileNotFoundError()
 
     @exe
-    def minimap2(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def minimap2(
+        self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None
+    ):
         raise FileNotFoundError()
 
     @exe
-    def fastp(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def fastp(self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None):
         raise FileNotFoundError()
 
     @exe
-    def bcftools(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def bcftools(
+        self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None
+    ):
         raise FileNotFoundError()
 
     @exe
-    def tabix(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def tabix(self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None):
         raise FileNotFoundError()
 
     @jar
-    def haplogrep(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def haplogrep(
+        self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None
+    ):
         raise FileNotFoundError()
 
     @jar
-    def FastQC(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def FastQC(
+        self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None
+    ):
         raise FileNotFoundError()
 
     @jar
-    def picard(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def picard(
+        self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None
+    ):
         raise FileNotFoundError()
 
     @jar
-    def DISCVRSeq(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+    def DISCVRSeq(
+        self, args=[], stdout=None, stdin=None, stderr=None, wait=False, io=None
+    ):
         raise FileNotFoundError()
```

### Comparing `wgse_ng-1.0.0a5/wgse/utility/file_type_checker.py` & `wgse_ng-1.0.0a7/wgse/utility/file_type_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,34 +21,34 @@
         ".7z": FileType.SEVENZIP,
         ".zip": FileType.ZIP,
         ".bz2": FileType.BZIP,
         ".bz": FileType.BZIP,
         ".gz": FileType.RAZF_GZIP,
         ".fa": FileType.DECOMPRESSED,
         ".fasta": FileType.DECOMPRESSED,
-        ".fna": FileType.DECOMPRESSED
+        ".fna": FileType.DECOMPRESSED,
     }
-    
+
     _TYPE_TO_EXT = {
         FileType.SEVENZIP: ".7z",
-        FileType.ZIP : ".zip",
+        FileType.ZIP: ".zip",
         FileType.BZIP: ".bz2",
-        FileType.RAZF_GZIP:".fa.gz",
-        FileType.GZIP:".fa.gz",
-        FileType.DECOMPRESSED: ".fa"
+        FileType.RAZF_GZIP: ".fa.gz",
+        FileType.GZIP: ".fa.gz",
+        FileType.DECOMPRESSED: ".fa",
     }
 
     _HTSFILE_TO_TYPE = {
         "BGZF": FileType.BGZIP,
         "gzip": FileType.RAZF_GZIP,
         "RAZF": FileType.RAZF_GZIP,
         "FASTA": FileType.DECOMPRESSED,
     }
 
-    def __init__(self, external: External=External()) -> None:
+    def __init__(self, external: External = External()) -> None:
         self._external = external
 
     def get_type(self, file: Path) -> FileType:
         """Get a Type starting from a file path.
 
         Args:
             file (Path): Path of the file to analyze.
@@ -73,8 +73,8 @@
         return None
 
     def get_extension(self, file: Path) -> str:
         type = self.get_type(file)
         matches = [x for x in FileTypeChecker._EXT_TO_TYPE.items() if x[1] == type]
         if len(matches) > 0:
             return matches[0][0]
-        return None
+        return None
```

### Comparing `wgse_ng-1.0.0a5/wgse/utility/mt_dna.py` & `wgse_ng-1.0.0a7/wgse/utility/mt_dna.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
-from pathlib import Path
 import re
+from pathlib import Path
 
 from wgse.configuration import MANAGER_CFG
+from wgse.data.mitochondrial_model import MitochondrialModel
 from wgse.data.mitochondrial_model_type import MitochondrialModelType
 from wgse.data.sequence import Sequence
-from wgse.data.mitochondrial_model import MitochondrialModel
 
 
 class MtDNA:
     def __init__(
         self,
         config=MANAGER_CFG.REPOSITORY,
     ) -> None:
@@ -21,32 +21,30 @@
         with self._mtdna_json.open("rt") as p:
             json_models = json.load(p)
 
         models = []
         for model in json_models:
             sequence = Sequence(model["name"], int(model["length"]), model["md5"])
             model = MitochondrialModel(
-                sequence,
-                model["url"],
-                MitochondrialModelType[model["name"]]
+                sequence, model["url"], MitochondrialModelType[model["name"]]
             )
             models.append(model)
 
         return models
 
     def get_by_md5(self, md5):
         for model in self.data:
             if model.sequence.md5 == md5:
                 return model
         return None
 
-    def get_by_length(self, length:int):
+    def get_by_length(self, length: int):
         for model in self.data:
             if model.sequence.length == length:
                 return model
         return None
 
     def get_by_type(self, type):
         for model in self.data:
             if model.type == type:
                 return model
-        return None
+        return None
```

### Comparing `wgse_ng-1.0.0a5/wgse/utility/regions.py` & `wgse_ng-1.0.0a7/wgse/utility/regions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Flag, auto
+
 from wgse.configuration import MANAGER_CFG
 
 
 class RegionType(Flag):
     Y = auto()
     MT = auto()
     WES = auto()
```

### Comparing `wgse_ng-1.0.0a5/wgse/utility/sequence_orderer.py` & `wgse_ng-1.0.0a7/wgse/utility/sequence_orderer.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 
         Yields:
             Tuple[int, str]: Tuple containing the index in the
                 original sequence its converted name.
 
         """
         for sequence in self.ordered_sequences:
-            yield self.sequence_map[sequence], SequenceOrderer.convert(sequence, self.target)
+            yield self.sequence_map[sequence], SequenceOrderer.convert(
+                sequence, self.target
+            )
 
     def _get_ordered(self):
         autosome = self._get_autosome()
         sexual = self._get_sexual()
         mitochondrial = self._get_mitochondrial()
         others = self._get_others(autosome, sexual, mitochondrial)
         merged = [*autosome, *sexual, *mitochondrial, *others]
@@ -60,23 +62,25 @@
             if not is_autosome and not is_sexual and not is_mitochondrial:
                 others.append(sequence)
         others.sort()
         return others
 
     def canonicalize(sequence_name: str) -> str:
         return SequenceOrderer.convert(sequence_name, ChromosomeNameType.Number)
-    
-    def convert(input : str, target : ChromosomeNameType):
+
+    def convert(input: str, target: ChromosomeNameType):
         normalized = input.lower()
         if normalized.startswith("chr"):
             normalized = normalized.replace("chr", "", 1)
         if normalized.startswith("mt"):
             normalized = normalized.replace("mt", "m", 1)
         if target == ChromosomeNameType.Chr:
             if normalized.isnumeric() or normalized == "m":
                 return "chr" + normalized
             return normalized
         elif target == ChromosomeNameType.Number:
             return normalized
         elif target == ChromosomeNameType.Accession:
-            raise NotImplementedError("Converting to Accession is not supported at the moment.")
+            raise NotImplementedError(
+                "Converting to Accession is not supported at the moment."
+            )
         raise ValueError(f"Converting to unrecognized target format: {target.name}")
```

### Comparing `wgse_ng-1.0.0a5/wgse/utility/sequencers.py` & `wgse_ng-1.0.0a7/wgse/utility/sequencers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.coord_order = coord_order
         self.url = url
 
 
 class Sequencers:
     def __init__(
         self,
-        config = MANAGER_CFG.REPOSITORY,
+        config=MANAGER_CFG.REPOSITORY,
     ) -> None:
         self._config = config
         self.data = self._load()
 
     def _load(self):
         content = None
         sequencer = self._config.metadata.joinpath("sequencers.json")
```

### Comparing `wgse_ng-1.0.0a5/wgse/utility/updater.py` & `wgse_ng-1.0.0a7/wgse/utility/updater.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 import subprocess
 import sys
-from importlib.metadata import version 
+from importlib.metadata import version
 
 
 class Updater:
 
     def __init__(self) -> None:
         self.packages = ["WGSE-NG", "WGSE-NG-3rd-party"]
         # Package Name -> (Current v., Latest v.)
-        self.versions = {
-            x: (version(x), self.check(x))
-            for x in self.packages
-        }
+        self.versions = {x: (version(x), self.check(x)) for x in self.packages}
 
     def check(self, package_name):
         latest_version = subprocess.check_output(
             [sys.executable, "-m", "pip", "index", "versions", package_name]
         ).decode("utf-8")
         latest_version = latest_version.split("Version: ")[1].split("\n")[0]
         return latest_version
 
     def update(self, package_name, versions):
         subprocess.check_call(
             [sys.executable, "-m", "pip", "install", "--upgrade", package_name]
         )
-        print(
-            f"Upgraded {package_name} from {versions[0]} to {versions[1]}"
-        )
-        
+        print(f"Upgraded {package_name} from {versions[0]} to {versions[1]}")
+
         sys.exit()
 
+
 if __name__ == "__main__":
     a = Updater()
     pass
-
```

