# Comparing `tmp/wgse_ng-1.0.0a7.tar.gz` & `tmp/wgse_ng-1.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-1.0.0a7.tar", last modified: Tue May 21 06:02:43 2024, max compression
+gzip compressed data, was "wgse_ng-1.0.0a8.tar", last modified: Tue May 21 17:26:35 2024, max compression
```

## Comparing `wgse_ng-1.0.0a7.tar` & `wgse_ng-1.0.0a8.tar`

### file list

```diff
@@ -1,184 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.879788 wgse_ng-1.0.0a7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.887788 wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/add-a-new-reference.md
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.887788 wgse_ng-1.0.0a7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.github/workflows/python-pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.887788 wgse_ng-1.0.0a7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/WGSE_NG.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.891788 wgse_ng-1.0.0a7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/basic-usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/reference-genome.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/docs/wgse-library.md
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/main.spec
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.891788 wgse_ng-1.0.0a7/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   116407 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/fake_genome.fasta
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/test_unknown_bases_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/test/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.891788 wgse_ng-1.0.0a7/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/fake_reference_genome_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/import_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/last_file_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/tools/reference_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.891788 wgse_ng-1.0.0a7/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 06:02:43.000000 wgse_ng-1.0.0a7/wgse/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.895788 wgse_ng-1.0.0a7/wgse/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/alignment_map_file_info_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/alignment_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/header_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/index_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/adapters/reference_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.895788 wgse_ng-1.0.0a7/wgse/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/alignment_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/depth_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/alignment_map/index_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.899788 wgse_ng-1.0.0a7/wgse/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/alignment_map_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/alignment_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/chromosome_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/genome.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/mitochondrial_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/mitochondrial_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/mitochondrial_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/read_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/data/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.899788 wgse_ng-1.0.0a7/wgse/fasta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/fasta_letter_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/fasta_stats_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/letter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/letter_run_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fasta/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.899788 wgse_ng-1.0.0a7/wgse/fastq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/fastq/fastq_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.903788 wgse_ng-1.0.0a7/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/WGSE-NG.pyproject
--rw-r--r--   0 runner    (1001) docker     (127)    11778 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/WGSE-NG.pyproject.user
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.903788 wgse_ng-1.0.0a7/wgse/gui/extract/
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/extract/extract_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/extract/format_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/extract/microarray_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/extract/sequence_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/form.ui
--rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/reference.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.903788 wgse_ng-1.0.0a7/wgse/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67343 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/resources/logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   327118 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/resources/logo_nXP_icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/resources.qrc
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/gui/ui_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.911788 wgse_ng-1.0.0a7/wgse/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:33.000000 wgse_ng-1.0.0a7/wgse/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/
--rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/19_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/19_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/38_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/38_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/bed_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/builds.json
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/mtdna.json
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/ploidy.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4213157 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/references.json
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/references_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/metadata/report_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/report_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_macro.html
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_simple.html
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_tab.html
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/sequencers.json
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/metadata/sources.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/microarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/microarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/microarray/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/microarray/microarray_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/microarray/raw_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/mtDNA/
--rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/CRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/RSRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/Yoruba.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/mtDNA/rCRS.fasta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.923789 wgse_ng-1.0.0a7/wgse/reference_genome/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/bgzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/decompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/genome_metadata_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/reference_genome/repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/wgse/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/renderers/csv_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/renderers/html_aligned_file_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/renderers/html_simple_table_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:43.927789 wgse_ng-1.0.0a7/wgse/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/check_prerequisites.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/file_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/mt_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/process_io_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/sequence_orderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/sequencers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/shortcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/simple_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/unit_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/utility/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-21 06:02:34.000000 wgse_ng-1.0.0a7/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.653771 wgse_ng-1.0.0a8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.657771 wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/add-a-new-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.657771 wgse_ng-1.0.0a8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/workflows/python-pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.657771 wgse_ng-1.0.0a8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.661771 wgse_ng-1.0.0a8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/basic-usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/reference-genome.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/wgse-library.md
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/main.spec
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.661771 wgse_ng-1.0.0a8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116407 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/fake_genome.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_unknown_bases_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.661771 wgse_ng-1.0.0a8/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/fake_reference_genome_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/import_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/last_file_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/reference_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.665771 wgse_ng-1.0.0a8/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/wgse/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.665771 wgse_ng-1.0.0a8/wgse/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/alignment_map_file_info_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/alignment_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/header_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/index_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/reference_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.665771 wgse_ng-1.0.0a8/wgse/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/alignment_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/depth_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/index_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.669771 wgse_ng-1.0.0a8/wgse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.669771 wgse_ng-1.0.0a8/wgse/data/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_read_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/chromosome_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/mitochondrial_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/mitochondrial_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/mitochondrial_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/read_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.669771 wgse_ng-1.0.0a8/wgse/fasta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/fasta_letter_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/fasta_stats_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/letter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/letter_run_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.669771 wgse_ng-1.0.0a8/wgse/fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fastq/fastq_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.673771 wgse_ng-1.0.0a8/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/WGSE-NG.pyproject
+-rw-r--r--   0 runner    (1001) docker     (127)    11778 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/WGSE-NG.pyproject.user
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.673771 wgse_ng-1.0.0a8/wgse/gui/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/extract/extract_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/extract/format_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/extract/microarray_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/extract/sequence_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/form.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/reference.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.673771 wgse_ng-1.0.0a8/wgse/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67343 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/resources/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   327118 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/resources/logo_nXP_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/resources.qrc
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/ui_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.681771 wgse_ng-1.0.0a8/wgse/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.693771 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/19_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/19_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/38_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/38_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/builds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/mtdna.json
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/ploidy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4213157 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/references.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/references_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.693771 wgse_ng-1.0.0a8/wgse/metadata/report_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/report_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_macro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/sequencers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.693771 wgse_ng-1.0.0a8/wgse/microarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/microarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/microarray/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/microarray/microarray_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/microarray/raw_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.697771 wgse_ng-1.0.0a8/wgse/mtDNA/
+-rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/CRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/RSRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/Yoruba.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/rCRS.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.697771 wgse_ng-1.0.0a8/wgse/reference_genome/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/bgzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/genome_metadata_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.697771 wgse_ng-1.0.0a8/wgse/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/renderers/csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/renderers/html_aligned_file_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/renderers/html_simple_table_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/wgse/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/check_prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/file_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/mt_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/process_io_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/sequence_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/sequencers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/simple_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/unit_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/variant_caller.py
```

### Comparing `wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/bug_report.md` & `wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/.github/ISSUE_TEMPLATE/feature_request.md` & `wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/.github/workflows/python-app.yml` & `wgse_ng-1.0.0a8/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/.github/workflows/python-publish.yml` & `wgse_ng-1.0.0a8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/.vscode/settings.json` & `wgse_ng-1.0.0a8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/LICENSE` & `wgse_ng-1.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/PKG-INFO` & `wgse_ng-1.0.0a8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Whole Genome Sequencing data manipulation tool
 Author-email: Multiple <unavailable@wgse-ng.com>
 License: MIT License
         
         Copyright (c) 2024 chaplin89
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -73,33 +73,29 @@
 [PyPi Package](https://pypi.org/project/WGSE-NG/)
 
 ### Documentation
 - [Read the docs](https://wgse-ng.readthedocs.io/en/latest/) (pretty much empty at this point)
 
 ### Launch
 The only currently supported way to install `WGSE-NG` is with a pypi package.
-This require python and pip installed. The procedure is the same on every supported OSs. Note WGSE-NG is still in alpha state and many things are not working or they may broke unexpectedly.
+This require python and pip installed. The procedure is the same on every supported OSs. Note WGSE-NG is still in alpha state and many things are not working or they may broke unexpectedly. A long term goal is get a [pyinstaller]() executable/installer for each supported platform. As of today, the GitHub action is there but it build a broken executable (and is for windows only).
 
 ```bash
+sudo apt install libqt6waylandclient6 samtools bcftools -y # Only for Linux
 python -m pip install wgse-ng
 wgse
 ```
 
+NOTE: on Windows all the executables needed beside WGSE-NG are shipped with another PyPI package upon which WGSE-NG depends. Installing through `pip` is hence sufficient to get `wgse-ng` working. On Linux `wgse-ng` expects all the executables to be available under `PATH`, consequentely there may be dependencies that need to be installed manually. The snippet above provide the dependencies list for Ubuntu, on other distro the command may change.
+
 ### Development
 This section explain how to configure WGSE-NG for development.
 
 _Note: The best experience for developing is with [VS Code](https://code.visualstudio.com/) as this project already contains sensible settings for VS code._
 
-This repository uses [pre-commit](https://pre-commit.com/#intro) to ensure linting, formatting, and isort are executed before commit.
-Its usage is optional but highly recommended. To install
-```
-python -m pip install pre-commit
-pre-commit install
-```
-
 #### Windows
 ```bash
 git clone https://github.com/WGSE-NG/WGSE-NG
 cd WGSE-NG
 python -m venv .venv
 .venv\Scripts\activate
 python -m pip install -e .
@@ -112,14 +108,22 @@
 cd WGSE-NG
 python -m venv .venv
 source ./.venv/bin/activate
 python -m pip install -e .
 wgse
 ```
 
+#### pre-commit 
+This repository uses [pre-commit](https://pre-commit.com/#intro) to ensure linting, formatting, and isort are executed before commit.
+Its usage is optional but highly recommended. To install
+```
+python -m pip install pre-commit
+pre-commit install
+```
+
 ## Troubleshooting
 - **pyside6-uic not found** when launching a debug from the IDE: you should restart the IDE. pyside6-uic executable (installed from a python dependency to compile .ui files into python modules) may not be found by the IDE if you just installed the dependency from a terminal inside the IDE it without restarting it first.
 - **symbol lookup error** after launching WGSE from command line on Linux/WSL: likely your version of `libqt6waylandclient6` or one of its dependencies is too old and the python module for Qt is trying to fetch some symbols from it that were added in a subsequent version. You can try to run a `sudo apt update && sudo apt upgrade` but if that doesn't work unfortunately you need to upgrade the Qt version manually or use another distribution.
 
 ## What's working
 
 - [x] Basic file info extraction
```

### Comparing `wgse_ng-1.0.0a7/README.md` & `wgse_ng-1.0.0a8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,33 +13,29 @@
 [PyPi Package](https://pypi.org/project/WGSE-NG/)
 
 ### Documentation
 - [Read the docs](https://wgse-ng.readthedocs.io/en/latest/) (pretty much empty at this point)
 
 ### Launch
 The only currently supported way to install `WGSE-NG` is with a pypi package.
-This require python and pip installed. The procedure is the same on every supported OSs. Note WGSE-NG is still in alpha state and many things are not working or they may broke unexpectedly.
+This require python and pip installed. The procedure is the same on every supported OSs. Note WGSE-NG is still in alpha state and many things are not working or they may broke unexpectedly. A long term goal is get a [pyinstaller]() executable/installer for each supported platform. As of today, the GitHub action is there but it build a broken executable (and is for windows only).
 
 ```bash
+sudo apt install libqt6waylandclient6 samtools bcftools -y # Only for Linux
 python -m pip install wgse-ng
 wgse
 ```
 
+NOTE: on Windows all the executables needed beside WGSE-NG are shipped with another PyPI package upon which WGSE-NG depends. Installing through `pip` is hence sufficient to get `wgse-ng` working. On Linux `wgse-ng` expects all the executables to be available under `PATH`, consequentely there may be dependencies that need to be installed manually. The snippet above provide the dependencies list for Ubuntu, on other distro the command may change.
+
 ### Development
 This section explain how to configure WGSE-NG for development.
 
 _Note: The best experience for developing is with [VS Code](https://code.visualstudio.com/) as this project already contains sensible settings for VS code._
 
-This repository uses [pre-commit](https://pre-commit.com/#intro) to ensure linting, formatting, and isort are executed before commit.
-Its usage is optional but highly recommended. To install
-```
-python -m pip install pre-commit
-pre-commit install
-```
-
 #### Windows
 ```bash
 git clone https://github.com/WGSE-NG/WGSE-NG
 cd WGSE-NG
 python -m venv .venv
 .venv\Scripts\activate
 python -m pip install -e .
@@ -52,14 +48,22 @@
 cd WGSE-NG
 python -m venv .venv
 source ./.venv/bin/activate
 python -m pip install -e .
 wgse
 ```
 
+#### pre-commit 
+This repository uses [pre-commit](https://pre-commit.com/#intro) to ensure linting, formatting, and isort are executed before commit.
+Its usage is optional but highly recommended. To install
+```
+python -m pip install pre-commit
+pre-commit install
+```
+
 ## Troubleshooting
 - **pyside6-uic not found** when launching a debug from the IDE: you should restart the IDE. pyside6-uic executable (installed from a python dependency to compile .ui files into python modules) may not be found by the IDE if you just installed the dependency from a terminal inside the IDE it without restarting it first.
 - **symbol lookup error** after launching WGSE from command line on Linux/WSL: likely your version of `libqt6waylandclient6` or one of its dependencies is too old and the python module for Qt is trying to fetch some symbols from it that were added in a subsequent version. You can try to run a `sudo apt update && sudo apt upgrade` but if that doesn't work unfortunately you need to upgrade the Qt version manually or use another distribution.
 
 ## What's working
 
 - [x] Basic file info extraction
```

### Comparing `wgse_ng-1.0.0a7/WGSE_NG.egg-info/PKG-INFO` & `wgse_ng-1.0.0a8/WGSE_NG.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Whole Genome Sequencing data manipulation tool
 Author-email: Multiple <unavailable@wgse-ng.com>
 License: MIT License
         
         Copyright (c) 2024 chaplin89
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -73,33 +73,29 @@
 [PyPi Package](https://pypi.org/project/WGSE-NG/)
 
 ### Documentation
 - [Read the docs](https://wgse-ng.readthedocs.io/en/latest/) (pretty much empty at this point)
 
 ### Launch
 The only currently supported way to install `WGSE-NG` is with a pypi package.
-This require python and pip installed. The procedure is the same on every supported OSs. Note WGSE-NG is still in alpha state and many things are not working or they may broke unexpectedly.
+This require python and pip installed. The procedure is the same on every supported OSs. Note WGSE-NG is still in alpha state and many things are not working or they may broke unexpectedly. A long term goal is get a [pyinstaller]() executable/installer for each supported platform. As of today, the GitHub action is there but it build a broken executable (and is for windows only).
 
 ```bash
+sudo apt install libqt6waylandclient6 samtools bcftools -y # Only for Linux
 python -m pip install wgse-ng
 wgse
 ```
 
+NOTE: on Windows all the executables needed beside WGSE-NG are shipped with another PyPI package upon which WGSE-NG depends. Installing through `pip` is hence sufficient to get `wgse-ng` working. On Linux `wgse-ng` expects all the executables to be available under `PATH`, consequentely there may be dependencies that need to be installed manually. The snippet above provide the dependencies list for Ubuntu, on other distro the command may change.
+
 ### Development
 This section explain how to configure WGSE-NG for development.
 
 _Note: The best experience for developing is with [VS Code](https://code.visualstudio.com/) as this project already contains sensible settings for VS code._
 
-This repository uses [pre-commit](https://pre-commit.com/#intro) to ensure linting, formatting, and isort are executed before commit.
-Its usage is optional but highly recommended. To install
-```
-python -m pip install pre-commit
-pre-commit install
-```
-
 #### Windows
 ```bash
 git clone https://github.com/WGSE-NG/WGSE-NG
 cd WGSE-NG
 python -m venv .venv
 .venv\Scripts\activate
 python -m pip install -e .
@@ -112,14 +108,22 @@
 cd WGSE-NG
 python -m venv .venv
 source ./.venv/bin/activate
 python -m pip install -e .
 wgse
 ```
 
+#### pre-commit 
+This repository uses [pre-commit](https://pre-commit.com/#intro) to ensure linting, formatting, and isort are executed before commit.
+Its usage is optional but highly recommended. To install
+```
+python -m pip install pre-commit
+pre-commit install
+```
+
 ## Troubleshooting
 - **pyside6-uic not found** when launching a debug from the IDE: you should restart the IDE. pyside6-uic executable (installed from a python dependency to compile .ui files into python modules) may not be found by the IDE if you just installed the dependency from a terminal inside the IDE it without restarting it first.
 - **symbol lookup error** after launching WGSE from command line on Linux/WSL: likely your version of `libqt6waylandclient6` or one of its dependencies is too old and the python module for Qt is trying to fetch some symbols from it that were added in a subsequent version. You can try to run a `sudo apt update && sudo apt upgrade` but if that doesn't work unfortunately you need to upgrade the Qt version manually or use another distribution.
 
 ## What's working
 
 - [x] Basic file info extraction
```

### Comparing `wgse_ng-1.0.0a7/WGSE_NG.egg-info/SOURCES.txt` & `wgse_ng-1.0.0a8/WGSE_NG.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,17 +30,18 @@
 docs/requirements.txt
 docs/wgse-library.md
 test/__init__.py
 test/fake_genome.fasta
 test/test_buckets.py
 test/test_fasta.py
 test/test_fasta_dictionary.py
+test/test_letter_run_collection.py
 test/test_microarray_converter.py
 test/test_raw_file.py
-test/test_sequence.py
+test/test_reference.py
 test/test_unknown_bases_stats.py
 test/utility.py
 tools/__init__.py
 tools/fake_reference_genome_generator.py
 tools/import_scanner.py
 tools/last_file_export.py
 tools/reference_stats.py
@@ -59,15 +60,14 @@
 wgse/alignment_map/alignment_map_file.py
 wgse/alignment_map/alignment_map_header.py
 wgse/alignment_map/alignment_map_row.py
 wgse/alignment_map/alignment_stats_calculator.py
 wgse/alignment_map/depth_analyzer.py
 wgse/alignment_map/index_stats_calculator.py
 wgse/data/__init__.py
-wgse/data/alignment_map_file_info.py
 wgse/data/alignment_stats.py
 wgse/data/build.py
 wgse/data/chromosome_name_type.py
 wgse/data/file_type.py
 wgse/data/gender.py
 wgse/data/genome.py
 wgse/data/microarray_converter.py
@@ -76,14 +76,19 @@
 wgse/data/mitochondrial_name_type.py
 wgse/data/read_type.py
 wgse/data/sequence.py
 wgse/data/sequence_type.py
 wgse/data/sorting.py
 wgse/data/source.py
 wgse/data/tabular_data.py
+wgse/data/alignment_map/alignment_map_file_info.py
+wgse/data/alignment_map/alignment_map_header_metadata.py
+wgse/data/alignment_map/alignment_map_header_program.py
+wgse/data/alignment_map/alignment_map_header_read_group.py
+wgse/data/alignment_map/alignment_map_header_sequence.py
 wgse/fasta/__init__.py
 wgse/fasta/fasta_letter_counter.py
 wgse/fasta/fasta_stats_files.py
 wgse/fasta/letter_run.py
 wgse/fasta/letter_run_buckets.py
 wgse/fasta/letter_run_collection.py
 wgse/fasta/reference.py
```

### Comparing `wgse_ng-1.0.0a7/docs/Makefile` & `wgse_ng-1.0.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/docs/basic-usage.md` & `wgse_ng-1.0.0a8/docs/basic-usage.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/docs/conf.py` & `wgse_ng-1.0.0a8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/docs/make.bat` & `wgse_ng-1.0.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/docs/reference-genome.md` & `wgse_ng-1.0.0a8/docs/reference-genome.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/docs/requirements.txt` & `wgse_ng-1.0.0a8/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/main.spec` & `wgse_ng-1.0.0a8/main.spec`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/pyproject.toml` & `wgse_ng-1.0.0a8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/test/fake_genome.fasta` & `wgse_ng-1.0.0a8/test/fake_genome.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/test/test_buckets.py` & `wgse_ng-1.0.0a8/test/test_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/test/test_fasta.py` & `wgse_ng-1.0.0a8/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/test/test_fasta_dictionary.py` & `wgse_ng-1.0.0a8/test/test_fasta_dictionary.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/test/test_microarray_converter.py` & `wgse_ng-1.0.0a8/test/test_microarray_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from pathlib import Path
 from test.test_fasta import MockPath
-from test.utility import MockFile
-from unittest.mock import patch
 
 import pytest
 
 from wgse.configuration import RepositoryConfig
-from wgse.data.microarray_converter import MicroarrayConverterTarget
 from wgse.microarray.microarray_converter import MicroarrayConverter
-from wgse.microarray.microarray_line_formatter import TARGET_FORMATTER_MAP
 
 # def test_every_target_has_formatter():
 #     assert all(x in TARGET_FORMATTER_MAP for x in MicroarrayConverterTarget)
 
 
 def test_inexistent_head_folder_raise():
     config = RepositoryConfig()
```

### Comparing `wgse_ng-1.0.0a7/test/test_raw_file.py` & `wgse_ng-1.0.0a8/test/test_raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/test/test_sequence.py` & `wgse_ng-1.0.0a8/test/test_letter_run_collection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/test/test_unknown_bases_stats.py` & `wgse_ng-1.0.0a8/test/test_unknown_bases_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/test/utility.py` & `wgse_ng-1.0.0a8/test/utility.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/tools/fake_reference_genome_generator.py` & `wgse_ng-1.0.0a8/tools/fake_reference_genome_generator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/tools/import_scanner.py` & `wgse_ng-1.0.0a8/tools/import_scanner.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/tools/last_file_export.py` & `wgse_ng-1.0.0a8/tools/last_file_export.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/tools/reference_stats.py` & `wgse_ng-1.0.0a8/tools/reference_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/__init__.py` & `wgse_ng-1.0.0a8/wgse/__init__.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/adapters/alignment_map_file_info_adapter.py` & `wgse_ng-1.0.0a8/wgse/adapters/alignment_map_file_info_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wgse.data.alignment_map_file_info import AlignmentMapFileInfo
+from wgse.data.alignment_map.alignment_map_file_info import AlignmentMapFileInfo
 from wgse.data.tabular_data import TabularData, TabularDataRow
 
 
 class AlignmentMapFileInfoAdapter:
     def adapt(stats: AlignmentMapFileInfo):
         label_map = {
             "path": "Path",
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

### Comparing `wgse_ng-1.0.0a7/wgse/adapters/alignment_stats_adapter.py` & `wgse_ng-1.0.0a8/wgse/adapters/alignment_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/adapters/header_adapter.py` & `wgse_ng-1.0.0a8/wgse/adapters/header_adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from wgse.alignment_map.alignment_map_header import (
-    AlignmentMapHeader,
+from wgse.alignment_map.alignment_map_header import AlignmentMapHeader
+from wgse.data.alignment_map.alignment_map_header_program import (
     AlignmentMapHeaderProgram,
+)
+from wgse.data.alignment_map.alignment_map_header_read_group import (
     AlignmentMapHeaderReadGroup,
+)
+from wgse.data.alignment_map.alignment_map_header_sequence import (
     AlignmentMapHeaderSequence,
 )
 from wgse.data.tabular_data import TabularData, TabularDataRow
 
 
 class HeaderSequenceAdapter:
     def adapt(input_data: list[AlignmentMapHeaderSequence]):
```

### Comparing `wgse_ng-1.0.0a7/wgse/adapters/index_stats_adapter.py` & `wgse_ng-1.0.0a8/wgse/adapters/index_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/adapters/reference_adapter.py` & `wgse_ng-1.0.0a8/wgse/adapters/reference_adapter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from wgse.alignment_map.index_stats_calculator import SequenceStatistics
-from wgse.data.sequence_type import SequenceType
 from wgse.data.tabular_data import TabularData, TabularDataRow
 from wgse.fasta.reference import Reference
 
 
 class ReferenceAdapter:
     def adapt(stats: Reference):
         # We've at least a match, build a table with it
```

### Comparing `wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_file.py` & `wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from wgse.alignment_map.alignment_map_header import AlignmentMapHeader
 from wgse.alignment_map.alignment_stats_calculator import AlignmentStatsCalculator
 from wgse.alignment_map.index_stats_calculator import (
     IndexStatsCalculator,
     SequenceStatistics,
 )
 from wgse.configuration import MANAGER_CFG
-from wgse.data.alignment_map_file_info import AlignmentMapFileInfo
+from wgse.data.alignment_map.alignment_map_file_info import AlignmentMapFileInfo
 from wgse.data.file_type import FileType
 from wgse.data.gender import Gender
 from wgse.data.mitochondrial_model_type import MitochondrialModelType
 from wgse.data.sequence_type import SequenceType
 from wgse.data.sorting import Sorting
 from wgse.fasta.reference import Reference
 from wgse.reference_genome.repository_manager import RepositoryManager
```

### Comparing `wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_header.py` & `wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_header.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,29 @@
 import logging
 import typing
 from collections import OrderedDict
 from pathlib import Path
 
+from wgse.data.alignment_map.alignment_map_header_metadata import (
+    AlignmentMapHeaderMetadata,
+)
+from wgse.data.alignment_map.alignment_map_header_program import (
+    AlignmentMapHeaderProgram,
+)
+from wgse.data.alignment_map.alignment_map_header_read_group import (
+    AlignmentMapHeaderReadGroup,
+)
+from wgse.data.alignment_map.alignment_map_header_sequence import (
+    AlignmentMapHeaderSequence,
+)
 from wgse.data.chromosome_name_type import ChromosomeNameType
 from wgse.data.mitochondrial_name_type import MitochondrialNameType
 from wgse.data.sorting import Sorting
 
 
-class AlignmentMapHeaderProgram:
-    def __init__(self) -> None:
-        self.id: str = None
-        self.name: str = None
-        self.command_line: str = None
-        self.previous: AlignmentMapHeaderProgram = None
-        self.description: str = None
-        self.program_version: str = None
-
-
-class AlignmentMapHeaderSequence:
-    def __init__(self) -> None:
-        self.name: str = None
-        self.length: int = None
-        self.md5: str = None
-        self.uri: str = None
-        self.alternate_locus: str = None
-        self.molecule_topology: str = None
-        self.species: str = None
-        self.alternative_names: str = None
-        self.genome_assembly_identifier: str = None
-        self.description: str = None
-
-    def __str__(self) -> str:
-        return f"{self.name}: Length {self.length}bp, MD5: {self.md5}"
-
-    def __repr__(self) -> str:
-        return self.__str__()
-
-
-class AlignmentMapHeaderReadGroup:
-    def __init__(self) -> None:
-        self.id: str = None
-        self.barcode: str = None
-        self.sequencing_center: str = None
-        self.description: str = None
-        self.date: str = None
-        self.flow_order: str = None
-        self.key_sequence: str = None
-        self.library: str = None
-        self.programs: str = None
-        self.predicted_median_insert_size: int = None
-        self.platform: str = None
-        self.platform_model: str = None
-        self.platform_unit: str = None
-        self.sample: str = None
-
-
-class AlignmentMapHeaderMetadata:
-    def __init__(self) -> None:
-        self.version: str = None
-        self.sorted: Sorting = None
-        self.grouping: str = None
-        self.subsorting: str = None
-
-
 class AlignmentMapHeader:
     """Parse the output from `samtools view -H`"""
 
     def __init__(self, lines) -> None:
         self.metadata = None
         self.sequences: OrderedDict[str, AlignmentMapHeaderSequence] = OrderedDict()
         self.programs: list[AlignmentMapHeaderProgram] = []
```

### Comparing `wgse_ng-1.0.0a7/wgse/alignment_map/alignment_map_row.py` & `wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_row.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/alignment_map/alignment_stats_calculator.py` & `wgse_ng-1.0.0a8/wgse/alignment_map/alignment_stats_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import logging
 import subprocess
 from math import sqrt
 
 from wgse.alignment_map.alignment_map_row import AlignmentMapFlag, AlignmentMapRow
 from wgse.configuration import MANAGER_CFG
-from wgse.data.alignment_map_file_info import AlignmentMapFileInfo
+from wgse.data.alignment_map.alignment_map_file_info import AlignmentMapFileInfo
 from wgse.data.alignment_stats import AlignmentStats
 from wgse.data.file_type import FileType
 from wgse.data.read_type import ReadType
 from wgse.utility.external import External
 from wgse.utility.sequencers import Sequencers
 
-logger = logging.getLogger(__name__)
-
 
 class AlignmentStatsCalculator:
     def __init__(
         self,
         path: AlignmentMapFileInfo,
         config=MANAGER_CFG.ALIGNMENT_STATS,
         external: External = External(),
         sequencers: Sequencers = Sequencers(),
+        logger=logging.getLogger(__name__),
     ) -> None:
         self.aligned_file = path
         self._config = config
         self._external = external
         self._sequencers = sequencers
+        self._logger = logger
 
     def get_stats(self):
         samples = self._read_samples(self._config.skip, self._config.samples)
         stats = self._process_samples(samples)
         # TODO: handle long reads
         return stats
 
@@ -68,15 +68,15 @@
             AlignmentMapFlag.DUPLICATE,
             AlignmentMapFlag.SUPPLEMENTARY_ALIGNMENT,
         ]
         read_type_count = 0
         considered_samples = 0
 
         if len(samples) == 0:
-            logger.error("Cannot compute alignment stats as the file is empty")
+            self._logger.error("Cannot compute alignment stats as the file is empty")
             return
 
         # Process the template name for 1st sample to determine the sequencer
         # as it should not give a different result on the other samples.
         sequencer = self._sequencers.determine_sequencer(samples[0].query_template_name)
 
         # Used to compute stats for read length
@@ -142,30 +142,30 @@
         read_type = ReadType.Unknown
         if read_type_count > majority:
             read_type = ReadType.Paired
         elif read_type_count < -majority:
             read_type = ReadType.Single
 
         if count_length <= 2:
-            logger.error(
+            self._logger.error(
                 "Unable to compute read length stats as the number of valid samples is less than 2."
             )
             return None
         if count_insert_size <= 2 and read_type == ReadType.Paired:
-            logger.error(
+            self._logger.error(
                 "Unable to compute insert size stats as the number of valid samples is less than 2."
             )
             return None
         if count_quality <= 2:
-            logger.error(
+            self._logger.error(
                 "Unable to compute alignment quality stats as the number of valid samples is less than 2."
             )
             return None
         if read_type == ReadType.Unknown:
-            logger.error(
+            self._logger.error(
                 "Unable to determine read type as there's a similar number of single vs paired reads."
             )
             return None
 
         stats = AlignmentStats()
         stats.samples_count = self._config.samples
         stats.skipped_samples = self._config.skip
```

### Comparing `wgse_ng-1.0.0a7/wgse/alignment_map/depth_analyzer.py` & `wgse_ng-1.0.0a8/wgse/alignment_map/depth_analyzer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/alignment_map/index_stats_calculator.py` & `wgse_ng-1.0.0a8/wgse/alignment_map/index_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/configuration.py` & `wgse_ng-1.0.0a8/wgse/configuration.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/data/alignment_map_file_info.py` & `wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_file_info.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/data/alignment_stats.py` & `wgse_ng-1.0.0a8/wgse/data/alignment_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/data/genome.py` & `wgse_ng-1.0.0a8/wgse/data/genome.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/data/microarray_converter.py` & `wgse_ng-1.0.0a8/wgse/data/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/data/mitochondrial_model.py` & `wgse_ng-1.0.0a8/wgse/data/mitochondrial_model.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/data/sequence.py` & `wgse_ng-1.0.0a8/wgse/data/sequence.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 class Sequence:
-    def __init__(self, name: str, length: int, md5: str = None) -> None:
+    def __init__(self, name: str, length: int, md5: str = None, parent=None) -> None:
         self.name = name
         self.length = length
         self.md5 = md5
-        self.__parent = None
+        self.__parent = parent
 
     @property
     def parent(self):
         return self.__parent
 
     @parent.setter
     def parent(self, value):
         self.__parent = value
 
+    @property
+    def type(self):
+        pass
+
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
         return f"{self.name}: Length: {self.length}bp, MD5: {self.md5}"
```

### Comparing `wgse_ng-1.0.0a7/wgse/fasta/fasta_letter_counter.py` & `wgse_ng-1.0.0a8/wgse/fasta/fasta_letter_counter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/fasta/fasta_stats_files.py` & `wgse_ng-1.0.0a8/wgse/fasta/fasta_stats_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python3
-# coding: utf8
 import csv
 import logging
 import math
 import statistics
 import typing
 from pathlib import Path
 
@@ -121,13 +119,11 @@
         self._generate_file(self._fasta_file.genome.bed, self.save_bed(sequences))
         self._generate_file(self._fasta_file.genome.nbin, self.save_nbin(sequences))
 
     def _load_files(self):
         pass
 
     def generate_stats(self):
-        logging.info(f"{self._fasta_file.genome.final_name.name}: Counting Ns.")
+        logging.info(f"{self._fasta_file.genome!s}: Counting Ns.")
         sequences = self._fasta_file.count_letters("N")
-        logging.info(
-            f"{self._fasta_file.genome.final_name.name}: Finished counting Ns."
-        )
+        logging.info(f"{self._fasta_file.genome!s}: Finished counting Ns.")
         self._generate_files(sequences)
```

### Comparing `wgse_ng-1.0.0a7/wgse/fasta/letter_run_buckets.py` & `wgse_ng-1.0.0a8/wgse/fasta/letter_run_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/fasta/letter_run_collection.py` & `wgse_ng-1.0.0a8/wgse/fasta/letter_run_collection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/fasta/reference.py` & `wgse_ng-1.0.0a8/wgse/fasta/reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import enum
 import logging
 from collections import OrderedDict
 
 from wgse.data.genome import Genome
 from wgse.data.sequence import Sequence
 
-logger = logging.getLogger(__name__)
-
 
 class ReferenceStatus(enum.Enum):
     Available = enum.auto()
     Downloadable = enum.auto()
     Buildable = enum.auto()
     Unknown = enum.auto()
 
 
 class Reference:
     """This class represent a reference genome."""
 
-    def __init__(self, reference_map: OrderedDict[Sequence, list[Sequence]]):
+    def __init__(
+        self,
+        reference_map: OrderedDict[Sequence, list[Sequence]],
+        logger=logging.getLogger(__name__),
+    ):
+        self._logger = logger
         self.reference_map = reference_map
         self._genome_map = self._index_by_genome()
         self.matching: list[Genome] = self._get_matching_genomes()
         self.build = set(x.build for x in self.matching)
         if len(self.build) > 1:
-            logger.warn(
+            self._logger.warn(
                 "Found more than one valid builds for the reference of the file. "
                 + "This is likely an issue with the reference genome metadata. "
                 + "Please open a bug report."
             )
         self.build = " ".join(self.build)
         self.ready_reference = None
         for match in self.matching:
@@ -104,15 +107,15 @@
                     if genome_sequence.md5 != query_sequence.md5:
                         matching = False
                         break
                 if query_sequence.length != query_sequence.length:
                     matching = False
                     break
             if matching:
-                logger.info(f"{genome!s} is a perfect match.")
+                self._logger.info(f"{genome!s} is a perfect match.")
                 match_list.append(genome)
         return match_list
 
     def __str__(self) -> str:
         return f"{self.build} ({self.status.name})"
 
     def __repr__(self) -> str:
```

### Comparing `wgse_ng-1.0.0a7/wgse/fastq/fastq_file.py` & `wgse_ng-1.0.0a8/wgse/fastq/fastq_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/WGSE-NG.pyproject.user` & `wgse_ng-1.0.0a8/wgse/gui/WGSE-NG.pyproject.user`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/extract/extract_wizard.py` & `wgse_ng-1.0.0a8/wgse/gui/extract/extract_wizard.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/extract/format_selection.py` & `wgse_ng-1.0.0a8/wgse/gui/extract/format_selection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/extract/microarray_selection.py` & `wgse_ng-1.0.0a8/wgse/gui/extract/microarray_selection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/extract/sequence_selection.py` & `wgse_ng-1.0.0a8/wgse/gui/extract/sequence_selection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/form.ui` & `wgse_ng-1.0.0a8/wgse/gui/form.ui`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/main.py` & `wgse_ng-1.0.0a8/wgse/gui/main.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/reference.ui` & `wgse_ng-1.0.0a8/wgse/gui/reference.ui`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/resources/logo.jpg` & `wgse_ng-1.0.0a8/wgse/gui/resources/logo.jpg`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/resources/logo_nXP_icon.ico` & `wgse_ng-1.0.0a8/wgse/gui/resources/logo_nXP_icon.ico`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/table_dialog.py` & `wgse_ng-1.0.0a8/wgse/gui/table_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/gui/ui_form.py` & `wgse_ng-1.0.0a8/wgse/gui/ui_form.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/bed_templates/19_wes.csv` & `wgse_ng-1.0.0a8/wgse/metadata/bed_templates/19_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/bed_templates/38_wes.csv` & `wgse_ng-1.0.0a8/wgse/metadata/bed_templates/38_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/bed_templates/38_y_mt.csv` & `wgse_ng-1.0.0a8/wgse/metadata/bed_templates/38_y_mt.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/mtdna.json` & `wgse_ng-1.0.0a8/wgse/metadata/mtdna.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/references.json` & `wgse_ng-1.0.0a8/wgse/metadata/references.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/references_template.json` & `wgse_ng-1.0.0a8/wgse/metadata/references_template.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_macro.html` & `wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_macro.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_simple.html` & `wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_simple.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/report_templates/table_tab.html` & `wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_tab.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/sequencers.json` & `wgse_ng-1.0.0a8/wgse/metadata/sequencers.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/metadata/sources.json` & `wgse_ng-1.0.0a8/wgse/metadata/sources.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/microarray/microarray_converter.py` & `wgse_ng-1.0.0a8/wgse/microarray/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/microarray/microarray_line_formatter.py` & `wgse_ng-1.0.0a8/wgse/microarray/microarray_line_formatter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/microarray/raw_file.py` & `wgse_ng-1.0.0a8/wgse/microarray/raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/mtDNA/CRS.fasta` & `wgse_ng-1.0.0a8/wgse/mtDNA/CRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/mtDNA/RSRS.fasta` & `wgse_ng-1.0.0a8/wgse/mtDNA/RSRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/mtDNA/Yoruba.fasta` & `wgse_ng-1.0.0a8/wgse/mtDNA/Yoruba.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/mtDNA/rCRS.fasta` & `wgse_ng-1.0.0a8/wgse/mtDNA/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/reference_genome/bgzip_compressor.py` & `wgse_ng-1.0.0a8/wgse/reference_genome/bgzip_compressor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/reference_genome/decompressor.py` & `wgse_ng-1.0.0a8/wgse/reference_genome/decompressor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/reference_genome/downloader.py` & `wgse_ng-1.0.0a8/wgse/reference_genome/downloader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/reference_genome/genome_metadata_loader.py` & `wgse_ng-1.0.0a8/wgse/reference_genome/genome_metadata_loader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/reference_genome/repository_manager.py` & `wgse_ng-1.0.0a8/wgse/reference_genome/repository_manager.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/renderers/html_aligned_file_report.py` & `wgse_ng-1.0.0a8/wgse/renderers/html_aligned_file_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/renderers/html_simple_table_report.py` & `wgse_ng-1.0.0a8/wgse/renderers/html_simple_table_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/check_prerequisites.py` & `wgse_ng-1.0.0a8/wgse/utility/check_prerequisites.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/external.py` & `wgse_ng-1.0.0a8/wgse/utility/external.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/file_type_checker.py` & `wgse_ng-1.0.0a8/wgse/utility/file_type_checker.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/mt_dna.py` & `wgse_ng-1.0.0a8/wgse/utility/mt_dna.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/process_io_monitor.py` & `wgse_ng-1.0.0a8/wgse/utility/process_io_monitor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/regions.py` & `wgse_ng-1.0.0a8/wgse/utility/regions.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/sequence_orderer.py` & `wgse_ng-1.0.0a8/wgse/utility/sequence_orderer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/sequencers.py` & `wgse_ng-1.0.0a8/wgse/utility/sequencers.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/shortcut.py` & `wgse_ng-1.0.0a8/wgse/utility/shortcut.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/simple_worker.py` & `wgse_ng-1.0.0a8/wgse/utility/simple_worker.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/utility/updater.py` & `wgse_ng-1.0.0a8/wgse/utility/updater.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a7/wgse/variant_caller.py` & `wgse_ng-1.0.0a8/wgse/variant_caller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import enum
 import logging
 import shlex
 import subprocess
 
 from wgse.alignment_map.alignment_map_file import AlignmentMapFile
 from wgse.configuration import MANAGER_CFG
-from wgse.data.sequence_type import SequenceType
 from wgse.utility.external import External
-from wgse.utility.process_io_monitor import ProcessIOMonitor
-
-logger = logging.getLogger(__name__)
 
 
 class VariantCallingType(enum.Enum):
     InDel = enum.auto()
     SNP = enum.auto()
     Both = enum.auto()
 
@@ -21,30 +17,32 @@
 class VariantCaller:
     def __init__(
         self,
         repo_config=MANAGER_CFG.REPOSITORY,
         ext_config=MANAGER_CFG.EXTERNAL,
         external: External = External(),
         progress=None,
+        logger=logging.getLogger(__name__),
     ) -> None:
         self._external = external
         self._ext_config = ext_config
         self._ploidy = str(repo_config.metadata.joinpath("ploidy.txt"))
         self._is_quitting = False
         self._current_operation = None
         self._progress = progress
+        self._logger = logger
 
     def call(self, aligned_file: AlignmentMapFile, type=VariantCallingType.Both):
         if aligned_file.file_info.index_stats is None:
             raise RuntimeError("Index stats cannot be None for variant calling")
         if aligned_file.file_info.reference_genome.ready_reference is None:
             raise RuntimeError("Reference cannot be None for variant calling")
         self.current_file = aligned_file
         reference = str(aligned_file.file_info.reference_genome.ready_reference.fasta)
-        logger.info(
+        self._logger.info(
             f"Calling variants with {aligned_file.file_info.reference_genome.ready_reference}"
         )
         input_file = aligned_file.path
 
         skip_variant_opt = ""
         if type == VariantCallingType.InDel:
             skip_variant_opt = "-V snps"
```

