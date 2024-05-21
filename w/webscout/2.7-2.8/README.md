# Comparing `tmp/webscout-2.7.tar.gz` & `tmp/webscout-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-2.7.tar", last modified: Sun May 19 15:12:42 2024, max compression
+gzip compressed data, was "webscout-2.8.tar", last modified: Tue May 21 05:25:53 2024, max compression
```

## Comparing `webscout-2.7.tar` & `webscout-2.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.745495 webscout-2.7/
-drwxrwxrwx   0        0        0        0 2024-05-19 15:12:41.857682 webscout-2.7/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:12:41.944679 webscout-2.7/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.080212 webscout-2.7/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.114214 webscout-2.7/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.7/LICENSE.md
--rw-rw-rw-   0        0        0    47655 2024-05-19 15:12:42.739491 webscout-2.7/PKG-INFO
--rw-rw-rw-   0        0        0    45203 2024-05-19 15:11:59.000000 webscout-2.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 15:12:42.746490 webscout-2.7/setup.cfg
--rw-rw-rw-   0        0        0     2723 2024-05-19 14:34:53.000000 webscout-2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.286992 webscout-2.7/webscout/
--rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.7/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.7/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33256 2024-05-14 14:10:47.000000 webscout-2.7/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.7/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.7/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.384003 webscout-2.7/webscout/Local/
--rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-2.7/webscout/Local/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-19 14:47:10.000000 webscout-2.7/webscout/Local/_version.py
--rw-rw-rw-   0        0        0    18994 2024-05-19 14:40:00.000000 webscout-2.7/webscout/Local/formats.py
--rw-rw-rw-   0        0        0    27618 2024-05-19 14:42:26.000000 webscout-2.7/webscout/Local/model.py
--rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-2.7/webscout/Local/samplers.py
--rw-rw-rw-   0        0        0    26925 2024-05-19 14:44:26.000000 webscout-2.7/webscout/Local/thread.py
--rw-rw-rw-   0        0        0     6108 2024-05-14 05:14:09.000000 webscout-2.7/webscout/Local/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.713469 webscout-2.7/webscout/Provider/
--rw-rw-rw-   0        0        0     8191 2024-05-16 04:06:55.000000 webscout-2.7/webscout/Provider/BasedGPT.py
--rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.7/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.7/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.7/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.7/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.7/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.7/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.7/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.7/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.7/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.7/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.7/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.7/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.7/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     7303 2024-05-14 14:08:46.000000 webscout-2.7/webscout/Provider/Poe.py
--rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.7/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.7/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.7/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.7/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.7/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1372 2024-05-16 04:09:11.000000 webscout-2.7/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     1840 2024-05-19 14:59:15.000000 webscout-2.7/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.7/webscout/__main__.py
--rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.7/webscout/async_providers.py
--rw-rw-rw-   0        0        0    18743 2024-05-19 12:59:44.000000 webscout-2.7/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.7/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.7/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.7/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.7/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.7/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.7/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-05-19 14:37:31.000000 webscout-2.7/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.7/webscout/voice.py
--rw-rw-rw-   0        0        0    85324 2024-05-14 14:12:32.000000 webscout-2.7/webscout/webai.py
--rw-rw-rw-   0        0        0    42650 2024-05-19 13:03:19.000000 webscout-2.7/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    14471 2024-05-19 13:04:35.000000 webscout-2.7/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.721488 webscout-2.7/webscout.egg-info/
--rw-rw-rw-   0        0        0    47655 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1827 2024-05-19 15:12:41.000000 webscout-2.7/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      379 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 05:25:53.771194 webscout-2.8/
+drwxrwxrwx   0        0        0        0 2024-05-21 05:25:51.983974 webscout-2.8/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 05:25:52.009972 webscout-2.8/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-21 05:25:52.041940 webscout-2.8/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-21 05:25:52.059958 webscout-2.8/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.8/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.8/LICENSE.md
+-rw-rw-rw-   0        0        0    47725 2024-05-21 05:25:53.762200 webscout-2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    45203 2024-05-19 15:11:59.000000 webscout-2.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 05:25:53.772191 webscout-2.8/setup.cfg
+-rw-rw-rw-   0        0        0     2784 2024-05-21 05:25:06.000000 webscout-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 05:25:52.297742 webscout-2.8/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.8/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.8/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33256 2024-05-14 14:10:47.000000 webscout-2.8/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.8/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     4184 2024-05-19 17:29:05.000000 webscout-2.8/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-21 05:25:52.913917 webscout-2.8/webscout/Local/
+-rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-2.8/webscout/Local/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-19 14:47:10.000000 webscout-2.8/webscout/Local/_version.py
+-rw-rw-rw-   0        0        0    18994 2024-05-19 14:40:00.000000 webscout-2.8/webscout/Local/formats.py
+-rw-rw-rw-   0        0        0    27618 2024-05-19 14:42:26.000000 webscout-2.8/webscout/Local/model.py
+-rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-2.8/webscout/Local/samplers.py
+-rw-rw-rw-   0        0        0    26925 2024-05-19 14:44:26.000000 webscout-2.8/webscout/Local/thread.py
+-rw-rw-rw-   0        0        0     6108 2024-05-14 05:14:09.000000 webscout-2.8/webscout/Local/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 05:25:53.577594 webscout-2.8/webscout/Provider/
+-rw-rw-rw-   0        0        0     8191 2024-05-16 04:06:55.000000 webscout-2.8/webscout/Provider/BasedGPT.py
+-rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.8/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.8/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.8/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.8/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.8/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.8/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.8/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.8/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.8/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.8/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.8/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.8/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.8/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     7303 2024-05-14 14:08:46.000000 webscout-2.8/webscout/Provider/Poe.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.8/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.8/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.8/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.8/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.8/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1372 2024-05-16 04:09:11.000000 webscout-2.8/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     1840 2024-05-19 14:59:15.000000 webscout-2.8/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.8/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.8/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    18743 2024-05-19 12:59:44.000000 webscout-2.8/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.8/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.8/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.8/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.8/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.8/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.8/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-19 14:37:31.000000 webscout-2.8/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.8/webscout/voice.py
+-rw-rw-rw-   0        0        0    85324 2024-05-14 14:12:32.000000 webscout-2.8/webscout/webai.py
+-rw-rw-rw-   0        0        0    42650 2024-05-19 13:03:19.000000 webscout-2.8/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    14471 2024-05-19 13:04:35.000000 webscout-2.8/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-21 05:25:53.735190 webscout-2.8/webscout.egg-info/
+-rw-rw-rw-   0        0        0    47725 2024-05-21 05:25:50.000000 webscout-2.8/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2024-05-21 05:25:51.000000 webscout-2.8/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 05:25:50.000000 webscout-2.8/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-21 05:25:50.000000 webscout-2.8/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      417 2024-05-21 05:25:50.000000 webscout-2.8/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-21 05:25:50.000000 webscout-2.8/webscout.egg-info/top_level.txt
```

### Comparing `webscout-2.7/DeepWEBS/documents/query_results_extractor.py` & `webscout-2.8/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-2.8/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/DeepWEBS/networks/filepath_converter.py` & `webscout-2.8/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/DeepWEBS/networks/google_searcher.py` & `webscout-2.8/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/DeepWEBS/networks/network_configs.py` & `webscout-2.8/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/DeepWEBS/networks/webpage_fetcher.py` & `webscout-2.8/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/DeepWEBS/utilsdw/enver.py` & `webscout-2.8/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/DeepWEBS/utilsdw/logger.py` & `webscout-2.8/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/LICENSE.md` & `webscout-2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-2.7/PKG-INFO` & `webscout-2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.7
+Version: 2.8
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -48,14 +48,16 @@
 Requires-Dist: PyYAML
 Requires-Dist: appdirs
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client
 Requires-Dist: clipman
 Requires-Dist: Helpingai-T2
 Requires-Dist: playsound
+Requires-Dist: poe_api_wrapper
+Requires-Dist: pyreqwest_impersonate
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 Provides-Extra: local
 Requires-Dist: llama-cpp-python; extra == "local"
 Requires-Dist: colorama; extra == "local"
 Requires-Dist: numpy; extra == "local"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.7 Summary: Search for anything
+Metadata-Version: 2.1 Name: webscout Version: 2.8 Summary: Search for anything
 using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
 videos, temporary email and phone number generation, has TTS support, webai
 (terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -22,16 +22,17 @@
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
 Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
 Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
 Requires-Dist: PyYAML Requires-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: Helpingai-T2
-Requires-Dist: playsound Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
-== "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" Provides-Extra: local
+Requires-Dist: playsound Requires-Dist: poe_api_wrapper Requires-Dist:
+pyreqwest_impersonate Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra ==
+"dev" Requires-Dist: pytest>=7.4.2; extra == "dev" Provides-Extra: local
 Requires-Dist: llama-cpp-python; extra == "local" Requires-Dist: colorama;
 extra == "local" Requires-Dist: numpy; extra == "local"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
```

### Comparing `webscout-2.7/README.md` & `webscout-2.8/README.md`

 * *Files identical despite different names*

### Comparing `webscout-2.7/setup.py` & `webscout-2.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="2.7",
+    version="2.8",
     description="Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
@@ -52,14 +52,16 @@
         "PyYAML",
         "appdirs",
         "GoogleBard1>=2.1.4",
         "tls_client",
         "clipman",
         "Helpingai-T2",
         "playsound",
+        "poe_api_wrapper",
+        "pyreqwest_impersonate"
     ],
     entry_points={
         "console_scripts": [
             "WEBS = webscout.cli:cli",
             "webscout = webscout.webai:main",
         ],
     },
```

### Comparing `webscout-2.7/webscout/AIauto.py` & `webscout-2.8/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/AIbase.py` & `webscout-2.8/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/AIutel.py` & `webscout-2.8/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/DWEBS.py` & `webscout-2.8/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/LLM.py` & `webscout-2.8/webscout/LLM.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-import argparse
 import requests
+import base64
+from typing import List, Dict, Union
 import json
+import requests
+import base64
 from typing import List, Dict, Union
 
 class LLM:
     def __init__(self, model: str, system_message: str = "You are a Helpful AI."):
         self.model = model
         self.conversation_history = [{"role": "system", "content": system_message}]
 
@@ -39,7 +42,59 @@
             }, separators=(',', ':')
         )
         try:
             result = requests.post(url=url, data=data, headers=headers)
             return result.json()['choices'][0]['message']['content']
         except:
             return None
+# def main():
+#     llm = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct")
+#     messages = [
+#         {"role": "user", "content": "Hello, how are you?"}
+#     ]
+#     response = llm.chat(messages)
+#     print(response)
+
+# if __name__ == "__main__":
+#     main()
+
+
+class VLM:
+    def __init__(self, model: str, system_message: str = "You are a Helpful AI."):
+        self.model = model
+        self.conversation_history = [{"role": "system", "content": system_message}]
+
+    def chat(self, messages: List[Dict[str, Union[str, List[Dict[str, Union[str, Dict[str, str]]]]]]]) -> Union[str, None]:
+        api_url = "https://api.deepinfra.com/v1/openai/chat/completions"
+        headers = {
+            'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36',
+            'Accept-Language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
+            'Cache-Control': 'no-cache',
+            'Connection': 'keep-alive',
+            'Content-Type': 'application/json',
+            'Origin': 'https://deepinfra.com',
+            'Pragma': 'no-cache',
+            'Referer': 'https://deepinfra.com/',
+            'Sec-Fetch-Dest': 'empty',
+            'Sec-Fetch-Mode': 'cors',
+            'Sec-Fetch-Site': 'same-site',
+            'X-Deepinfra-Source': 'web-embed',
+            'accept': 'text/event-stream',
+            'sec-ch-ua': '"Google Chrome";v="119", "Chromium";v="119", "Not?A_Brand";v="24"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"macOS"'
+        }
+        payload = {
+            "model": self.model,
+            "messages": messages,
+            "stream": False
+        }
+        try:
+            response = requests.post(api_url, headers=headers, json=payload)
+            return response.json()['choices'][0]['message']['content']
+        except Exception as e:
+            print(f"An error occurred: {e}")
+            return None
+
+def encode_image_to_base64(image_path: str) -> str:
+    with open(image_path, "rb") as image_file:
+        return base64.b64encode(image_file.read()).decode("utf-8")
```

### Comparing `webscout-2.7/webscout/Local/formats.py` & `webscout-2.8/webscout/Local/formats.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Local/model.py` & `webscout-2.8/webscout/Local/model.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Local/samplers.py` & `webscout-2.8/webscout/Local/samplers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Local/thread.py` & `webscout-2.8/webscout/Local/thread.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Local/utils.py` & `webscout-2.8/webscout/Local/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/BasedGPT.py` & `webscout-2.8/webscout/Provider/BasedGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Berlin4h.py` & `webscout-2.8/webscout/Provider/Berlin4h.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Blackboxai.py` & `webscout-2.8/webscout/Provider/Blackboxai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/ChatGPTUK.py` & `webscout-2.8/webscout/Provider/ChatGPTUK.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Cohere.py` & `webscout-2.8/webscout/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Gemini.py` & `webscout-2.8/webscout/Provider/Gemini.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Groq.py` & `webscout-2.8/webscout/Provider/Groq.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Koboldai.py` & `webscout-2.8/webscout/Provider/Koboldai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Leo.py` & `webscout-2.8/webscout/Provider/Leo.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Llama2.py` & `webscout-2.8/webscout/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/OpenGPT.py` & `webscout-2.8/webscout/Provider/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Openai.py` & `webscout-2.8/webscout/Provider/Openai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Perplexity.py` & `webscout-2.8/webscout/Provider/Perplexity.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Phind.py` & `webscout-2.8/webscout/Provider/Phind.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Poe.py` & `webscout-2.8/webscout/Provider/Poe.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Reka.py` & `webscout-2.8/webscout/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/ThinkAnyAI.py` & `webscout-2.8/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Xjai.py` & `webscout-2.8/webscout/Provider/Xjai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Yepchat.py` & `webscout-2.8/webscout/Provider/Yepchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/Youchat.py` & `webscout-2.8/webscout/Provider/Youchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/Provider/__init__.py` & `webscout-2.8/webscout/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/__init__.py` & `webscout-2.8/webscout/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/async_providers.py` & `webscout-2.8/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/cli.py` & `webscout-2.8/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/g4f.py` & `webscout-2.8/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/models.py` & `webscout-2.8/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/tempid.py` & `webscout-2.8/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/transcriber.py` & `webscout-2.8/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/utils.py` & `webscout-2.8/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/voice.py` & `webscout-2.8/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/webai.py` & `webscout-2.8/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/webscout_search.py` & `webscout-2.8/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout/webscout_search_async.py` & `webscout-2.8/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-2.7/webscout.egg-info/PKG-INFO` & `webscout-2.8/webscout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.7
+Version: 2.8
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -48,14 +48,16 @@
 Requires-Dist: PyYAML
 Requires-Dist: appdirs
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client
 Requires-Dist: clipman
 Requires-Dist: Helpingai-T2
 Requires-Dist: playsound
+Requires-Dist: poe_api_wrapper
+Requires-Dist: pyreqwest_impersonate
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 Provides-Extra: local
 Requires-Dist: llama-cpp-python; extra == "local"
 Requires-Dist: colorama; extra == "local"
 Requires-Dist: numpy; extra == "local"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.7 Summary: Search for anything
+Metadata-Version: 2.1 Name: webscout Version: 2.8 Summary: Search for anything
 using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
 videos, temporary email and phone number generation, has TTS support, webai
 (terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -22,16 +22,17 @@
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
 Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
 Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
 Requires-Dist: PyYAML Requires-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: Helpingai-T2
-Requires-Dist: playsound Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
-== "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" Provides-Extra: local
+Requires-Dist: playsound Requires-Dist: poe_api_wrapper Requires-Dist:
+pyreqwest_impersonate Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra ==
+"dev" Requires-Dist: pytest>=7.4.2; extra == "dev" Provides-Extra: local
 Requires-Dist: llama-cpp-python; extra == "local" Requires-Dist: colorama;
 extra == "local" Requires-Dist: numpy; extra == "local"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
```

### Comparing `webscout-2.7/webscout.egg-info/SOURCES.txt` & `webscout-2.8/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

