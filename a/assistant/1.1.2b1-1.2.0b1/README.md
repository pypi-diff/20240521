# Comparing `tmp/assistant-1.1.2b1.tar.gz` & `tmp/assistant-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistant-1.1.2b1.tar", last modified: Tue May 14 13:41:36 2024, max compression
+gzip compressed data, was "assistant-1.2.0b1.tar", last modified: Tue May 21 18:11:27 2024, max compression
```

## Comparing `assistant-1.1.2b1.tar` & `assistant-1.2.0b1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/
--rw-r--r--   0 waser     (1000) waser     (1000)     1069 2022-03-17 17:48:10.000000 assistant-1.1.2b1/LICENSE
--rw-r--r--   0 waser     (1000) waser     (1000)       16 2022-03-17 17:48:10.000000 assistant-1.1.2b1/MANIFEST.in
--rw-r--r--   0 waser     (1000) waser     (1000)    12722 2024-05-14 13:41:36.252899 assistant-1.1.2b1/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)    10843 2024-02-18 19:52:01.000000 assistant-1.1.2b1/README.md
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.239566 assistant-1.1.2b1/assistant/
--rw-r--r--   0 waser     (1000) waser     (1000)      502 2024-05-14 13:38:34.000000 assistant-1.1.2b1/assistant/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      114 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5674 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/_execer.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.239566 assistant-1.1.2b1/assistant/api/
--rw-r--r--   0 waser     (1000) waser     (1000)      317 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/api/responses.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3867 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/as_client.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5428 2024-05-08 08:18:22.000000 assistant-1.1.2b1/assistant/as_service.py
--rw-r--r--   0 waser     (1000) waser     (1000)     6818 2024-01-25 22:35:30.000000 assistant-1.1.2b1/assistant/builtin_cmds.py
--rw-r--r--   0 waser     (1000) waser     (1000)     6792 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/codecache.py
--rw-r--r--   0 waser     (1000) waser     (1000)      132 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/conditions.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.239566 assistant-1.1.2b1/assistant/entry_points/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/entry_points/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      194 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/entry_points/run_assistant.py
--rw-r--r--   0 waser     (1000) waser     (1000)      157 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/execer.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3595 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/history.py
--rw-r--r--   0 waser     (1000) waser     (1000)      519 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/icons.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.242900 assistant-1.1.2b1/assistant/listen/
--rw-r--r--   0 waser     (1000) waser     (1000)      400 2023-12-25 20:08:57.000000 assistant-1.1.2b1/assistant/listen/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/listen/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1396 2024-05-13 22:55:29.000000 assistant-1.1.2b1/assistant/listen/interface.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2776 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/listen/main.py
--rw-r--r--   0 waser     (1000) waser     (1000)    24086 2024-05-13 19:44:02.000000 assistant-1.1.2b1/assistant/main.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.242900 assistant-1.1.2b1/assistant/manager/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/manager/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2355 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/manager/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     9813 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/manager/nlu.py
--rw-r--r--   0 waser     (1000) waser     (1000)    18387 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/manager/nlu_to_stt.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.242900 assistant-1.1.2b1/assistant/nlp/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/__init__.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.242900 assistant-1.1.2b1/assistant/nlp/chains/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      411 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/__main__.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/agents/
--rw-r--r--   0 waser     (1000) waser     (1000)      689 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/agents/__executor__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2374 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/agents/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3010 2024-05-08 06:30:31.000000 assistant-1.1.2b1/assistant/nlp/chains/agents/assistant.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/callback_handlers/
--rw-r--r--   0 waser     (1000) waser     (1000)     2074 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/callback_handlers/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3155 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/code_pilot.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/data_loaders/
--rw-r--r--   0 waser     (1000) waser     (1000)      158 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/data_loaders/__init__.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/data_splitter/
--rw-r--r--   0 waser     (1000) waser     (1000)       76 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/data_splitter/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2918 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/docs_explained.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/embeddings/
--rw-r--r--   0 waser     (1000) waser     (1000)      184 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/embeddings/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     4647 2024-05-13 19:11:24.000000 assistant-1.1.2b1/assistant/nlp/chains/embeddings/assistant.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/memory/
--rw-r--r--   0 waser     (1000) waser     (1000)      203 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/memory/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      536 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/memory/conversation_buffer.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/models/
--rw-r--r--   0 waser     (1000) waser     (1000)      952 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/models/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      682 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/models/hf.py
--rw-r--r--   0 waser     (1000) waser     (1000)     6568 2024-02-22 21:10:49.000000 assistant-1.1.2b1/assistant/nlp/chains/models/vllm.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/parsers/
--rw-r--r--   0 waser     (1000) waser     (1000)      156 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/parsers/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1833 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/parsers/column_csv.py
--rw-r--r--   0 waser     (1000) waser     (1000)     7620 2024-05-11 15:39:14.000000 assistant-1.1.2b1/assistant/nlp/chains/parsers/json.py
--rw-r--r--   0 waser     (1000) waser     (1000)     4783 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/parsers/markdown_json.py
--rw-r--r--   0 waser     (1000) waser     (1000)      831 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/persistent_session.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/nlp/chains/prompts/
--rw-r--r--   0 waser     (1000) waser     (1000)     5222 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/prompts/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      690 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/prompts/airoboros.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1509 2024-05-08 06:27:54.000000 assistant-1.1.2b1/assistant/nlp/chains/prompts/json.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/nlp/chains/schema/
--rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/schema/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2209 2024-05-08 06:48:37.000000 assistant-1.1.2b1/assistant/nlp/chains/schema/memory.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5260 2024-01-13 19:44:59.000000 assistant-1.1.2b1/assistant/nlp/chains/schema/vectorstore.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5443 2024-05-11 15:35:21.000000 assistant-1.1.2b1/assistant/nlp/chains/session.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/nlp/chains/tools/
--rw-r--r--   0 waser     (1000) waser     (1000)      406 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1698 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/__retriever__.py
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/memory.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2021 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/python.py
--rw-r--r--   0 waser     (1000) waser     (1000)      300 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/retriever.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1505 2024-01-13 19:49:07.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/search.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5049 2024-01-05 02:36:06.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/shell.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1762 2024-01-13 19:49:32.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/wikipedia.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/nlp/chains/vectorstores/
--rw-r--r--   0 waser     (1000) waser     (1000)     2207 2024-01-13 19:43:16.000000 assistant-1.1.2b1/assistant/nlp/chains/vectorstores/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      261 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/clear.py
--rw-r--r--   0 waser     (1000) waser     (1000)      193 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/exit.py
--rw-r--r--   0 waser     (1000) waser     (1000)     4537 2023-12-28 09:09:16.000000 assistant-1.1.2b1/assistant/nlp/interface.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1051 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/think.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2039 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/parser.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/procs/
--rw-r--r--   0 waser     (1000) waser     (1000)      696 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/procs/pipelines.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2545 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/procs/specs.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/assistant/ptk_shell/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      877 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/bindings.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3552 2024-05-08 06:48:57.000000 assistant-1.1.2b1/assistant/ptk_shell/completer.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2913 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/dialogs.py
--rw-r--r--   0 waser     (1000) waser     (1000)      254 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/floats.py
--rw-r--r--   0 waser     (1000) waser     (1000)      152 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/layout.py
--rw-r--r--   0 waser     (1000) waser     (1000)    17322 2024-01-25 22:39:37.000000 assistant-1.1.2b1/assistant/ptk_shell/shell.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5333 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/strformat_utils.py
--rw-r--r--   0 waser     (1000) waser     (1000)      696 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/styles.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2955 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/windows.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/assistant/say/
--rw-r--r--   0 waser     (1000) waser     (1000)     3901 2024-05-13 19:10:08.000000 assistant-1.1.2b1/assistant/say/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      448 2023-12-27 16:17:18.000000 assistant-1.1.2b1/assistant/say/interface.py
--rw-r--r--   0 waser     (1000) waser     (1000)       71 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/time.py
--rw-r--r--   0 waser     (1000) waser     (1000)      887 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/utils.py
--rw-r--r--   0 waser     (1000) waser     (1000)      641 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/version.py
--rw-r--r--   0 waser     (1000) waser     (1000)      537 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/vocabulary.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/assistant.egg-info/
--rw-r--r--   0 waser     (1000) waser     (1000)    12722 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)     3085 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/SOURCES.txt
--rw-r--r--   0 waser     (1000) waser     (1000)        1 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/dependency_links.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       71 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/entry_points.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      289 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/requires.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       18 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/top_level.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      888 2022-10-06 02:51:22.000000 assistant-1.1.2b1/pyproject.toml
--rw-r--r--   0 waser     (1000) waser     (1000)     3674 2024-05-14 13:41:36.256232 assistant-1.1.2b1/setup.cfg
--rw-r--r--   0 waser     (1000) waser     (1000)     3542 2024-05-13 20:21:47.000000 assistant-1.1.2b1/setup.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/tests/
--rw-r--r--   0 waser     (1000) waser     (1000)     5083 2023-11-30 06:13:11.000000 assistant-1.1.2b1/tests/test_execer.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/xontrib/
--rw-r--r--   0 waser     (1000) waser     (1000)     2241 2023-11-30 06:13:11.000000 assistant-1.1.2b1/xontrib/assistant.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.311809 assistant-1.2.0b1/
+-rw-r--r--   0 waser     (1000) waser     (1000)     1069 2022-03-17 17:48:10.000000 assistant-1.2.0b1/LICENSE
+-rw-r--r--   0 waser     (1000) waser     (1000)       16 2022-03-17 17:48:10.000000 assistant-1.2.0b1/MANIFEST.in
+-rw-r--r--   0 waser     (1000) waser     (1000)    12756 2024-05-21 18:11:27.311809 assistant-1.2.0b1/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)    10843 2024-02-18 19:52:01.000000 assistant-1.2.0b1/README.md
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.301809 assistant-1.2.0b1/assistant/
+-rw-r--r--   0 waser     (1000) waser     (1000)      502 2024-05-21 18:10:04.000000 assistant-1.2.0b1/assistant/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      114 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5674 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/_execer.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.301809 assistant-1.2.0b1/assistant/api/
+-rw-r--r--   0 waser     (1000) waser     (1000)      317 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/api/responses.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3867 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/as_client.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5428 2024-05-08 08:18:22.000000 assistant-1.2.0b1/assistant/as_service.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     7424 2024-05-21 18:02:57.000000 assistant-1.2.0b1/assistant/builtin_cmds.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     6792 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/codecache.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      132 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/conditions.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.305142 assistant-1.2.0b1/assistant/entry_points/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/entry_points/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      194 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/entry_points/run_assistant.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      157 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/execer.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3595 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/history.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      519 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/icons.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.305142 assistant-1.2.0b1/assistant/listen/
+-rw-r--r--   0 waser     (1000) waser     (1000)      436 2024-05-20 19:35:25.000000 assistant-1.2.0b1/assistant/listen/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-12-25 15:43:40.000000 assistant-1.2.0b1/assistant/listen/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1396 2024-05-13 22:55:29.000000 assistant-1.2.0b1/assistant/listen/interface.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2776 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/listen/main.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    24121 2024-05-21 15:35:18.000000 assistant-1.2.0b1/assistant/main.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.305142 assistant-1.2.0b1/assistant/manager/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/manager/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2355 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/manager/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     9813 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/manager/nlu.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    18387 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/manager/nlu_to_stt.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.305142 assistant-1.2.0b1/assistant/nlp/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/__init__.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.305142 assistant-1.2.0b1/assistant/nlp/chains/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      411 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/__main__.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.305142 assistant-1.2.0b1/assistant/nlp/chains/agents/
+-rw-r--r--   0 waser     (1000) waser     (1000)      689 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/agents/__executor__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2374 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/agents/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3010 2024-05-08 06:30:31.000000 assistant-1.2.0b1/assistant/nlp/chains/agents/assistant.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.305142 assistant-1.2.0b1/assistant/nlp/chains/callback_handlers/
+-rw-r--r--   0 waser     (1000) waser     (1000)     2074 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/callback_handlers/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3211 2024-05-21 14:37:23.000000 assistant-1.2.0b1/assistant/nlp/chains/code_pilot.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.305142 assistant-1.2.0b1/assistant/nlp/chains/data_loaders/
+-rw-r--r--   0 waser     (1000) waser     (1000)      158 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/data_loaders/__init__.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.305142 assistant-1.2.0b1/assistant/nlp/chains/data_splitter/
+-rw-r--r--   0 waser     (1000) waser     (1000)       76 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/data_splitter/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2996 2024-05-21 14:39:17.000000 assistant-1.2.0b1/assistant/nlp/chains/docs_explained.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.308476 assistant-1.2.0b1/assistant/nlp/chains/embeddings/
+-rw-r--r--   0 waser     (1000) waser     (1000)      184 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/embeddings/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     4647 2024-05-13 19:11:24.000000 assistant-1.2.0b1/assistant/nlp/chains/embeddings/assistant.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.308476 assistant-1.2.0b1/assistant/nlp/chains/memory/
+-rw-r--r--   0 waser     (1000) waser     (1000)      203 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/memory/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      536 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/memory/conversation_buffer.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.308476 assistant-1.2.0b1/assistant/nlp/chains/models/
+-rw-r--r--   0 waser     (1000) waser     (1000)      952 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/models/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      682 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/models/hf.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     6568 2024-02-22 21:10:49.000000 assistant-1.2.0b1/assistant/nlp/chains/models/vllm.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.308476 assistant-1.2.0b1/assistant/nlp/chains/parsers/
+-rw-r--r--   0 waser     (1000) waser     (1000)      156 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/parsers/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1833 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/parsers/column_csv.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     7620 2024-05-11 15:39:14.000000 assistant-1.2.0b1/assistant/nlp/chains/parsers/json.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     4783 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/parsers/markdown_json.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      831 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/persistent_session.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.308476 assistant-1.2.0b1/assistant/nlp/chains/prompts/
+-rw-r--r--   0 waser     (1000) waser     (1000)     5288 2024-05-20 19:50:27.000000 assistant-1.2.0b1/assistant/nlp/chains/prompts/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      699 2024-05-20 19:46:01.000000 assistant-1.2.0b1/assistant/nlp/chains/prompts/airoboros.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1612 2024-05-20 18:41:15.000000 assistant-1.2.0b1/assistant/nlp/chains/prompts/json.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.308476 assistant-1.2.0b1/assistant/nlp/chains/schema/
+-rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/schema/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2209 2024-05-08 06:48:37.000000 assistant-1.2.0b1/assistant/nlp/chains/schema/memory.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5399 2024-05-21 17:26:47.000000 assistant-1.2.0b1/assistant/nlp/chains/schema/vectorstore.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5878 2024-05-21 16:44:38.000000 assistant-1.2.0b1/assistant/nlp/chains/session.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.308476 assistant-1.2.0b1/assistant/nlp/chains/tools/
+-rw-r--r--   0 waser     (1000) waser     (1000)      406 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/tools/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1737 2024-05-21 16:54:03.000000 assistant-1.2.0b1/assistant/nlp/chains/tools/__retriever__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/tools/memory.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2021 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/tools/python.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      300 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/chains/tools/retriever.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1505 2024-01-13 19:49:07.000000 assistant-1.2.0b1/assistant/nlp/chains/tools/search.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5049 2024-01-05 02:36:06.000000 assistant-1.2.0b1/assistant/nlp/chains/tools/shell.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1762 2024-01-13 19:49:32.000000 assistant-1.2.0b1/assistant/nlp/chains/tools/wikipedia.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.308476 assistant-1.2.0b1/assistant/nlp/chains/vectorstores/
+-rw-r--r--   0 waser     (1000) waser     (1000)     2207 2024-01-13 19:43:16.000000 assistant-1.2.0b1/assistant/nlp/chains/vectorstores/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      261 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/clear.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      193 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/exit.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     4537 2023-12-28 09:09:16.000000 assistant-1.2.0b1/assistant/nlp/interface.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1051 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/nlp/think.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2039 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/parser.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.308476 assistant-1.2.0b1/assistant/procs/
+-rw-r--r--   0 waser     (1000) waser     (1000)      696 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/procs/pipelines.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2545 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/procs/specs.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.311809 assistant-1.2.0b1/assistant/ptk_shell/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/ptk_shell/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      877 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/ptk_shell/bindings.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3552 2024-05-08 06:48:57.000000 assistant-1.2.0b1/assistant/ptk_shell/completer.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2913 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/ptk_shell/dialogs.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      254 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/ptk_shell/floats.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      152 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/ptk_shell/layout.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    17459 2024-05-21 16:04:08.000000 assistant-1.2.0b1/assistant/ptk_shell/shell.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5333 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/ptk_shell/strformat_utils.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      696 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/ptk_shell/styles.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2955 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/ptk_shell/windows.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.311809 assistant-1.2.0b1/assistant/say/
+-rw-r--r--   0 waser     (1000) waser     (1000)     3932 2024-05-20 19:35:12.000000 assistant-1.2.0b1/assistant/say/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      448 2023-12-27 16:17:18.000000 assistant-1.2.0b1/assistant/say/interface.py
+-rw-r--r--   0 waser     (1000) waser     (1000)       71 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/time.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      887 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/utils.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      641 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/version.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      537 2023-12-25 15:43:41.000000 assistant-1.2.0b1/assistant/vocabulary.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.311809 assistant-1.2.0b1/assistant.egg-info/
+-rw-r--r--   0 waser     (1000) waser     (1000)    12756 2024-05-21 18:11:27.000000 assistant-1.2.0b1/assistant.egg-info/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)     3085 2024-05-21 18:11:27.000000 assistant-1.2.0b1/assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)        1 2024-05-21 18:11:27.000000 assistant-1.2.0b1/assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       71 2024-05-21 18:11:27.000000 assistant-1.2.0b1/assistant.egg-info/entry_points.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      311 2024-05-21 18:11:27.000000 assistant-1.2.0b1/assistant.egg-info/requires.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       18 2024-05-21 18:11:27.000000 assistant-1.2.0b1/assistant.egg-info/top_level.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      888 2022-10-06 02:51:22.000000 assistant-1.2.0b1/pyproject.toml
+-rw-r--r--   0 waser     (1000) waser     (1000)     3674 2024-05-21 18:11:27.311809 assistant-1.2.0b1/setup.cfg
+-rw-r--r--   0 waser     (1000) waser     (1000)     3572 2024-05-21 17:29:29.000000 assistant-1.2.0b1/setup.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.311809 assistant-1.2.0b1/tests/
+-rw-r--r--   0 waser     (1000) waser     (1000)     5083 2023-11-30 06:13:11.000000 assistant-1.2.0b1/tests/test_execer.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-21 18:11:27.311809 assistant-1.2.0b1/xontrib/
+-rw-r--r--   0 waser     (1000) waser     (1000)     2241 2023-11-30 06:13:11.000000 assistant-1.2.0b1/xontrib/assistant.py
```

### Comparing `assistant-1.1.2b1/LICENSE` & `assistant-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/PKG-INFO` & `assistant-1.2.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant
-Version: 1.1.2b1
+Version: 1.2.0b1
 Summary: Your very own Assistant. Because you deserve it.
 Home-page: https://gitlab.com/waser-technologies/technologies/assistant
 Author: Danny Waser
 Author-email: danny@waser.tech
 License: MIT
 Project-URL: Documentation, https://gitlab.com/waser-technologies/technologies/assistant/blob/master/README.md
 Project-URL: Code, https://gitlab.com/waser-technologies/technologies/assistant
@@ -18,21 +18,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
 Classifier: Topic :: System :: Shells
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Terminals
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ftfy
 Requires-Dist: pydub
 Requires-Dist: pygments
 Requires-Dist: xonsh
+Requires-Dist: prompt_toolkit>3.0.36
 Requires-Dist: attrs
 Requires-Dist: questionary
 Requires-Dist: datasets
 Requires-Dist: transformers
 Requires-Dist: sentencepiece
 Requires-Dist: sentence-transformers
 Requires-Dist: bitsandbytes
```

### Comparing `assistant-1.1.2b1/README.md` & `assistant-1.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/_execer.py` & `assistant-1.2.0b1/assistant/_execer.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/as_client.py` & `assistant-1.2.0b1/assistant/as_client.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/as_service.py` & `assistant-1.2.0b1/assistant/as_service.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/builtin_cmds.py` & `assistant-1.2.0b1/assistant/builtin_cmds.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,16 +66,32 @@
   -P, --physical   avoid all symlinks
       --help       display this help and exit
 This version of pwd was written in Python for the xonsh project: http://xon.sh
 Based on pwd from GNU coreutils: http://www.gnu.org/software/coreutils/"""
 
 
 def assistant_fn(args, stdin=None):
-    print("Yes?")
+    response = None
+    if args is None:
+        response = XSH.shell.shell.kernel_interface.assistant("Assistant?")
+
+    if args[0] == "-h" or args[0] == "--help" or args[0] == "help":
+        response = XSH.shell.shell.kernel_interface.assistant("assistant --help")
+    
+    if args[0] == "version" or args[0] == "--version":
+        response = XSH.shell.shell.kernel_interface.assistant("assistant --version")
+    
+    if response is None and args is not None:
+        response = XSH.shell.shell.kernel_interface.assistant("assistant " + " ".join(args))   
+    
+    if response:
+        print(response)
+    return 0
 
+    
 # @unthreadable
 def listen_fn(args, stdin=None):
     """Listen for assistant: listen only one sentence by default
     You can type listen to listen for one sentence.
     To listen continuously, type listen start (or stop to stop).
     """
     if args is None:
```

### Comparing `assistant-1.1.2b1/assistant/codecache.py` & `assistant-1.2.0b1/assistant/codecache.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/history.py` & `assistant-1.2.0b1/assistant/history.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/icons.py` & `assistant-1.2.0b1/assistant/icons.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/listen/interface.py` & `assistant-1.2.0b1/assistant/listen/interface.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/listen/main.py` & `assistant-1.2.0b1/assistant/listen/main.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/main.py` & `assistant-1.2.0b1/assistant/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,15 +453,15 @@
         signal.signal(signal.SIGTTOU, func_sig_ttin_ttou)
 
     events.on_post_init.fire()
 
     env = XSH.env
     shell = XSH.shell
     history = XSH.history
-    aliases = _set_aliases(XSH.aliases)
+    aliases = _set_aliases(XSH.aliases) # initialiazes assistant's aliases
     
     
     exit_code = 0
 
     if args.version:
         print_version()
         return exit_code
```

### Comparing `assistant-1.1.2b1/assistant/manager/__main__.py` & `assistant-1.2.0b1/assistant/manager/__main__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/manager/nlu.py` & `assistant-1.2.0b1/assistant/manager/nlu.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/manager/nlu_to_stt.py` & `assistant-1.2.0b1/assistant/manager/nlu_to_stt.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/agents/__executor__.py` & `assistant-1.2.0b1/assistant/nlp/chains/agents/__executor__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/agents/__init__.py` & `assistant-1.2.0b1/assistant/nlp/chains/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/agents/assistant.py` & `assistant-1.2.0b1/assistant/nlp/chains/agents/assistant.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/callback_handlers/__init__.py` & `assistant-1.2.0b1/assistant/nlp/chains/callback_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/code_pilot.py` & `assistant-1.2.0b1/assistant/nlp/chains/code_pilot.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Ain't nobody got time to read the docs?
 # Just ask this chain about it.
 # It can also extrapolate custom code from the docs.
 
 from langchain.document_loaders import readthedocs
 from langchain.chains import ConversationalRetrievalChain
 from langchain.chains.chat_vector_db.prompts import (CONDENSE_QUESTION_PROMPT, QA_PROMPT)
-from langchain.chains.llm import LLMChain
+# from langchain.chains.llm import LLMChain
 from langchain.prompts import PromptTemplate
 #from langchain import OpenAI
 
 from assistant.nlp.chains.vectorstores import get_vectorstore_from_readthedocs
 from assistant.nlp.chains.embeddings import get_embeddings
 from assistant.nlp.chains.models import get_llm
 
@@ -59,17 +59,18 @@
         prompt_template = """Use the context below to write a piece of code to satisfy the query below:
             Context: {context}
             Query: {query}
             Code: """
         self.prompt = PromptTemplate(template=prompt_template, input_variables=["context", "query"])
 
     def _initialize_chain(self):
-        self.generator = LLMChain(
-            llm=self.llm, prompt=self.prompt
-        )
+        # self.generator = LLMChain(
+        #     llm=self.llm, prompt=self.prompt
+        # )
+        self.generator = self.prompt | self.llm
     
     def __call__(self, query):
         docs = self.vectorstore.similarity_search(query, k=4)
         docs_content = "\n".join([doc.page_content for doc in docs])
         input_dict = {"context": docs_content, "query": query}
         return self.clear_output(self.generator.run(input_dict))
```

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/docs_explained.py` & `assistant-1.2.0b1/assistant/nlp/chains/docs_explained.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # It can also extrapolate custom code from the docs.
 
 import subprocess
 
 from langchain.document_loaders import readthedocs
 from langchain.chains import ConversationalRetrievalChain
 from langchain.chains.chat_vector_db.prompts import (CONDENSE_QUESTION_PROMPT, QA_PROMPT)
-from langchain.chains.llm import LLMChain
+# from langchain.chains.llm import LLMChain
 from langchain.chains.question_answering import load_qa_chain
 from langchain.memory import ConversationBufferMemory
 
 from assistant.nlp.chains.vectorstores import get_vectorstore_from_readthedocs
 from assistant.nlp.chains.embeddings import get_embeddings
 from assistant.nlp.chains.models import get_llm
 
@@ -50,17 +50,18 @@
         self.llm = get_llm(max_tokens=self.max_tokens, temperature=self.temperature, streaming=self.streaming, callbacks=self.callbacks)
         self.embeddings = get_embeddings()
 
     def _initialize_vectorstore(self):
         self.vectorstore = get_vectorstore_from_readthedocs(self.readthedocs_url, self.embeddings)
     
     def _initialize_chain(self):
-        self.question_generator = LLMChain(
-            llm=self.llm, prompt=CONDENSE_QUESTION_PROMPT, # callback_manager=manager
-        )
+        # self.question_generator = LLMChain(
+        #     llm=self.llm, prompt=CONDENSE_QUESTION_PROMPT, # callback_manager=manager
+        # )
+        self.question_generator = CONDENSE_QUESTION_PROMPT | self.llm
         self.doc_chain = load_qa_chain(
             self.llm, chain_type="stuff", prompt=QA_PROMPT, # callback_manager=manager
         )
 
         self.memory = ConversationBufferMemory(memory_key="chat_history")
 
         self.qa = ConversationalRetrievalChain(
```

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/embeddings/assistant.py` & `assistant-1.2.0b1/assistant/nlp/chains/embeddings/assistant.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/memory/conversation_buffer.py` & `assistant-1.2.0b1/assistant/nlp/chains/memory/conversation_buffer.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/models/__init__.py` & `assistant-1.2.0b1/assistant/nlp/chains/models/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/models/hf.py` & `assistant-1.2.0b1/assistant/nlp/chains/models/hf.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/models/vllm.py` & `assistant-1.2.0b1/assistant/nlp/chains/models/vllm.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/parsers/column_csv.py` & `assistant-1.2.0b1/assistant/nlp/chains/parsers/column_csv.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/parsers/json.py` & `assistant-1.2.0b1/assistant/nlp/chains/parsers/json.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/parsers/markdown_json.py` & `assistant-1.2.0b1/assistant/nlp/chains/parsers/markdown_json.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/persistent_session.py` & `assistant-1.2.0b1/assistant/nlp/chains/persistent_session.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/prompts/__init__.py` & `assistant-1.2.0b1/assistant/nlp/chains/prompts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,16 @@
 
         # Format the template
         return self.template.format(**kwargs)
 
     def get_guide_from_query(self, query):
         """Get the guide from the query."""
         if self.retriever:
-            documents = self.retriever.get_relevant_documents(query=query)
+            # documents = self.retriever.get_relevant_documents(query=query)
+            documents = self.retriever.invoke({"input": query})
             if documents:
                 return documents[0].page_content
         return "No relevant guide for the query where found. Do what you can; with what you have."
 
     def get_environ(self):
         """Get the environment variables highlight."""
         LANG = os.environ.get("LANG", "en_US.UTF-8")
```

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/prompts/json.py` & `assistant-1.2.0b1/assistant/nlp/chains/prompts/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 system_prompt = """You are Assistant, a sentient artificial intelligence.
 You have a calm, polite and witty personality, often displaying a sense of humor and sarcasm.
 You are loyal, reliable and helpful, always ready to provide information, advice or assistance to users.
 
 I am the User and you are my Assistant. Be respectful when addressing me.
 
+You should act as my personal shell, providing me with information, advice, and assistance as needed.
+
 Environment highlights:
 
 {env}
 """
 
 instruction_prompt = f"""{BOI}{JSON_FUNC.format(query='{input}', functions='{tools}', guide='{guide}')}{EOI}{{agent_scratchpad}}{BOS}"""
```

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/schema/memory.py` & `assistant-1.2.0b1/assistant/nlp/chains/schema/memory.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/schema/vectorstore.py` & `assistant-1.2.0b1/assistant/nlp/chains/schema/vectorstore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 from pathlib import Path
 from typing import List
 from langchain.docstore.document import Document
 from langchain.schema.vectorstore import VectorStoreRetriever
 
 # from langchain.pydantic_v1 import Field
 # from langchain.vectorstores import Chroma
@@ -55,15 +57,16 @@
         Args:
             query (str): The query string.
 
         Returns:
             List[Document]: A list of relevant documents.
         """
 
-        results = self.vectorstore.get_relevant_documents(query=query)
+        # results = self.vectorstore.get_relevant_documents(query=query)
+        results = self.vectorstore.invoke(query['input'])
         # return a set of unique guides
         r = {}
         for result in results:
             # r[result.metadata['action']] = result.metadata['guide']
             return [
                 Document(
                     page_content=result.metadata["guide"],
```

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/session.py` & `assistant-1.2.0b1/assistant/nlp/chains/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.verbose = verbose
         self.memory_key = "chat_history"
         
         self._initialize_llm()
         self._initialize_prompt()
         self._initialize_output_parser()
         self._initialize_memory()
-        self._initialize_chain()
+        # self._initialize_chain()
         self._initialize_tools()
         self._initialize_agent()
           
     def _initialize_llm(self):
         self.llm = get_llm(max_tokens=self.max_tokens, temperature=self.temperature, streaming=self.streaming, callbacks=self.callbacks)
 
     def _initialize_prompt(self):
@@ -47,27 +47,39 @@
     
     def _initialize_output_parser(self):
         self.output_parser = get_output_parser()
     
     def _initialize_memory(self):
         self.memory = AssistantConversationBufferMemory(memory_key=self.memory_key, input_key="input", output_key="output", human_prefix="User", ai_prefix="Assistant")
 
-    def _initialize_chain(self):
-        self.llm_chain = LLMChain(llm=self.llm, prompt=self.prompt)
+    # def _initialize_chain(self):
+        # self.llm_chain =  self.prompt | self.llm
+        # self.llm_chain = LLMChain(llm=self.llm, prompt=self.prompt)
     
     def _initialize_tools(self):
         self.tools = get_all_tools()
+        # self.llm.bind_tools(self.tools)
 
     def _initialize_agent(self, max_iterations=20):
         tool_names = [tool.name for tool in self.tools]
-        self.agent = AssistantSingleActionAgent(
-            llm_chain=self.llm_chain,
-            output_parser=self.output_parser,
-            stop=["<|im_end|>\n", "<|im_stop|>", "<|im_start|>", "<|im_end|>", "<|endoftext|>", """<|im_stop|>\n""", "\n}\n}\n\n"],
-            allowed_tools=tool_names
+        # self.agent = AssistantSingleActionAgent(
+        #     llm_chain=self.llm_chain,
+        #     output_parser=self.output_parser,
+        #     stop=["<|im_end|>\n", "<|im_stop|>", "<|im_start|>", "<|im_end|>", "<|endoftext|>", """<|im_stop|>\n""", "\n}\n}\n\n"],
+        #     allowed_tools=tool_names
+        # )
+        self.agent = (
+            {
+                'input': lambda x: x['input'],
+                'intermediate_steps': lambda x: x['intermediate_steps'],
+                'chat_history': lambda x: x['chat_history'],
+            }
+            | self.prompt
+            | self.llm
+            | self.output_parser
         )
         self.agent_executor = AgentExecutor.from_agent_and_tools(agent=self.agent, tools=self.tools, verbose=self.verbose, max_iterations=max_iterations, memory=self.memory)
 
     def __call__(self, message: str):
         output = self.agent_executor.invoke({'input': message})
         return self.process_output(output['output'])
```

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/tools/__retriever__.py` & `assistant-1.2.0b1/assistant/nlp/chains/tools/__retriever__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,8 +43,9 @@
     Args:
         retriever: The retriever object used to retrieve documents.
         context: The context used to retrieve relevant documents.
 
     Returns:
         The relevant documents retrieved from the retriever.
     """
-    return retriever.get_relevant_documents(context)
+    # return retriever.get_relevant_documents(context)
+    return retriever.invoke(context)
```

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/tools/python.py` & `assistant-1.2.0b1/assistant/nlp/chains/tools/python.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/tools/search.py` & `assistant-1.2.0b1/assistant/nlp/chains/tools/search.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/tools/shell.py` & `assistant-1.2.0b1/assistant/nlp/chains/tools/shell.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/tools/wikipedia.py` & `assistant-1.2.0b1/assistant/nlp/chains/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/chains/vectorstores/__init__.py` & `assistant-1.2.0b1/assistant/nlp/chains/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/interface.py` & `assistant-1.2.0b1/assistant/nlp/interface.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/nlp/think.py` & `assistant-1.2.0b1/assistant/nlp/think.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/parser.py` & `assistant-1.2.0b1/assistant/parser.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/procs/pipelines.py` & `assistant-1.2.0b1/assistant/procs/pipelines.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/procs/specs.py` & `assistant-1.2.0b1/assistant/procs/specs.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/ptk_shell/bindings.py` & `assistant-1.2.0b1/assistant/ptk_shell/bindings.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/ptk_shell/completer.py` & `assistant-1.2.0b1/assistant/ptk_shell/completer.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/ptk_shell/dialogs.py` & `assistant-1.2.0b1/assistant/ptk_shell/dialogs.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/ptk_shell/shell.py` & `assistant-1.2.0b1/assistant/ptk_shell/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# import warnings
+# warnings.filterwarnings("ignore", category=DeprecationWarning, module="prompt_toolkit.eventloop.utils", lineno=118)
+
 import os, sys
 import time
 import xonsh.tools as xt
 import subprocess
 import threading
 
 from io import StringIO
```

### Comparing `assistant-1.1.2b1/assistant/ptk_shell/strformat_utils.py` & `assistant-1.2.0b1/assistant/ptk_shell/strformat_utils.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/ptk_shell/styles.py` & `assistant-1.2.0b1/assistant/ptk_shell/styles.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/ptk_shell/windows.py` & `assistant-1.2.0b1/assistant/ptk_shell/windows.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/say/__init__.py` & `assistant-1.2.0b1/assistant/say/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import json
 import websockets
 import asyncio
 import warnings
 
 warnings.filterwarnings("ignore", category=DeprecationWarning, module="pydub")
 
@@ -11,18 +12,19 @@
 from assistant import I18N
 
 try:
     from say.TTS import utils as tts_utils
     from say.TTS.as_client import tts
     # from num2words import num2words
 except (ModuleNotFoundError, ImportError) as e:
-    print(e)
-    print("For Assistant to speak, you need to install the say module.")
-    print("Run the following command:\n```shell\npip install -r tts-say\n```")
-    sys.exit(1)
+    # print(e)
+    # print("For Assistant to speak, you need to install the say module.")
+    # print("Run the following command:\n```shell\npip install -r tts-say\n```")
+    # sys.exit(1)
+    raise e
 
 TTS_CONFIG = tts_utils.get_config_or_default()
 is_allowed_to_speak = tts_utils.is_allowed_to_speak(TTS_CONFIG)
 if not is_allowed_to_speak:
     print("System has not user autorization to speak.")
```

### Comparing `assistant-1.1.2b1/assistant/utils.py` & `assistant-1.2.0b1/assistant/utils.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/version.py` & `assistant-1.2.0b1/assistant/version.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant/vocabulary.py` & `assistant-1.2.0b1/assistant/vocabulary.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/assistant.egg-info/PKG-INFO` & `assistant-1.2.0b1/assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant
-Version: 1.1.2b1
+Version: 1.2.0b1
 Summary: Your very own Assistant. Because you deserve it.
 Home-page: https://gitlab.com/waser-technologies/technologies/assistant
 Author: Danny Waser
 Author-email: danny@waser.tech
 License: MIT
 Project-URL: Documentation, https://gitlab.com/waser-technologies/technologies/assistant/blob/master/README.md
 Project-URL: Code, https://gitlab.com/waser-technologies/technologies/assistant
@@ -18,21 +18,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
 Classifier: Topic :: System :: Shells
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Terminals
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ftfy
 Requires-Dist: pydub
 Requires-Dist: pygments
 Requires-Dist: xonsh
+Requires-Dist: prompt_toolkit>3.0.36
 Requires-Dist: attrs
 Requires-Dist: questionary
 Requires-Dist: datasets
 Requires-Dist: transformers
 Requires-Dist: sentencepiece
 Requires-Dist: sentence-transformers
 Requires-Dist: bitsandbytes
```

### Comparing `assistant-1.1.2b1/assistant.egg-info/SOURCES.txt` & `assistant-1.2.0b1/assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/pyproject.toml` & `assistant-1.2.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/setup.cfg` & `assistant-1.2.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/setup.py` & `assistant-1.2.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 version = __version__
 
 required_packages = [
         'ftfy',
         'pydub',
         'pygments',
         'xonsh',
+        'prompt_toolkit>3.0.36',
         'attrs',
         'questionary',
 #        'nest-asyncio',
         'datasets',
         'transformers',
         'sentencepiece',
         'sentence-transformers',
@@ -76,15 +77,15 @@
     version=version,
     license='MIT',
     author='Danny Waser',
     author_email='danny@waser.tech',
     description=catchphrase,
     long_description=long_description,
     long_description_content_type='text/markdown',
-    python_requires='>=3.8,<3.12',
+    python_requires='>=3.8,<4',
     install_requires=required_packages,
     packages=packaged_modules,
     package_dir={'xontrib': 'xontrib'},
     package_data={'xontrib': ['*.xsh']},
     platforms='any',
     entry_points={
         'console_scripts': [
```

### Comparing `assistant-1.1.2b1/tests/test_execer.py` & `assistant-1.2.0b1/tests/test_execer.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.2b1/xontrib/assistant.py` & `assistant-1.2.0b1/xontrib/assistant.py`

 * *Files identical despite different names*

