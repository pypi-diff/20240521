# Comparing `tmp/ont-bonito-0.7.3.tar.gz` & `tmp/ont-bonito-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ont-bonito-0.7.3.tar", last modified: Tue Dec 12 17:14:02 2023, max compression
+gzip compressed data, was "ont-bonito-0.8.1.tar", last modified: Tue May 21 15:20:47 2024, max compression
```

## Comparing `ont-bonito-0.7.3.tar` & `ont-bonito-0.8.1.tar`

### file list

```diff
@@ -1,58 +1,63 @@
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.307775 ont-bonito-0.7.3/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    14470 2023-09-28 14:20:31.000000 ont-bonito-0.7.3/LICENCE.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      179 2023-09-28 14:20:31.000000 ont-bonito-0.7.3/MANIFEST.in
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5024 2023-12-12 17:14:02.303879 ont-bonito-0.7.3/PKG-INFO
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4772 2023-09-28 21:11:43.000000 ont-bonito-0.7.3/README.md
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.188202 ont-bonito-0.7.3/bonito/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      937 2023-12-12 17:13:00.000000 ont-bonito-0.7.3/bonito/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       31 2023-09-28 21:11:43.000000 ont-bonito-0.7.3/bonito/__main__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1550 2022-01-09 17:00:34.000000 ont-bonito-0.7.3/bonito/aligner.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.224398 ont-bonito-0.7.3/bonito/cli/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)        0 2021-10-27 17:31:47.000000 ont-bonito-0.7.3/bonito/cli/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     8361 2023-12-12 17:08:45.000000 ont-bonito-0.7.3/bonito/cli/basecaller.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5152 2023-09-28 21:11:43.000000 ont-bonito-0.7.3/bonito/cli/convert.py
--rwxr-xr-x   0 cseymour  (5744) domain users  (1113)     5002 2023-12-12 17:08:45.000000 ont-bonito-0.7.3/bonito/cli/download.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    12570 2023-04-01 22:07:04.000000 ont-bonito-0.7.3/bonito/cli/duplex.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     3647 2022-02-13 12:34:47.000000 ont-bonito-0.7.3/bonito/cli/evaluate.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     6898 2023-09-30 19:04:38.000000 ont-bonito-0.7.3/bonito/cli/export.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4704 2023-05-05 09:40:35.000000 ont-bonito-0.7.3/bonito/cli/train.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      567 2021-10-27 17:31:47.000000 ont-bonito-0.7.3/bonito/cli/view.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.234826 ont-bonito-0.7.3/bonito/crf/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.3/bonito/crf/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     2632 2023-10-03 11:51:54.000000 ont-bonito-0.7.3/bonito/crf/basecall.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    10057 2023-12-12 17:08:45.000000 ont-bonito-0.7.3/bonito/crf/model.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.244324 ont-bonito-0.7.3/bonito/ctc/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.3/bonito/ctc/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     2018 2022-02-13 12:34:47.000000 ont-bonito-0.7.3/bonito/ctc/basecall.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     7110 2022-11-17 14:06:33.000000 ont-bonito-0.7.3/bonito/ctc/model.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.248400 ont-bonito-0.7.3/bonito/data/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       95 2021-10-27 17:31:47.000000 ont-bonito-0.7.3/bonito/data/README.md
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     2868 2023-04-01 22:07:04.000000 ont-bonito-0.7.3/bonito/data.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     6829 2023-12-12 17:08:45.000000 ont-bonito-0.7.3/bonito/fast5.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    19373 2023-04-03 09:38:52.000000 ont-bonito-0.7.3/bonito/io.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     3249 2023-09-28 21:11:43.000000 ont-bonito-0.7.3/bonito/mod_util.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.252256 ont-bonito-0.7.3/bonito/models/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      115 2021-10-27 17:31:47.000000 ont-bonito-0.7.3/bonito/models/README.md
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.265540 ont-bonito-0.7.3/bonito/models/configs/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1206 2021-10-27 17:31:47.000000 ont-bonito-0.7.3/bonito/models/configs/dna_r9.4.1@v1.toml
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1289 2021-10-27 17:31:47.000000 ont-bonito-0.7.3/bonito/models/configs/dna_r9.4.1@v2.toml
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      290 2021-10-27 17:31:48.000000 ont-bonito-0.7.3/bonito/models/configs/dna_r9.4.1@v3.toml
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     7948 2021-12-03 16:22:18.000000 ont-bonito-0.7.3/bonito/multiprocessing.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    12149 2023-12-12 17:08:45.000000 ont-bonito-0.7.3/bonito/nn.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4817 2023-12-12 17:08:45.000000 ont-bonito-0.7.3/bonito/pod5.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5324 2023-12-12 17:08:45.000000 ont-bonito-0.7.3/bonito/reader.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     3330 2021-11-22 13:56:15.000000 ont-bonito-0.7.3/bonito/schedule.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    10538 2023-12-12 17:08:45.000000 ont-bonito-0.7.3/bonito/training.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.269189 ont-bonito-0.7.3/bonito/transformer/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     7354 2023-10-02 15:31:29.000000 ont-bonito-0.7.3/bonito/transformer/rote.py
--rwxr-xr-x   0 cseymour  (5744) domain users  (1113)    13291 2023-10-04 22:21:51.000000 ont-bonito-0.7.3/bonito/util.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-12-12 17:14:02.298854 ont-bonito-0.7.3/ont_bonito.egg-info/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5024 2023-12-12 17:14:01.000000 ont-bonito-0.7.3/ont_bonito.egg-info/PKG-INFO
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1033 2023-12-12 17:14:02.000000 ont-bonito-0.7.3/ont_bonito.egg-info/SOURCES.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       39 2023-12-12 17:14:01.000000 ont-bonito-0.7.3/ont_bonito.egg-info/dependency_links.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       39 2023-12-12 17:14:01.000000 ont-bonito-0.7.3/ont_bonito.egg-info/entry_points.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      260 2023-12-12 17:14:01.000000 ont-bonito-0.7.3/ont_bonito.egg-info/requires.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)        7 2023-12-12 17:14:01.000000 ont-bonito-0.7.3/ont_bonito.egg-info/top_level.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      303 2023-12-12 17:08:40.000000 ont-bonito-0.7.3/requirements.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       38 2023-12-12 17:14:02.309227 ont-bonito-0.7.3/setup.cfg
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1270 2023-09-28 14:20:31.000000 ont-bonito-0.7.3/setup.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:47.079631 ont-bonito-0.8.1/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    14470 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/LICENCE.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      179 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/MANIFEST.in
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     6271 2024-05-21 15:20:47.077639 ont-bonito-0.8.1/PKG-INFO
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     5951 2024-05-21 08:56:26.000000 ont-bonito-0.8.1/README.md
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:46.937746 ont-bonito-0.8.1/bonito/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      897 2024-05-21 15:20:19.000000 ont-bonito-0.8.1/bonito/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       31 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/__main__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1549 2024-05-20 21:29:05.000000 ont-bonito-0.8.1/bonito/aligner.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:46.965792 ont-bonito-0.8.1/bonito/cli/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)        0 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/cli/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     8657 2024-05-20 21:29:05.000000 ont-bonito-0.8.1/bonito/cli/basecaller.py
+-rwxr-xr-x   0 cseymour  (5744) domain users  (1113)     5164 2024-05-20 21:29:05.000000 ont-bonito-0.8.1/bonito/cli/download.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    12708 2024-05-20 21:29:05.000000 ont-bonito-0.8.1/bonito/cli/duplex.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     3901 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/cli/evaluate.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4247 2024-05-13 14:46:40.000000 ont-bonito-0.8.1/bonito/cli/export.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4807 2024-04-12 08:55:41.000000 ont-bonito-0.8.1/bonito/cli/train.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      702 2024-03-31 13:50:03.000000 ont-bonito-0.8.1/bonito/cli/view.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:46.978702 ont-bonito-0.8.1/bonito/crf/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/crf/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2632 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/crf/basecall.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    10109 2024-05-18 18:39:41.000000 ont-bonito-0.8.1/bonito/crf/model.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:46.991648 ont-bonito-0.8.1/bonito/ctc/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/ctc/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2018 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/ctc/basecall.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     7110 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/ctc/model.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:46.996108 ont-bonito-0.8.1/bonito/data/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       95 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/data/README.md
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2868 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/data.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     6985 2024-05-18 18:39:41.000000 ont-bonito-0.8.1/bonito/fast5.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    19464 2024-04-12 08:55:41.000000 ont-bonito-0.8.1/bonito/io.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     3249 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/mod_util.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:47.000984 ont-bonito-0.8.1/bonito/models/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      115 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/models/README.md
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:47.014578 ont-bonito-0.8.1/bonito/models/configs/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1206 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/models/configs/dna_r9.4.1@v1.toml
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1289 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/models/configs/dna_r9.4.1@v2.toml
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      290 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/models/configs/dna_r9.4.1@v3.toml
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     7948 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/multiprocessing.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    14466 2024-04-16 08:34:48.000000 ont-bonito-0.8.1/bonito/nn.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4959 2024-05-18 18:39:41.000000 ont-bonito-0.8.1/bonito/pod5.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     5524 2024-05-18 18:39:41.000000 ont-bonito-0.8.1/bonito/reader.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     3330 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/schedule.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    10582 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/bonito/training.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:47.031223 ont-bonito-0.8.1/bonito/transformer/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2024-03-28 11:36:25.000000 ont-bonito-0.8.1/bonito/transformer/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       32 2024-03-28 11:36:25.000000 ont-bonito-0.8.1/bonito/transformer/basecall.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     5242 2024-04-16 08:34:48.000000 ont-bonito-0.8.1/bonito/transformer/model.py
+-rwxr-xr-x   0 cseymour  (5744) domain users  (1113)    13861 2024-05-20 21:29:05.000000 ont-bonito-0.8.1/bonito/util.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:47.057040 ont-bonito-0.8.1/ont_bonito.egg-info/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     6271 2024-05-21 15:20:46.000000 ont-bonito-0.8.1/ont_bonito.egg-info/PKG-INFO
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1130 2024-05-21 15:20:46.000000 ont-bonito-0.8.1/ont_bonito.egg-info/SOURCES.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)        1 2024-05-21 15:20:46.000000 ont-bonito-0.8.1/ont_bonito.egg-info/dependency_links.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       39 2024-05-21 15:20:46.000000 ont-bonito-0.8.1/ont_bonito.egg-info/entry_points.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      217 2024-05-21 15:20:46.000000 ont-bonito-0.8.1/ont_bonito.egg-info/requires.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       12 2024-05-21 15:20:46.000000 ont-bonito-0.8.1/ont_bonito.egg-info/top_level.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      412 2024-05-18 18:39:35.000000 ont-bonito-0.8.1/requirements.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       38 2024-05-21 15:20:47.080912 ont-bonito-0.8.1/setup.cfg
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1415 2024-05-18 18:39:35.000000 ont-bonito-0.8.1/setup.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2024-05-21 15:20:47.071414 ont-bonito-0.8.1/test/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)        0 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/test/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      415 2024-03-27 16:08:36.000000 ont-bonito-0.8.1/test/test_cli.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2126 2024-04-12 08:55:41.000000 ont-bonito-0.8.1/test/test_download.py
```

### Comparing `ont-bonito-0.7.3/LICENCE.txt` & `ont-bonito-0.8.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/PKG-INFO` & `ont-bonito-0.8.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,97 @@
-Metadata-Version: 2.1
-Name: ont-bonito
-Version: 0.7.3
-Home-page: https://github.com/nanoporetech/bonito
-Author: Oxford Nanopore Technologies, Ltd
-Author-email: support@nanoporetech.com
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
 # Bonito
 
-[![PyPI version](https://badge.fury.io/py/ont-bonito.svg)](https://badge.fury.io/py/ont-bonito) 
+[![PyPI version](https://badge.fury.io/py/ont-bonito.svg)](https://badge.fury.io/py/ont-bonito)
 [![py38](https://img.shields.io/badge/python-3.8-brightgreen.svg)](https://img.shields.io/badge/python-3.8-brightgreen.svg)
 [![py39](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://img.shields.io/badge/python-3.9-brightgreen.svg)
 [![py310](https://img.shields.io/badge/python-3.10-brightgreen.svg)](https://img.shields.io/badge/python-3.10-brightgreen.svg)
 [![py311](https://img.shields.io/badge/python-3.11-brightgreen.svg)](https://img.shields.io/badge/python-3.11-brightgreen.svg)
-[![cu117](https://img.shields.io/badge/cuda-11.7-blue.svg)](https://img.shields.io/badge/cuda-11.7-blue.svg)
+[![cu118](https://img.shields.io/badge/cuda-11.8-blue.svg)](https://img.shields.io/badge/cuda-11.8-blue.svg)
 
 Bonito is an open source research basecaller for Oxford Nanopore reads.
 
 For anything other than basecaller training or method development please use [dorado](https://github.com/nanoporetech/dorado).
 
 ```bash
 $ pip install --upgrade pip
 $ pip install ont-bonito
-$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v4.0.0 /data/reads > basecalls.bam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 /data/reads > basecalls.bam
 ```
 
 Bonito supports writing aligned/unaligned `{fastq, sam, bam, cram}`.
 
 ```bash
-$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v4.0.0 --reference reference.mmi /data/reads > basecalls.bam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 --reference reference.mmi /data/reads > basecalls.bam
 ```
 
 Bonito will download and cache the basecalling model automatically on first use but all models can be downloaded with -
 
 ``` bash
 $ bonito download --models --show  # show all available models
 $ bonito download --models         # download all available models
 ```
 
+## Transformer Models
+
+The `bonito.transformer` package requires
+[flash-attn](https://github.com/Dao-AILab/flash-attention?tab=readme-ov-file#installation-and-features).
+
+This must be manually installed as the `flash-attn` packaging system prevents it from being listed as a normal dependency.
+
+Setting `CUDA_HOME` to the relevant library directory will help avoid CUDA version mismatches between packages.
+
 ## Modified Bases
 
 Modified base calling is handled by [Remora](https://github.com/nanoporetech/remora).
 
 ```bash
-$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v4.0.0 /data/reads --modified-bases 5mC --reference ref.mmi > basecalls_with_mods.bam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 /data/reads --modified-bases 5mC --reference ref.mmi > basecalls_with_mods.bam
 ```
 
 See available modified base models with the ``remora model list_pretrained`` command.
 
 ## Training your own model
 
 To train a model using your own reads, first basecall the reads with the additional `--save-ctc` flag and use the output directory as the input directory for training.
 
 ```bash
-$ bonito basecaller dna_r9.4.1 --save-ctc --reference reference.mmi /data/reads > /data/training/ctc-data/basecalls.sam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 --save-ctc --reference reference.mmi /data/reads > /data/training/ctc-data/basecalls.sam
 $ bonito train --directory /data/training/ctc-data /data/training/model-dir
 ```
 
-In addition to training a new model from scratch you can also easily fine tune one of the pretrained models.  
+In addition to training a new model from scratch you can also easily fine tune one of the pretrained models.
 
 ```bash
-bonito train --epochs 1 --lr 5e-4 --pretrained dna_r10.4.1_e8.2_400bps_hac@v4.0.0 --directory /data/training/ctc-data /data/training/fine-tuned-model
+bonito train --epochs 1 --lr 5e-4 --pretrained dna_r10.4.1_e8.2_400bps_hac@v5.0.0 --directory /data/training/ctc-data /data/training/fine-tuned-model
 ```
 
 If you are interested in method development and don't have you own set of reads then a pre-prepared set is provide.
 
 ```bash
 $ bonito download --training
 $ bonito train /data/training/model-dir
 ```
 
-All training calls use Automatic Mixed Precision to speed up training. To disable this, set the `--no-amp` flag to True. 
+All training calls use Automatic Mixed Precision to speed up training. To disable this, set the `--no-amp` flag to True.
 
 ## Developer Quickstart
 
 ```bash
 $ git clone https://github.com/nanoporetech/bonito.git  # or fork first and clone that
 $ cd bonito
 $ python3 -m venv venv3
 $ source venv3/bin/activate
 (venv3) $ pip install --upgrade pip
-(venv3) $ pip install -e .
+(venv3) $ pip install -e .[cu118] --extra-index-url https://download.pytorch.org/whl/cu118
 ```
 
+The `ont-bonito[cu118]` and `ont-bonito[cu121]` optional dependencies can be used, along
+with the corresponding `--extra-index-url`, to ensure the PyTorch package matches the
+local CUDA setup.
+
 ## Interface
 
  - `bonito view` - view a model architecture for a given `.toml` file and the number of parameters in the network.
  - `bonito train` - train a bonito model.
  - `bonito evaluate` - evaluate a model performance.
  - `bonito download` - download pretrained models and training datasets.
  - `bonito basecaller` - basecaller *(`.fast5` -> `.bam`)*.
@@ -105,7 +109,20 @@
 Technologies, Ltd.  Public License, v. 1.0.  If a copy of the License
 was not distributed with this file, You can obtain one at
 http://nanoporetech.com
 
 ### Research Release
 
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
+
+### Citation
+
+```
+@software{bonito,
+  title = {Bonito: A PyTorch Basecaller for Oxford Nanopore Reads},
+  author = {{Chris Seymour, Oxford Nanopore Technologies Ltd.}},
+  year = {2019},
+  url = {https://github.com/nanoporetech/bonito},
+  note = {Oxford Nanopore Technologies, Ltd. Public License, v. 1.0},
+  abstract = {Bonito is an open source research basecaller for Oxford Nanopore reads. It provides a flexible platform for training and developing basecalling models using PyTorch.}
+}
+```
```

### Comparing `ont-bonito-0.7.3/README.md` & `ont-bonito-0.8.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,109 @@
+Metadata-Version: 2.1
+Name: ont-bonito
+Version: 0.8.1
+Home-page: https://github.com/nanoporetech/bonito
+Author: Oxford Nanopore Technologies, Ltd
+Author-email: support@nanoporetech.com
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: cu118
+Provides-Extra: cu121
+License-File: LICENCE.txt
+
 # Bonito
 
-[![PyPI version](https://badge.fury.io/py/ont-bonito.svg)](https://badge.fury.io/py/ont-bonito) 
+[![PyPI version](https://badge.fury.io/py/ont-bonito.svg)](https://badge.fury.io/py/ont-bonito)
 [![py38](https://img.shields.io/badge/python-3.8-brightgreen.svg)](https://img.shields.io/badge/python-3.8-brightgreen.svg)
 [![py39](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://img.shields.io/badge/python-3.9-brightgreen.svg)
 [![py310](https://img.shields.io/badge/python-3.10-brightgreen.svg)](https://img.shields.io/badge/python-3.10-brightgreen.svg)
 [![py311](https://img.shields.io/badge/python-3.11-brightgreen.svg)](https://img.shields.io/badge/python-3.11-brightgreen.svg)
-[![cu117](https://img.shields.io/badge/cuda-11.7-blue.svg)](https://img.shields.io/badge/cuda-11.7-blue.svg)
+[![cu118](https://img.shields.io/badge/cuda-11.8-blue.svg)](https://img.shields.io/badge/cuda-11.8-blue.svg)
 
 Bonito is an open source research basecaller for Oxford Nanopore reads.
 
 For anything other than basecaller training or method development please use [dorado](https://github.com/nanoporetech/dorado).
 
 ```bash
 $ pip install --upgrade pip
 $ pip install ont-bonito
-$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v4.0.0 /data/reads > basecalls.bam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 /data/reads > basecalls.bam
 ```
 
 Bonito supports writing aligned/unaligned `{fastq, sam, bam, cram}`.
 
 ```bash
-$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v4.0.0 --reference reference.mmi /data/reads > basecalls.bam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 --reference reference.mmi /data/reads > basecalls.bam
 ```
 
 Bonito will download and cache the basecalling model automatically on first use but all models can be downloaded with -
 
 ``` bash
 $ bonito download --models --show  # show all available models
 $ bonito download --models         # download all available models
 ```
 
+## Transformer Models
+
+The `bonito.transformer` package requires
+[flash-attn](https://github.com/Dao-AILab/flash-attention?tab=readme-ov-file#installation-and-features).
+
+This must be manually installed as the `flash-attn` packaging system prevents it from being listed as a normal dependency.
+
+Setting `CUDA_HOME` to the relevant library directory will help avoid CUDA version mismatches between packages.
+
 ## Modified Bases
 
 Modified base calling is handled by [Remora](https://github.com/nanoporetech/remora).
 
 ```bash
-$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v4.0.0 /data/reads --modified-bases 5mC --reference ref.mmi > basecalls_with_mods.bam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 /data/reads --modified-bases 5mC --reference ref.mmi > basecalls_with_mods.bam
 ```
 
 See available modified base models with the ``remora model list_pretrained`` command.
 
 ## Training your own model
 
 To train a model using your own reads, first basecall the reads with the additional `--save-ctc` flag and use the output directory as the input directory for training.
 
 ```bash
-$ bonito basecaller dna_r9.4.1 --save-ctc --reference reference.mmi /data/reads > /data/training/ctc-data/basecalls.sam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 --save-ctc --reference reference.mmi /data/reads > /data/training/ctc-data/basecalls.sam
 $ bonito train --directory /data/training/ctc-data /data/training/model-dir
 ```
 
-In addition to training a new model from scratch you can also easily fine tune one of the pretrained models.  
+In addition to training a new model from scratch you can also easily fine tune one of the pretrained models.
 
 ```bash
-bonito train --epochs 1 --lr 5e-4 --pretrained dna_r10.4.1_e8.2_400bps_hac@v4.0.0 --directory /data/training/ctc-data /data/training/fine-tuned-model
+bonito train --epochs 1 --lr 5e-4 --pretrained dna_r10.4.1_e8.2_400bps_hac@v5.0.0 --directory /data/training/ctc-data /data/training/fine-tuned-model
 ```
 
 If you are interested in method development and don't have you own set of reads then a pre-prepared set is provide.
 
 ```bash
 $ bonito download --training
 $ bonito train /data/training/model-dir
 ```
 
-All training calls use Automatic Mixed Precision to speed up training. To disable this, set the `--no-amp` flag to True. 
+All training calls use Automatic Mixed Precision to speed up training. To disable this, set the `--no-amp` flag to True.
 
 ## Developer Quickstart
 
 ```bash
 $ git clone https://github.com/nanoporetech/bonito.git  # or fork first and clone that
 $ cd bonito
 $ python3 -m venv venv3
 $ source venv3/bin/activate
 (venv3) $ pip install --upgrade pip
-(venv3) $ pip install -e .
+(venv3) $ pip install -e .[cu118] --extra-index-url https://download.pytorch.org/whl/cu118
 ```
 
+The `ont-bonito[cu118]` and `ont-bonito[cu121]` optional dependencies can be used, along
+with the corresponding `--extra-index-url`, to ensure the PyTorch package matches the
+local CUDA setup.
+
 ## Interface
 
  - `bonito view` - view a model architecture for a given `.toml` file and the number of parameters in the network.
  - `bonito train` - train a bonito model.
  - `bonito evaluate` - evaluate a model performance.
  - `bonito download` - download pretrained models and training datasets.
  - `bonito basecaller` - basecaller *(`.fast5` -> `.bam`)*.
@@ -96,7 +121,20 @@
 Technologies, Ltd.  Public License, v. 1.0.  If a copy of the License
 was not distributed with this file, You can obtain one at
 http://nanoporetech.com
 
 ### Research Release
 
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
+
+### Citation
+
+```
+@software{bonito,
+  title = {Bonito: A PyTorch Basecaller for Oxford Nanopore Reads},
+  author = {{Chris Seymour, Oxford Nanopore Technologies Ltd.}},
+  year = {2019},
+  url = {https://github.com/nanoporetech/bonito},
+  note = {Oxford Nanopore Technologies, Ltd. Public License, v. 1.0},
+  abstract = {Bonito is an open source research basecaller for Oxford Nanopore reads. It provides a flexible platform for training and developing basecalling models using PyTorch.}
+}
+```
```

### Comparing `ont-bonito-0.7.3/bonito/__init__.py` & `ont-bonito-0.8.1/bonito/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
-from bonito.cli import basecaller, train, evaluate, view, convert, download, export, duplex
+
+from bonito.cli import basecaller, download, duplex, evaluate, export, train, view
 
 modules = [
-    'basecaller', 'train', 'evaluate', 'view', 'convert', 'download', 'export', 'duplex'
+    'basecaller', 'download', 'duplex', 'evaluate', 'export', 'train', 'view',
 ]
 
-__version__ = '0.7.3'
+__version__ = '0.8.1'
 
 
 def main():
-    parser = ArgumentParser(
-        'bonito',
-        formatter_class=ArgumentDefaultsHelpFormatter
-    )
+    parser = ArgumentParser('bonito', formatter_class=ArgumentDefaultsHelpFormatter)
 
     parser.add_argument(
         '-v', '--version', action='version',
         version='%(prog)s {}'.format(__version__)
     )
 
     subparsers = parser.add_subparsers(
```

### Comparing `ont-bonito-0.7.3/bonito/aligner.py` & `ont-bonito-0.8.1/bonito/aligner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Bonito Aligner
 """
-
 from threading import Thread
 from functools import partial
 from mappy import Aligner, ThreadBuffer
 
 from bonito.multiprocessing import ThreadMap
```

### Comparing `ont-bonito-0.7.3/bonito/cli/basecaller.py` & `ont-bonito-0.8.1/bonito/cli/basecaller.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 from tqdm import tqdm
 from time import perf_counter
 from functools import partial
 from datetime import timedelta
 from itertools import islice as take
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 
+from bonito.nn import fuse_bn_
 from bonito.aligner import align_map, Aligner
 from bonito.reader import read_chunks, Reader
 from bonito.io import CTCWriter, Writer, biofmt
 from bonito.mod_util import call_mods, load_mods_model
-from bonito.cli.download import File, models, __models__
+from bonito.cli.download import Downloader, models, __models_dir__
 from bonito.multiprocessing import process_cancel, process_itemmap
-from bonito.util import column_to_set, load_symbol, load_model, init
+from bonito.util import column_to_set, load_symbol, load_model, init, tqdm_environ
 
 
 def main(args):
 
     init(args.seed, args.device)
 
     try:
@@ -38,30 +39,31 @@
         sys.stderr.write("> error: reference cannot be a .mmi when outputting cram\n")
         exit(1)
     elif args.reference and fmt.name == "fastq":
         sys.stderr.write(f"> warning: did you really want {fmt.aligned} {fmt.name}?\n")
     else:
         sys.stderr.write(f"> outputting {fmt.aligned} {fmt.name}\n")
 
-    if args.model_directory in models and args.model_directory not in os.listdir(__models__):
+    if args.model_directory in models and not (__models_dir__ / args.model_directory).exists():
         sys.stderr.write("> downloading model\n")
-        File(__models__, args.model_directory).download()
+        Downloader(__models_dir__).download(args.model_directory)
 
     sys.stderr.write(f"> loading model {args.model_directory}\n")
     try:
         model = load_model(
             args.model_directory,
             args.device,
             weights=args.weights if args.weights > 0 else None,
             chunksize=args.chunksize,
             overlap=args.overlap,
             batchsize=args.batchsize,
             quantize=args.quantize,
             use_koi=True,
         )
+        model = model.apply(fuse_bn_)
     except FileNotFoundError:
         sys.stderr.write(f"> error: failed to load {args.model_directory}\n")
         sys.stderr.write(f"> available models:\n")
         for model in sorted(models): sys.stderr.write(f" - {model}\n")
         exit(1)
 
     if args.verbose:
@@ -76,15 +78,15 @@
             args.modified_bases, args.model_directory, args.modified_base_model,
             device=args.modified_device,
         )
         sys.stderr.write(f"> {mods_model[1]['alphabet_str']}\n")
 
     if args.reference:
         sys.stderr.write("> loading reference\n")
-        aligner = Aligner(args.reference, preset='map-ont', best_n=1)
+        aligner = Aligner(args.reference, preset=args.mm2_preset)
         if not aligner:
             sys.stderr.write("> failed to load/build index\n")
             exit(1)
     else:
         aligner = None
 
     if args.save_ctc and not args.reference:
@@ -116,14 +118,16 @@
     )
 
     if args.verbose:
         sys.stderr.write(f"> read scaling: {model.config.get('scaling')}\n")
     
     if args.max_reads:
         reads = take(reads, args.max_reads)
+        if num_reads is not None:
+            num_reads = min(num_reads, args.max_reads)
 
     if args.save_ctc:
         reads = (
             chunk for read in reads
             for chunk in read_chunks(
                 read,
                 chunksize=model.config["basecaller"]["chunksize"],
@@ -158,15 +162,16 @@
                      'min_qscore': args.min_qscore}
     if args.save_ctc:
         writer_kwargs['rna'] = args.rna
         writer_kwargs['min_accuracy'] = args.min_accuracy_save_ctc
         
     writer = ResultsWriter(
         fmt.mode, tqdm(results, desc="> calling", unit=" reads", leave=False,
-                       total=num_reads, smoothing=0, ascii=True, ncols=100),
+                       total=num_reads, smoothing=0, ascii=True, ncols=100,
+                       **tqdm_environ()),
         **writer_kwargs)
 
     t0 = perf_counter()
     writer.start()
     writer.join()
     duration = perf_counter() - t0
     num_samples = sum(num_samples for read_id, num_samples in writer.log)
@@ -206,9 +211,10 @@
     parser.add_argument("--overlap", default=None, type=int)
     parser.add_argument("--chunksize", default=None, type=int)
     parser.add_argument("--batchsize", default=None, type=int)
     parser.add_argument("--max-reads", default=0, type=int)
     parser.add_argument("--min-qscore", default=0, type=int)
     parser.add_argument("--min-accuracy-save-ctc", default=0.99, type=float)
     parser.add_argument("--alignment-threads", default=8, type=int)
+    parser.add_argument("--mm2-preset", default='lr:hq', type=str)
     parser.add_argument('-v', '--verbose', action='count', default=0)
     return parser
```

### Comparing `ont-bonito-0.7.3/bonito/cli/duplex.py` & `ont-bonito-0.8.1/bonito/cli/duplex.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from mappy import revcomp
 from edlib import align as edlib_align
 from parasail import dnafull, sg_trace_scan_32
 
 from bonito.io import DuplexWriter, biofmt
 from bonito.aligner import align_map, Aligner
 from bonito.multiprocessing import ProcessMap
+from bonito.util import tqdm_environ
 
 
 # Cigar int code ops are: MIDNSHP=X
 CODE_TO_OP = OrderedDict(
     (
         ("M", pysam.CMATCH),
         ("I", pysam.CINS),
@@ -64,15 +65,16 @@
 
     def compute_read_index(self):
         def read_is_primary(read):
             return not (read.is_supplementary or read.is_secondary)
 
         self.bam_idx = {} if self.skip_non_primary else defaultdict(list)
         self.open_bam()
-        pbar = tqdm(smoothing=0, unit=" Reads", desc="> indexing BAM by read id", leave=False)
+        pbar = tqdm(smoothing=0, unit=" Reads", desc="> indexing BAM by read id",
+                    leave=False, **tqdm_environ())
         # iterating over file handle gives incorrect pointers
         while True:
             read_ptr = self.bam_fh.tell()
             try:
                 read = next(self.bam_fh)
             except StopIteration:
                 break
@@ -341,15 +343,15 @@
             temp_rid, comp_rid = line.split()
             duplex_pairs.append(
                 ((temp_rid, comp_rid), (temp_rid, comp_rid))
             )
 
     if args.reference:
         sys.stderr.write("> loading reference\n")
-        aligner = Aligner(args.reference, preset='map-ont', best_n=1)
+        aligner = Aligner(args.reference, preset=args.mm2_preset)
         if not aligner:
             sys.stderr.write("> failed to load/build index\n")
             exit(1)
     else:
         aligner = None
 
     results = ProcessMap(
@@ -387,8 +389,9 @@
     parser.add_argument("in_bam")
     parser.add_argument("duplex_pairs_file")
     parser.add_argument("--reference")
     parser.add_argument("--min-qscore", default=0, type=int)
     parser.add_argument("--no-header", action="store_true") # skip-header?
     parser.add_argument("--threads", default=8, type=int)
     parser.add_argument("--alignment-threads", default=8, type=int)
+    parser.add_argument("--mm2-preset", default='lr:hq', type=str)
     return parser
```

### Comparing `ont-bonito-0.7.3/bonito/cli/evaluate.py` & `ont-bonito-0.8.1/bonito/cli/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Bonito model evaluator
 """
 
-import os
 import time
 import torch
 import numpy as np
 from itertools import starmap
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from pathlib import Path
 
 from bonito.data import load_numpy, load_script
 from bonito.util import accuracy, poa, decode_ref, half_supported
-from bonito.util import init, load_model, concat, permute
+from bonito.util import init, load_model, permute
 
 from torch.utils.data import DataLoader
 
 
 def main(args):
 
     poas = []
@@ -42,22 +41,27 @@
 
     for w in [int(i) for i in args.weights.split(',')]:
 
         seqs = []
 
         print("* loading model", w)
         model = load_model(args.model_directory, args.device, weights=w)
+        mean = model.config.get("standardisation", {}).get("mean", 0.0)
+        stdev = model.config.get("standardisation", {}).get("stdev", 1.0)
+        print(f"* * signal standardisation params: mean={mean}, stdev={stdev}")
 
         print("* calling")
         t0 = time.perf_counter()
 
         targets = []
 
         with torch.no_grad():
             for data, target, *_ in dataloader:
+                data = (data - mean) / stdev
+
                 targets.extend(torch.unbind(target, 0))
                 if half_supported():
                     data = data.type(torch.float16).to(args.device)
                 else:
                     data = data.to(args.device)
 
                 log_probs = model(data)
```

### Comparing `ont-bonito-0.7.3/bonito/cli/train.py` & `ont-bonito-0.8.1/bonito/cli/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 import os
 from argparse import ArgumentParser
 from argparse import ArgumentDefaultsHelpFormatter
 from pathlib import Path
 from importlib import import_module
 
 from bonito.data import load_numpy, load_script
-from bonito.util import __models__, default_config, default_data
+from bonito.util import __models_dir__, default_config
 from bonito.util import load_model, load_symbol, init, half_supported
-from bonito.training import load_state, Trainer
+from bonito.training import Trainer
 
 import toml
 import torch
-import numpy as np
 from torch.utils.data import DataLoader
 
 
 def main(args):
 
     workdir = os.path.expanduser(args.training_directory)
 
@@ -32,16 +31,16 @@
     init(args.seed, args.device, (not args.nondeterministic))
     device = torch.device(args.device)
 
     if not args.pretrained:
         config = toml.load(args.config)
     else:
         dirname = args.pretrained
-        if not os.path.isdir(dirname) and os.path.isdir(os.path.join(__models__, dirname)):
-            dirname = os.path.join(__models__, dirname)
+        if not os.path.isdir(dirname) and os.path.isdir(os.path.join(__models_dir__, dirname)):
+            dirname = os.path.join(__models_dir__, dirname)
         pretrain_file = os.path.join(dirname, 'config.toml')
         config = toml.load(pretrain_file)
         if 'lr_scheduler' in config:
             print(f"[ignoring 'lr_scheduler' in --pretrained config]")
             del config['lr_scheduler']
 
     argsdict = dict(training=vars(args))
@@ -65,15 +64,15 @@
             chunks=args.chunks,
             valid_chunks=args.valid_chunks,
             n_pre_context_bases=getattr(model, "n_pre_context_bases", 0),
             n_post_context_bases=getattr(model, "n_post_context_bases", 0),
         )
 
     loader_kwargs = {
-        "batch_size": args.batch, "num_workers": 4, "pin_memory": True
+        "batch_size": args.batch, "num_workers": args.num_workers, "pin_memory": True
     }
     train_loader = DataLoader(**loader_kwargs, **train_loader_kwargs)
     valid_loader = DataLoader(**loader_kwargs, **valid_loader_kwargs)
 
     os.makedirs(workdir, exist_ok=True)
     toml.dump({**config, **argsdict}, open(os.path.join(workdir, 'config.toml'), 'w'))
 
@@ -95,15 +94,16 @@
         quantile_grad_clip=args.quantile_grad_clip
     )
 
     if (',' in args.lr):
         lr = [float(x) for x in args.lr.split(',')]
     else:
         lr = float(args.lr)
-    trainer.fit(workdir, args.epochs, lr)
+    optim_kwargs = config.get("optim", {})
+    trainer.fit(workdir, args.epochs, lr, **optim_kwargs)
 
 def argparser():
     parser = ArgumentParser(
         formatter_class=ArgumentDefaultsHelpFormatter,
         add_help=False
     )
     parser.add_argument("training_directory")
@@ -121,8 +121,9 @@
     parser.add_argument("--no-amp", action="store_true", default=False)
     parser.add_argument("-f", "--force", action="store_true", default=False)
     parser.add_argument("--restore-optim", action="store_true", default=False)
     parser.add_argument("--nondeterministic", action="store_true", default=False)
     parser.add_argument("--save-optim-every", default=10, type=int)
     parser.add_argument("--grad-accum-split", default=1, type=int)
     parser.add_argument("--quantile-grad-clip", action="store_true", default=False)
+    parser.add_argument("--num-workers", default=4, type=int)
     return parser
```

### Comparing `ont-bonito-0.7.3/bonito/crf/basecall.py` & `ont-bonito-0.8.1/bonito/crf/basecall.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/bonito/crf/model.py` & `ont-bonito-0.8.1/bonito/crf/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Bonito CTC-CRF Model.
 """
 
 import torch
 import numpy as np
 
-import koi
+import koi.lstm
 from koi.ctc import SequenceDist, Max, Log, semiring
 from koi.ctc import logZ_cu, viterbi_alignments, logZ_cu_sparse, bwd_scores_cu_sparse, fwd_scores_cu_sparse
 
 from bonito.nn import Module, Convolution, LinearCRFEncoder, Serial, Permute, layers, to_dict, from_dict, register
 
 
 def get_stride(m, stride=1):
@@ -143,19 +143,19 @@
         return viterbi_alignments(stay_scores, move_scores, target_lengths + 1 - self.state_len)
 
 
 def conv(c_in, c_out, ks, stride=1, bias=False, activation=None, norm=None):
     return Convolution(c_in, c_out, ks, stride=stride, padding=ks//2, bias=bias, activation=activation, norm=norm)
 
 
-def rnn_encoder(n_base, state_len, insize=1, stride=5, winlen=19, activation='swish', rnn_type='lstm', features=768, scale=5.0, blank_score=None, expand_blanks=True, num_layers=5, norm=None):
+def rnn_encoder(n_base, state_len, insize=1, first_conv_size=4, stride=5, winlen=19, activation='swish', rnn_type='lstm', features=768, scale=5.0, blank_score=None, expand_blanks=True, num_layers=5, norm=None):
     rnn = layers[rnn_type]
     return Serial([
-        conv(insize, 4, ks=5, bias=True, activation=activation, norm=norm),
-        conv(4, 16, ks=5, bias=True, activation=activation, norm=norm),
+        conv(insize, first_conv_size, ks=5, bias=True, activation=activation, norm=norm),
+        conv(first_conv_size, 16, ks=5, bias=True, activation=activation, norm=norm),
         conv(16, features, ks=winlen, stride=stride, bias=True, activation=activation, norm=norm),
         Permute([2, 0, 1]),
         *(rnn(features, features, reverse=(num_layers - i) % 2) for i in range(num_layers)),
         LinearCRFEncoder(
             features, n_base, state_len, activation='tanh', scale=scale,
             blank_score=blank_score, expand_blanks=expand_blanks
         )
```

### Comparing `ont-bonito-0.7.3/bonito/ctc/basecall.py` & `ont-bonito-0.8.1/bonito/ctc/basecall.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/bonito/ctc/model.py` & `ont-bonito-0.8.1/bonito/ctc/model.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/bonito/data.py` & `ont-bonito-0.8.1/bonito/data.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/bonito/fast5.py` & `ont-bonito-0.8.1/bonito/fast5.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,16 @@
         start_time = exp_start_dt + timedelta(seconds=self.start)
         self.start_time = start_time.astimezone(timezone.utc).isoformat(timespec="milliseconds")
 
         raw = read.handle[read.raw_dataset_name][:]
         self.scaled = np.array(self.scaling * (raw + self.offset), dtype=np.float32)
         self.num_samples = len(self.scaled)
 
+        self.scaling_strategy = ("quantile" if scaling_strategy is None else
+                                 scaling_strategy.get("strategy","quantile")) 
         self.shift, self.scale = bonito.reader.normalisation(self.scaled, scaling_strategy, norm_params)
         self.trimmed_samples = bonito.reader.trim(self.scaled, threshold=self.scale * 2.4 + self.shift) if do_trim else 0
         self.template_start = self.start + (self.trimmed_samples / self.sample_rate)
         self.template_duration = self.duration - (self.trimmed_samples / self.sample_rate)
 
         self.signal = (self.scaled[self.trimmed_samples:] - self.shift) / self.scale
```

### Comparing `ont-bonito-0.7.3/bonito/io.py` & `ont-bonito-0.8.1/bonito/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 from os.path import realpath, splitext, dirname
 
 import mappy
 import numpy as np
 from pysam import AlignmentFile, AlignmentHeader, AlignedSegment
 
 import bonito
-from bonito.cli.convert import typical_indices
 from bonito.util import mean_qscore_from_qstring
 
 
 logger = getLogger('bonito')
 Format = namedtuple("Format", "aligned name mode")
 
 __ont_bam_spec__ = "0.0.2"
 
 
+def typical_indices(x, n=2.5):
+    mu, sd = np.mean(x), np.std(x)
+    idx, = np.where((mu - n*sd < x) & (x < mu + n*sd))
+    return idx
+
+
 def biofmt(aligned=False):
     """
     Select the output format.
     """
     mode, name = ('w', 'sam') if aligned else ('wfq', 'fastq')
     aligned = "aligned" if aligned else "unaligned"
     stdout = realpath('/dev/fd/1')
```

### Comparing `ont-bonito-0.7.3/bonito/mod_util.py` & `ont-bonito-0.8.1/bonito/mod_util.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/bonito/models/configs/dna_r9.4.1@v1.toml` & `ont-bonito-0.8.1/bonito/models/configs/dna_r9.4.1@v1.toml`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/bonito/models/configs/dna_r9.4.1@v2.toml` & `ont-bonito-0.8.1/bonito/models/configs/dna_r9.4.1@v2.toml`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/bonito/multiprocessing.py` & `ont-bonito-0.8.1/bonito/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/bonito/nn.py` & `ont-bonito-0.8.1/bonito/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Bonito nn modules.
 """
 
+from collections import OrderedDict
+
 import torch
 from torch.nn import Module
 from torch.nn.init import orthogonal_
 from torch.nn.utils.fusion import fuse_conv_bn_eval
 
 
 layers = {}
@@ -90,14 +92,89 @@
         return {
             'sublayers': [to_dict(layer, include_weights) for layer in self._modules.values()]
         }
 
     def __repr__(self):
         return torch.nn.ModuleList.__repr__(self)
 
+
+@register
+class Stack(Serial):
+    @classmethod
+    def from_dict(cls, model_dict, layer_types=None):
+        return cls([from_dict(model_dict["layer"], layer_types) for _ in range(model_dict["depth"])])
+
+    def to_dict(self, include_weights=False):
+        if include_weights:
+            raise NotImplementedError
+        layer_dicts = [to_dict(layer) for layer in self]
+        for layer_dict in layer_dicts[1:]:
+            assert layer_dict == layer_dicts[0], "all layers should be the same"
+        return {"layer": layer_dicts[0], "depth": len(self)}
+
+
+@register
+class NamedSerial(torch.nn.Sequential):
+    @classmethod
+    def from_dict(cls, model_dict, layer_types=None):
+        return cls({k: from_dict(v, layer_types) for k, v in model_dict.items()})
+
+    def __init__(self, layers):
+        # Sequential throws error if given dict
+        super().__init__(OrderedDict(layers.items()))
+
+    def to_dict(self, include_weights=False):
+        if include_weights:
+            raise NotImplementedError
+        return {k: to_dict(v) for k, v in self.named_children()}
+
+
+class MakeContiguous(Module):
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, x):
+        return x.contiguous()
+
+
+@register
+class LinearUpsample(Module):
+    """
+    Applies a linear transformation to upsample the sequence length by ``scale_factor``.
+    """
+
+    def __init__(self, d_model, scale_factor, batch_first=True):
+        super().__init__()
+        self.d_model = d_model
+        self.scale_factor = scale_factor
+        self.batch_first = batch_first
+        self.linear = torch.nn.Linear(d_model, self.scale_factor * d_model)
+
+    def forward(self, src):
+        if not self.batch_first:
+            src = src.permute([1, 0, 2])
+        N, L, E = src.shape
+        h = self.linear(src).reshape(N, self.scale_factor * L, E)
+        if not self.batch_first:
+            h = h.permute([1, 0, 2])
+        return h
+
+    def output_stride(self, input_stride):
+        return input_stride // self.scale_factor
+
+    def to_dict(self, include_weights=False):
+        if include_weights:
+            raise NotImplementedError
+        return {
+            "d_model": self.d_model,
+            "scale_factor": self.scale_factor,
+            "batch_first": self.batch_first
+        }
+
+
 @register
 class Reverse(Module):
 
     def __init__(self, sublayers):
         super().__init__()
         self.layer = Serial(sublayers) if isinstance(sublayers, list) else sublayers
 
@@ -244,15 +321,15 @@
     def extra_repr(self):
         rep = 'n_base={}, state_len={}, scale={}, blank_score={}, expand_blanks={}'.format(
             self.n_base, self.state_len, self.scale, self.blank_score, self.expand_blanks
         )
         if self.permute:
             rep += f', permute={self.permute}'
         return rep
-            
+
 
 @register
 class Permute(Module):
 
     def __init__(self, dims):
         super().__init__()
         self.dims = dims
```

### Comparing `ont-bonito-0.7.3/bonito/pod5.py` & `ont-bonito-0.8.1/bonito/pod5.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from uuid import UUID
 from pathlib import Path
 from collections import OrderedDict
 from datetime import timedelta, timezone
 
 import numpy as np
 import bonito.reader
-from tqdm import tqdm
 from pod5 import Reader
 
 
 class Read(bonito.reader.Read):
 
     def __init__(self, read, filename, meta=False, do_trim=True, scaling_strategy=None, norm_params=None):
 
@@ -52,15 +51,17 @@
 
         self.raw = read.signal
 
         self.calibration = read.calibration
         self.scaling = self.calibration.scale
         self.offset = self.calibration.offset
         self.scaled = self.scaling * (self.raw.astype(np.float32) + self.offset)
-
+        self.scaling_strategy = ("quantile" if scaling_strategy is None else
+                                 scaling_strategy.get("strategy","quantile")) 
+        
         self.shift, self.scale = bonito.reader.normalisation(self.scaled, scaling_strategy, norm_params)
         self.trimmed_samples = bonito.reader.trim(self.scaled, threshold=self.scale * 2.4 + self.shift) if do_trim else 0
 
         self.template_start = self.start + (self.trimmed_samples / self.sample_rate)
         self.template_duration = self.duration - (self.trimmed_samples / self.sample_rate)
 
         self.signal = (self.scaled[self.trimmed_samples:] - self.shift) / self.scale
```

### Comparing `ont-bonito-0.7.3/bonito/reader.py` & `ont-bonito-0.8.1/bonito/reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Bonito Read Utils
 """
-
+import sys
 from glob import iglob
 from collections import OrderedDict
 from importlib import import_module
 
 import torch
 import numpy as np
-from scipy.signal import find_peaks
 
 
-__formats__ = ["fast5", "pod5"]
+__formats__ = ["pod5", "fast5"]
 
 # Normalisation parameters for kit 14 DNA
 # Different parameters can be specified in the 'normalisation' section
 # of a bonito config file
 __default_norm_params__ = {'quantile_a' : 0.2,
                            'quantile_b' : 0.9,
                            'shift_multiplier' : 0.51,
@@ -29,15 +28,19 @@
             pattern = f"**/*.{fmt}" if recursive else f"*.{fmt}"
             match = next(iglob(directory + "/" + pattern, recursive=True), None)
             if match is not None:
                 self.fmt = fmt
                 break
         else:
             raise FileNotFoundError()
-
+        if self.fmt == "fast5":
+            sys.stderr.write(
+                "DeprecationWarning: fast5 support will be deprecated in a "
+                "future bonito version. Please use pod5\n"
+            )
         _reader = import_module(f"bonito.{self.fmt}")
         self._get_reads = getattr(_reader, "get_reads")
         self._get_read_groups = getattr(_reader, "get_read_groups")
 
     def get_reads(self, *args, **kwargs):
         return self._get_reads(*args, **kwargs)
 
@@ -75,15 +78,15 @@
             f"ch:i:{self.channel}",
             f"st:Z:{self.start_time}",
             f"du:f:{self.duration}",
             f"rn:i:{self.read_number}",
             f"f5:Z:{self.filename}",
             f"sm:f:{self.shift}",
             f"sd:f:{self.scale}",
-            f"sv:Z:quantile",
+            f"sv:Z:{self.scaling_strategy}",
         ]
 
 
 class ReadChunk:
 
     def __init__(self, read, chunk, i, n):
         self.read_id = "%s:%i:%i" % (read.read_id, i, n)
```

### Comparing `ont-bonito-0.7.3/bonito/schedule.py` & `ont-bonito-0.8.1/bonito/schedule.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.3/bonito/training.py` & `ont-bonito-0.8.1/bonito/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from glob import glob
 from functools import partial
 from time import perf_counter
 from collections import OrderedDict
 from datetime import datetime
 
 from bonito.schedule import linear_warmup_cosine_decay
-from bonito.util import accuracy, decode_ref, permute, concat, match_names
+from bonito.util import accuracy, decode_ref, permute, concat, match_names, tqdm_environ
 import bonito
 
 import torch
 import numpy as np
 import torch.nn as nn
 from tqdm import tqdm
 import torch.cuda.amp as amp
@@ -145,15 +145,16 @@
     def train_one_epoch(self, loss_log, lr_scheduler):
         t0 = perf_counter()
         chunks = 0
         self.model.train()
 
         progress_bar = tqdm(
             total=len(self.train_loader), desc='[0/{}]'.format(len(self.train_loader.sampler)),
-            ascii=True, leave=True, ncols=100, bar_format='{l_bar}{bar}| [{elapsed}{postfix}]'
+            ascii=True, leave=True, ncols=100, bar_format='{l_bar}{bar}| [{elapsed}{postfix}]',
+            **tqdm_environ()
         )
         smoothed_loss = None
 
         with progress_bar:
 
             for batch in self.train_loader:
```

### Comparing `ont-bonito-0.7.3/bonito/util.py` & `ont-bonito-0.8.1/bonito/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """
 Bonito utils
 """
 
 import os
 import re
-import sys
 import random
 from glob import glob
 from itertools import groupby
+from logging import getLogger
 from operator import itemgetter
 from importlib import import_module
-from collections import deque, defaultdict, OrderedDict
-from torch.utils.data import DataLoader
+from collections import defaultdict, OrderedDict
+from pathlib import Path
 
 import toml
 import torch
-import koi.lstm
+
 import parasail
 import numpy as np
 from torch.cuda import get_device_capability
 
 try:
     from claragenomics.bindings import cuda
     from claragenomics.bindings.cudapoa import CudaPoaBatch
 except ImportError:
     pass
 
 
-__dir__ = os.path.dirname(os.path.realpath(__file__))
-__data__ = os.path.join(__dir__, "data")
-__models__ = os.path.join(__dir__, "models")
-__configs__ = os.path.join(__dir__, "models/configs")
+__dir__ = Path(__file__).parent
+__models_dir__ = __dir__ / "models"
+__data_dir__ = __dir__ / "data"
 
 split_cigar = re.compile(r"(?P<len>\d+)(?P<op>\D+)")
-default_data = os.path.join(__data__, "dna_r9.4.1")
-default_config = os.path.join(__configs__, "dna_r9.4.1@v3.1.toml")
+default_config = __dir__ / "models/configs/dna_r9.4.1@v3.1.toml"
+
 
+logger = getLogger('bonito')
 
 def init(seed, device, deterministic=True):
     """
     Initialise random libs and setup cudnn
 
     https://pytorch.org/docs/stable/notes/randomness.html
     """
@@ -231,16 +231,16 @@
 
 
 def load_symbol(config, symbol):
     """
     Dynamic load a symbol from module specified in model config.
     """
     if not isinstance(config, dict):
-        if not os.path.isdir(config) and os.path.isdir(os.path.join(__models__, config)):
-            dirname = os.path.join(__models__, config)
+        if not os.path.isdir(config) and os.path.isdir(os.path.join(__models_dir__, config)):
+            dirname = os.path.join(__models_dir__, config)
         else:
             dirname = config
         config = toml.load(os.path.join(dirname, 'config.toml'))
     imported = import_module(config['model']['package'])
     return getattr(imported, symbol)
 
 
@@ -276,32 +276,31 @@
     return config
 
 
 def load_model(dirname, device, weights=None, half=None, chunksize=None, batchsize=None, overlap=None, quantize=False, use_koi=False):
     """
     Load a model config and weights off disk from `dirname`.
     """
-    if not os.path.isdir(dirname) and os.path.isdir(os.path.join(__models__, dirname)):
-        dirname = os.path.join(__models__, dirname)
+    if not os.path.isdir(dirname) and os.path.isdir(os.path.join(__models_dir__, dirname)):
+        dirname = os.path.join(__models_dir__, dirname)
     weights = get_last_checkpoint(dirname) if weights is None else os.path.join(dirname, 'weights_%s.tar' % weights)
     config = toml.load(os.path.join(dirname, 'config.toml'))
     config = set_config_defaults(config, chunksize, batchsize, overlap, quantize)
     return _load_model(weights, config, device, half, use_koi)
 
 
 def _load_model(model_file, config, device, half=None, use_koi=False):
     device = torch.device(device)
     Model = load_symbol(config, "Model")
     model = Model(config)
 
-    config["basecaller"]["chunksize"] -= config["basecaller"]["chunksize"] % model.stride
-    # overlap must be even multiple of stride for correct stitching
-    config["basecaller"]["overlap"] -= config["basecaller"]["overlap"] % (model.stride * 2)
-
     if use_koi:
+        config["basecaller"]["chunksize"] -= config["basecaller"]["chunksize"] % model.stride
+        # overlap must be even multiple of stride for correct stitching
+        config["basecaller"]["overlap"] -= config["basecaller"]["overlap"] % (model.stride * 2)
         model.use_koi(
             batchsize=config["basecaller"]["batchsize"],
             chunksize=config["basecaller"]["chunksize"],
             quantize=config["basecaller"]["quantize"],
         )
 
     state_dict = torch.load(model_file, map_location=device)
@@ -415,7 +414,26 @@
             consensus, coverage, status = batch.get_consensus()
             results.extend(consensus)
 
             batch.reset()
             group_status, seq_status = batch.add_poa_group(group)
 
     return results
+
+def tqdm_environ():
+    """Get tqdm settings from environment variables"""
+    kwargs = {}
+    try:
+        interval = os.getenv("BONITO_PBAR_INTERVAL", None)
+        if interval is not None:
+            kwargs.update(dict(mininterval=float(interval), maxinterval=float(interval)))
+    except ValueError as exc:
+        logger.warning(f"Couldn't parse BONITO_PBAR_INTERVAL as float - {exc}")
+
+    try:
+        disable = os.getenv("BONITO_PBAR_DISABLE", None)
+        if disable is not None:
+            kwargs.update(dict(disable=bool(int(disable))))
+    except ValueError as exc:
+        logger.warning(f"couldn't parse BONITO_PBAR_DISABLE as bool - {exc}")
+
+    return kwargs
```

### Comparing `ont-bonito-0.7.3/ont_bonito.egg-info/PKG-INFO` & `ont-bonito-0.8.1/ont_bonito.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,109 @@
 Metadata-Version: 2.1
 Name: ont-bonito
-Version: 0.7.3
+Version: 0.8.1
 Home-page: https://github.com/nanoporetech/bonito
 Author: Oxford Nanopore Technologies, Ltd
 Author-email: support@nanoporetech.com
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: cu118
+Provides-Extra: cu121
 License-File: LICENCE.txt
 
 # Bonito
 
-[![PyPI version](https://badge.fury.io/py/ont-bonito.svg)](https://badge.fury.io/py/ont-bonito) 
+[![PyPI version](https://badge.fury.io/py/ont-bonito.svg)](https://badge.fury.io/py/ont-bonito)
 [![py38](https://img.shields.io/badge/python-3.8-brightgreen.svg)](https://img.shields.io/badge/python-3.8-brightgreen.svg)
 [![py39](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://img.shields.io/badge/python-3.9-brightgreen.svg)
 [![py310](https://img.shields.io/badge/python-3.10-brightgreen.svg)](https://img.shields.io/badge/python-3.10-brightgreen.svg)
 [![py311](https://img.shields.io/badge/python-3.11-brightgreen.svg)](https://img.shields.io/badge/python-3.11-brightgreen.svg)
-[![cu117](https://img.shields.io/badge/cuda-11.7-blue.svg)](https://img.shields.io/badge/cuda-11.7-blue.svg)
+[![cu118](https://img.shields.io/badge/cuda-11.8-blue.svg)](https://img.shields.io/badge/cuda-11.8-blue.svg)
 
 Bonito is an open source research basecaller for Oxford Nanopore reads.
 
 For anything other than basecaller training or method development please use [dorado](https://github.com/nanoporetech/dorado).
 
 ```bash
 $ pip install --upgrade pip
 $ pip install ont-bonito
-$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v4.0.0 /data/reads > basecalls.bam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 /data/reads > basecalls.bam
 ```
 
 Bonito supports writing aligned/unaligned `{fastq, sam, bam, cram}`.
 
 ```bash
-$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v4.0.0 --reference reference.mmi /data/reads > basecalls.bam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 --reference reference.mmi /data/reads > basecalls.bam
 ```
 
 Bonito will download and cache the basecalling model automatically on first use but all models can be downloaded with -
 
 ``` bash
 $ bonito download --models --show  # show all available models
 $ bonito download --models         # download all available models
 ```
 
+## Transformer Models
+
+The `bonito.transformer` package requires
+[flash-attn](https://github.com/Dao-AILab/flash-attention?tab=readme-ov-file#installation-and-features).
+
+This must be manually installed as the `flash-attn` packaging system prevents it from being listed as a normal dependency.
+
+Setting `CUDA_HOME` to the relevant library directory will help avoid CUDA version mismatches between packages.
+
 ## Modified Bases
 
 Modified base calling is handled by [Remora](https://github.com/nanoporetech/remora).
 
 ```bash
-$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v4.0.0 /data/reads --modified-bases 5mC --reference ref.mmi > basecalls_with_mods.bam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 /data/reads --modified-bases 5mC --reference ref.mmi > basecalls_with_mods.bam
 ```
 
 See available modified base models with the ``remora model list_pretrained`` command.
 
 ## Training your own model
 
 To train a model using your own reads, first basecall the reads with the additional `--save-ctc` flag and use the output directory as the input directory for training.
 
 ```bash
-$ bonito basecaller dna_r9.4.1 --save-ctc --reference reference.mmi /data/reads > /data/training/ctc-data/basecalls.sam
+$ bonito basecaller dna_r10.4.1_e8.2_400bps_hac@v5.0.0 --save-ctc --reference reference.mmi /data/reads > /data/training/ctc-data/basecalls.sam
 $ bonito train --directory /data/training/ctc-data /data/training/model-dir
 ```
 
-In addition to training a new model from scratch you can also easily fine tune one of the pretrained models.  
+In addition to training a new model from scratch you can also easily fine tune one of the pretrained models.
 
 ```bash
-bonito train --epochs 1 --lr 5e-4 --pretrained dna_r10.4.1_e8.2_400bps_hac@v4.0.0 --directory /data/training/ctc-data /data/training/fine-tuned-model
+bonito train --epochs 1 --lr 5e-4 --pretrained dna_r10.4.1_e8.2_400bps_hac@v5.0.0 --directory /data/training/ctc-data /data/training/fine-tuned-model
 ```
 
 If you are interested in method development and don't have you own set of reads then a pre-prepared set is provide.
 
 ```bash
 $ bonito download --training
 $ bonito train /data/training/model-dir
 ```
 
-All training calls use Automatic Mixed Precision to speed up training. To disable this, set the `--no-amp` flag to True. 
+All training calls use Automatic Mixed Precision to speed up training. To disable this, set the `--no-amp` flag to True.
 
 ## Developer Quickstart
 
 ```bash
 $ git clone https://github.com/nanoporetech/bonito.git  # or fork first and clone that
 $ cd bonito
 $ python3 -m venv venv3
 $ source venv3/bin/activate
 (venv3) $ pip install --upgrade pip
-(venv3) $ pip install -e .
+(venv3) $ pip install -e .[cu118] --extra-index-url https://download.pytorch.org/whl/cu118
 ```
 
+The `ont-bonito[cu118]` and `ont-bonito[cu121]` optional dependencies can be used, along
+with the corresponding `--extra-index-url`, to ensure the PyTorch package matches the
+local CUDA setup.
+
 ## Interface
 
  - `bonito view` - view a model architecture for a given `.toml` file and the number of parameters in the network.
  - `bonito train` - train a bonito model.
  - `bonito evaluate` - evaluate a model performance.
  - `bonito download` - download pretrained models and training datasets.
  - `bonito basecaller` - basecaller *(`.fast5` -> `.bam`)*.
@@ -105,7 +121,20 @@
 Technologies, Ltd.  Public License, v. 1.0.  If a copy of the License
 was not distributed with this file, You can obtain one at
 http://nanoporetech.com
 
 ### Research Release
 
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
+
+### Citation
+
+```
+@software{bonito,
+  title = {Bonito: A PyTorch Basecaller for Oxford Nanopore Reads},
+  author = {{Chris Seymour, Oxford Nanopore Technologies Ltd.}},
+  year = {2019},
+  url = {https://github.com/nanoporetech/bonito},
+  note = {Oxford Nanopore Technologies, Ltd. Public License, v. 1.0},
+  abstract = {Bonito is an open source research basecaller for Oxford Nanopore reads. It provides a flexible platform for training and developing basecalling models using PyTorch.}
+}
+```
```

### Comparing `ont-bonito-0.7.3/ont_bonito.egg-info/SOURCES.txt` & `ont-bonito-0.8.1/ont_bonito.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 bonito/pod5.py
 bonito/reader.py
 bonito/schedule.py
 bonito/training.py
 bonito/util.py
 bonito/cli/__init__.py
 bonito/cli/basecaller.py
-bonito/cli/convert.py
 bonito/cli/download.py
 bonito/cli/duplex.py
 bonito/cli/evaluate.py
 bonito/cli/export.py
 bonito/cli/train.py
 bonito/cli/view.py
 bonito/crf/__init__.py
@@ -33,14 +32,19 @@
 bonito/ctc/basecall.py
 bonito/ctc/model.py
 bonito/data/README.md
 bonito/models/README.md
 bonito/models/configs/dna_r9.4.1@v1.toml
 bonito/models/configs/dna_r9.4.1@v2.toml
 bonito/models/configs/dna_r9.4.1@v3.toml
-bonito/transformer/rote.py
+bonito/transformer/__init__.py
+bonito/transformer/basecall.py
+bonito/transformer/model.py
 ont_bonito.egg-info/PKG-INFO
 ont_bonito.egg-info/SOURCES.txt
 ont_bonito.egg-info/dependency_links.txt
 ont_bonito.egg-info/entry_points.txt
 ont_bonito.egg-info/requires.txt
-ont_bonito.egg-info/top_level.txt
+ont_bonito.egg-info/top_level.txt
+test/__init__.py
+test/test_cli.py
+test/test_download.py
```

