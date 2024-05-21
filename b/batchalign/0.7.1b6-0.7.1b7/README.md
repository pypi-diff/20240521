# Comparing `tmp/batchalign-0.7.1b6.tar.gz` & `tmp/batchalign-0.7.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchalign-0.7.1b6.tar", last modified: Fri May 17 19:31:01 2024, max compression
+gzip compressed data, was "batchalign-0.7.1b7.tar", last modified: Tue May 21 16:28:14 2024, max compression
```

## Comparing `batchalign-0.7.1b6.tar` & `batchalign-0.7.1b7.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.911154 batchalign-0.7.1b6/
--rw-r--r--   0 houjun     (501) staff       (20)     1464 2024-01-21 18:39:49.000000 batchalign-0.7.1b6/LICENSE
--rw-r--r--   0 houjun     (501) staff       (20)      149 2024-04-04 00:32:13.000000 batchalign-0.7.1b6/MANIFEST.in
--rw-r--r--   0 houjun     (501) staff       (20)    11951 2024-05-17 19:31:01.910881 batchalign-0.7.1b6/PKG-INFO
--rw-r--r--   0 houjun     (501) staff       (20)     9074 2024-05-12 20:56:18.000000 batchalign-0.7.1b6/README.md
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.892410 batchalign-0.7.1b6/batchalign/
--rw-r--r--   0 houjun     (501) staff       (20)      497 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)       63 2023-12-17 23:06:14.000000 batchalign-0.7.1b6/batchalign/__main__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.893691 batchalign-0.7.1b6/batchalign/cli/
--rw-r--r--   0 houjun     (501) staff       (20)       28 2023-12-17 01:12:36.000000 batchalign-0.7.1b6/batchalign/cli/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     9892 2024-04-14 17:16:38.000000 batchalign-0.7.1b6/batchalign/cli/cli.py
--rw-r--r--   0 houjun     (501) staff       (20)     7568 2024-04-14 17:16:00.000000 batchalign-0.7.1b6/batchalign/cli/dispatch.py
--rw-r--r--   0 houjun     (501) staff       (20)      777 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/constants.py
--rw-r--r--   0 houjun     (501) staff       (20)    14798 2024-04-20 21:56:18.000000 batchalign-0.7.1b6/batchalign/document.py
--rw-r--r--   0 houjun     (501) staff       (20)      199 2023-12-17 07:10:18.000000 batchalign-0.7.1b6/batchalign/errors.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.894142 batchalign-0.7.1b6/batchalign/formats/
--rw-r--r--   0 houjun     (501) staff       (20)       62 2024-03-18 04:57:14.000000 batchalign-0.7.1b6/batchalign/formats/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      246 2023-12-18 07:14:44.000000 batchalign-0.7.1b6/batchalign/formats/base.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.895531 batchalign-0.7.1b6/batchalign/formats/chat/
--rw-r--r--   0 houjun     (501) staff       (20)       27 2024-03-18 04:57:14.000000 batchalign-0.7.1b6/batchalign/formats/chat/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     4676 2024-04-05 17:07:15.000000 batchalign-0.7.1b6/batchalign/formats/chat/file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3701 2024-04-05 17:08:43.000000 batchalign-0.7.1b6/batchalign/formats/chat/generator.py
--rw-r--r--   0 houjun     (501) staff       (20)     7481 2023-12-28 03:10:19.000000 batchalign-0.7.1b6/batchalign/formats/chat/lexer.py
--rw-r--r--   0 houjun     (501) staff       (20)    12408 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/formats/chat/parser.py
--rw-r--r--   0 houjun     (501) staff       (20)     5217 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/formats/chat/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.896357 batchalign-0.7.1b6/batchalign/formats/textgrid/
--rw-r--r--   0 houjun     (501) staff       (20)       31 2023-12-18 07:14:59.000000 batchalign-0.7.1b6/batchalign/formats/textgrid/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3340 2024-03-18 04:57:14.000000 batchalign-0.7.1b6/batchalign/formats/textgrid/file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3485 2023-12-18 07:35:03.000000 batchalign-0.7.1b6/batchalign/formats/textgrid/generator.py
--rw-r--r--   0 houjun     (501) staff       (20)     3888 2023-12-18 05:59:42.000000 batchalign-0.7.1b6/batchalign/formats/textgrid/parser.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.896912 batchalign-0.7.1b6/batchalign/models/
--rw-r--r--   0 houjun     (501) staff       (20)      195 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      454 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/models/resolve.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.897512 batchalign-0.7.1b6/batchalign/models/speaker/
--rw-r--r--   0 houjun     (501) staff       (20)       36 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/speaker/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     5583 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/speaker/config.yaml
--rw-r--r--   0 houjun     (501) staff       (20)     3246 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/speaker/infer.py
--rw-r--r--   0 houjun     (501) staff       (20)     1808 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/speaker/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.897876 batchalign-0.7.1b6/batchalign/models/training/
--rw-r--r--   0 houjun     (501) staff       (20)       22 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/models/training/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      576 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/training/run.py
--rw-r--r--   0 houjun     (501) staff       (20)     3357 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/models/training/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     3081 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/models/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.898625 batchalign-0.7.1b6/batchalign/models/utterance/
--rw-r--r--   0 houjun     (501) staff       (20)       39 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/utterance/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     5447 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/utterance/dataset.py
--rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/utterance/execute.py
--rw-r--r--   0 houjun     (501) staff       (20)     3179 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/utterance/infer.py
--rw-r--r--   0 houjun     (501) staff       (20)     3057 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/utterance/prep.py
--rw-r--r--   0 houjun     (501) staff       (20)     4359 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/utterance/train.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.899001 batchalign-0.7.1b6/batchalign/models/whisper/
--rw-r--r--   0 houjun     (501) staff       (20)       76 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/whisper/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     7340 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/models/whisper/infer_asr.py
--rw-r--r--   0 houjun     (501) staff       (20)     5264 2024-04-08 19:13:44.000000 batchalign-0.7.1b6/batchalign/models/whisper/infer_fa.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.899661 batchalign-0.7.1b6/batchalign/pipelines/
--rw-r--r--   0 houjun     (501) staff       (20)      449 2024-04-14 00:00:03.000000 batchalign-0.7.1b6/batchalign/pipelines/__init__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.899974 batchalign-0.7.1b6/batchalign/pipelines/analysis/
--rw-r--r--   0 houjun     (501) staff       (20)       35 2024-02-05 03:35:25.000000 batchalign-0.7.1b6/batchalign/pipelines/analysis/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     2557 2024-02-05 03:35:25.000000 batchalign-0.7.1b6/batchalign/pipelines/analysis/eval.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.900832 batchalign-0.7.1b6/batchalign/pipelines/asr/
--rw-r--r--   0 houjun     (501) staff       (20)       99 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/pipelines/asr/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3723 2024-04-14 05:49:03.000000 batchalign-0.7.1b6/batchalign/pipelines/asr/rev.py
--rw-r--r--   0 houjun     (501) staff       (20)     7227 2024-04-14 04:23:55.000000 batchalign-0.7.1b6/batchalign/pipelines/asr/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     2063 2024-04-14 05:49:03.000000 batchalign-0.7.1b6/batchalign/pipelines/asr/whisper.py
--rw-r--r--   0 houjun     (501) staff       (20)     4403 2024-04-14 05:49:03.000000 batchalign-0.7.1b6/batchalign/pipelines/asr/whisperx.py
--rw-r--r--   0 houjun     (501) staff       (20)     1994 2024-02-05 03:35:25.000000 batchalign-0.7.1b6/batchalign/pipelines/base.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.901852 batchalign-0.7.1b6/batchalign/pipelines/cleanup/
--rw-r--r--   0 houjun     (501) staff       (20)       52 2023-12-16 19:37:43.000000 batchalign-0.7.1b6/batchalign/pipelines/cleanup/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)       93 2023-12-17 00:16:09.000000 batchalign-0.7.1b6/batchalign/pipelines/cleanup/cleanup.py
--rw-r--r--   0 houjun     (501) staff       (20)      579 2024-02-05 03:35:25.000000 batchalign-0.7.1b6/batchalign/pipelines/cleanup/disfluencies.py
--rw-r--r--   0 houjun     (501) staff       (20)     2161 2023-12-08 20:58:29.000000 batchalign-0.7.1b6/batchalign/pipelines/cleanup/parse_support.py
--rw-r--r--   0 houjun     (501) staff       (20)     2624 2024-02-05 03:35:25.000000 batchalign-0.7.1b6/batchalign/pipelines/cleanup/retrace.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.902189 batchalign-0.7.1b6/batchalign/pipelines/cleanup/support/
--rw-r--r--   0 houjun     (501) staff       (20)      141 2023-12-09 06:23:35.000000 batchalign-0.7.1b6/batchalign/pipelines/cleanup/support/filled_pauses.eng
--rw-r--r--   0 houjun     (501) staff       (20)      213 2023-12-09 06:23:34.000000 batchalign-0.7.1b6/batchalign/pipelines/cleanup/support/replacements.eng
--rw-r--r--   0 houjun     (501) staff       (20)      203 2024-03-18 04:54:03.000000 batchalign-0.7.1b6/batchalign/pipelines/cleanup/support/test.test
--rw-r--r--   0 houjun     (501) staff       (20)     4135 2024-05-17 19:29:50.000000 batchalign-0.7.1b6/batchalign/pipelines/dispatch.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.902542 batchalign-0.7.1b6/batchalign/pipelines/fa/
--rw-r--r--   0 houjun     (501) staff       (20)       40 2023-12-16 01:03:14.000000 batchalign-0.7.1b6/batchalign/pipelines/fa/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     7492 2024-04-20 18:30:40.000000 batchalign-0.7.1b6/batchalign/pipelines/fa/whisper_fa.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.902852 batchalign-0.7.1b6/batchalign/pipelines/morphosyntax/
--rw-r--r--   0 houjun     (501) staff       (20)       29 2023-12-16 23:54:03.000000 batchalign-0.7.1b6/batchalign/pipelines/morphosyntax/__init__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.903055 batchalign-0.7.1b6/batchalign/pipelines/morphosyntax/fr/
--rw-r--r--   0 houjun     (501) staff       (20)     1147 2023-12-29 00:44:35.000000 batchalign-0.7.1b6/batchalign/pipelines/morphosyntax/fr/case.py
--rw-r--r--   0 houjun     (501) staff       (20)    28591 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/pipelines/morphosyntax/ud.py
--rw-r--r--   0 houjun     (501) staff       (20)     7482 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/pipelines/pipeline.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.903421 batchalign-0.7.1b6/batchalign/pipelines/speaker/
--rw-r--r--   0 houjun     (501) staff       (20)       44 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/pipelines/speaker/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     2367 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/batchalign/pipelines/speaker/nemo_speaker.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.904086 batchalign-0.7.1b6/batchalign/pipelines/utr/
--rw-r--r--   0 houjun     (501) staff       (20)       76 2024-01-03 22:34:21.000000 batchalign-0.7.1b6/batchalign/pipelines/utr/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3525 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/pipelines/utr/rev_utr.py
--rw-r--r--   0 houjun     (501) staff       (20)     2303 2024-04-19 03:00:06.000000 batchalign-0.7.1b6/batchalign/pipelines/utr/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     1559 2024-02-05 03:35:25.000000 batchalign-0.7.1b6/batchalign/pipelines/utr/whisper_utr.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.904493 batchalign-0.7.1b6/batchalign/pipelines/utterance/
--rw-r--r--   0 houjun     (501) staff       (20)       48 2024-04-13 19:17:01.000000 batchalign-0.7.1b6/batchalign/pipelines/utterance/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)    10922 2024-04-16 21:19:29.000000 batchalign-0.7.1b6/batchalign/pipelines/utterance/ud_utterance.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.905140 batchalign-0.7.1b6/batchalign/tests/
--rw-r--r--   0 houjun     (501) staff       (20)        0 2023-11-18 22:44:12.000000 batchalign-0.7.1b6/batchalign/tests/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     1497 2024-03-18 04:54:03.000000 batchalign-0.7.1b6/batchalign/tests/conftest.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.890016 batchalign-0.7.1b6/batchalign/tests/formats/
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.906120 batchalign-0.7.1b6/batchalign/tests/formats/chat/
--rw-r--r--   0 houjun     (501) staff       (20)      999 2024-03-18 04:57:14.000000 batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3913 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_generator.py
--rw-r--r--   0 houjun     (501) staff       (20)      714 2023-12-24 23:29:13.000000 batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_lexer.py
--rw-r--r--   0 houjun     (501) staff       (20)    10624 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_parser.py
--rw-r--r--   0 houjun     (501) staff       (20)     1046 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.906263 batchalign-0.7.1b6/batchalign/tests/formats/textgrid/
--rw-r--r--   0 houjun     (501) staff       (20)     2699 2024-03-18 04:54:03.000000 batchalign-0.7.1b6/batchalign/tests/formats/textgrid/test_textgrid.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.906832 batchalign-0.7.1b6/batchalign/tests/pipelines/
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.906980 batchalign-0.7.1b6/batchalign/tests/pipelines/analysis/
--rw-r--r--   0 houjun     (501) staff       (20)      604 2024-02-05 03:35:25.000000 batchalign-0.7.1b6/batchalign/tests/pipelines/analysis/test_eval.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.907345 batchalign-0.7.1b6/batchalign/tests/pipelines/asr/
--rw-r--r--   0 houjun     (501) staff       (20)      938 2024-03-18 04:54:03.000000 batchalign-0.7.1b6/batchalign/tests/pipelines/asr/test_asr_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)     1570 2024-01-02 20:37:42.000000 batchalign-0.7.1b6/batchalign/tests/pipelines/asr/test_asr_utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.907716 batchalign-0.7.1b6/batchalign/tests/pipelines/cleanup/
--rw-r--r--   0 houjun     (501) staff       (20)     2716 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/tests/pipelines/cleanup/test_disfluency.py
--rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-03-18 04:54:03.000000 batchalign-0.7.1b6/batchalign/tests/pipelines/cleanup/test_parse_support.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.907860 batchalign-0.7.1b6/batchalign/tests/pipelines/fa/
--rw-r--r--   0 houjun     (501) staff       (20)      261 2024-04-08 19:15:55.000000 batchalign-0.7.1b6/batchalign/tests/pipelines/fa/test_fa_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)      977 2024-03-18 04:54:03.000000 batchalign-0.7.1b6/batchalign/tests/pipelines/fixures.py
--rw-r--r--   0 houjun     (501) staff       (20)     4441 2024-03-18 04:54:03.000000 batchalign-0.7.1b6/batchalign/tests/pipelines/test_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)      555 2024-03-18 04:54:03.000000 batchalign-0.7.1b6/batchalign/tests/pipelines/test_pipeline_models.py
--rw-r--r--   0 houjun     (501) staff       (20)     2472 2024-03-18 04:54:03.000000 batchalign-0.7.1b6/batchalign/tests/test_document.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.908643 batchalign-0.7.1b6/batchalign/utils/
--rw-r--r--   0 houjun     (501) staff       (20)       21 2023-12-16 23:44:38.000000 batchalign-0.7.1b6/batchalign/utils/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3513 2023-12-23 18:18:28.000000 batchalign-0.7.1b6/batchalign/utils/config.py
--rw-r--r--   0 houjun     (501) staff       (20)     7689 2024-01-18 23:05:56.000000 batchalign-0.7.1b6/batchalign/utils/dp.py
--rw-r--r--   0 houjun     (501) staff       (20)     2788 2024-04-01 06:52:40.000000 batchalign-0.7.1b6/batchalign/utils/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)       49 2024-05-17 19:30:14.000000 batchalign-0.7.1b6/batchalign/version
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-17 19:31:01.893109 batchalign-0.7.1b6/batchalign.egg-info/
--rw-r--r--   0 houjun     (501) staff       (20)    11951 2024-05-17 19:31:01.000000 batchalign-0.7.1b6/batchalign.egg-info/PKG-INFO
--rw-r--r--   0 houjun     (501) staff       (20)     3776 2024-05-17 19:31:01.000000 batchalign-0.7.1b6/batchalign.egg-info/SOURCES.txt
--rw-r--r--   0 houjun     (501) staff       (20)        1 2024-05-17 19:31:01.000000 batchalign-0.7.1b6/batchalign.egg-info/dependency_links.txt
--rw-r--r--   0 houjun     (501) staff       (20)       61 2024-05-17 19:31:01.000000 batchalign-0.7.1b6/batchalign.egg-info/entry_points.txt
--rw-r--r--   0 houjun     (501) staff       (20)      902 2024-05-17 19:31:01.000000 batchalign-0.7.1b6/batchalign.egg-info/requires.txt
--rw-r--r--   0 houjun     (501) staff       (20)       11 2024-05-17 19:31:01.000000 batchalign-0.7.1b6/batchalign.egg-info/top_level.txt
--rw-r--r--   0 houjun     (501) staff       (20)       38 2024-05-17 19:31:01.911192 batchalign-0.7.1b6/setup.cfg
--rw-r--r--   0 houjun     (501) staff       (20)     2983 2024-04-01 06:52:43.000000 batchalign-0.7.1b6/setup.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.886170 batchalign-0.7.1b7/
+-rw-r--r--   0 houjun     (501) staff       (20)     1464 2024-01-21 18:39:49.000000 batchalign-0.7.1b7/LICENSE
+-rw-r--r--   0 houjun     (501) staff       (20)      149 2024-04-04 00:32:13.000000 batchalign-0.7.1b7/MANIFEST.in
+-rw-r--r--   0 houjun     (501) staff       (20)    11951 2024-05-21 16:28:14.885648 batchalign-0.7.1b7/PKG-INFO
+-rw-r--r--   0 houjun     (501) staff       (20)     9074 2024-05-12 20:56:18.000000 batchalign-0.7.1b7/README.md
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.864568 batchalign-0.7.1b7/batchalign/
+-rw-r--r--   0 houjun     (501) staff       (20)      497 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)       63 2023-12-17 23:06:14.000000 batchalign-0.7.1b7/batchalign/__main__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.865772 batchalign-0.7.1b7/batchalign/cli/
+-rw-r--r--   0 houjun     (501) staff       (20)       28 2023-12-17 01:12:36.000000 batchalign-0.7.1b7/batchalign/cli/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)    10089 2024-05-21 16:25:29.000000 batchalign-0.7.1b7/batchalign/cli/cli.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7568 2024-04-14 17:16:00.000000 batchalign-0.7.1b7/batchalign/cli/dispatch.py
+-rw-r--r--   0 houjun     (501) staff       (20)      777 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/constants.py
+-rw-r--r--   0 houjun     (501) staff       (20)    14798 2024-04-20 21:56:18.000000 batchalign-0.7.1b7/batchalign/document.py
+-rw-r--r--   0 houjun     (501) staff       (20)      199 2023-12-17 07:10:18.000000 batchalign-0.7.1b7/batchalign/errors.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.866367 batchalign-0.7.1b7/batchalign/formats/
+-rw-r--r--   0 houjun     (501) staff       (20)       62 2024-03-18 04:57:14.000000 batchalign-0.7.1b7/batchalign/formats/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      246 2023-12-18 07:14:44.000000 batchalign-0.7.1b7/batchalign/formats/base.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.867651 batchalign-0.7.1b7/batchalign/formats/chat/
+-rw-r--r--   0 houjun     (501) staff       (20)       27 2024-03-18 04:57:14.000000 batchalign-0.7.1b7/batchalign/formats/chat/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4676 2024-04-05 17:07:15.000000 batchalign-0.7.1b7/batchalign/formats/chat/file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3701 2024-04-05 17:08:43.000000 batchalign-0.7.1b7/batchalign/formats/chat/generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7481 2023-12-28 03:10:19.000000 batchalign-0.7.1b7/batchalign/formats/chat/lexer.py
+-rw-r--r--   0 houjun     (501) staff       (20)    12453 2024-05-20 21:27:23.000000 batchalign-0.7.1b7/batchalign/formats/chat/parser.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5217 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/formats/chat/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.868632 batchalign-0.7.1b7/batchalign/formats/textgrid/
+-rw-r--r--   0 houjun     (501) staff       (20)       31 2023-12-18 07:14:59.000000 batchalign-0.7.1b7/batchalign/formats/textgrid/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3340 2024-03-18 04:57:14.000000 batchalign-0.7.1b7/batchalign/formats/textgrid/file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3485 2023-12-18 07:35:03.000000 batchalign-0.7.1b7/batchalign/formats/textgrid/generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3888 2023-12-18 05:59:42.000000 batchalign-0.7.1b7/batchalign/formats/textgrid/parser.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.869551 batchalign-0.7.1b7/batchalign/models/
+-rw-r--r--   0 houjun     (501) staff       (20)      195 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      454 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/models/resolve.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.870539 batchalign-0.7.1b7/batchalign/models/speaker/
+-rw-r--r--   0 houjun     (501) staff       (20)       36 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/speaker/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5583 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/speaker/config.yaml
+-rw-r--r--   0 houjun     (501) staff       (20)     3246 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/speaker/infer.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1808 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/speaker/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.870938 batchalign-0.7.1b7/batchalign/models/training/
+-rw-r--r--   0 houjun     (501) staff       (20)       22 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/models/training/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      576 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/training/run.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3357 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/models/training/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3081 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/models/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.871750 batchalign-0.7.1b7/batchalign/models/utterance/
+-rw-r--r--   0 houjun     (501) staff       (20)       39 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/utterance/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5447 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/utterance/dataset.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/utterance/execute.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3179 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/utterance/infer.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3057 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/utterance/prep.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4359 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/utterance/train.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.872136 batchalign-0.7.1b7/batchalign/models/whisper/
+-rw-r--r--   0 houjun     (501) staff       (20)       76 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/whisper/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7340 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/models/whisper/infer_asr.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5264 2024-04-08 19:13:44.000000 batchalign-0.7.1b7/batchalign/models/whisper/infer_fa.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.873106 batchalign-0.7.1b7/batchalign/pipelines/
+-rw-r--r--   0 houjun     (501) staff       (20)      449 2024-04-14 00:00:03.000000 batchalign-0.7.1b7/batchalign/pipelines/__init__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.873452 batchalign-0.7.1b7/batchalign/pipelines/analysis/
+-rw-r--r--   0 houjun     (501) staff       (20)       35 2024-02-05 03:35:25.000000 batchalign-0.7.1b7/batchalign/pipelines/analysis/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2557 2024-02-05 03:35:25.000000 batchalign-0.7.1b7/batchalign/pipelines/analysis/eval.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.874544 batchalign-0.7.1b7/batchalign/pipelines/asr/
+-rw-r--r--   0 houjun     (501) staff       (20)       99 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/pipelines/asr/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3723 2024-04-14 05:49:03.000000 batchalign-0.7.1b7/batchalign/pipelines/asr/rev.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7227 2024-04-14 04:23:55.000000 batchalign-0.7.1b7/batchalign/pipelines/asr/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2063 2024-04-14 05:49:03.000000 batchalign-0.7.1b7/batchalign/pipelines/asr/whisper.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4403 2024-04-14 05:49:03.000000 batchalign-0.7.1b7/batchalign/pipelines/asr/whisperx.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1994 2024-02-05 03:35:25.000000 batchalign-0.7.1b7/batchalign/pipelines/base.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.875538 batchalign-0.7.1b7/batchalign/pipelines/cleanup/
+-rw-r--r--   0 houjun     (501) staff       (20)       52 2023-12-16 19:37:43.000000 batchalign-0.7.1b7/batchalign/pipelines/cleanup/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)       93 2023-12-17 00:16:09.000000 batchalign-0.7.1b7/batchalign/pipelines/cleanup/cleanup.py
+-rw-r--r--   0 houjun     (501) staff       (20)      579 2024-02-05 03:35:25.000000 batchalign-0.7.1b7/batchalign/pipelines/cleanup/disfluencies.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2161 2023-12-08 20:58:29.000000 batchalign-0.7.1b7/batchalign/pipelines/cleanup/parse_support.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2624 2024-02-05 03:35:25.000000 batchalign-0.7.1b7/batchalign/pipelines/cleanup/retrace.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.876129 batchalign-0.7.1b7/batchalign/pipelines/cleanup/support/
+-rw-r--r--   0 houjun     (501) staff       (20)      141 2023-12-09 06:23:35.000000 batchalign-0.7.1b7/batchalign/pipelines/cleanup/support/filled_pauses.eng
+-rw-r--r--   0 houjun     (501) staff       (20)      213 2023-12-09 06:23:34.000000 batchalign-0.7.1b7/batchalign/pipelines/cleanup/support/replacements.eng
+-rw-r--r--   0 houjun     (501) staff       (20)      203 2024-03-18 04:54:03.000000 batchalign-0.7.1b7/batchalign/pipelines/cleanup/support/test.test
+-rw-r--r--   0 houjun     (501) staff       (20)     4135 2024-05-17 19:29:50.000000 batchalign-0.7.1b7/batchalign/pipelines/dispatch.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.876749 batchalign-0.7.1b7/batchalign/pipelines/fa/
+-rw-r--r--   0 houjun     (501) staff       (20)       40 2023-12-16 01:03:14.000000 batchalign-0.7.1b7/batchalign/pipelines/fa/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7492 2024-04-20 18:30:40.000000 batchalign-0.7.1b7/batchalign/pipelines/fa/whisper_fa.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.877229 batchalign-0.7.1b7/batchalign/pipelines/morphosyntax/
+-rw-r--r--   0 houjun     (501) staff       (20)       29 2023-12-16 23:54:03.000000 batchalign-0.7.1b7/batchalign/pipelines/morphosyntax/__init__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.877369 batchalign-0.7.1b7/batchalign/pipelines/morphosyntax/fr/
+-rw-r--r--   0 houjun     (501) staff       (20)     1147 2023-12-29 00:44:35.000000 batchalign-0.7.1b7/batchalign/pipelines/morphosyntax/fr/case.py
+-rw-r--r--   0 houjun     (501) staff       (20)    29617 2024-05-20 21:54:38.000000 batchalign-0.7.1b7/batchalign/pipelines/morphosyntax/ud.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7482 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/pipelines/pipeline.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.877733 batchalign-0.7.1b7/batchalign/pipelines/speaker/
+-rw-r--r--   0 houjun     (501) staff       (20)       44 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/pipelines/speaker/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2367 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/batchalign/pipelines/speaker/nemo_speaker.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.878523 batchalign-0.7.1b7/batchalign/pipelines/utr/
+-rw-r--r--   0 houjun     (501) staff       (20)       76 2024-01-03 22:34:21.000000 batchalign-0.7.1b7/batchalign/pipelines/utr/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3525 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/pipelines/utr/rev_utr.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2303 2024-04-19 03:00:06.000000 batchalign-0.7.1b7/batchalign/pipelines/utr/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1559 2024-02-05 03:35:25.000000 batchalign-0.7.1b7/batchalign/pipelines/utr/whisper_utr.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.879052 batchalign-0.7.1b7/batchalign/pipelines/utterance/
+-rw-r--r--   0 houjun     (501) staff       (20)       48 2024-04-13 19:17:01.000000 batchalign-0.7.1b7/batchalign/pipelines/utterance/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)    10922 2024-04-16 21:19:29.000000 batchalign-0.7.1b7/batchalign/pipelines/utterance/ud_utterance.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.879633 batchalign-0.7.1b7/batchalign/tests/
+-rw-r--r--   0 houjun     (501) staff       (20)        0 2023-11-18 22:44:12.000000 batchalign-0.7.1b7/batchalign/tests/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1497 2024-03-18 04:54:03.000000 batchalign-0.7.1b7/batchalign/tests/conftest.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.862311 batchalign-0.7.1b7/batchalign/tests/formats/
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.880764 batchalign-0.7.1b7/batchalign/tests/formats/chat/
+-rw-r--r--   0 houjun     (501) staff       (20)      999 2024-03-18 04:57:14.000000 batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3913 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)      714 2023-12-24 23:29:13.000000 batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_lexer.py
+-rw-r--r--   0 houjun     (501) staff       (20)    10624 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_parser.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1046 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.880902 batchalign-0.7.1b7/batchalign/tests/formats/textgrid/
+-rw-r--r--   0 houjun     (501) staff       (20)     2699 2024-03-18 04:54:03.000000 batchalign-0.7.1b7/batchalign/tests/formats/textgrid/test_textgrid.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.881465 batchalign-0.7.1b7/batchalign/tests/pipelines/
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.881595 batchalign-0.7.1b7/batchalign/tests/pipelines/analysis/
+-rw-r--r--   0 houjun     (501) staff       (20)      604 2024-02-05 03:35:25.000000 batchalign-0.7.1b7/batchalign/tests/pipelines/analysis/test_eval.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.881965 batchalign-0.7.1b7/batchalign/tests/pipelines/asr/
+-rw-r--r--   0 houjun     (501) staff       (20)      938 2024-03-18 04:54:03.000000 batchalign-0.7.1b7/batchalign/tests/pipelines/asr/test_asr_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1570 2024-01-02 20:37:42.000000 batchalign-0.7.1b7/batchalign/tests/pipelines/asr/test_asr_utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.882331 batchalign-0.7.1b7/batchalign/tests/pipelines/cleanup/
+-rw-r--r--   0 houjun     (501) staff       (20)     2716 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/tests/pipelines/cleanup/test_disfluency.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-03-18 04:54:03.000000 batchalign-0.7.1b7/batchalign/tests/pipelines/cleanup/test_parse_support.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.882466 batchalign-0.7.1b7/batchalign/tests/pipelines/fa/
+-rw-r--r--   0 houjun     (501) staff       (20)      261 2024-04-08 19:15:55.000000 batchalign-0.7.1b7/batchalign/tests/pipelines/fa/test_fa_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)      977 2024-03-18 04:54:03.000000 batchalign-0.7.1b7/batchalign/tests/pipelines/fixures.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4441 2024-03-18 04:54:03.000000 batchalign-0.7.1b7/batchalign/tests/pipelines/test_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)      555 2024-03-18 04:54:03.000000 batchalign-0.7.1b7/batchalign/tests/pipelines/test_pipeline_models.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2472 2024-03-18 04:54:03.000000 batchalign-0.7.1b7/batchalign/tests/test_document.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.883569 batchalign-0.7.1b7/batchalign/utils/
+-rw-r--r--   0 houjun     (501) staff       (20)       21 2023-12-16 23:44:38.000000 batchalign-0.7.1b7/batchalign/utils/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3513 2023-12-23 18:18:28.000000 batchalign-0.7.1b7/batchalign/utils/config.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7689 2024-01-18 23:05:56.000000 batchalign-0.7.1b7/batchalign/utils/dp.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2788 2024-04-01 06:52:40.000000 batchalign-0.7.1b7/batchalign/utils/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)       65 2024-05-21 16:27:08.000000 batchalign-0.7.1b7/batchalign/version
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-21 16:28:14.865263 batchalign-0.7.1b7/batchalign.egg-info/
+-rw-r--r--   0 houjun     (501) staff       (20)    11951 2024-05-21 16:28:14.000000 batchalign-0.7.1b7/batchalign.egg-info/PKG-INFO
+-rw-r--r--   0 houjun     (501) staff       (20)     3776 2024-05-21 16:28:14.000000 batchalign-0.7.1b7/batchalign.egg-info/SOURCES.txt
+-rw-r--r--   0 houjun     (501) staff       (20)        1 2024-05-21 16:28:14.000000 batchalign-0.7.1b7/batchalign.egg-info/dependency_links.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       61 2024-05-21 16:28:14.000000 batchalign-0.7.1b7/batchalign.egg-info/entry_points.txt
+-rw-r--r--   0 houjun     (501) staff       (20)      902 2024-05-21 16:28:14.000000 batchalign-0.7.1b7/batchalign.egg-info/requires.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       11 2024-05-21 16:28:14.000000 batchalign-0.7.1b7/batchalign.egg-info/top_level.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       38 2024-05-21 16:28:14.886216 batchalign-0.7.1b7/setup.cfg
+-rw-r--r--   0 houjun     (501) staff       (20)     2983 2024-04-01 06:52:43.000000 batchalign-0.7.1b7/setup.py
```

### Comparing `batchalign-0.7.1b6/LICENSE` & `batchalign-0.7.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/PKG-INFO` & `batchalign-0.7.1b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchalign
-Version: 0.7.1b6
+Version: 0.7.1b7
 Summary: Python Speech Language Sample Analysis
 Author: Brian MacWhinney, Houjun Liu
 Author-email: macw@cmu.edu, houjun@cmu.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `batchalign-0.7.1b6/README.md` & `batchalign-0.7.1b7/README.md`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/cli/cli.py` & `batchalign-0.7.1b7/batchalign/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,27 +145,30 @@
               default=False, help="Should we write word level alignment line? Default to no.")
 @click.pass_context
 def transcribe(ctx, in_dir, out_dir, lang, num_speakers, **kwargs):
     """Create a transcript from audio files."""
     def loader(file):
         return file
 
+    asr = "rev"
+    if kwargs["whisper"]:
+        asr = "whisper"
+    if kwargs["whisperx"]:
+        asr = "whisperx"
+
+
     def writer(doc, output):
+        doc.content.insert(0, CustomLine(id="Comment", type=CustomLineType.INDEPENDENT,
+                                         content=f"Batchalign {VERSION_NUMBER.strip()}, ASR Engine {asr}"))
         CHATFile(doc=doc, special_mor_=True).write(output
                                                    .replace(".wav", ".cha")
                                                    .replace(".mp4", ".cha")
                                                    .replace(".mp3", ".cha"),
                                                    write_wor=kwargs.get("wor", False))
 
-    asr = "rev"
-    if kwargs["whisper"]:
-        asr = "whisper"
-    if kwargs["whisperx"]:
-        asr = "whisperx"
-
     if kwargs.get("diarize"):
         _dispatch("transcribe_s",
                   lang, num_speakers, ["mp3", "mp4", "wav"], ctx,
                   in_dir, out_dir,
                   loader, writer, C,
                   asr=asr, **kwargs)
     else:
```

### Comparing `batchalign-0.7.1b6/batchalign/cli/dispatch.py` & `batchalign-0.7.1b7/batchalign/cli/dispatch.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/constants.py` & `batchalign-0.7.1b7/batchalign/constants.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/document.py` & `batchalign-0.7.1b7/batchalign/document.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/formats/chat/file.py` & `batchalign-0.7.1b7/batchalign/formats/chat/file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/formats/chat/generator.py` & `batchalign-0.7.1b7/batchalign/formats/chat/generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/formats/chat/lexer.py` & `batchalign-0.7.1b7/batchalign/formats/chat/lexer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/formats/chat/parser.py` & `batchalign-0.7.1b7/batchalign/formats/chat/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 
             # we throw away participants because there are duplicate
             # info of the same thing in @ID
             if "@Participants" in line or "@Options" in line:
                 continue
             # we split because there are multiple languages possible 
             elif "@Languages" in line.strip():
-                results["langs"] = [i.strip() for i in line.strip("@Languages:").strip().split(",")]
+                results["langs"] = [i.strip() for i in line.strip("@Languages:").strip().replace(" ", ",").strip().split(",") if i.strip() != ""]
                 if len(results["langs"]) > 0 and results["langs"][0] == "eng" and special_mor:
                     use_special_mor = True
             # parse participants; the number of | delinates the metedata field
             elif "@ID" in line.strip():
                 participant = line.strip("@ID:").strip().split("|")
 
                 tier = Tier(lang=participant[0], corpus=participant[1],
```

### Comparing `batchalign-0.7.1b6/batchalign/formats/chat/utils.py` & `batchalign-0.7.1b7/batchalign/formats/chat/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/formats/textgrid/file.py` & `batchalign-0.7.1b7/batchalign/formats/textgrid/file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/formats/textgrid/generator.py` & `batchalign-0.7.1b7/batchalign/formats/textgrid/generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/formats/textgrid/parser.py` & `batchalign-0.7.1b7/batchalign/formats/textgrid/parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/speaker/config.yaml` & `batchalign-0.7.1b7/batchalign/models/speaker/config.yaml`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/speaker/infer.py` & `batchalign-0.7.1b7/batchalign/models/speaker/infer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/speaker/utils.py` & `batchalign-0.7.1b7/batchalign/models/speaker/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/training/run.py` & `batchalign-0.7.1b7/batchalign/models/training/run.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/training/utils.py` & `batchalign-0.7.1b7/batchalign/models/training/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/utils.py` & `batchalign-0.7.1b7/batchalign/models/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/utterance/dataset.py` & `batchalign-0.7.1b7/batchalign/models/utterance/dataset.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/utterance/execute.py` & `batchalign-0.7.1b7/batchalign/models/utterance/execute.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/utterance/infer.py` & `batchalign-0.7.1b7/batchalign/models/utterance/infer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/utterance/prep.py` & `batchalign-0.7.1b7/batchalign/models/utterance/prep.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/utterance/train.py` & `batchalign-0.7.1b7/batchalign/models/utterance/train.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/whisper/infer_asr.py` & `batchalign-0.7.1b7/batchalign/models/whisper/infer_asr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/models/whisper/infer_fa.py` & `batchalign-0.7.1b7/batchalign/models/whisper/infer_fa.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/analysis/eval.py` & `batchalign-0.7.1b7/batchalign/pipelines/analysis/eval.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/asr/rev.py` & `batchalign-0.7.1b7/batchalign/pipelines/asr/rev.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/asr/utils.py` & `batchalign-0.7.1b7/batchalign/pipelines/asr/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/asr/whisper.py` & `batchalign-0.7.1b7/batchalign/pipelines/asr/whisper.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/asr/whisperx.py` & `batchalign-0.7.1b7/batchalign/pipelines/asr/whisperx.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/base.py` & `batchalign-0.7.1b7/batchalign/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/cleanup/disfluencies.py` & `batchalign-0.7.1b7/batchalign/pipelines/cleanup/disfluencies.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/cleanup/parse_support.py` & `batchalign-0.7.1b7/batchalign/pipelines/cleanup/parse_support.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/cleanup/retrace.py` & `batchalign-0.7.1b7/batchalign/pipelines/cleanup/retrace.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/dispatch.py` & `batchalign-0.7.1b7/batchalign/pipelines/dispatch.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/fa/whisper_fa.py` & `batchalign-0.7.1b7/batchalign/pipelines/fa/whisper_fa.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/morphosyntax/fr/case.py` & `batchalign-0.7.1b7/batchalign/pipelines/morphosyntax/fr/case.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/morphosyntax/ud.py` & `batchalign-0.7.1b7/batchalign/pipelines/morphosyntax/ud.py`

 * *Files 2% similar despite different names*

```diff
@@ -804,15 +804,35 @@
                 continue
 
             if retokenize:
                 # rewrite the sentence with our desired tokenizations
                 ut, end = chat_parse_utterance(" ".join([i.text for i in sents[0].tokens])+" "+ending,
                                           mor, gra,
                                           None, None)
+                # JANK add a space after every form being analyzed
+                text_fixed = []
+                text_orig = i.text
+                # we do this to force one replacement of the token
+                # for every input token
+                for i in sents[0].tokens:
+                    try:
+                        before, after = text_orig.split(i.text, 1)
+                        text_fixed.append(before.strip())
+                        text_fixed.append(i.text.strip())
+                        text_orig = after
+                    except ValueError:
+                        # we give up on that token; likely not found
+                        # because there we tokenization issues (i.e.
+                        # existing tokenization)
+                        continue
+                text_fixed.append(text_orig.strip())
+                text_fixed = " ".join(text_fixed).strip()
+                text_fixed = re.sub(r" +", " ", text_fixed)
                 doc.content[indx] = Utterance(content=ut,
+                                              text=text_fixed,
                                               tier=doc.content[indx].tier,
                                               time=doc.content[indx].time,
                                               custom_dependencies=doc.content[indx].custom_dependencies)
                                           
             else:
                 # insert morphology into the parsed forms
                 forms, _ = chat_parse_utterance(line, mor, gra, None, None)
```

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/pipeline.py` & `batchalign-0.7.1b7/batchalign/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/speaker/nemo_speaker.py` & `batchalign-0.7.1b7/batchalign/pipelines/speaker/nemo_speaker.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/utr/rev_utr.py` & `batchalign-0.7.1b7/batchalign/pipelines/utr/rev_utr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/utr/utils.py` & `batchalign-0.7.1b7/batchalign/pipelines/utr/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/utr/whisper_utr.py` & `batchalign-0.7.1b7/batchalign/pipelines/utr/whisper_utr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/pipelines/utterance/ud_utterance.py` & `batchalign-0.7.1b7/batchalign/pipelines/utterance/ud_utterance.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/conftest.py` & `batchalign-0.7.1b7/batchalign/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_file.py` & `batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_generator.py` & `batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_lexer.py` & `batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_lexer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_parser.py` & `batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/formats/chat/test_chat_utils.py` & `batchalign-0.7.1b7/batchalign/tests/formats/chat/test_chat_utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/formats/textgrid/test_textgrid.py` & `batchalign-0.7.1b7/batchalign/tests/formats/textgrid/test_textgrid.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/pipelines/analysis/test_eval.py` & `batchalign-0.7.1b7/batchalign/tests/pipelines/analysis/test_eval.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/pipelines/asr/test_asr_pipeline.py` & `batchalign-0.7.1b7/batchalign/tests/pipelines/asr/test_asr_pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/pipelines/asr/test_asr_utils.py` & `batchalign-0.7.1b7/batchalign/tests/pipelines/asr/test_asr_utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/pipelines/cleanup/test_disfluency.py` & `batchalign-0.7.1b7/batchalign/tests/pipelines/cleanup/test_disfluency.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/pipelines/cleanup/test_parse_support.py` & `batchalign-0.7.1b7/batchalign/tests/pipelines/cleanup/test_parse_support.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/pipelines/fixures.py` & `batchalign-0.7.1b7/batchalign/tests/pipelines/fixures.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/pipelines/test_pipeline.py` & `batchalign-0.7.1b7/batchalign/tests/pipelines/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/pipelines/test_pipeline_models.py` & `batchalign-0.7.1b7/batchalign/tests/pipelines/test_pipeline_models.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/tests/test_document.py` & `batchalign-0.7.1b7/batchalign/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/utils/config.py` & `batchalign-0.7.1b7/batchalign/utils/config.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/utils/dp.py` & `batchalign-0.7.1b7/batchalign/utils/dp.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign/utils/utils.py` & `batchalign-0.7.1b7/batchalign/utils/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign.egg-info/PKG-INFO` & `batchalign-0.7.1b7/batchalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchalign
-Version: 0.7.1b6
+Version: 0.7.1b7
 Summary: Python Speech Language Sample Analysis
 Author: Brian MacWhinney, Houjun Liu
 Author-email: macw@cmu.edu, houjun@cmu.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `batchalign-0.7.1b6/batchalign.egg-info/SOURCES.txt` & `batchalign-0.7.1b7/batchalign.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/batchalign.egg-info/requires.txt` & `batchalign-0.7.1b7/batchalign.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b6/setup.py` & `batchalign-0.7.1b7/setup.py`

 * *Files identical despite different names*

