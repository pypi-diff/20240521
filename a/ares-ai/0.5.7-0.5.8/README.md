# Comparing `tmp/ares_ai-0.5.7.tar.gz` & `tmp/ares_ai-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ares_ai-0.5.7.tar", last modified: Tue May  7 04:44:37 2024, max compression
+gzip compressed data, was "ares_ai-0.5.8.tar", last modified: Tue May 21 12:11:56 2024, max compression
```

## Comparing `ares_ai-0.5.7.tar` & `ares_ai-0.5.8.tar`

### file list

```diff
@@ -1,102 +1,100 @@
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.896593 ares_ai-0.5.7/
--rw-rw-rw-   0 manihani (23549) future   (20099)     5064 2024-05-07 01:11:49.000000 ares_ai-0.5.7/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.5.7/CHANGELOG.md
--rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.5.7/LICENSE
--rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.5.7/MANIFEST.in
--rw-r--r--   0 manihani (23549) future   (20099)    27877 2024-05-07 04:44:37.895593 ares_ai-0.5.7/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)    12338 2024-05-07 04:39:23.000000 ares_ai-0.5.7/README.md
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.753600 ares_ai-0.5.7/ares/
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.765599 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/
--rw-rw-rw-   0 manihani (23549) future   (20099)     6952 2024-04-26 08:46:18.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    29888 2024-04-28 07:14:55.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    25648 2024-04-26 09:23:11.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    17172 2024-04-26 08:52:43.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__init__.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.786598 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)     4441 2024-04-26 08:48:35.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9231 2024-05-07 02:24:59.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    16781 2024-04-28 07:17:44.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    37386 2024-05-07 02:24:59.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    11077 2024-04-26 09:25:16.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    21777 2024-05-07 02:24:37.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9237 2024-04-26 08:55:30.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    17731 2024-05-07 02:24:59.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      175 2024-05-07 02:24:37.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.801597 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/
--rw-rw-rw-   0 manihani (23549) future   (20099)    34416 2024-05-07 02:25:28.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    46672 2024-05-06 07:40:45.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     7091 2024-04-30 23:25:14.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     8000 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__init__.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.829596 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)    12031 2024-05-07 03:12:34.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    32115 2024-05-07 02:30:43.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    23567 2024-05-06 07:41:23.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    49640 2024-05-07 02:25:02.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    19694 2024-05-07 02:25:08.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     4250 2024-04-30 23:25:39.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9532 2024-05-07 02:25:08.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      174 2024-05-07 02:25:02.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     8966 2024-04-24 01:01:00.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    19175 2024-05-07 02:25:02.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/__init__.py
--rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.5.7/ares/__init__.pyc
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.858595 ares_ai-0.5.7/ares/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.5.7/ares/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      196 2024-05-07 02:24:37.000000 ares_ai-0.5.7/ares/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7721 2024-05-07 03:42:06.000000 ares_ai-0.5.7/ares/__pycache__/ares.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    10977 2024-05-07 02:55:57.000000 ares_ai-0.5.7/ares/__pycache__/ares.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4163 2024-04-24 11:55:12.000000 ares_ai-0.5.7/ares/__pycache__/binary_classifier.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7124 2024-05-07 02:24:59.000000 ares_ai-0.5.7/ares/__pycache__/binary_classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.5.7/ares/__pycache__/kilt_filter.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      469 2024-05-07 02:25:08.000000 ares_ai-0.5.7/ares/__pycache__/kilt_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2509 2024-05-04 10:00:37.000000 ares_ai-0.5.7/ares/__pycache__/rag_scoring.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     3941 2024-05-07 02:25:02.000000 ares_ai-0.5.7/ares/__pycache__/rag_scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.5.7/ares/__pycache__/superglue_filter.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      442 2024-05-07 02:25:08.000000 ares_ai-0.5.7/ares/__pycache__/superglue_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2419 2024-04-26 07:58:28.000000 ares_ai-0.5.7/ares/__pycache__/synthetic_generator.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     3518 2024-05-07 02:24:37.000000 ares_ai-0.5.7/ares/__pycache__/synthetic_generator.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     5123 2024-05-07 03:50:35.000000 ares_ai-0.5.7/ares/__pycache__/ues_idp.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    10990 2024-05-07 03:18:13.000000 ares_ai-0.5.7/ares/__pycache__/ues_idp.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    11926 2024-05-07 03:41:04.000000 ares_ai-0.5.7/ares/ares.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.869594 ares_ai-0.5.7/ares/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.5.7/ares/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.5.7/ares/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.5.7/ares/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.5.7/ares/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.5.7/ares/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.5.7/ares/ares_ai.egg-info/top_level.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)     8082 2024-04-24 11:17:32.000000 ares_ai-0.5.7/ares/binary_classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/kilt_filter.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.873594 ares_ai-0.5.7/ares/ppi/
--rw-rw-rw-   0 manihani (23549) future   (20099)     6148 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/ppi/.DS_Store
--rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/ppi/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     9196 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/ppi/ppi_testing.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     6220 2024-05-04 09:59:26.000000 ares_ai-0.5.7/ares/rag_scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.5.7/ares/superglue_filter.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     4332 2024-04-26 07:54:48.000000 ares_ai-0.5.7/ares/synthetic_generator.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    13832 2024-05-07 03:50:01.000000 ares_ai-0.5.7/ares/ues_idp.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.893593 ares_ai-0.5.7/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    27877 2024-05-07 04:44:32.000000 ares_ai-0.5.7/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)     4221 2024-05-07 04:44:37.000000 ares_ai-0.5.7/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-05-07 04:44:32.000000 ares_ai-0.5.7/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-05-07 04:44:32.000000 ares_ai-0.5.7/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      682 2024-05-07 04:44:32.000000 ares_ai-0.5.7/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-05-07 04:44:32.000000 ares_ai-0.5.7/ares_ai.egg-info/top_level.txt
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.889593 ares_ai-0.5.7/checkpoints/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:34.000000 ares_ai-0.5.7/checkpoints/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)     2905 2024-05-07 03:52:24.000000 ares_ai-0.5.7/pyproject.toml
--rw-rw-rw-   0 manihani (23549) future   (20099)     5066 2024-04-26 03:07:42.000000 ares_ai-0.5.7/requirements.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-05-07 04:44:37.898593 ares_ai-0.5.7/setup.cfg
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-07 04:44:37.891593 ares_ai-0.5.7/tests/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.5.7/tests/.gitignore
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.356146 ares_ai-0.5.8/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5118 2024-05-21 10:25:44.000000 ares_ai-0.5.8/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.5.8/CHANGELOG.md
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.5.8/LICENSE
+-rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.5.8/MANIFEST.in
+-rw-r--r--   0 manihani (23549) future   (20099)    28486 2024-05-21 12:11:56.355147 ares_ai-0.5.8/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)    12916 2024-05-21 10:19:09.000000 ares_ai-0.5.8/README.md
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:55.671177 ares_ai-0.5.8/ares/
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:55.729175 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10726 2024-05-15 09:28:04.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    39458 2024-05-20 03:54:50.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    26352 2024-05-16 09:44:16.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    27757 2024-05-15 04:45:07.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__init__.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:55.855169 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7375 2024-05-15 22:43:28.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9231 2024-05-07 02:24:59.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    27821 2024-05-20 22:16:50.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    37386 2024-05-07 02:24:59.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    19424 2024-05-16 10:41:36.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    21777 2024-05-07 02:24:37.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    18303 2024-05-15 07:02:35.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    17731 2024-05-07 02:24:59.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      175 2024-05-07 02:24:37.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:55.951165 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    55776 2024-05-15 03:08:44.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    65743 2024-05-21 11:18:53.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-05-18 12:00:35.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7091 2024-04-30 23:25:14.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__init__.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.109158 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    31119 2024-05-15 03:09:09.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    32115 2024-05-07 02:30:43.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    39819 2024-05-21 11:24:33.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    49640 2024-05-07 02:25:02.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    19694 2024-05-07 02:25:08.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     4250 2024-04-30 23:25:39.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9532 2024-05-07 02:25:08.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      174 2024-05-07 02:25:02.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      172 2024-05-07 22:44:26.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/counter.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    17791 2024-05-21 10:44:15.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    19175 2024-05-07 02:25:02.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    21593 2024-05-21 10:43:03.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/ppi.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/__init__.py
+-rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.5.8/ares/__init__.pyc
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.239152 ares_ai-0.5.8/ares/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.5.8/ares/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      196 2024-05-07 02:24:37.000000 ares_ai-0.5.8/ares/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     8166 2024-05-21 06:03:02.000000 ares_ai-0.5.8/ares/__pycache__/ares.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10977 2024-05-07 02:55:57.000000 ares_ai-0.5.8/ares/__pycache__/ares.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5615 2024-05-15 22:43:28.000000 ares_ai-0.5.8/ares/__pycache__/binary_classifier.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7124 2024-05-07 02:24:59.000000 ares_ai-0.5.8/ares/__pycache__/binary_classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.5.8/ares/__pycache__/kilt_filter.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      469 2024-05-07 02:25:08.000000 ares_ai-0.5.8/ares/__pycache__/kilt_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     1908 2024-05-13 22:37:10.000000 ares_ai-0.5.8/ares/__pycache__/prompts.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     4799 2024-05-21 06:06:29.000000 ares_ai-0.5.8/ares/__pycache__/rag_scoring.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     3941 2024-05-07 02:25:02.000000 ares_ai-0.5.8/ares/__pycache__/rag_scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.5.8/ares/__pycache__/superglue_filter.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      442 2024-05-07 02:25:08.000000 ares_ai-0.5.8/ares/__pycache__/superglue_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4330 2024-05-16 10:41:36.000000 ares_ai-0.5.8/ares/__pycache__/synthetic_generator.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     3518 2024-05-07 02:24:37.000000 ares_ai-0.5.8/ares/__pycache__/synthetic_generator.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9413 2024-05-15 09:11:08.000000 ares_ai-0.5.8/ares/__pycache__/ues_idp.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10990 2024-05-07 03:18:13.000000 ares_ai-0.5.8/ares/__pycache__/ues_idp.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11647 2024-05-21 06:01:01.000000 ares_ai-0.5.8/ares/ares.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.316148 ares_ai-0.5.8/ares/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/top_level.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8374 2024-05-15 22:27:43.000000 ares_ai-0.5.8/ares/binary_classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/kilt_filter.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     1862 2024-05-13 05:25:48.000000 ares_ai-0.5.8/ares/prompts.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8433 2024-05-21 06:06:15.000000 ares_ai-0.5.8/ares/rag_scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/superglue_filter.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5844 2024-05-16 09:46:01.000000 ares_ai-0.5.8/ares/synthetic_generator.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    15573 2024-05-15 09:10:54.000000 ares_ai-0.5.8/ares/ues_idp.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.349147 ares_ai-0.5.8/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    28486 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4238 2024-05-21 12:11:55.000000 ares_ai-0.5.8/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      698 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/top_level.txt
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.343147 ares_ai-0.5.8/checkpoints/
+-rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:34.000000 ares_ai-0.5.8/checkpoints/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2929 2024-05-21 10:28:26.000000 ares_ai-0.5.8/pyproject.toml
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5082 2024-05-19 01:32:03.000000 ares_ai-0.5.8/requirements.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-05-21 12:11:56.359146 ares_ai-0.5.8/setup.cfg
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.346147 ares_ai-0.5.8/tests/
+-rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.5.8/tests/.gitignore
```

### Comparing `ares_ai-0.5.7/.gitignore` & `ares_ai-0.5.8/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -201,7 +201,8 @@
 synthetic_queries_1.tsv
 add.py
 change.py
 few_shot_example.tsv
 filter_v4.py
 filter_v5.py
 package_test.py
+ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
```

### Comparing `ares_ai-0.5.7/LICENSE` & `ares_ai-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/PKG-INFO` & `ares_ai-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.5.7
+Version: 0.5.8
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,14 +218,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate<1.0.0,>=0.21.0
 Requires-Dist: anthropic>=0.25.7
 Requires-Dist: Cython>=0.29.35
 Requires-Dist: datasets>=2.12.0
+Requires-Dist: evaluate==0.4.2
 Requires-Dist: fastapi==0.110.2
 Requires-Dist: faiss-cpu>=1.8.0
 Requires-Dist: ipywidgets<9.0.0,>=8.0.6
 Requires-Dist: ipython<9.0.0,>=8.12.2
 Requires-Dist: ipykernel<7.0.0,>=6.23.1
 Requires-Dist: joblib<2.0.0,>=1.2.0
 Requires-Dist: matplotlib<4.0.0,>=3.7.1
@@ -374,15 +375,15 @@
 
 <hr>
 
 To get started with ARES's PPI, you'll need to set up your configuration. Below is an example of a configuration for ARES!
 
 Just copy-paste as you go to see ARES in action!
 
-#### Step 1) Run the following to retrive the UES/IDP scores with GPT3.5!
+#### Step 1) Run the following to retrieve the UES/IDP scores with GPT3.5!
 
 ```python
 from ares import ARES
 
 ues_idp_config = {
     "in_domain_prompts_dataset": "nq_few_shot_prompt_for_judge_scoring.tsv",
     "unlabeled_evaluation_set": "nq_unlabeled_output.tsv", 
@@ -472,36 +473,52 @@
 
 ares = ARES(classifier_model=classifier_config)
 results = ares.train_classifier()
 print(results)
 ```
 
 Note: This code creates a checkpoint for the trained classifier.
-Training may take some time. You can download the checkpoint here:
-[Download Checkpoint](https://drive.google.com/file/d/1dsUzL01a53ictjMaUI6RqEvHY5vColcL/view?usp=sharing)
+Training may take some time. You can download our jointly trained checkpoint on context relevance here!:
+[Download Checkpoint](https://drive.google.com/file/d/15poFyeoqdnaNZVjl41HllL2213DKyZjH/view?usp=sharing)
+
+Alternatively, you can download our jointly trained checkpoint on answer relevance here! Be sure to change the parameters in the config to match the label "Answer_Relevance_Label"
+[Download Checkpoint](https://drive.google.com/file/d/1wGcgELBfnCGqXlPEbpPmf7LJ53DPWVXI/view?usp=sharing)
+
 
 <hr>
 
 #### Step 4) Run the following to see ARES's PPI in action!
 ```python
 
 from ares import ARES
 
 ppi_config = { 
     "evaluation_datasets": ['nq_unlabeled_output.tsv'], 
-    "few_shot_examples_filepath": "nq_few_shot_prompt_for_judge_scoring.tsv",
     "checkpoints": ["Context_Relevance_Label_nq_labeled_output_date_time.pt"], 
     "rag_type": "question_answering", 
     "labels": ["Context_Relevance_Label"], 
     "gold_label_path": "nq_labeled_output.tsv", 
 }
 
 ares = ARES(ppi=ppi_config)
 results = ares.evaluate_RAG()
 print(results)
+
+# Output Should be: 
+""" 
+Context_Relevance_Label Scoring
+ARES Ranking
+ARES Prediction: [0.6056978059262574]
+ARES Confidence Interval: [[0.547, 0.664]]
+Number of Examples in Evaluation Set: [4421]
+Ground Truth Performance: [0.6]
+ARES LLM Judge Accuracy on Ground Truth Labels: [0.789]
+Annotated Examples used for PPI: 300
+"""
+
 ```
 
 <br>
 
 ### 🚀 Local Model Execution with vLLM
 
 ARES supports [vLLM](https://github.com/vllm-project/vllm), allowing for local execution of LLM models, offering enhanced privacy and the ability to operate ARES offline. Below are steps to vLLM for ARES's UES/IDP and PPI!
@@ -509,15 +526,15 @@
 #### 1) UES/IDP w/ vLLM
 
 ```python
 from ares import ARES
 
 ues_idp_config = {
     "in_domain_prompts_dataset": "nq_few_shot_prompt_for_judge_scoring.tsv",
-    "unlabeled_evaluation_set": "nq_unalebed_output.tsv", 
+    "unlabeled_evaluation_set": "nq_unlabeled_output.tsv", 
     "model_choice": "meta-llama/Llama-2-13b-hf", # Specify vLLM model
     "vllm": True, # Toggle vLLM to True 
     "host_url": "http://0.0.0.0:8000/v1" # Replace with server hosting model followed by "/v1"
 } 
 
 ares = ARES(ues_idp=ues_idp_config)
 results = ares.ues_idp()
```

### Comparing `ares_ai-0.5.7/README.md` & `ares_ai-0.5.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 <hr>
 
 To get started with ARES's PPI, you'll need to set up your configuration. Below is an example of a configuration for ARES!
 
 Just copy-paste as you go to see ARES in action!
 
-#### Step 1) Run the following to retrive the UES/IDP scores with GPT3.5!
+#### Step 1) Run the following to retrieve the UES/IDP scores with GPT3.5!
 
 ```python
 from ares import ARES
 
 ues_idp_config = {
     "in_domain_prompts_dataset": "nq_few_shot_prompt_for_judge_scoring.tsv",
     "unlabeled_evaluation_set": "nq_unlabeled_output.tsv", 
@@ -219,36 +219,52 @@
 
 ares = ARES(classifier_model=classifier_config)
 results = ares.train_classifier()
 print(results)
 ```
 
 Note: This code creates a checkpoint for the trained classifier.
-Training may take some time. You can download the checkpoint here:
-[Download Checkpoint](https://drive.google.com/file/d/1dsUzL01a53ictjMaUI6RqEvHY5vColcL/view?usp=sharing)
+Training may take some time. You can download our jointly trained checkpoint on context relevance here!:
+[Download Checkpoint](https://drive.google.com/file/d/15poFyeoqdnaNZVjl41HllL2213DKyZjH/view?usp=sharing)
+
+Alternatively, you can download our jointly trained checkpoint on answer relevance here! Be sure to change the parameters in the config to match the label "Answer_Relevance_Label"
+[Download Checkpoint](https://drive.google.com/file/d/1wGcgELBfnCGqXlPEbpPmf7LJ53DPWVXI/view?usp=sharing)
+
 
 <hr>
 
 #### Step 4) Run the following to see ARES's PPI in action!
 ```python
 
 from ares import ARES
 
 ppi_config = { 
     "evaluation_datasets": ['nq_unlabeled_output.tsv'], 
-    "few_shot_examples_filepath": "nq_few_shot_prompt_for_judge_scoring.tsv",
     "checkpoints": ["Context_Relevance_Label_nq_labeled_output_date_time.pt"], 
     "rag_type": "question_answering", 
     "labels": ["Context_Relevance_Label"], 
     "gold_label_path": "nq_labeled_output.tsv", 
 }
 
 ares = ARES(ppi=ppi_config)
 results = ares.evaluate_RAG()
 print(results)
+
+# Output Should be: 
+""" 
+Context_Relevance_Label Scoring
+ARES Ranking
+ARES Prediction: [0.6056978059262574]
+ARES Confidence Interval: [[0.547, 0.664]]
+Number of Examples in Evaluation Set: [4421]
+Ground Truth Performance: [0.6]
+ARES LLM Judge Accuracy on Ground Truth Labels: [0.789]
+Annotated Examples used for PPI: 300
+"""
+
 ```
 
 <br>
 
 ### 🚀 Local Model Execution with vLLM
 
 ARES supports [vLLM](https://github.com/vllm-project/vllm), allowing for local execution of LLM models, offering enhanced privacy and the ability to operate ARES offline. Below are steps to vLLM for ARES's UES/IDP and PPI!
@@ -256,15 +272,15 @@
 #### 1) UES/IDP w/ vLLM
 
 ```python
 from ares import ARES
 
 ues_idp_config = {
     "in_domain_prompts_dataset": "nq_few_shot_prompt_for_judge_scoring.tsv",
-    "unlabeled_evaluation_set": "nq_unalebed_output.tsv", 
+    "unlabeled_evaluation_set": "nq_unlabeled_output.tsv", 
     "model_choice": "meta-llama/Llama-2-13b-hf", # Specify vLLM model
     "vllm": True, # Toggle vLLM to True 
     "host_url": "http://0.0.0.0:8000/v1" # Replace with server hosting model followed by "/v1"
 } 
 
 ares = ARES(ues_idp=ues_idp_config)
 results = ares.ues_idp()
```

#### html2text {}

```diff
@@ -62,15 +62,15 @@
 our quick start guide, we rename nq_ratio_0.5 to nq_unlabeled_output and
 nq_labeled_output. ```
 ===============================================================================
 ### ð Quick Start - #1
 ===============================================================================
 To get started with ARES's PPI, you'll need to set up your configuration. Below
 is an example of a configuration for ARES! Just copy-paste as you go to see
-ARES in action! #### Step 1) Run the following to retrive the UES/IDP scores
+ARES in action! #### Step 1) Run the following to retrieve the UES/IDP scores
 with GPT3.5! ```python from ares import ARES ues_idp_config =
 { "in_domain_prompts_dataset": "nq_few_shot_prompt_for_judge_scoring.tsv",
 "unlabeled_evaluation_set": "nq_unlabeled_output.tsv", "model_choice" : "gpt-
 3.5-turbo-0125" } ares = ARES(ues_idp=ues_idp_config) results = ares.ues_idp()
 print(results) # {'Context Relevance Scores': [Score], 'Answer Faithfulness
 Scores': [Score], 'Answer Relevance Scores': [Score]} ``` #### Step 2) Run the
 following to retrive ARES's PPI scores with GPT3.5! ```python ppi_config =
@@ -102,32 +102,40 @@
 ```python from ares import ARES classifier_config = { "training_dataset":
 ["synthetic_queries_1.tsv"], "validation_set": ["nq_labeled_output.tsv"],
 "label_column": ["Context_Relevance_Label"], "num_epochs": 10,
 "patience_value": 3, "learning_rate": 5e-6, "assigned_batch_size": 1,
 "gradient_accumulation_multiplier": 32, } ares = ARES
 (classifier_model=classifier_config) results = ares.train_classifier() print
 (results) ``` Note: This code creates a checkpoint for the trained classifier.
-Training may take some time. You can download the checkpoint here: [Download
-Checkpoint](https://drive.google.com/file/d/1dsUzL01a53ictjMaUI6RqEvHY5vColcL/
-view?usp=sharing)
+Training may take some time. You can download our jointly trained checkpoint on
+context relevance here!: [Download Checkpoint](https://drive.google.com/file/d/
+15poFyeoqdnaNZVjl41HllL2213DKyZjH/view?usp=sharing) Alternatively, you can
+download our jointly trained checkpoint on answer relevance here! Be sure to
+change the parameters in the config to match the label "Answer_Relevance_Label"
+[Download Checkpoint](https://drive.google.com/file/d/
+1wGcgELBfnCGqXlPEbpPmf7LJ53DPWVXI/view?usp=sharing)
 ===============================================================================
 #### Step 4) Run the following to see ARES's PPI in action! ```python from ares
 import ARES ppi_config = { "evaluation_datasets": ['nq_unlabeled_output.tsv'],
-"few_shot_examples_filepath": "nq_few_shot_prompt_for_judge_scoring.tsv",
 "checkpoints": ["Context_Relevance_Label_nq_labeled_output_date_time.pt"],
 "rag_type": "question_answering", "labels": ["Context_Relevance_Label"],
 "gold_label_path": "nq_labeled_output.tsv", } ares = ARES(ppi=ppi_config)
-results = ares.evaluate_RAG() print(results) ```
+results = ares.evaluate_RAG() print(results) # Output Should be: """
+Context_Relevance_Label Scoring ARES Ranking ARES Prediction:
+[0.6056978059262574] ARES Confidence Interval: [[0.547, 0.664]] Number of
+Examples in Evaluation Set: [4421] Ground Truth Performance: [0.6] ARES LLM
+Judge Accuracy on Ground Truth Labels: [0.789] Annotated Examples used for PPI:
+300 """ ```
 ### ð Local Model Execution with vLLM ARES supports [vLLM](https://
 github.com/vllm-project/vllm), allowing for local execution of LLM models,
 offering enhanced privacy and the ability to operate ARES offline. Below are
 steps to vLLM for ARES's UES/IDP and PPI! #### 1) UES/IDP w/ vLLM ```python
 from ares import ARES ues_idp_config = { "in_domain_prompts_dataset":
 "nq_few_shot_prompt_for_judge_scoring.tsv", "unlabeled_evaluation_set":
-"nq_unalebed_output.tsv", "model_choice": "meta-llama/Llama-2-13b-hf", #
+"nq_unlabeled_output.tsv", "model_choice": "meta-llama/Llama-2-13b-hf", #
 Specify vLLM model "vllm": True, # Toggle vLLM to True "host_url": "http://
 0.0.0.0:8000/v1" # Replace with server hosting model followed by "/v1" } ares =
 ARES(ues_idp=ues_idp_config) results = ares.ues_idp() print(results) ```
 ===============================================================================
 #### 2) PPI w/ vLLM ```python from ares import ARES ppi_config =
 { "evaluation_datasets": ['nq_unabeled_output.tsv'],
 "few_shot_examples_filepath": "nq_few_shot_prompt_for_judge_scoring.tsv",
```

### Comparing `ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py` & `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,457 +1,541 @@
-import requests
-import time
-import pandas as pd
+import argparse
 import ast
-import json
 import copy
-import openai
-from tqdm import tqdm
 import csv
-from datasets import Dataset
-from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, AutoConfig, AutoModelForCausalLM, BitsAndBytesConfig
-import torch
-import numpy as np
-from sklearn.model_selection import train_test_split
-import re
-import argparse
+import json
 import pdb
+import re
+import requests
 import sys
+import time
 import warnings
 
-from ares.LLM_as_a_Judge_Adaptation.LLM_Generation_Functions import generate_synthetic_query_openai_approach, generate_answer_from_context, generate_contradictory_answer_from_context
-from ares.LLM_as_a_Judge_Adaptation.LLM_Generation_Functions import check_generated_answer, generate_contradictory_answer_examples, generate_synthetic_query_llm_approach, generate_answer_llm_approach
-
-from ares.LLM_as_a_Judge_Adaptation.Filter_Synthetic_Queries import get_embedding, generate_index, filter_synthetic_queries, generate_additional_negatives, generate_additional_positives
-#from Instruction_Finetune import instruction_finetune
-#from Instruction_Finetune_V2 import instruction_finetune_v2
-#from Instruction_Finetune_v3 import instruction_finetune_v3
-
-pd.set_option('display.max_columns', None)  # Show all columns - TEST
-pd.set_option('display.max_rows', None)  # Show all rows - TEST
-pd.set_option('display.max_colwidth', None)  # Show full content of each column - TEST
-
-#################################################
+import numpy as np
+import openai
+import pandas as pd
+import torch
+from datasets import Dataset
+from sklearn.model_selection import train_test_split
+from tqdm import tqdm
+from transformers import (AutoConfig, AutoModelForCausalLM, AutoModelForSeq2SeqLM,
+                          AutoTokenizer, BitsAndBytesConfig)
 
-def clean_document(document: str):
-    cleaned_document = re.sub(r'\n+', '\n', document.replace("\r"," ").replace("\t"," ")).strip()
+from ares.LLM_as_a_Judge_Adaptation.Filter_Synthetic_Queries import (filter_synthetic_queries,
+                                                                      generate_additional_negatives,
+                                                                      generate_additional_positives,
+                                                                      generate_index, get_embedding)
+from ares.LLM_as_a_Judge_Adaptation.LLM_Generation_Functions import (check_generated_answer,
+                                                                      generate_answer_from_context,
+                                                                      generate_answer_llm_approach,
+                                                                      generate_contradictory_answer_examples,
+                                                                      generate_contradictory_answer_from_context,
+                                                                      generate_synthetic_query_llm_approach,
+                                                                      generate_synthetic_query_openai_approach)
+
+pd.set_option('display.max_columns', None) 
+pd.set_option('display.max_rows', None)  
+pd.set_option('display.max_colwidth', None) 
+
+def clean_document(document: str) -> str:
+    """
+    Cleans the input document by removing unnecessary whitespace characters and replacing certain punctuation.
+
+    Args:
+        document (str): The original document text that needs to be cleaned.
+
+    Returns:
+        str: The cleaned document text.
+    """
+    # Replace carriage returns and tabs with a space, and reduce multiple newlines to a single newline
+    cleaned_document = re.sub(r'\n+', '\n', document.replace("\r", " ").replace("\t", " ")).strip()
+    # Replace equals signs and hyphens with spaces
     cleaned_document = cleaned_document.replace("=", " ").replace("-", " ")
+    # Reduce multiple spaces to a single space
     cleaned_document = re.sub(r'\s+', ' ', cleaned_document).strip()
-    cleaned_document = (" ").join(cleaned_document.split(" ")) #[:512]
+    # Join words with a single space (this line seems redundant and could be removed if confirmed)
+    cleaned_document = (" ").join(cleaned_document.split(" "))  # [:512] - this part is commented out and can be ignored or removed
     return cleaned_document
 
-    # Load model for synthetic query generation 
-
-def validate_input_file(df, required_columns) -> bool: 
+def validate_input_file(df: pd.DataFrame, required_columns: list[str]) -> bool:
+    """
+    Validates that the DataFrame contains all required columns. Exits the program if any are missing.
+
+    Args:
+        df (pd.DataFrame): The DataFrame to validate.
+        required_columns (List[str]): A list of strings representing the column names that are required in the DataFrame.
+
+    Returns:
+        bool: True if the DataFrame contains all required columns, otherwise the program will exit with an error.
+    """
+    # Identify any missing columns
     missing_columns = [col for col in required_columns if col not in df.columns]
+    # Exit the program with an error message if there are missing columns
     if missing_columns:
         sys.exit(f"Error: The DataFrame is missing the following required column(s): {', '.join(missing_columns)}.")
-############
+    return True
 
-def load_model(flan_approach, model_choice):
-    if flan_approach:
-        tokenizer = AutoTokenizer.from_pretrained(model_choice)
-        model = AutoModelForSeq2SeqLM.from_pretrained(model_choice)
-
-        torch.no_grad()
-        model.eval()
-
-        device = "cuda:0"
-        device = torch.device(device)
-        model.to(device)
+def load_model(model_choice: str) -> tuple:
+    """
+    Loads the specified model and tokenizer, and sets the model to evaluation mode on the appropriate device.
+
+    Args:
+        model_choice (str): The model identifier to load from the Hugging Face model hub.
+
+    Returns:
+        tuple: A tuple containing the model, tokenizer, and device.
+    """
+    # Load the tokenizer and model from the specified model choice
+    tokenizer = AutoTokenizer.from_pretrained(model_choice)
+    model = AutoModelForSeq2SeqLM.from_pretrained(model_choice)
+
+    # Disable gradient calculations and set the model to evaluation mode
+    torch.no_grad()
+    model.eval()
+
+    # Set the device to CUDA if available
+    device = torch.device("cuda:0")
+    model.to(device)
+    
     return model, tokenizer, device
 
-#############
-
-# Load documents for synthetic query and answer generation
-def load_documents(document_filepath, clean_documents, documents_sampled):
+def load_documents(document_filepath: str, clean_documents: bool, documents_sampled: int) -> pd.DataFrame:
+    """
+    Loads and processes documents for synthetic query and answer generation.
+
+    Args:
+        document_filepath (str): The path to the document file.
+        clean_documents (bool): Flag indicating whether to clean the documents.
+        documents_sampled (int): The number of documents to sample.
+
+    Returns:
+        pd.DataFrame: A DataFrame containing the processed documents.
+    """
     documents = []
     required_columns = ['Query', 'Document', 'Answer']
 
     if "docs_aws" in document_filepath:
-
         with open(document_filepath, "r") as json_file:
             json_data = json.load(json_file)
             documents = [x['text'] for x in json_data]
 
             # Clean document
             if clean_documents:
                 documents = [clean_document(text) for text in documents]
 
         documents = pd.DataFrame(documents, columns=["document"])
-
     else:
         if not document_filepath.endswith('.tsv'):
             sys.exit(f"Error: The file {document_filepath} is not a TSV file.")
         try:
             documents = pd.read_csv(document_filepath, sep="\t")
             validate_input_file(documents, required_columns)
             documents.rename(columns={"Document": "document"}, inplace=True)
             documents['document'] = documents['document'].str.strip()
         except Exception as e:
             sys.exit(f"Error reading the file {document_filepath}: {e}")
 
-
     initial_count = len(documents)
-    documents = documents[documents['document'].str.split().apply(len) >= 50] # Filter documents w/ less than 50 words.
+    documents = documents[documents['document'].str.split().apply(len) >= 50]  # Filter documents with less than 50 words.
     after_filter_count = len(documents)
 
     count = initial_count - after_filter_count
 
-    if(after_filter_count == 0): 
-        sys.exit(f"All documents were less than 50 words, please provide dataset with documents containing more than 50 words")
+    if after_filter_count == 0:
+        sys.exit("All documents were less than 50 words, please provide a dataset with documents containing more than 50 words.")
 
     if documents_sampled > initial_count:
         print(f"\nThe `documents_sampled` parameter ({documents_sampled}) exceeds the available number of documents ({initial_count}). Sampling will be adjusted to the maximum available documents ({initial_count}).\n")
         documents_sampled = initial_count
 
-    if count > 0: 
-        print(f"Filtered out {count} documents because they had less than 50 words. Sampling will be be adjusted to {after_filter_count} documents\n")
-        documents_sampled = after_filter_count
-
-    documents = documents.sample(n=documents_sampled, random_state=43)
-
-    #documents = documents[:10]
-    # print("documents") - CHANGED
-    # print(len(documents)) - CHANGED
-    # print(documents.head()) - CHANGED
-    return documents
+    if count > 0:
+        print(f"Filtered out {count} documents because they had less than 50 words.")
+        if documents_sampled > after_filter_count: 
+            print(f"Document sample is greater than document count. Sampling will be adjusted to {after_filter_count} documents\n")
+            documents_sampled = after_filter_count
+
+    documents = documents.sample(n=documents_sampled)
 
-################
+    return documents
 
-# Load few-shot prompt
-def load_few_shot_prompt(few_shot_prompt_filename,for_fever_dataset,for_wow_dataset):
+def load_few_shot_prompt(few_shot_prompt_filename: str, for_fever_dataset: bool, for_wow_dataset: bool) -> tuple[str, int]:
+    """
+    Loads and processes a few-shot prompt from a TSV file.
+
+    Args:
+        few_shot_prompt_filename (str): The filename of the TSV file containing the few-shot prompts.
+        for_fever_dataset (bool): Flag indicating if the prompts are for the FEVER dataset.
+        for_wow_dataset (bool): Flag indicating if the prompts are for the WoW dataset.
+
+    Returns:
+        tuple[str, int]: A tuple containing the few-shot examples as a string and the length of the few-shot prompt.
+    """
     few_shot_prompt = pd.read_csv(few_shot_prompt_filename, sep="\t")
     few_shot_prompt = few_shot_prompt[few_shot_prompt['Context_Relevance_Label'] == "[[Yes]]"]
+    
     if "Query" not in few_shot_prompt:
         few_shot_prompt['Query'] = few_shot_prompt['Question']
 
     length_of_fewshot_prompt = len(few_shot_prompt)
     few_shot_examples = ""
+
     for row in range(len(few_shot_prompt)):
-        few_shot_examples += "Example " + str(row + 1) + ":\n"
-        few_shot_examples += "Document: " + clean_document(few_shot_prompt.iloc[row]['Document']) + "\n"
+        few_shot_examples += f"Example {row + 1}:\n"
+        few_shot_examples += f"Document: {clean_document(few_shot_prompt.iloc[row]['Document'])}\n"
+        
         if for_fever_dataset:
-            few_shot_examples += "Statement: " + few_shot_prompt.iloc[row]['Query'] + "\n\n"
+            few_shot_examples += f"Statement: {few_shot_prompt.iloc[row]['Query']}\n\n"
         elif for_wow_dataset:
-            few_shot_examples += "Dialogue: " + few_shot_prompt.iloc[row]['Query'] + "\n\n"
+            few_shot_examples += f"Dialogue: {few_shot_prompt.iloc[row]['Query']}\n\n"
         else:
-            few_shot_examples += "Question: " + few_shot_prompt.iloc[row]['Query'] + "\n\n"
+            few_shot_examples += f"Question: {few_shot_prompt.iloc[row]['Query']}\n\n"
 
-    # print("Fewshot Prompt") - CHANGED
-    # print(few_shot_examples) - CHANGED 
-    # print("Finished loading dataset + model") - CHANGED
     return few_shot_examples, length_of_fewshot_prompt
 
-#################################################
-def generate_contradictory_answers(few_shot_prompt_filename,generate_contradictory_answers_with_flan,for_fever_dataset,for_wow_dataset): 
+def generate_contradictory_answers(few_shot_prompt_filename: str, for_fever_dataset: bool, for_wow_dataset: bool) -> str:
+    """
+    Generates few-shot examples for contradictory answers based on the provided dataset.
+
+    Args:
+        few_shot_prompt_filename (str): The filename of the TSV file containing the few-shot prompts.
+        for_fever_dataset (bool): Flag indicating if the prompts are for the FEVER dataset.
+        for_wow_dataset (bool): Flag indicating if the prompts are for the WoW dataset.
+
+    Returns:
+        str: A string containing the few-shot examples for contradictory answers.
+    """
+    # Load the few-shot prompt data
     few_shot_prompt_for_contradictory_answers = pd.read_csv(few_shot_prompt_filename, sep="\t")
-    few_shot_prompt_for_contradictory_answers = few_shot_prompt_for_contradictory_answers[few_shot_prompt_for_contradictory_answers['Contradictory_Answer'].str.len() > 4]
+    few_shot_prompt_for_contradictory_answers = few_shot_prompt_for_contradictory_answers[
+        few_shot_prompt_for_contradictory_answers['Contradictory_Answer'].str.len() > 4
+    ]
+
+    # Initialize the few-shot examples string
+    few_shot_examples_for_contradictory_answers = ""
+
+    for row in range(len(few_shot_prompt_for_contradictory_answers)):
+        few_shot_examples_for_contradictory_answers += f"Example {row + 1}:\n"
+        few_shot_examples_for_contradictory_answers += f"Document: {few_shot_prompt_for_contradictory_answers.iloc[row]['Document']}\n"
+        
+        if for_fever_dataset:
+            few_shot_examples_for_contradictory_answers += f"Statement: {few_shot_prompt_for_contradictory_answers.iloc[row]['Query']}\n"
+            few_shot_examples_for_contradictory_answers += f"Incorrect Answer: {few_shot_prompt_for_contradictory_answers.iloc[row]['Contradictory_Answer']}\n\n"
+        elif for_wow_dataset:
+            few_shot_examples_for_contradictory_answers += f"Dialogue: {few_shot_prompt_for_contradictory_answers.iloc[row]['Query']}\n"
+            few_shot_examples_for_contradictory_answers += f"Incorrect Response: {few_shot_prompt_for_contradictory_answers.iloc[row]['Contradictory_Answer']}\n\n"
+        else:
+            few_shot_examples_for_contradictory_answers += f"Question: {few_shot_prompt_for_contradictory_answers.iloc[row]['Query']}\n"
+            few_shot_examples_for_contradictory_answers += f"Incorrect Answer: {few_shot_prompt_for_contradictory_answers.iloc[row]['Contradictory_Answer']}\n\n"
 
-    if generate_contradictory_answers_with_flan:
-        few_shot_examples_for_contradictory_answers = ""
-        for row in range(len(few_shot_prompt_for_contradictory_answers)):
-            few_shot_examples_for_contradictory_answers += "Example " + str(row + 1) +":\n"
-            few_shot_examples_for_contradictory_answers += "Document: " + few_shot_prompt_for_contradictory_answers.iloc[row]['Document'] + "\n"
-            if for_fever_dataset:
-                few_shot_examples_for_contradictory_answers += "Statement: " + few_shot_prompt_for_contradictory_answers.iloc[row]['Query'] + "\n"
-                few_shot_examples_for_contradictory_answers += "Incorrect Answer: " + few_shot_prompt_for_contradictory_answers.iloc[row]['Contradictory_Answer'] + "\n\n"
-            elif for_wow_dataset:
-                few_shot_examples_for_contradictory_answers += "Dialogue: " + few_shot_prompt_for_contradictory_answers.iloc[row]['Query'] + "\n"
-                few_shot_examples_for_contradictory_answers += "Incorrect Response: " + few_shot_prompt_for_contradictory_answers.iloc[row]['Contradictory_Answer'] + "\n\n"
-            else:
-                few_shot_examples_for_contradictory_answers += "Question: " + few_shot_prompt_for_contradictory_answers.iloc[row]['Query'] + "\n"
-                few_shot_examples_for_contradictory_answers += "Incorrect Answer: " + few_shot_prompt_for_contradictory_answers.iloc[row]['Contradictory_Answer'] + "\n\n"
     return few_shot_examples_for_contradictory_answers
 
-def generate_few_shot_prompts(few_shot_prompt_filename,for_fever_dataset,for_wow_dataset):
+def generate_few_shot_prompts(few_shot_prompt_filename: str, for_fever_dataset: bool, for_wow_dataset: bool) -> tuple[str, int]:
+    """
+    Generates few-shot prompts for answer generation based on the provided dataset.
+
+    Args:
+        few_shot_prompt_filename (str): The filename of the TSV file containing the few-shot prompts.
+        for_fever_dataset (bool): Flag indicating if the prompts are for the FEVER dataset.
+        for_wow_dataset (bool): Flag indicating if the prompts are for the WoW dataset.
+
+    Returns:
+        tuple: A tuple containing the few-shot examples string and the length of the few-shot prompt.
+    """
+    # Load the few-shot prompt data
     answer_gen_few_shot_prompt = pd.read_csv(few_shot_prompt_filename, sep="\t")
-    answer_gen_few_shot_prompt = answer_gen_few_shot_prompt[answer_gen_few_shot_prompt['Answer_Relevance_Label'] == "[[Yes]]"]
-    answer_gen_few_shot_prompt = answer_gen_few_shot_prompt[answer_gen_few_shot_prompt['Answer_Faithfulness_Label'] == "[[Yes]]"]
-    #answer_gen_few_shot_prompt = answer_gen_few_shot_prompt[:4]
+    
+    # Filter the prompts based on relevance and faithfulness labels
+    answer_gen_few_shot_prompt = answer_gen_few_shot_prompt[
+        (answer_gen_few_shot_prompt['Answer_Relevance_Label'] == "[[Yes]]") & 
+        (answer_gen_few_shot_prompt['Answer_Faithfulness_Label'] == "[[Yes]]")
+    ]
+    
+    # Get the length of the few-shot prompt
     length_of_fewshot_prompt_answer_gen = len(answer_gen_few_shot_prompt)
+    
+    # Rename 'Query' column to 'Question' if it exists
     if "Query" in answer_gen_few_shot_prompt.columns:
         answer_gen_few_shot_prompt['Question'] = answer_gen_few_shot_prompt['Query']
-
+    
+    # Initialize the few-shot examples string
     answer_gen_few_shot_examples = ""
+    
+    # Construct the few-shot examples
     for row in range(len(answer_gen_few_shot_prompt)):
-        answer_gen_few_shot_examples += "Example " + str(row + 1) +":\n"
-        answer_gen_few_shot_examples += "Document: " + answer_gen_few_shot_prompt.iloc[row]['Document'] + "\n"
+        answer_gen_few_shot_examples += f"Example {row + 1}:\n"
+        answer_gen_few_shot_examples += f"Document: {answer_gen_few_shot_prompt.iloc[row]['Document']}\n"
+        
         if for_fever_dataset:
-            answer_gen_few_shot_examples += "Statement: " + answer_gen_few_shot_prompt.iloc[row]['Query'] + "\n"
-            answer_gen_few_shot_examples += "Answer: " + answer_gen_few_shot_prompt.iloc[row]['Answer'] + "\n\n"
+            answer_gen_few_shot_examples += f"Statement: {answer_gen_few_shot_prompt.iloc[row]['Query']}\n"
+            answer_gen_few_shot_examples += f"Answer: {answer_gen_few_shot_prompt.iloc[row]['Answer']}\n\n"
         elif for_wow_dataset:
-            answer_gen_few_shot_examples += "Dialogue: " + answer_gen_few_shot_prompt.iloc[row]['Query'] + "\n"
-            answer_gen_few_shot_examples += "Response: " + answer_gen_few_shot_prompt.iloc[row]['Answer'] + "\n\n"
+            answer_gen_few_shot_examples += f"Dialogue: {answer_gen_few_shot_prompt.iloc[row]['Query']}\n"
+            answer_gen_few_shot_examples += f"Response: {answer_gen_few_shot_prompt.iloc[row]['Answer']}\n\n"
         else:
-            answer_gen_few_shot_examples += "Question: " + answer_gen_few_shot_prompt.iloc[row]['Query'] + "\n"
-            answer_gen_few_shot_examples += "Answer: " + answer_gen_few_shot_prompt.iloc[row]['Answer'] + "\n\n"
-
-    # print("answer_gen_few_shot_examples") - CHANGED
-    # print(answer_gen_few_shot_examples) - CHANGED
+            answer_gen_few_shot_examples += f"Question: {answer_gen_few_shot_prompt.iloc[row]['Query']}\n"
+            answer_gen_few_shot_examples += f"Answer: {answer_gen_few_shot_prompt.iloc[row]['Answer']}\n\n"
+    
     return answer_gen_few_shot_examples, length_of_fewshot_prompt_answer_gen
 
-##############################
-
- # Save Synthetic Queries
-def save_synthetic_queries(documents, regenerate_synth_questions, flan_approach, few_shot_examples, 
-    length_of_fewshot_prompt, device, tokenizer, model, percentiles, for_fever_dataset, for_wow_dataset, 
-    synthetic_query_prompt, synthetic_queries_filename, question_temperatures): 
-
-    # print("documents") - CHANGED 
-    # print(len(documents)) - CHANGED
-    # print(documents.head()) - CHANGED
-
-    if regenerate_synth_questions:
-        print("Beginning synthetic query generation!")
-        tqdm.pandas(desc="Generating synthetic queries...", total=documents.shape[0])
-        if flan_approach:
-            # Testing
-            # subset_documents = documents.head(10)  #
-            # subset_documents["synthetic_query"] = subset_documents.apply(lambda x: generate_synthetic_query_llm_approach(x["document"], few_shot_examples, length_of_fewshot_prompt, device, tokenizer, model, percentiles, for_fever_dataset=for_fever_dataset, for_wow_dataset=for_wow_dataset), axis=1)
-            # print(subset_documents[["document", "synthetic_query"]])
-            # breakpoint()
-            # synthetic_query = generate_synthetic_query_llm_approach(test_doc["document"], few_shot_examples, length_of_fewshot_prompt, device, tokenizer, model, percentiles, for_fever_dataset=for_fever_dataset, for_wow_dataset=for_wow_dataset) #
-            # print(synthetic_query)
-            documents["synthetic_query"] = documents.progress_apply(lambda x: generate_synthetic_query_llm_approach(x["document"], few_shot_examples, length_of_fewshot_prompt, device, tokenizer, model, percentiles, for_fever_dataset=for_fever_dataset, for_wow_dataset=for_wow_dataset), axis=1)
-        else:
-            documents["synthetic_query"] = documents.progress_apply(lambda x: generate_synthetic_query_openai_approach(x["document"], synthetic_query_prompt, few_shot_examples, question_temperatures, length_of_fewshot_prompt), axis=1)
-        documents = documents.explode("synthetic_query", ignore_index=True)
-        documents = documents.drop_duplicates(subset=['synthetic_query'])
-        documents.to_csv(synthetic_queries_filename, index=False, sep="\t")
-        print("Saved synthetic queries to: " + synthetic_queries_filename)
-
-################################################
-
-# Generate synthetic queries and their answers for training set
-def Generate_Synthetic_Answers(synthetic_queries_filename,
-    regenerate_answers, flan_approach, answer_gen_few_shot_examples, length_of_fewshot_prompt_answer_gen, 
-    device, tokenizer, model, for_fever_dataset, for_wow_dataset, generate_contradictory_answers_with_flan,
-    few_shot_examples_for_contradictory_answers, number_of_negatives_added_ratio,
-    lower_bound_for_negatives, number_of_contradictory_answers_added_ratio, number_of_positives_added_ratio, regenerate_embeddings): 
-    synth_queries = pd.read_csv(synthetic_queries_filename, sep="\t")
-    # print("Filtered synth queries")
-    # print(len(synth_queries))
-    synth_queries = synth_queries[synth_queries["synthetic_query"].str.len() > 10]
-    # print(len(synth_queries))
-
-    if regenerate_answers:
-        print("Beginning answer generation!")
-        
-        tqdm.pandas(desc="Generating answers...", total=synth_queries.shape[0])
-        if flan_approach:
-            synth_queries["generated_answer"] = synth_queries.progress_apply(lambda x: generate_answer_llm_approach(x["document"], x["synthetic_query"], answer_gen_few_shot_examples, length_of_fewshot_prompt_answer_gen, device, tokenizer, model, for_fever_dataset=for_fever_dataset, for_wow_dataset=for_wow_dataset), axis=1)
-        else:
-            synth_queries["generated_answer"] = synth_queries.progress_apply(lambda x: generate_answer_from_context(x["document"], x["synthetic_query"]), axis=1)
-        synth_queries.to_csv(synthetic_queries_filename, index=False, sep="\t")
-        print("Saved answers to: " + synthetic_queries_filename)
+def generate_query(document: str, settings: dict) -> list:
+    """
+    Generates synthetic queries for a given document.
+
+    Args:
+        document (str): The document text.
+        settings (dict): Dictionary containing various settings and parameters required for generating synthetic queries.
+
+    Returns:
+        list: List of generated synthetic queries.
+    """
+    return generate_synthetic_query_llm_approach(
+        document, 
+        settings['few_shot_examples'], 
+        settings['length_of_fewshot_prompt'], 
+        settings['device'], 
+        settings['tokenizer'], 
+        settings['model'], 
+        settings['percentiles'], 
+        settings['for_fever_dataset'], 
+        settings['for_wow_dataset']
+    )
+
+def process_documents(documents: pd.DataFrame, settings: dict) -> pd.DataFrame:
+    """
+    Processes the documents to generate synthetic queries and remove duplicates.
+
+    Args:
+        documents (pd.DataFrame): DataFrame containing the documents.
+        settings (dict): Dictionary containing various settings and parameters required for generating synthetic queries.
+
+    Returns:
+        pd.DataFrame: DataFrame containing the documents with the generated synthetic queries.
+    """
+    tqdm.pandas(desc="Generating synthetic queries (FLAN)...", total=documents.shape[0])
+    documents["synthetic_query"] = documents.progress_apply(
+        lambda x: generate_query(x["document"], settings), axis=1
+    )
+    documents = documents.explode("synthetic_query", ignore_index=True)
+    documents = documents.drop_duplicates(subset=['synthetic_query'])
+    return documents
 
-        #################################################
+def save_synthetic_queries(documents: pd.DataFrame, filename: str) -> None:
+    """
+    Saves the generated synthetic queries to a TSV file.
+
+    Args:
+        documents (pd.DataFrame): DataFrame containing the documents with the generated synthetic queries.
+        filename (str): Filename to save the generated synthetic queries.
+    """
+    documents.to_csv(filename, index=False, sep="\t")
+    print("Saved synthetic queries to: " + filename)
+
+def generate_synthetic_queries(documents: pd.DataFrame, settings: dict) -> pd.DataFrame:
+    """
+    Generate synthetic queries using the FLAN approach.
+
+    Args:
+        documents (pd.DataFrame): DataFrame containing the documents for which synthetic queries are to be generated.
+        settings (dict): Dictionary containing various settings and parameters required for generating synthetic queries.
+
+    Returns:
+        pd.DataFrame: DataFrame containing the documents with the generated synthetic queries.
+    """
+    print("Beginning synthetic query generation!")
+    documents = process_documents(documents, settings)
+    save_synthetic_queries(documents, settings['synthetic_queries_filename'])
+    return documents
 
-        #  for idx, row in synth_queries.iterrows():
-        #     print(f"Document: {row['document']}\nSynthetic Query: {row['synthetic_query']}\nGenerated Answer: {row['generated_answer']}\n---\n")
-        # breakpoint()
+def generate_answers(synthetic_queries: pd.DataFrame, answer_generation_settings: dict) -> pd.DataFrame:
+    """
+    Generate synthetic answers using the FLAN approach.
+
+    Args:
+        synthetic_queries (pd.DataFrame): DataFrame containing the synthetic queries.
+        answer_generation_settings (dict): Dictionary containing settings and parameters for answer generation.
+
+    Returns:
+        pd.DataFrame: DataFrame containing the synthetic queries with generated answers.
+    """
+    tqdm.pandas(desc="Generating answers...", total=synthetic_queries.shape[0])
+    
+    synthetic_queries["generated_answer"] = synthetic_queries.progress_apply(
+        lambda x: generate_answer_llm_approach(
+            x["document"], 
+            x["synthetic_query"], 
+            answer_generation_settings['answer_gen_few_shot_examples'], 
+            answer_generation_settings['length_of_fewshot_prompt_answer_gen'], 
+            answer_generation_settings['device'], 
+            answer_generation_settings['tokenizer'], 
+            answer_generation_settings['model'], 
+            answer_generation_settings['for_fever_dataset'], 
+            answer_generation_settings['for_wow_dataset']
+        ), 
+        axis=1
+    )
+    
+    return synthetic_queries
 
-        synth_queries["Answer_Faithfulness_Label"] = [check_generated_answer(synth_queries.iloc[i]['generated_answer']) for i in range(len(synth_queries))]
-        synth_queries["Answer_Relevance_Label"] = [check_generated_answer(synth_queries.iloc[i]['generated_answer']) for i in range(len(synth_queries))]
-        print("Generating contradictory answers!")
-        if generate_contradictory_answers_with_flan:
-            synth_queries = generate_contradictory_answer_examples(synth_queries, int(len(synth_queries) * number_of_contradictory_answers_added_ratio), few_shot_examples_for_contradictory_answers=few_shot_examples_for_contradictory_answers, device=device, tokenizer=tokenizer, model=model, for_fever_dataset=for_fever_dataset, for_wow_dataset=for_wow_dataset)
-        else:
-            synth_queries = generate_contradictory_answer_examples(synth_queries, int(len(synth_queries) * number_of_contradictory_answers_added_ratio))
-        # print(synth_queries.columns)  # List all column names to understand the structure
-        # print(synth_queries.head()) 
-        synth_queries.to_csv(synthetic_queries_filename, index=False, sep="\t")
-        print("Saved answers to: " + synthetic_queries_filename)
+def label_answers(synthetic_queries: pd.DataFrame) -> pd.DataFrame:
+    """
+    Label the generated answers for faithfulness and relevance.
+
+    This function takes a DataFrame containing synthetic queries and their generated answers,
+    and labels each answer for faithfulness and relevance. The labels are added as new columns
+    in the DataFrame.
+
+    Args:
+        synthetic_queries (pd.DataFrame): DataFrame containing the synthetic queries and their generated answers.
+
+    Returns:
+        pd.DataFrame: DataFrame with additional columns for answer faithfulness and relevance labels.
+    """
+    # Label each generated answer for faithfulness
+    synthetic_queries["Answer_Faithfulness_Label"] = [
+        check_generated_answer(synthetic_queries.iloc[i]['generated_answer']) for i in range(len(synthetic_queries))
+    ]
+    
+    # Label each generated answer for relevance
+    synthetic_queries["Answer_Relevance_Label"] = [
+        check_generated_answer(synthetic_queries.iloc[i]['generated_answer']) for i in range(len(synthetic_queries))
+    ]
+    
+    return synthetic_queries
 
-    #################################################
+def generate_contradictory_answers_wrapper(synthetic_queries: pd.DataFrame, answer_generation_settings: dict) -> pd.DataFrame:
+    """
+    Generate contradictory answers using the specified approach.
+
+    This function generates contradictory answers for the given synthetic queries based on the provided settings.
+
+    Args:
+        synthetic_queries (pd.DataFrame): DataFrame containing the synthetic queries.
+        answer_generation_settings (dict): Dictionary containing settings for answer generation, including:
+            - 'number_of_contradictory_answers_added_ratio' (float): Ratio to determine the number of contradictory answers to add.
+            - 'few_shot_examples_for_contradictory_answers' (list): Few-shot examples for generating contradictory answers (if applicable).
+            - 'device' (str): Device to use for model inference.
+            - 'tokenizer' (transformers.PreTrainedTokenizer): Tokenizer for the model.
+            - 'model' (transformers.PreTrainedModel): Model to use for generating answers.
+            - 'for_fever_dataset' (bool): Flag indicating if the dataset is for FEVER.
+            - 'for_wow_dataset' (bool): Flag indicating if the dataset is for WoW.
+
+    Returns:
+        pd.DataFrame: DataFrame with added contradictory answers.
+    """
+    synthetic_queries = generate_contradictory_answer_examples(
+        synthetic_queries, 
+        int(len(synthetic_queries) * answer_generation_settings['number_of_contradictory_answers_added_ratio']), 
+        few_shot_examples_for_contradictory_answers=answer_generation_settings['few_shot_examples_for_contradictory_answers'], 
+        device=answer_generation_settings['device'], 
+        tokenizer=answer_generation_settings['tokenizer'], 
+        model=answer_generation_settings['model'], 
+        for_fever_dataset=answer_generation_settings['for_fever_dataset'], 
+        for_wow_dataset=answer_generation_settings['for_wow_dataset']
+    )
+    return synthetic_queries
+
+def process_embeddings(synthetic_queries: pd.DataFrame, answer_generation_settings: dict) -> pd.DataFrame:
+    """
+    Handle embedding generation and additional negatives/positives.
+
+    This function processes the embeddings for the synthetic queries based on the provided settings.
+    It generates an index, filters the synthetic queries, and adds additional negatives and positives.
+
+    Args:
+        synthetic_queries (pd.DataFrame): DataFrame containing the synthetic queries.
+        answer_generation_settings (dict): Dictionary containing settings for answer generation, including:
+            - 'regenerate_embeddings' (bool): Flag to determine if embeddings should be regenerated.
+            - 'number_of_negatives_added_ratio' (float): Ratio to determine the number of additional negatives to add.
+            - 'lower_bound_for_negatives' (int): Lower bound for the number of negatives.
+            - 'number_of_positives_added_ratio' (float): Ratio to determine the number of additional positives to add.
+
+    Returns:
+        pd.DataFrame: DataFrame with processed embeddings and additional negatives/positives.
+    """
+    if answer_generation_settings['regenerate_embeddings']:
+        print("Generating index and negatives!")
+        documentation_index = generate_index(synthetic_queries)
+        synthetic_queries = filter_synthetic_queries(synthetic_queries, documentation_index)
+        synthetic_queries = generate_additional_negatives(
+            synthetic_queries, 
+            documentation_index, 
+            answer_generation_settings['number_of_negatives_added_ratio'], 
+            answer_generation_settings['lower_bound_for_negatives']
+        )
+        synthetic_queries = generate_additional_positives(
+            synthetic_queries, 
+            documentation_index, 
+            answer_generation_settings['number_of_positives_added_ratio']
+        )
+    return synthetic_queries
+
+def shuffle_and_save(synthetic_queries: pd.DataFrame, synthetic_queries_filename: str) -> None:
+    """
+    Shuffle and save the synthetic queries to a specified file.
+
+    This function shuffles the rows of the synthetic queries DataFrame and saves the result to a file in TSV format.
+
+    Args:
+        synthetic_queries (pd.DataFrame): The DataFrame containing synthetic queries to be shuffled and saved.
+        synthetic_queries_filename (str): The filename where the shuffled synthetic queries will be saved.
+
+    Returns:
+        None
+    """
+    # Shuffle the synthetic queries DataFrame with a fixed random state for reproducibility
+    synthetic_queries = synthetic_queries.sample(n=len(synthetic_queries), random_state=42)
+    
+    # Save the shuffled DataFrame to a TSV file without the index
+    synthetic_queries.to_csv(synthetic_queries_filename, index=False, sep="\t")
+    
+    # Print completion messages
+    print("Completed synthetic generation!")
+    print(f"Saved synthetic queries file to: {synthetic_queries_filename}")
 
+def Generate_Synthetic_Answers(synthetic_queries_filename: str, answer_generation_settings: dict) -> None:
+    """
+    Main function to generate and save synthetic answers.
+
+    This function reads synthetic queries from a file, processes them to generate answers,
+    labels, and contradictory answers, and then saves the results back to the file. It also
+    processes embeddings and shuffles the synthetic queries before saving.
+
+    Args:
+        synthetic_queries_filename (str): The filename where the synthetic queries are stored.
+        answer_generation_settings (dict): Dictionary containing settings for answer generation, including:
+            - 'regenerate_answers' (bool): Flag to determine if answers should be regenerated.
+            - 'regenerate_embeddings' (bool): Flag to determine if embeddings should be regenerated.
+            - 'number_of_negatives_added_ratio' (float): Ratio to determine the number of additional negatives to add.
+            - 'lower_bound_for_negatives' (int): Lower bound for the number of negatives.
+            - 'number_of_positives_added_ratio' (float): Ratio to determine the number of additional positives to add.
+
+    Returns:
+        None
+    """
+    # Read the synthetic queries from the specified file
     synth_queries = pd.read_csv(synthetic_queries_filename, sep="\t")
+    # Filter out queries with a length of 10 or less
     synth_queries = synth_queries[synth_queries["synthetic_query"].str.len() > 10]
 
-    # print("synth_queries")
-    # print(len(synth_queries))
-    # print(synth_queries.head())
-    
-
-    if regenerate_embeddings:
-        print("Generating index and negatives!")
-        documentation_index = generate_index(synth_queries)
-        synth_queries = filter_synthetic_queries(synth_queries, documentation_index)
-        synth_queries = generate_additional_negatives(synth_queries, documentation_index, number_of_negatives_added_ratio, lower_bound_for_negatives)
-        synth_queries = generate_additional_positives(synth_queries, documentation_index, number_of_positives_added_ratio)
+    # Check if answers need to be regenerated
+    if answer_generation_settings['regenerate_answers']:
+        print("Beginning answer generation!")
+        # Generate answers for the synthetic queries
+        synth_queries = generate_answers(synth_queries, answer_generation_settings)
+        # Label the generated answers
+        synth_queries = label_answers(synth_queries)
+        print("Generating contradictory answers!")
+        # Generate contradictory answers
+        synth_queries = generate_contradictory_answers_wrapper(synth_queries, answer_generation_settings)
+        # Save the synthetic queries with answers back to the file
         synth_queries.to_csv(synthetic_queries_filename, index=False, sep="\t")
+        print(f"Saved answers to: {synthetic_queries_filename}")
 
-    #################################################
-
+    # Re-read the synthetic queries from the file
     synth_queries = pd.read_csv(synthetic_queries_filename, sep="\t")
+    # Filter out queries with a length of 10 or less
+    synth_queries = synth_queries[synth_queries["synthetic_query"].str.len() > 10]
 
-    #Shuffle queries
-    synth_queries = synth_queries.sample(n=len(synth_queries), random_state=42)
-
-    # print("Label Sets for each Metric")
-    # print(set(synth_queries['Context_Relevance_Label'].tolist()))
-    # print(set(synth_queries['Answer_Faithfulness_Label'].tolist()))
-    # print(set(synth_queries['Answer_Relevance_Label'].tolist()))
-
-    # print("synth_queries filtered")
-    # print(len(synth_queries))
-    # print(synth_queries.head())
-
-    # print("Positive and Negative Counts")
-    # print("Context Relevance")
-    # print(len(synth_queries[synth_queries['Context_Relevance_Label'] == "Yes"]))
-    # print(len(synth_queries[synth_queries['Context_Relevance_Label'] == "No"]))
-    # print("Answer Faithfulness")
-    # print(len(synth_queries[synth_queries['Answer_Faithfulness_Label'] == "Yes"]))
-    # print(len(synth_queries[synth_queries['Answer_Faithfulness_Label'] == "No"]))
-    # print("Answer Relevance")
-    # print(len(synth_queries[synth_queries['Answer_Relevance_Label'] == "Yes"]))
-    # print(len(synth_queries[synth_queries['Answer_Relevance_Label'] == "No"]))
-
-    synth_queries.to_csv(synthetic_queries_filename, index=False, sep="\t")
-    print("Completed synthetic generation!")
-    print("Saved synthetic queries file to: " + synthetic_queries_filename)
-
-# def print_synthetic_queries(filename): 
-#     queries = pd.read_csv(filename,sep='\t')
-    
-#     for index, row in queries.head(6).iterrows(): 
-#         print(f"Document {index}: {row['document']}")
-#         print(f"Synthetic Query: {row['synthetic_query']}")
-#         print(f"Answer: {row['generated_answer']}")
-#         print("-" * 50)
-
-# def synthetic_generator_config(document_filepath: str, few_shot_prompt_filename: str,
-#                                synthetic_queries_filename: str, documents_sampled: int,
-#                                flan_approach: bool = True, clean_documents: bool = False,
-#                                regenerate_synth_questions: bool = True, 
-#                                percentiles: list = [0.05, 0.25, 0.5, 0.95], 
-#                                question_temperatures: list = [2.0, 1.5, 1.0, 0.5, 0.0],
-#                                regenerate_answers: bool = True,
-#                                generate_contradictory_answers_with_flan: bool = True, 
-#                                number_of_negatives_added_ratio: float = 0.5, # Check whether can also be an int
-#                                lower_bound_for_negatives: int = 5, # Need to be an int value
-#                                number_of_contradictory_answers_added_ratio: float = 0.67, # Check whether can also be an int
-#                                number_of_positives_added_ratio: float = 0.0, # Check whether can also be an int
-#                                regenerate_embeddings: float = True, 
-#                                synthetic_query_prompt: str = "You are an expert question-answering system. You must create a question for the provided document. The question must be answerable within the context of the document.\n\n"
-#                                ): 
-#     for_fever_dataset = False
-#     if "fever" in document_filepath.lower():
-#         for_fever_dataset = True
-#     for_wow_dataset = False
-#     if "wow" in document_filepath.lower():
-#         for_wow_dataset = True
-
-#     model, model_choice, tokenizer, device = load_model(flan_approach)
-
-#     documents = load_documents(document_filepath, clean_documents, documents_sampled)
-
-#     few_shot_examples, length_of_fewshot_prompt = load_few_shot_prompt(few_shot_prompt_filename,for_fever_dataset,for_wow_dataset)
-
-#     few_shot_examples_for_contradictory_answers = generate_contradictory_answers(few_shot_prompt_filename,generate_contradictory_answers_with_flan,for_fever_dataset,for_wow_dataset)
-
-#     answer_gen_few_shot_examples, length_of_fewshot_prompt_answer_gen = generate_few_shot_prompts(few_shot_prompt_filename,for_fever_dataset,for_wow_dataset)
-
-#     save_synthetic_queries(documents, regenerate_synth_questions, flan_approach, few_shot_examples, 
-#     length_of_fewshot_prompt, device, tokenizer, model, percentiles, for_fever_dataset, for_wow_dataset, 
-#     synthetic_query_prompt, synthetic_queries_filename, question_temperatures)
-
-#     Generate_Synthetic_Queries_and_Answers(synthetic_queries_filename,
-#     regenerate_answers, flan_approach, answer_gen_few_shot_examples, length_of_fewshot_prompt_answer_gen, 
-#     device, tokenizer, model, for_fever_dataset, for_wow_dataset, generate_contradictory_answers_with_flan,
-#     few_shot_examples_for_contradictory_answers, number_of_negatives_added_ratio, lower_bound_for_negatives, number_of_contradictory_answers_added_ratio, number_of_positives_added_ratio, regenerate_embeddings)
-
-#     print_synthetic_queries(synthetic_queries_filename)
-
-#################################################
-
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser()
-
-    parser.add_argument("--document_filepath", type=str, required=True)
-    parser.add_argument("--few_shot_prompt_filename", type=str, required=True)
-    parser.add_argument("--synthetic_queries_filename", type=str, required=True)
-    parser.add_argument("--flan_approach", type=bool, default="True", required=False)
-    parser.add_argument("--documents_sampled", type=int, required=True)
-
-    args = parser.parse_args()
-
-    ### Instructions
-
-    document_filepath = args.document_filepath
-    few_shot_prompt_filename = args.few_shot_prompt_filename
-    synthetic_queries_filename = args.synthetic_queries_filename
-    flan_approach = args.flan_approach
-    if flan_approach == "True":
-        flan_approach = True 
-    else:
-        flan_approach = False
-    documents_sampled = args.documents_sampled
-
-    ########################################################
-
-    for_fever_dataset = False
-    if "fever" in document_filepath.lower():
-        for_fever_dataset = True
-    for_wow_dataset = False
-    if "wow" in document_filepath.lower():
-        for_wow_dataset = True
-
-    regenerate_synth_questions = True
-    regenerate_answers = True
-    regenerate_embeddings = True
-
-    lower_bound_for_negatives = 20
-    number_of_negatives_added_ratio = 0.5
-    number_of_positives_added_ratio = 0.0 #0.2
-    number_of_contradictory_answers_added_ratio = 0.67
-    clean_documents = False
-
-    question_temperatures = [2.0, 1.5, 1.0, 0.5, 0.0] #[2.0, 0.9, 0.7, 0.5]
-    percentiles = [0.05, 0.25, 0.5, 0.95] #[0.01, 0.05, 0.25, 0.5, 0.95]
-    clean_few_shot_prompt_docs = False
-
-    flan_approach = True
-    generate_contradictory_answers_with_flan = True
-
-    #################################################
-
-    synthetic_query_prompt = "You are an expert question-answering system. You must create a question for the provided document. The question must be answerable within the context of the document.\n\n"
-
-    print("------------------------------------------------------------")
-    print("Document File: " + document_filepath)
-    print("Synthetic File Path: " + synthetic_queries_filename)
-    print("number_of_negatives_added_ratio: " + str(number_of_negatives_added_ratio))
-    print("number_of_positives_added_ratio: " + str(number_of_positives_added_ratio))
-    print("number_of_contradictory_answers_added_ratio: " + str(number_of_contradictory_answers_added_ratio))
-    print("clean_documents: " + str(clean_documents))
-    print("question_temperatures: " + str(question_temperatures))
-    print("percentiles: " + str(percentiles))
-    print("lower_bound_for_negatives: " + str(lower_bound_for_negatives))
-    print("for_fever_dataset: " + str(for_fever_dataset))
-    print("for_wow_dataset: " + str(for_wow_dataset))
-    print("------------------------------------------------------------")
-
-    # model, model_choice, tokenizer, device = load_model(flan_approach)
-
-    # documents = load_documents(document_filepath, clean_documents)
-
-    # few_shot_examples, length_of_fewshot_prompt = load_few_shot_prompt(few_shot_prompt_filename,for_fever_dataset)
-
-    # few_shot_examples_for_contradictory_answers = generate_contradictory_answers(few_shot_prompt_filename)
-
-    # answer_gen_few_shot_examples, length_of_fewshot_prompt_answer_gen = generate_few_shot_prompts(few_shot_prompt_filename)
-
-    # save_synthetic_queries(documents, regenerate_synth_questions, flan_approach, few_shot_examples, 
-    # length_of_fewshot_prompt, device, tokenizer, model, percentiles, for_fever_dataset, for_wow_dataset, 
-    # synthetic_query_prompt, synthetic_queries_filename, question_temperatures)
-
-    # Generate_Synthetic_Queries_and_Answers(synthetic_queries_filename,
-    # regenerate_answers, flan_approach, answer_gen_few_shot_examples, length_of_fewshot_prompt_answer_gen, 
-    # device, tokenizer, model, for_fever_dataset, for_wow_dataset, generate_contradictory_answers_with_flan,
-    # number_of_contradictory_answers_added_ratio, few_shot_examples_for_contradictory_answers, number_of_negatives_added_ratio
-    # lower_bound_for_negatives, number_of_contradictory_answers_added_ratio, number_of_positives_added_ratio, regenerate_embeddings): 
-
-    ######################################################################
+    # Process embeddings for the synthetic queries
+    synth_queries = process_embeddings(synth_queries, answer_generation_settings)
+    # Shuffle and save the synthetic queries
+    shuffle_and_save(synth_queries, synthetic_queries_filename)
```

### Comparing `ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc` & `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc` & `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc` & `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc` & `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc` & `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py` & `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc` & `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/__pycache__/ares.cpython-311.pyc` & `ares_ai-0.5.8/ares/__pycache__/ares.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/__pycache__/binary_classifier.cpython-311.pyc` & `ares_ai-0.5.8/ares/__pycache__/binary_classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/__pycache__/rag_scoring.cpython-311.pyc` & `ares_ai-0.5.8/ares/__pycache__/rag_scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/__pycache__/synthetic_generator.cpython-311.pyc` & `ares_ai-0.5.8/ares/__pycache__/synthetic_generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/__pycache__/ues_idp.cpython-311.pyc` & `ares_ai-0.5.8/ares/__pycache__/ues_idp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.5.8/ares/ares_ai.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/ares_ai.egg-info/requires.txt` & `ares_ai-0.5.8/ares/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.7/ares/ues_idp.py` & `ares_ai-0.5.8/ares/ues_idp.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,244 +11,299 @@
 from ares.RAG_Automatic_Evaluation.Evaluation_Functions import few_shot_answer_relevance_scoring_togetherai
 from ares.RAG_Automatic_Evaluation.Evaluation_Functions import few_shot_context_relevance_scoring_claude 
 from ares.RAG_Automatic_Evaluation.Evaluation_Functions import few_shot_answer_faithfulness_scoring_claude
 from ares.RAG_Automatic_Evaluation.Evaluation_Functions import few_shot_answer_relevance_scoring_claude
 from ares.RAG_Automatic_Evaluation.Evaluation_Functions import few_shot_context_relevance_scoring_vllm
 from ares.RAG_Automatic_Evaluation.Evaluation_Functions import few_shot_answer_faithfulness_scoring_vllm
 from ares.RAG_Automatic_Evaluation.Evaluation_Functions import few_shot_answer_relevance_scoring_vllm
+failed_extraction_count = {'failed': 0}
 
 if 'ipykernel' in sys.modules:
     # We are in a Jupyter notebook or similar (uses IPython kernel)
     from tqdm.notebook import tqdm
 else:
     # We are in a regular Python environment (e.g., terminal or script)
     from tqdm import tqdm
 
-def ues_idp_config(in_domain_prompts_dataset: str, unlabeled_evaluation_set: str, context_relevance_system_prompt: str, answer_relevance_system_prompt: str, answer_faithfulness_system_prompt: str, debug_mode: bool, documents: int, model_choice: str, vllm: bool, host_url: str, request_delay: int) -> dict:
-    """Configures UES and IDP for evaluation"""
+def validate_inputs(vllm: bool, host_url: str, in_domain_prompts_dataset: str, unlabeled_evaluation_set: str, documents: int) -> tuple:
+    """
+    Validates the input parameters for the evaluation process.
+
+    Parameters:
+    vllm (bool): Indicates if vLLM is being used.
+    host_url (str): The URL of the host if vLLM is used.
+    in_domain_prompts_dataset (str): Path to the in-domain prompts dataset file.
+    unlabeled_evaluation_set (str): Path to the unlabeled evaluation set file.
+    documents (int): Number of documents to be processed.
+
+    Returns:
+    tuple: A tuple containing the in-domain prompts dataset and the unlabeled evaluation set as pandas DataFrames.
+
+    Raises:
+    ValueError: If the input parameters are not valid.
+    SystemExit: If the documents size is larger than the documents present in the unlabeled evaluation set.
+    """
 
-    # Check if both vllm and host_url are provided together
+    # Validate vLLM and host_url relationship
     if vllm and host_url == "None":
         raise ValueError("host_url must be provided if vllm is True.")
-    elif not vllm and host_url != "None": 
+    elif not vllm and host_url != "None":
         raise ValueError("vLLM must be set to True if host_url is provided")
-    
+
+    # Load in-domain prompts dataset if provided
     if in_domain_prompts_dataset is not None:
-            in_domain_prompts_dataset = pd.read_csv(in_domain_prompts_dataset, sep='\t')
+        in_domain_prompts_dataset = pd.read_csv(in_domain_prompts_dataset, sep='\t')
     else:
-        in_domain_prompts_dataset = None 
+        in_domain_prompts_dataset = None
 
+    # Load unlabeled evaluation set if provided
     if unlabeled_evaluation_set is not None:
         unlabeled_evaluation_set = pd.read_csv(unlabeled_evaluation_set, sep='\t')
     else:
         unlabeled_evaluation_set = None
-    if in_domain_prompts_dataset is None and unlabeled_evaluation_set is None: 
-        print(f"Error: UES and IDP are not provided")
+
+    # Check if both datasets are provided
+    if in_domain_prompts_dataset is None and unlabeled_evaluation_set is None:
+        print("Error: UES and IDP are not provided")
         exit()
-    if in_domain_prompts_dataset is None: 
-        print(f"Error: IDP is not provided")
+    if in_domain_prompts_dataset is None:
+        print("Error: IDP is not provided")
         exit()
-    if unlabeled_evaluation_set is None: 
-        print(f"Error: UES is not provided")
+    if unlabeled_evaluation_set is None:
+        print("Error: UES is not provided")
         exit()
 
-    if documents > len(unlabeled_evaluation_set): 
+    # Validate documents size
+    if documents > len(unlabeled_evaluation_set):
         sys.exit("Error: documents size passed in is larger than documents present in unlabeled evaluation set")
-    
-    if documents == 0: 
+
+    # Set documents to the length of the unlabeled evaluation set if documents is 0
+    if documents == 0:
         documents = len(unlabeled_evaluation_set)
 
-    # context_relevance_answers = unlabeled_evaluation_set["Context_Relevance_Label"].tolist()
-    # answer_relevance_answers = unlabeled_evaluation_set["Answer_Relevance_Label"].tolist()
-    # answer_faithfulness_answers = unlabeled_evaluation_set["Answer_Faithfulness_Label"].tolist()
+    return in_domain_prompts_dataset, unlabeled_evaluation_set
+
+def extract_query(row: pd.Series, in_domain_prompts_dataset: pd.DataFrame) -> tuple:
+    """
+    Extracts the query from a given row and determines the query identifier.
+
+    Parameters:
+    row (pd.Series): A row from the dataset containing the query or question.
+    in_domain_prompts_dataset (pd.DataFrame): The in-domain prompts dataset to check for the query identifier.
+
+    Returns:
+    tuple: A tuple containing the extracted query and the query identifier.
+
+    Raises:
+    SystemExit: If both 'Query' and 'Question' keys are missing in the given row.
+    """
+    try:
+        query = row['Query']
+    except KeyError:
+        query = row['Question']
+    
+    try:
+        _ = in_domain_prompts_dataset.iloc[0]['Query']
+        query_id = "Query"
+    except KeyError:
+        try:
+            _ = in_domain_prompts_dataset.iloc[0]['Question']
+            query_id = "Question"
+        except KeyError:
+            sys.exit("Both 'Query' and 'Question' keys are missing for the given row.")
+    
+    return query, query_id
+
+def score_row(row: pd.Series, 
+              in_domain_prompts_dataset: pd.DataFrame, 
+              context_relevance_system_prompt: str, 
+              answer_relevance_system_prompt: str, 
+              answer_faithfulness_system_prompt: str, 
+              model_choice: str, 
+              query_id: str, 
+              debug_mode: bool, 
+              request_delay: int, 
+              vllm: bool, 
+              host_url: str) -> tuple:
+    """
+    Scores a row based on context relevance, answer relevance, and answer faithfulness.
+
+    Parameters:
+    row (pd.Series): A row from the dataset containing the query, document, and answer.
+    in_domain_prompts_dataset (pd.DataFrame): The in-domain prompts dataset.
+    context_relevance_system_prompt (str): The system prompt for context relevance scoring.
+    answer_relevance_system_prompt (str): The system prompt for answer relevance scoring.
+    answer_faithfulness_system_prompt (str): The system prompt for answer faithfulness scoring.
+    model_choice (str): The model choice for scoring (e.g., "gpt", "claude").
+    query_id (str): The query identifier.
+    debug_mode (bool): Flag to enable or disable debug mode.
+    request_delay (int): The delay between requests.
+    vllm (bool): Flag to indicate if vllm is used.
+    host_url (str): The host URL for the scoring service.
+
+    Returns:
+    tuple: A tuple containing context score, answer relevance score, and answer faithfulness score.
+    """
+    query, query_id = extract_query(row, in_domain_prompts_dataset)
+    document = row['Document']
+    answer = row['Answer']
+
+    if vllm:
+        context_score = few_shot_context_relevance_scoring_vllm(
+            context_relevance_system_prompt, query, document, model_choice, query_id, debug_mode, host_url, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+        
+        if context_score == 0:
+            return 0, 0, 0
+        else:
+            answer_relevance_score = few_shot_answer_relevance_scoring_vllm(
+                answer_relevance_system_prompt, query, document, answer, model_choice, query_id, debug_mode, host_url, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+            answer_faithfulness_score = few_shot_answer_faithfulness_scoring_vllm(
+                answer_faithfulness_system_prompt, query, document, answer, model_choice, query_id, debug_mode, host_url, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+    else:
+        if "gpt" in model_choice:
+            context_score = few_shot_context_relevance_scoring(
+                context_relevance_system_prompt, query, document, model_choice, query_id, debug_mode, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+        elif "claude" in model_choice:
+            context_score = few_shot_context_relevance_scoring_claude(
+                context_relevance_system_prompt, query, document, model_choice, query_id, debug_mode, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+        else:
+            context_score = few_shot_context_relevance_scoring_togetherai(
+                context_relevance_system_prompt, query, document, model_choice, query_id, debug_mode, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+        
+        if context_score == 0:
+            return 0, 0, 0
+        else:
+            if "gpt" in model_choice:
+                answer_relevance_score = few_shot_answer_relevance_scoring(
+                    answer_relevance_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+                answer_faithfulness_score = few_shot_answer_faithfulness_scoring(
+                    answer_faithfulness_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+            elif "claude" in model_choice:
+                answer_relevance_score = few_shot_answer_relevance_scoring_claude(
+                    answer_relevance_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+                answer_faithfulness_score = few_shot_answer_faithfulness_scoring_claude(
+                    answer_faithfulness_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+            else:
+                answer_relevance_score = few_shot_answer_relevance_scoring_togetherai(
+                    answer_relevance_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+                answer_faithfulness_score = few_shot_answer_faithfulness_scoring_togetherai(
+                    answer_faithfulness_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, failed_extraction_count, in_domain_prompts_dataset)
+    
+    return context_score, answer_relevance_score, answer_faithfulness_score
+
+def evaluate_documents(
+    unlabeled_evaluation_set: pd.DataFrame, 
+    in_domain_prompts_dataset: str, 
+    context_relevance_system_prompt: str, 
+    answer_relevance_system_prompt: str, 
+    answer_faithfulness_system_prompt: str, 
+    model_choice: str, 
+    debug_mode: bool, 
+    request_delay: int, 
+    vllm: bool, 
+    host_url: str, 
+    documents: int
+) -> tuple[list[float], list[float], list[float]]:
+    """
+    Evaluates a subset of documents for context relevance, answer relevance, and answer faithfulness.
+
+    Parameters:
+    unlabeled_evaluation_set (pd.DataFrame): The dataset containing the documents to be evaluated.
+    in_domain_prompts_dataset (str): Path to the in-domain prompts dataset.
+    context_relevance_system_prompt (str): System prompt for context relevance scoring.
+    answer_relevance_system_prompt (str): System prompt for answer relevance scoring.
+    answer_faithfulness_system_prompt (str): System prompt for answer faithfulness scoring.
+    model_choice (str): The model choice for evaluation.
+    debug_mode (bool): Flag to enable or disable debug mode.
+    request_delay (int): Delay between requests in seconds.
+    vllm (bool): Flag to indicate if vllm is used.
+    host_url (str): The host URL for the model.
+    documents (int): Number of documents to evaluate.
+
+    Returns:
+    tuple: A tuple containing three lists - context relevance scores, answer relevance scores, and answer faithfulness scores.
+    """
     context_relevance_scores = []
     answer_relevance_scores = []
     answer_faithfulness_scores = []
 
-    required_columns = ['Query', 'Document', 'Answer']
-    missing_columns = [col for col in required_columns if col not in unlabeled_evaluation_set.columns]
-    if missing_columns:
-        print(f"Missing columns in the DataFrame: {missing_columns}")
-
-
-    if "gpt" in model_choice:
-        with tqdm(total=documents, desc=f"Evaluating large subset with {model_choice}") as pbar:
-            for index, row in unlabeled_evaluation_set[:documents].iterrows():
-                # Extract query, document, and answer from the row
-                try:
-                    query = row['Query']
-                except KeyError:
-                    query = row['Question']
-                
-                try:
-                    _ = in_domain_prompts_dataset.iloc[0]['Query']
-                    query_id = "Query"
-                except KeyError:
-                    try:
-                        _ = in_domain_prompts_dataset.iloc[0]['Question']
-                        query_id = "Question"
-                    except KeyError:
-                        sys.exit("Both 'Query' and 'Question' keys are missing for the given row.")
-
-                document = row['Document']
-                answer = row['Answer']
-                                
-                # Scoring
-                if vllm: 
-                    context_score = few_shot_context_relevance_scoring_vllm(
-                    context_relevance_system_prompt, query, document, model_choice, query_id, debug_mode, host_url, request_delay, in_domain_prompts_dataset) 
-                    
-                    # If context relevance is 0, set answer scores to 0.
-                    if context_score == 0:
-                        answer_relevance_score = 0
-                        answer_faithfulness_score = 0
-                    else:
-                        answer_relevance_score = few_shot_answer_relevance_scoring_vllm(
-                        answer_relevance_system_prompt, query, document, answer, model_choice, query_id, debug_mode, host_url, request_delay, in_domain_prompts_dataset)
-
-                        answer_faithfulness_score = few_shot_answer_faithfulness_scoring_vllm(answer_faithfulness_system_prompt, query, document, answer, model_choice, query_id, debug_mode, host_url, request_delay, in_domain_prompts_dataset)
-
-                else: 
-                    context_score = few_shot_context_relevance_scoring(
-                        context_relevance_system_prompt, query, document, model_choice, query_id, debug_mode, request_delay, in_domain_prompts_dataset)
-                    
-                    # If context relevance is 0, set answer scores to 0.
-                    if context_score == 0:
-                        answer_relevance_score = 0
-                        answer_faithfulness_score = 0
-                    else:
-                        answer_relevance_score = few_shot_answer_relevance_scoring(
-                            answer_relevance_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, in_domain_prompts_dataset)
-                        
-                        answer_faithfulness_score = few_shot_answer_faithfulness_scoring(answer_faithfulness_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, in_domain_prompts_dataset)
-
-                # Append scores to respective lists
-                context_relevance_scores.append(context_score)
-                answer_relevance_scores.append(answer_relevance_score)
-                answer_faithfulness_scores.append(answer_faithfulness_score)
-
-                pbar.update(1)
-    elif "claude" in model_choice:
-        with tqdm(total=documents, desc=f"Evaluating large subset with {model_choice}") as pbar:
-            for index, row in unlabeled_evaluation_set[:documents].iterrows():
-                # Extract query, document, and answer from the row
-                try:
-                    query = row['Query']
-                except KeyError:
-                    query = row['Question']
-                
-                try:
-                    _ = in_domain_prompts_dataset.iloc[0]['Query']
-                    query_id = "Query"
-                except KeyError:
-                    try:
-                        _ = in_domain_prompts_dataset.iloc[0]['Question']
-                        query_id = "Question"
-                    except KeyError:
-                        sys.exit("Both 'Query' and 'Question' keys are missing for the given row.")
-
-                document = row['Document']
-                answer = row['Answer']
-
-                # Scoring
-                context_score = few_shot_context_relevance_scoring_claude(
-                    context_relevance_system_prompt, query, document, model_choice, query_id, debug_mode, request_delay, in_domain_prompts_dataset)
-
-                # If context relevance is 0, set answer scores to 0.
-                if context_score == 0:
-                    answer_relevance_score = 0
-                    answer_faithfulness_score = 0
-                else: 
-                    answer_relevance_score = few_shot_answer_relevance_scoring_claude(
-                        answer_relevance_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, in_domain_prompts_dataset)
-                    
-                    answer_faithfulness_score = few_shot_answer_faithfulness_scoring_claude(answer_faithfulness_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, in_domain_prompts_dataset)
-
-                # Append scores to respective lists
-                context_relevance_scores.append(context_score)
-                answer_relevance_scores.append(answer_relevance_score)
-                answer_faithfulness_scores.append(answer_faithfulness_score)
-
-                pbar.update(1)
-    else: 
-        with tqdm(total=documents, desc=f"Evaluating large subset with {model_choice}") as pbar:
-            for index, row in unlabeled_evaluation_set[:documents].iterrows():
-                # Extract query, document, and answer from the row
-                try:
-                    query = row['Query']
-                except KeyError:
-                    query = row['Question']
-                
-                try:
-                    _ = in_domain_prompts_dataset.iloc[0]['Query']
-                    query_id = "Query"
-                except KeyError:
-                    try:
-                        _ = in_domain_prompts_dataset.iloc[0]['Question']
-                        query_id = "Question"
-                    except KeyError:
-                        sys.exit("Both 'Query' and 'Question' keys are missing for the given row.")
-
-                document = row['Document']
-                answer = row['Answer']
-                
-                # Scoring
-                if vllm: 
-                    context_score = few_shot_context_relevance_scoring_vllm(
-                    context_relevance_system_prompt, query, document, model_choice, query_id, debug_mode, host_url, request_delay, in_domain_prompts_dataset) 
-                    
-                    # If context relevance is 0, set answer scores to 0.
-                    if context_score == 0:
-                        answer_relevance_score = 0
-                        answer_faithfulness_score = 0
-                    else: 
-                        answer_relevance_score = few_shot_answer_relevance_scoring_vllm(
-                        answer_relevance_system_prompt, query, document, answer, model_choice, query_id, debug_mode, host_url, request_delay, in_domain_prompts_dataset)
-
-                        answer_faithfulness_score = few_shot_answer_faithfulness_scoring_vllm(answer_faithfulness_system_prompt, query, document, answer, model_choice, query_id, debug_mode, host_url, request_delay, in_domain_prompts_dataset)
-                    
-                else: 
-                    context_score = few_shot_context_relevance_scoring_togetherai(
-                        context_relevance_system_prompt, query, document, model_choice, query_id, debug_mode, request_delay, in_domain_prompts_dataset)
-                    
-                    # If context relevance is 0, set answer scores to 0.
-                    if context_score == 0:
-                        answer_relevance_score = 0
-                        answer_faithfulness_score = 0
-                    else:
-                        answer_relevance_score = few_shot_answer_relevance_scoring_togetherai(
-                            answer_relevance_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, in_domain_prompts_dataset)
-                        
-                        answer_faithfulness_score = few_shot_answer_faithfulness_scoring_togetherai(answer_faithfulness_system_prompt, query, document, answer, model_choice, query_id, debug_mode, request_delay, in_domain_prompts_dataset)
-
-                # Append scores to respective lists
-                context_relevance_scores.append(context_score)
-                answer_relevance_scores.append(answer_relevance_score)
-                answer_faithfulness_scores.append(answer_faithfulness_score)
+    with tqdm(total=documents, desc=f"Evaluating large subset with {model_choice}") as pbar:
+        for index, row in unlabeled_evaluation_set[:documents].iterrows():
+            context_score, answer_relevance_score, answer_faithfulness_score = score_row(
+                row, in_domain_prompts_dataset, context_relevance_system_prompt, answer_relevance_system_prompt, answer_faithfulness_system_prompt, model_choice, "Query", debug_mode, request_delay, vllm, host_url)
+            
+            context_relevance_scores.append(context_score)
+            answer_relevance_scores.append(answer_relevance_score)
+            answer_faithfulness_scores.append(answer_faithfulness_score)
 
-                pbar.update(1)
+            pbar.update(1)
+    
+    return context_relevance_scores, answer_relevance_scores, answer_faithfulness_scores
 
-    # Convert score lists to DataFrame
+def ues_idp_config(
+    in_domain_prompts_dataset: str, 
+    unlabeled_evaluation_set: str, 
+    context_relevance_system_prompt: str, 
+    answer_relevance_system_prompt: str, 
+    answer_faithfulness_system_prompt: str, 
+    debug_mode: bool, 
+    documents: int, 
+    model_choice: str, 
+    vllm: bool, 
+    host_url: str, 
+    request_delay: int
+) -> dict:
+    """
+    Configures UES and IDP for evaluation.
+
+    Parameters:
+    in_domain_prompts_dataset (str): Path to the in-domain prompts dataset.
+    unlabeled_evaluation_set (str): Path to the unlabeled evaluation set.
+    context_relevance_system_prompt (str): System prompt for context relevance scoring.
+    answer_relevance_system_prompt (str): System prompt for answer relevance scoring.
+    answer_faithfulness_system_prompt (str): System prompt for answer faithfulness scoring.
+    debug_mode (bool): Flag to enable or disable debug mode.
+    documents (int): Number of documents to evaluate.
+    model_choice (str): The model choice for evaluation.
+    vllm (bool): Flag to indicate if vllm is used.
+    host_url (str): The host URL for the model.
+    request_delay (int): Delay between requests in seconds.
+
+    Returns:
+    dict: A dictionary containing the mean scores for context relevance, answer faithfulness, and answer relevance.
+    """
+    
+    # Validate inputs and get the processed datasets
+    in_domain_prompts_dataset, unlabeled_evaluation_set = validate_inputs(
+        vllm, host_url, in_domain_prompts_dataset, unlabeled_evaluation_set, documents
+    )
+
+    # Evaluate the documents and get the scores
+    context_relevance_scores, answer_relevance_scores, answer_faithfulness_scores = evaluate_documents(
+        unlabeled_evaluation_set, in_domain_prompts_dataset, context_relevance_system_prompt, 
+        answer_relevance_system_prompt, answer_faithfulness_system_prompt, model_choice, 
+        debug_mode, request_delay, vllm, host_url, documents
+    )
+
+    # Create a DataFrame to store the results
     results_df = pd.DataFrame({
         'Context_Relevance_Score': context_relevance_scores,
         'Answer_Relevance_Score': answer_relevance_scores,
         'Answer_Faithfulness_Score': answer_faithfulness_scores
     })
 
-    # Apply filtering to remove invalid rows
+    # Filter out invalid results
     valid_results_df = results_df[
         ~((results_df['Context_Relevance_Score'] == 0) & 
         ((results_df['Answer_Relevance_Score'] == 1) | 
         (results_df['Answer_Faithfulness_Score'] == 1)))
     ]
+    
+    # Print the number of failed extractions
+    print("Number of times did not extract Yes or No:", failed_extraction_count['failed'])
 
-    print("Original rows:", len(results_df))
-    print("Rows after filtering:", len(valid_results_df))
-
-    # Return the average scores from the filtered DataFrame
+    # Return the mean scores rounded to three decimal places
     return {
         "Context Relevance Scores": round(valid_results_df['Context_Relevance_Score'].mean(), 3),
         "Answer Faithfulness Scores": round(valid_results_df['Answer_Faithfulness_Score'].mean(), 3),
         "Answer Relevance Scores": round(valid_results_df['Answer_Relevance_Score'].mean(), 3)
-    }
-
-    
+    }
```

### Comparing `ares_ai-0.5.7/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.5.8/ares_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.5.7
+Version: 0.5.8
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,14 +218,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate<1.0.0,>=0.21.0
 Requires-Dist: anthropic>=0.25.7
 Requires-Dist: Cython>=0.29.35
 Requires-Dist: datasets>=2.12.0
+Requires-Dist: evaluate==0.4.2
 Requires-Dist: fastapi==0.110.2
 Requires-Dist: faiss-cpu>=1.8.0
 Requires-Dist: ipywidgets<9.0.0,>=8.0.6
 Requires-Dist: ipython<9.0.0,>=8.12.2
 Requires-Dist: ipykernel<7.0.0,>=6.23.1
 Requires-Dist: joblib<2.0.0,>=1.2.0
 Requires-Dist: matplotlib<4.0.0,>=3.7.1
@@ -374,15 +375,15 @@
 
 <hr>
 
 To get started with ARES's PPI, you'll need to set up your configuration. Below is an example of a configuration for ARES!
 
 Just copy-paste as you go to see ARES in action!
 
-#### Step 1) Run the following to retrive the UES/IDP scores with GPT3.5!
+#### Step 1) Run the following to retrieve the UES/IDP scores with GPT3.5!
 
 ```python
 from ares import ARES
 
 ues_idp_config = {
     "in_domain_prompts_dataset": "nq_few_shot_prompt_for_judge_scoring.tsv",
     "unlabeled_evaluation_set": "nq_unlabeled_output.tsv", 
@@ -472,36 +473,52 @@
 
 ares = ARES(classifier_model=classifier_config)
 results = ares.train_classifier()
 print(results)
 ```
 
 Note: This code creates a checkpoint for the trained classifier.
-Training may take some time. You can download the checkpoint here:
-[Download Checkpoint](https://drive.google.com/file/d/1dsUzL01a53ictjMaUI6RqEvHY5vColcL/view?usp=sharing)
+Training may take some time. You can download our jointly trained checkpoint on context relevance here!:
+[Download Checkpoint](https://drive.google.com/file/d/15poFyeoqdnaNZVjl41HllL2213DKyZjH/view?usp=sharing)
+
+Alternatively, you can download our jointly trained checkpoint on answer relevance here! Be sure to change the parameters in the config to match the label "Answer_Relevance_Label"
+[Download Checkpoint](https://drive.google.com/file/d/1wGcgELBfnCGqXlPEbpPmf7LJ53DPWVXI/view?usp=sharing)
+
 
 <hr>
 
 #### Step 4) Run the following to see ARES's PPI in action!
 ```python
 
 from ares import ARES
 
 ppi_config = { 
     "evaluation_datasets": ['nq_unlabeled_output.tsv'], 
-    "few_shot_examples_filepath": "nq_few_shot_prompt_for_judge_scoring.tsv",
     "checkpoints": ["Context_Relevance_Label_nq_labeled_output_date_time.pt"], 
     "rag_type": "question_answering", 
     "labels": ["Context_Relevance_Label"], 
     "gold_label_path": "nq_labeled_output.tsv", 
 }
 
 ares = ARES(ppi=ppi_config)
 results = ares.evaluate_RAG()
 print(results)
+
+# Output Should be: 
+""" 
+Context_Relevance_Label Scoring
+ARES Ranking
+ARES Prediction: [0.6056978059262574]
+ARES Confidence Interval: [[0.547, 0.664]]
+Number of Examples in Evaluation Set: [4421]
+Ground Truth Performance: [0.6]
+ARES LLM Judge Accuracy on Ground Truth Labels: [0.789]
+Annotated Examples used for PPI: 300
+"""
+
 ```
 
 <br>
 
 ### 🚀 Local Model Execution with vLLM
 
 ARES supports [vLLM](https://github.com/vllm-project/vllm), allowing for local execution of LLM models, offering enhanced privacy and the ability to operate ARES offline. Below are steps to vLLM for ARES's UES/IDP and PPI!
@@ -509,15 +526,15 @@
 #### 1) UES/IDP w/ vLLM
 
 ```python
 from ares import ARES
 
 ues_idp_config = {
     "in_domain_prompts_dataset": "nq_few_shot_prompt_for_judge_scoring.tsv",
-    "unlabeled_evaluation_set": "nq_unalebed_output.tsv", 
+    "unlabeled_evaluation_set": "nq_unlabeled_output.tsv", 
     "model_choice": "meta-llama/Llama-2-13b-hf", # Specify vLLM model
     "vllm": True, # Toggle vLLM to True 
     "host_url": "http://0.0.0.0:8000/v1" # Replace with server hosting model followed by "/v1"
 } 
 
 ares = ARES(ues_idp=ues_idp_config)
 results = ares.ues_idp()
```

### Comparing `ares_ai-0.5.7/ares_ai.egg-info/SOURCES.txt` & `ares_ai-0.5.8/ares_ai.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 requirements.txt
 setup.cfg
 ares/__init__.py
 ares/__init__.pyc
 ares/ares.py
 ares/binary_classifier.py
 ares/kilt_filter.py
+ares/prompts.py
 ares/rag_scoring.py
 ares/superglue_filter.py
 ares/synthetic_generator.py
 ares/ues_idp.py
 ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
 ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
 ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
@@ -33,56 +34,54 @@
 ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
 ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
 ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
 ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
 ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
 ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
 ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
-ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py
 ares/RAG_Automatic_Evaluation/__init__.py
 ares/RAG_Automatic_Evaluation/ppi.py
 ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
+ares/RAG_Automatic_Evaluation/__pycache__/counter.cpython-310.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
 ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
 ares/__pycache__/__init__.cpython-310.pyc
 ares/__pycache__/__init__.cpython-311.pyc
 ares/__pycache__/ares.cpython-310.pyc
 ares/__pycache__/ares.cpython-311.pyc
 ares/__pycache__/binary_classifier.cpython-310.pyc
 ares/__pycache__/binary_classifier.cpython-311.pyc
 ares/__pycache__/kilt_filter.cpython-310.pyc
 ares/__pycache__/kilt_filter.cpython-311.pyc
+ares/__pycache__/prompts.cpython-310.pyc
 ares/__pycache__/rag_scoring.cpython-310.pyc
 ares/__pycache__/rag_scoring.cpython-311.pyc
 ares/__pycache__/superglue_filter.cpython-310.pyc
 ares/__pycache__/superglue_filter.cpython-311.pyc
 ares/__pycache__/synthetic_generator.cpython-310.pyc
 ares/__pycache__/synthetic_generator.cpython-311.pyc
 ares/__pycache__/ues_idp.cpython-310.pyc
 ares/__pycache__/ues_idp.cpython-311.pyc
 ares/ares_ai.egg-info/PKG-INFO
 ares/ares_ai.egg-info/SOURCES.txt
 ares/ares_ai.egg-info/dependency_links.txt
 ares/ares_ai.egg-info/entry_points.txt
 ares/ares_ai.egg-info/requires.txt
 ares/ares_ai.egg-info/top_level.txt
-ares/ppi/.DS_Store
-ares/ppi/ppi.py
-ares/ppi/ppi_testing.py
 ares_ai.egg-info/PKG-INFO
 ares_ai.egg-info/SOURCES.txt
 ares_ai.egg-info/dependency_links.txt
 ares_ai.egg-info/entry_points.txt
 ares_ai.egg-info/requires.txt
 ares_ai.egg-info/top_level.txt
 checkpoints/.gitignore
```

### Comparing `ares_ai-0.5.7/ares_ai.egg-info/requires.txt` & `ares_ai-0.5.8/ares_ai.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 accelerate<1.0.0,>=0.21.0
 anthropic>=0.25.7
 Cython>=0.29.35
 datasets>=2.12.0
+evaluate==0.4.2
 fastapi==0.110.2
 faiss-cpu>=1.8.0
 ipywidgets<9.0.0,>=8.0.6
 ipython<9.0.0,>=8.12.2
 ipykernel<7.0.0,>=6.23.1
 joblib<2.0.0,>=1.2.0
 matplotlib<4.0.0,>=3.7.1
```

### Comparing `ares_ai-0.5.7/pyproject.toml` & `ares_ai-0.5.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ares-ai"
-version = "0.5.7"
+version = "0.5.8"
 description = """ 
 ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 utilizing fine-tuned classifiers and synthetic data to assess performance efficiently. It streamlines 
 the evaluation of context relevance, answer faithfulness, and answer relevance with minimal human annotations.
 """
 readme = "README.md"
 authors = [
@@ -33,26 +33,27 @@
 "Answer Relevance", "Synthetic Queries", "Synthetic Answers", "In-Domain Passages", "Key Performance Metrics", "Human Preference Validation Set"]
 
 dependencies = [
     "accelerate >=0.21.0, <1.0.0",
     "anthropic >= 0.25.7",
     "Cython >=0.29.35",
     "datasets >=2.12.0",
+    "evaluate==0.4.2",
     "fastapi == 0.110.2",
     "faiss-cpu >= 1.8.0", 
     "ipywidgets >=8.0.6, <9.0.0",
     "ipython >=8.12.2, <9.0.0",
     "ipykernel >=6.23.1, <7.0.0",
     "joblib >=1.2.0, <2.0.0",
     "matplotlib >=3.7.1, <4.0.0",
     "matplotlib-inline >=0.1.6, <0.2.0",
     "nltk >=3.8.1, <4.0.0",
     "numexpr >=2.8.4, <3.0.0",
     "numpy >=1.20.0, <2.0.0",
-    "openai ==1.14.2",
+    "openai == 1.14.2",
     "pandas >= 2.0.1",
     "python-dateutil >=2.8.2,<3.0.0",
     "pytorch-ranger >=0.1.1,<0.2.0",
     "pytz >=2023.3,<2024.0",
     "PyYAML >=6.0,<7.0",
     "requests >=2.25.1, <3.0.0",
     "scikit-learn >=1.2.2,<1.3.0",
```

### Comparing `ares_ai-0.5.7/requirements.txt` & `ares_ai-0.5.8/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 torch-optimizer==0.3.0
 torchaudio==0.13.1
 torchmetrics==0.11.3
 torchtext==0.14.1
 torchvision==0.14.1
 together == 1.1.2
 accelerate==0.21.0
-aiohttp==3.9.0
+aiohttp==3.9.4
 aiosignal==1.3.1
 antlr4-python3-runtime==4.9.3
 anyio==3.6.2
 appdirs==1.4.4
 argcomplete==3.1.1
 argon2-cffi==21.3.0
 argon2-cffi-bindings==21.2.0
@@ -50,14 +50,15 @@
 debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
 dill==0.3.6
 docker==6.1.3
 docker-pycreds==0.4.0
 einops==0.5.0
+evaluate==0.4.2
 executing==1.2.0
 faiss-gpu==1.7.2
 fastjsonschema==2.16.3
 fastrlock==0.8.1
 filelock==3.12.0
 Flask==2.3.2
 flatbuffers==23.5.26
@@ -79,34 +80,34 @@
 ipython==8.12.2
 ipython-genutils==0.2.0
 ipywidgets==8.0.6
 ir-datasets==0.5.4
 isoduration==20.11.0
 itsdangerous==2.1.2
 jedi==0.18.2
-Jinja2==3.1.2
+Jinja2==3.1.4
 jmespath==1.0.1
 joblib==1.2.0
 json5==0.9.14
 jsonlines==3.1.0
 jsonpointer==2.3
 jsonschema==4.17.3
 jupyter==1.0.0
 jupyter-client==8.2.0
 jupyter-console==6.6.3
 jupyter-core==5.3.0
-jupyter-lsp==2.1.0
+jupyter-lsp==2.2.2
 jupyter-server==2.11.2
 jupyter-server-terminals==0.4.4
-jupyterlab==4.0.0
+jupyterlab==4.0.11
 jupyterlab-pygments==0.2.2
 jupyterlab-server==2.22.1
 jupyterlab-widgets==3.0.7
 kiwisolver==1.4.4
-langchain==0.0.329
+langchain==0.1.0
 langchainplus-sdk==0.0.16
 langcodes==3.3.0
 lightgbm==3.3.5
 lit==16.0.6
 lxml==4.9.2
 lz4==4.3.2
 mkdocs
@@ -183,15 +184,15 @@
 pure-eval==0.2.2
 py-cpuinfo==9.0.0
 py7zr==0.20.5
 pyarrow==14.0.1
 pybcj==1.0.1
 pybind11==2.6.1
 pycryptodomex==3.19.1
-pydantic==1.10.7
+pydantic==1.10.13
 Pygments==2.15.1
 pyjnius==1.5.0
 PyNaCl==1.5.0
 pyparsing==3.0.9
 pyppmd==1.0.0
 pyrsistent==0.19.3
 pyserini==0.21.0
@@ -243,15 +244,15 @@
 thinc==8.1.10
 threadpoolctl==3.1.0
 tiktoken==0.4.0
 tinycss2==1.2.1
 tokenizers==0.13.3
 tomli==2.0.1
 tornado==6.3.3
-tqdm==4.65.0
+tqdm==4.66.3
 traitlets==5.9.0
 transformers==4.36.0
 trec-car-tools==2.6
 triton==2.0.0.dev20221103
 trl==0.4.4
 typer==0.7.0
 typing-inspect==0.9.0
@@ -266,14 +267,14 @@
 warc3-wet-clueweb09==0.2.5
 wasabi==1.1.1
 wcwidth==0.2.6
 webcolors==1.13
 webencodings==0.5.1
 websocket-client==1.5.1
 websockets==10.4
-Werkzeug==2.3.8
+Werkzeug==3.0.3
 widgetsnbextension==4.0.7
 xxhash==3.2.0
 yarl==1.9.2
 zipp==3.15.0
 zlib-state==0.1.5
 zstd==1.5.5.1
```

