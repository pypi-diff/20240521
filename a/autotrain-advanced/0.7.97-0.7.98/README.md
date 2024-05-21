# Comparing `tmp/autotrain-advanced-0.7.97.tar.gz` & `tmp/autotrain-advanced-0.7.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.7.97.tar", last modified: Fri May 17 15:15:05 2024, max compression
+gzip compressed data, was "autotrain-advanced-0.7.98.tar", last modified: Tue May 21 08:35:44 2024, max compression
```

## Comparing `autotrain-advanced-0.7.97.tar` & `autotrain-advanced-0.7.98.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.476853 autotrain-advanced-0.7.97/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.97/LICENSE
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-17 15:15:05.476853 autotrain-advanced-0.7.97/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3113 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.97/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-17 15:15:05.476853 autotrain-advanced-0.7.97/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.97/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.444854 autotrain-advanced-0.7.97/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.444854 autotrain-advanced-0.7.97/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1652 2024-05-17 15:14:34.000000 autotrain-advanced-0.7.97/src/autotrain/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.444854 autotrain-advanced-0.7.97/src/autotrain/app/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.97/src/autotrain/app/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.97/src/autotrain/app/api_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.97/src/autotrain/app/app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16255 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.97/src/autotrain/app/colab.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.97/src/autotrain/app/db.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.97/src/autotrain/app/models.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.97/src/autotrain/app/oauth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19137 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.97/src/autotrain/app/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.444854 autotrain-advanced-0.7.97/src/autotrain/app/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.97/src/autotrain/app/static/logo.png
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.448854 autotrain-advanced-0.7.97/src/autotrain/app/templates/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.97/src/autotrain/app/templates/duplicate.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.97/src/autotrain/app/templates/error.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.97/src/autotrain/app/templates/index.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.97/src/autotrain/app/templates/login.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1923 2024-05-17 06:28:50.000000 autotrain-advanced-0.7.97/src/autotrain/app/training_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17665 2024-05-17 15:11:13.000000 autotrain-advanced-0.7.97/src/autotrain/app/ui_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3409 2024-05-17 06:28:48.000000 autotrain-advanced-0.7.97/src/autotrain/app/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.448854 autotrain-advanced-0.7.97/src/autotrain/backends/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.97/src/autotrain/backends/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/backends/base.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.97/src/autotrain/backends/endpoints.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.97/src/autotrain/backends/local.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.97/src/autotrain/backends/ngc.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.97/src/autotrain/backends/nvcf.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.97/src/autotrain/backends/spaces.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.448854 autotrain-advanced-0.7.97/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.97/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4099 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8313 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_object_detection.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10504 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_seq2seq.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_spacerunner.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8591 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8535 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_text_regression.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8512 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_token_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.97/src/autotrain/cli/run_tools.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/cli/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/commands.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.97/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.97/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.97/src/autotrain/logging.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7034 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.97/src/autotrain/parser.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.448854 autotrain-advanced-0.7.97/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.97/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.97/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.97/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.97/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.448854 autotrain-advanced-0.7.97/src/autotrain/tools/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.97/src/autotrain/tools/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.97/src/autotrain/tools/convert_to_kohya.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.97/src/autotrain/tools/merge_adapter.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.452854 autotrain-advanced-0.7.97/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.452854 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_default.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_dpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_orpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_reward.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_sft.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/clm/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8222 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/common.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.452854 autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/train.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/train_xl.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.452854 autotrain-advanced-0.7.97/src/autotrain/trainers/generic/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/generic/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/generic/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/generic/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/generic/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.452854 autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1985 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.452854 autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7185 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2143 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7592 2024-05-14 11:01:54.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.456853 autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8908 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.456853 autotrain-advanced-0.7.97/src/autotrain/trainers/tabular/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/tabular/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/tabular/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/tabular/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/tabular/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.456853 autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7738 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2037 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.456853 autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7019 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2036 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.456853 autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7519 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2038 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.97/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.456853 autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-17 15:15:05.000000 autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4912 2024-05-17 15:15:05.000000 autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-17 15:15:05.000000 autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-17 15:15:05.000000 autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-17 15:15:05.000000 autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-17 15:15:05.000000 autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-17 15:15:05.456853 autotrain-advanced-0.7.97/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.97/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.307764 autotrain-advanced-0.7.98/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.98/LICENSE
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-21 08:35:44.307764 autotrain-advanced-0.7.98/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3113 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-21 08:35:44.307764 autotrain-advanced-0.7.98/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.271765 autotrain-advanced-0.7.98/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1652 2024-05-21 08:35:23.000000 autotrain-advanced-0.7.98/src/autotrain/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/app/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/app/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.98/src/autotrain/app/api_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.98/src/autotrain/app/app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16255 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/app/colab.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/app/db.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.98/src/autotrain/app/models.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/app/oauth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19137 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/app/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/app/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/app/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/app/templates/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/src/autotrain/app/templates/duplicate.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/src/autotrain/app/templates/error.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/src/autotrain/app/templates/index.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/src/autotrain/app/templates/login.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1923 2024-05-17 06:28:50.000000 autotrain-advanced-0.7.98/src/autotrain/app/training_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17665 2024-05-17 15:11:13.000000 autotrain-advanced-0.7.98/src/autotrain/app/ui_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3409 2024-05-17 06:28:48.000000 autotrain-advanced-0.7.98/src/autotrain/app/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/backends/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.98/src/autotrain/backends/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/backends/base.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/backends/endpoints.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.98/src/autotrain/backends/local.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.98/src/autotrain/backends/ngc.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.98/src/autotrain/backends/nvcf.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.98/src/autotrain/backends/spaces.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.98/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4099 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8313 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_object_detection.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10504 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_seq2seq.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_spacerunner.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8591 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8535 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_text_regression.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8512 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_token_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_tools.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/cli/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/commands.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.98/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.98/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.98/src/autotrain/logging.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7034 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/parser.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/tools/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.98/src/autotrain/tools/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.98/src/autotrain/tools/convert_to_kohya.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.98/src/autotrain/tools/merge_adapter.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_default.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_dpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_orpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_reward.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_sft.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20755 2024-05-21 08:33:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8222 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/common.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/train.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/train_xl.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1985 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4608 2024-05-21 08:33:42.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7185 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2143 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7743 2024-05-21 08:33:52.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8908 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1793 2024-05-21 08:34:03.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7738 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2037 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3460 2024-05-21 08:34:15.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7019 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2036 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2268 2024-05-21 08:34:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7519 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2038 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1826 2024-05-21 08:34:34.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.287765 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4912 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.287765 autotrain-advanced-0.7.98/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.98/static/logo.png
```

### Comparing `autotrain-advanced-0.7.97/LICENSE` & `autotrain-advanced-0.7.98/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/PKG-INFO` & `autotrain-advanced-0.7.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.97
+Version: 0.7.98
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.97/README.md` & `autotrain-advanced-0.7.98/README.md`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/setup.py` & `autotrain-advanced-0.7.98/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/__init__.py` & `autotrain-advanced-0.7.98/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 warnings.filterwarnings("ignore", category=UserWarning, module="peft")
 warnings.filterwarnings("ignore", category=UserWarning, module="accelerate")
 warnings.filterwarnings("ignore", category=UserWarning, module="datasets")
 warnings.filterwarnings("ignore", category=FutureWarning, module="accelerate")
 warnings.filterwarnings("ignore", category=UserWarning, module="huggingface_hub")
 
 logger = Logger().get_logger()
-__version__ = "0.7.97"
+__version__ = "0.7.98"
 
 
 def is_colab():
     try:
         import google.colab
 
         return True
```

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/api_routes.py` & `autotrain-advanced-0.7.98/src/autotrain/app/api_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/app.py` & `autotrain-advanced-0.7.98/src/autotrain/app/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/colab.py` & `autotrain-advanced-0.7.98/src/autotrain/app/colab.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/db.py` & `autotrain-advanced-0.7.98/src/autotrain/app/db.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/models.py` & `autotrain-advanced-0.7.98/src/autotrain/app/models.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/oauth.py` & `autotrain-advanced-0.7.98/src/autotrain/app/oauth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/params.py` & `autotrain-advanced-0.7.98/src/autotrain/app/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/static/logo.png` & `autotrain-advanced-0.7.98/src/autotrain/app/static/logo.png`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/templates/duplicate.html` & `autotrain-advanced-0.7.98/src/autotrain/app/templates/duplicate.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/templates/error.html` & `autotrain-advanced-0.7.98/src/autotrain/app/templates/error.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/templates/index.html` & `autotrain-advanced-0.7.98/src/autotrain/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/templates/login.html` & `autotrain-advanced-0.7.98/src/autotrain/app/templates/login.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/training_api.py` & `autotrain-advanced-0.7.98/src/autotrain/app/training_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/ui_routes.py` & `autotrain-advanced-0.7.98/src/autotrain/app/ui_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/app/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/app/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/backends/base.py` & `autotrain-advanced-0.7.98/src/autotrain/backends/base.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/backends/endpoints.py` & `autotrain-advanced-0.7.98/src/autotrain/backends/endpoints.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/backends/ngc.py` & `autotrain-advanced-0.7.98/src/autotrain/backends/ngc.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/backends/nvcf.py` & `autotrain-advanced-0.7.98/src/autotrain/backends/nvcf.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/backends/spaces.py` & `autotrain-advanced-0.7.98/src/autotrain/backends/spaces.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_api.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_image_classification.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_object_detection.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_object_detection.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_seq2seq.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_seq2seq.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_spacerunner.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_spacerunner.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_tabular.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_text_classification.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_text_regression.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_text_regression.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_token_classification.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_token_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/run_tools.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/run_tools.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/cli/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/cli/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/commands.py` & `autotrain-advanced-0.7.98/src/autotrain/commands.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/dataset.py` & `autotrain-advanced-0.7.98/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/help.py` & `autotrain-advanced-0.7.98/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/logging.py` & `autotrain-advanced-0.7.98/src/autotrain/logging.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/parser.py` & `autotrain-advanced-0.7.98/src/autotrain/parser.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.7.98/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.7.98/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.7.98/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.7.98/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/project.py` & `autotrain-advanced-0.7.98/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/tasks.py` & `autotrain-advanced-0.7.98/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/tools/convert_to_kohya.py` & `autotrain-advanced-0.7.98/src/autotrain/tools/convert_to_kohya.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/tools/merge_adapter.py` & `autotrain-advanced-0.7.98/src/autotrain/tools/merge_adapter.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/clm/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/clm/callbacks.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/clm/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_default.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_default.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_dpo.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_dpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_orpo.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_orpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_reward.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_reward.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/clm/train_clm_sft.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_sft.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/clm/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 - text-generation-inference
 - text-generation{peft}
 library_name: transformers
 widget:
   - messages:
       - role: user
         content: What is your favorite condiment?
-license: other
+license: other{dataset_tag}
 ---
 
 # Model Trained Using AutoTrain
 
 This model was trained using AutoTrain. For more information, please visit [AutoTrain](https://hf.co/docs/autotrain).
 
 # Usage
@@ -193,15 +193,25 @@
 
 
 def create_model_card(config):
     if config.peft:
         peft = "\n- peft"
     else:
         peft = ""
-    return MODEL_CARD.format(peft=peft).strip()
+
+    if config.data_path == f"{config.project_name}/autotrain-data":
+        dataset_tag = ""
+    else:
+        dataset_tag = f"\n- dataset: {config.data_path}"
+
+    model_card = MODEL_CARD.format(
+        dataset_tag=dataset_tag,
+        peft=peft,
+    )
+    return model_card.strip()
 
 
 def pause_endpoint(params):
     endpoint_id = os.environ["ENDPOINT_ID"]
     username = endpoint_id.split("/")[0]
     project_name = endpoint_id.split("/")[1]
     api_url = f"https://api.endpoints.huggingface.cloud/v2/endpoint/{username}/{project_name}/pause"
```

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/common.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/common.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/train.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/train.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/train_xl.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/train_xl.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/generic/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/generic/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/generic/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/generic/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/generic/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/generic/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/dataset.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/image_classification/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,17 +35,15 @@
 - image-classification
 widget:
 - src: https://huggingface.co/datasets/mishig/sample_images/resolve/main/tiger.jpg
   example_title: Tiger
 - src: https://huggingface.co/datasets/mishig/sample_images/resolve/main/teapot.jpg
   example_title: Teapot
 - src: https://huggingface.co/datasets/mishig/sample_images/resolve/main/palace.jpg
-  example_title: Palace
-datasets:
-- {dataset}
+  example_title: Palace{dataset_tag}
 ---
 
 # Model Trained Using AutoTrain
 
 - Problem type: Image Classification
 
 ## Validation Metrics
@@ -126,12 +124,17 @@
         )
         eval_scores = [f"{k[len('eval_'):]}: {v}" for k, v in eval_scores.items() if k in valid_metrics]
         eval_scores = "\n\n".join(eval_scores)
 
     else:
         eval_scores = "No validation metrics available"
 
+    if config.data_path == f"{config.project_name}/autotrain-data":
+        dataset_tag = ""
+    else:
+        dataset_tag = f"\n- dataset: {config.data_path}"
+
     model_card = MODEL_CARD.format(
-        dataset=config.data_path,
+        dataset_tag=dataset_tag,
         validation_metrics=eval_scores,
     )
     return model_card
```

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/dataset.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/object_detection/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,15 @@
 - vision
 widget:
 - src: https://huggingface.co/datasets/mishig/sample_images/resolve/main/tiger.jpg
   example_title: Tiger
 - src: https://huggingface.co/datasets/mishig/sample_images/resolve/main/teapot.jpg
   example_title: Teapot
 - src: https://huggingface.co/datasets/mishig/sample_images/resolve/main/palace.jpg
-  example_title: Palace
-datasets:
-- {dataset}
+  example_title: Palace{dataset_tag}
 ---
 
 # Model Trained Using AutoTrain
 
 - Problem type: Object Detection
 
 ## Validation Metrics
@@ -201,12 +199,17 @@
         eval_scores = trainer.evaluate()
         eval_scores = [f"{k[len('eval_'):]}: {v}" for k, v in eval_scores.items() if k in VALID_METRICS]
         eval_scores = "\n\n".join(eval_scores)
 
     else:
         eval_scores = "No validation metrics available"
 
+    if config.data_path == f"{config.project_name}/autotrain-data":
+        dataset_tag = ""
+    else:
+        dataset_tag = f"\n- dataset: {config.data_path}"
+
     model_card = MODEL_CARD.format(
-        dataset=config.data_path,
+        dataset_tag=dataset_tag,
         validation_metrics=eval_scores,
     )
     return model_card
```

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/dataset.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/seq2seq/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 MODEL_CARD = """
 ---
 tags:
 - autotrain
 - text2text-generation
 widget:
-- text: "I love AutoTrain"
-datasets:
-- {dataset}
+- text: "I love AutoTrain"{dataset_tag}
 ---
 
 # Model Trained Using AutoTrain
 
 - Problem type: Seq2Seq
 
 ## Validation Metrics
@@ -49,12 +47,17 @@
         eval_scores = trainer.evaluate()
         eval_scores = [f"{k[len('eval_'):]}: {v}" for k, v in eval_scores.items()]
         eval_scores = "\n\n".join(eval_scores)
 
     else:
         eval_scores = "No validation metrics available"
 
+    if config.data_path == f"{config.project_name}/autotrain-data":
+        dataset_tag = ""
+    else:
+        dataset_tag = f"\n- dataset: {config.data_path}"
+
     model_card = MODEL_CARD.format(
-        dataset=config.data_path,
+        dataset_tag=dataset_tag,
         validation_metrics=eval_scores,
     )
     return model_card
```

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/tabular/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/tabular/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/tabular/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/dataset.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/text_classification/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,15 @@
 
 MODEL_CARD = """
 ---
 tags:
 - autotrain
 - text-classification
 widget:
-- text: "I love AutoTrain"
-datasets:
-- {dataset}
+- text: "I love AutoTrain"{dataset_tag}
 ---
 
 # Model Trained Using AutoTrain
 
 - Problem type: Text Classification
 
 ## Validation Metrics
@@ -87,16 +85,21 @@
         )
         eval_scores = [f"{k[len('eval_'):]}: {v}" for k, v in eval_scores.items() if k in valid_metrics]
         eval_scores = "\n\n".join(eval_scores)
 
     else:
         eval_scores = "No validation metrics available"
 
+    if config.data_path == f"{config.project_name}/autotrain-data":
+        dataset_tag = ""
+    else:
+        dataset_tag = f"\n- dataset: {config.data_path}"
+
     model_card = MODEL_CARD.format(
-        dataset=config.data_path,
+        dataset_tag=dataset_tag,
         validation_metrics=eval_scores,
     )
     return model_card
 
 
 def pause_endpoint(params):
     endpoint_id = os.environ["ENDPOINT_ID"]
```

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/dataset.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/text_regression/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
 MODEL_CARD = """
 ---
 tags:
 - autotrain
 - text-regression
 widget:
-- text: "I love AutoTrain"
-datasets:
-- {dataset}
+- text: "I love AutoTrain"{dataset_tag}
 ---
 
 # Model Trained Using AutoTrain
 
 - Problem type: Text Regression
 
 ## Validation Metrics
@@ -69,12 +67,17 @@
             f"{k[len('eval_'):]}: {v}" for k, v in eval_scores.items() if k in SINGLE_COLUMN_REGRESSION_EVAL_METRICS
         ]
         eval_scores = "\n\n".join(eval_scores)
 
     else:
         eval_scores = "No validation metrics available"
 
+    if config.data_path == f"{config.project_name}/autotrain-data":
+        dataset_tag = ""
+    else:
+        dataset_tag = f"\n- dataset: {config.data_path}"
+
     model_card = MODEL_CARD.format(
-        dataset=config.data_path,
+        dataset_tag=dataset_tag,
         validation_metrics=eval_scores,
     )
     return model_card
```

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/__main__.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/dataset.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/params.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain/trainers/token_classification/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 MODEL_CARD = """
 ---
 tags:
 - autotrain
 - token-classification
 widget:
-- text: "I love AutoTrain"
-datasets:
-- {dataset}
+- text: "I love AutoTrain"{dataset_tag}
 ---
 
 # Model Trained Using AutoTrain
 
 - Problem type: Token Classification
 
 ## Validation Metrics
@@ -49,12 +47,17 @@
         eval_scores = trainer.evaluate()
         valid_metrics = ["eval_loss", "eval_precision", "eval_recall", "eval_f1", "eval_accuracy"]
         eval_scores = [f"{k[len('eval_'):]}: {v}" for k, v in eval_scores.items() if k in valid_metrics]
         eval_scores = "\n\n".join(eval_scores)
     else:
         eval_scores = "No validation metrics available"
 
+    if config.data_path == f"{config.project_name}/autotrain-data":
+        dataset_tag = ""
+    else:
+        dataset_tag = f"\n- dataset: {config.data_path}"
+
     model_card = MODEL_CARD.format(
-        dataset=config.data_path,
+        dataset_tag=dataset_tag,
         validation_metrics=eval_scores,
     )
     return model_card
```

### Comparing `autotrain-advanced-0.7.97/src/autotrain/utils.py` & `autotrain-advanced-0.7.98/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.97
+Version: 0.7.98
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.97/static/logo.png` & `autotrain-advanced-0.7.98/static/logo.png`

 * *Files identical despite different names*

