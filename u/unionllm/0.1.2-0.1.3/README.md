# Comparing `tmp/unionllm-0.1.2.tar.gz` & `tmp/unionllm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unionllm-0.1.2.tar", last modified: Thu May 16 03:41:15 2024, max compression
+gzip compressed data, was "unionllm-0.1.3.tar", last modified: Tue May 21 08:56:12 2024, max compression
```

## Comparing `unionllm-0.1.2.tar` & `unionllm-0.1.3.tar`

### file list

```diff
@@ -1,59 +1,72 @@
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:41:15.304809 unionllm-0.1.2/
--rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 unionllm-0.1.2/LICENSE
--rw-r--r--   0 everfly    (501) staff       (20)      491 2024-05-16 03:41:15.304626 unionllm-0.1.2/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)       81 2024-05-08 02:19:48.000000 unionllm-0.1.2/README.md
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:41:15.300128 unionllm-0.1.2/cookbook/
--rw-r--r--   0 everfly    (501) staff       (20)     1752 2024-05-12 16:23:53.000000 unionllm-0.1.2/cookbook/chat_with_zhipu.ipynb
--rw-r--r--   0 everfly    (501) staff       (20)     8970 2024-05-08 17:11:35.000000 unionllm-0.1.2/cookbook/coze_non_stream.ipynb
--rw-r--r--   0 everfly    (501) staff       (20)    11763 2024-05-12 22:37:43.000000 unionllm-0.1.2/cookbook/coze_non_stream_func.ipynb
--rw-r--r--   0 everfly    (501) staff       (20)    82911 2024-05-12 09:05:55.000000 unionllm-0.1.2/cookbook/test_generation_by_coze_eval_by_chatglm_faithfulness.ipynb
--rw-r--r--   0 everfly    (501) staff       (20)    29653 2024-05-12 09:05:53.000000 unionllm-0.1.2/cookbook/test_zeval.ipynb
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:41:15.300259 unionllm-0.1.2/examples/
--rw-r--r--   0 everfly    (501) staff       (20)       46 2024-05-08 02:19:48.000000 unionllm-0.1.2/examples/example_usage.py
--rw-r--r--   0 everfly    (501) staff       (20)      427 2024-05-16 03:40:26.000000 unionllm-0.1.2/pyproject.toml
--rw-r--r--   0 everfly    (501) staff       (20)      133 2024-05-12 14:58:23.000000 unionllm-0.1.2/pytest.ini
--rw-r--r--   0 everfly    (501) staff       (20)       95 2024-05-16 03:33:55.000000 unionllm-0.1.2/requirements.txt
--rw-r--r--   0 everfly    (501) staff       (20)       38 2024-05-16 03:41:15.304841 unionllm-0.1.2/setup.cfg
--rw-r--r--   0 everfly    (501) staff       (20)      563 2024-05-16 03:41:10.000000 unionllm-0.1.2/setup.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:41:15.301655 unionllm-0.1.2/tests/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.2/tests/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)     1409 2024-05-12 15:47:41.000000 unionllm-0.1.2/tests/test_baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)     1403 2024-05-13 00:05:32.000000 unionllm-0.1.2/tests/test_coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     1423 2024-05-12 23:54:14.000000 unionllm-0.1.2/tests/test_dify.py
--rw-r--r--   0 everfly    (501) staff       (20)     1406 2024-05-12 23:47:08.000000 unionllm-0.1.2/tests/test_fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     1137 2024-05-13 00:21:07.000000 unionllm-0.1.2/tests/test_litellm.py
--rw-r--r--   0 everfly    (501) staff       (20)     1422 2024-05-12 23:15:34.000000 unionllm-0.1.2/tests/test_minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     1407 2024-05-12 15:50:43.000000 unionllm-0.1.2/tests/test_moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     1377 2024-05-12 22:48:43.000000 unionllm-0.1.2/tests/test_qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     1457 2024-05-12 15:56:14.000000 unionllm-0.1.2/tests/test_tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     4838 2024-05-16 03:29:43.000000 unionllm-0.1.2/tests/test_unionchat.py
--rw-r--r--   0 everfly    (501) staff       (20)     1444 2024-05-12 16:01:29.000000 unionllm-0.1.2/tests/test_wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     1021 2024-05-12 16:19:20.000000 unionllm-0.1.2/tests/test_xunfei.py
--rw-r--r--   0 everfly    (501) staff       (20)     1371 2024-05-12 22:47:46.000000 unionllm-0.1.2/tests/test_zhipu.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:41:15.302155 unionllm-0.1.2/unionllm/
--rw-r--r--   0 everfly    (501) staff       (20)       54 2024-05-09 01:57:24.000000 unionllm-0.1.2/unionllm/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)      302 2024-05-12 09:13:50.000000 unionllm-0.1.2/unionllm/exceptions.py
--rw-r--r--   0 everfly    (501) staff       (20)     4049 2024-05-16 03:23:15.000000 unionllm-0.1.2/unionllm/main.py
--rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 unionllm-0.1.2/unionllm/models.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:41:15.304272 unionllm-0.1.2/unionllm/providers/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.2/unionllm/providers/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)     5579 2024-05-12 10:20:45.000000 unionllm-0.1.2/unionllm/providers/baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)     3484 2024-05-16 03:12:50.000000 unionllm-0.1.2/unionllm/providers/base_provider.py
--rw-r--r--   0 everfly    (501) staff       (20)    10431 2024-05-14 02:35:52.000000 unionllm-0.1.2/unionllm/providers/coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     7740 2024-05-12 23:53:57.000000 unionllm-0.1.2/unionllm/providers/dify.py
--rw-r--r--   0 everfly    (501) staff       (20)     7162 2024-05-14 02:35:50.000000 unionllm-0.1.2/unionllm/providers/fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     2119 2024-05-13 16:15:14.000000 unionllm-0.1.2/unionllm/providers/litellm.py
--rw-r--r--   0 everfly    (501) staff       (20)     5247 2024-05-12 22:57:26.000000 unionllm-0.1.2/unionllm/providers/minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2832 2024-05-13 16:15:40.000000 unionllm-0.1.2/unionllm/providers/moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     7055 2024-05-12 10:20:45.000000 unionllm-0.1.2/unionllm/providers/qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     6425 2024-05-12 16:00:03.000000 unionllm-0.1.2/unionllm/providers/tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     6891 2024-05-16 03:05:33.000000 unionllm-0.1.2/unionllm/providers/wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     9372 2024-05-12 10:04:56.000000 unionllm-0.1.2/unionllm/providers/xunfei.py
--rw-r--r--   0 everfly    (501) staff       (20)     2533 2024-05-16 03:04:34.000000 unionllm-0.1.2/unionllm/providers/zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)    14331 2024-05-13 16:45:47.000000 unionllm-0.1.2/unionllm/utils.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:41:15.304415 unionllm-0.1.2/unionllm.egg-info/
--rw-r--r--   0 everfly    (501) staff       (20)      491 2024-05-16 03:41:15.000000 unionllm-0.1.2/unionllm.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)     1257 2024-05-16 03:41:15.000000 unionllm-0.1.2/unionllm.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) staff       (20)        1 2024-05-16 03:41:15.000000 unionllm-0.1.2/unionllm.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) staff       (20)       84 2024-05-16 03:41:15.000000 unionllm-0.1.2/unionllm.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) staff       (20)       15 2024-05-16 03:41:15.000000 unionllm-0.1.2/unionllm.egg-info/top_level.txt
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.278652 unionllm-0.1.3/
+-rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 unionllm-0.1.3/LICENSE
+-rw-r--r--   0 everfly    (501) staff       (20)      491 2024-05-21 08:56:12.278478 unionllm-0.1.3/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)     4978 2024-05-20 03:58:24.000000 unionllm-0.1.3/README.md
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.270245 unionllm-0.1.3/cookbook/
+-rw-r--r--   0 everfly    (501) staff       (20)     1752 2024-05-12 16:23:53.000000 unionllm-0.1.3/cookbook/chat_with_zhipu.ipynb
+-rw-r--r--   0 everfly    (501) staff       (20)     8970 2024-05-08 17:11:35.000000 unionllm-0.1.3/cookbook/coze_non_stream.ipynb
+-rw-r--r--   0 everfly    (501) staff       (20)    11763 2024-05-12 22:37:43.000000 unionllm-0.1.3/cookbook/coze_non_stream_func.ipynb
+-rw-r--r--   0 everfly    (501) staff       (20)    82911 2024-05-12 09:05:55.000000 unionllm-0.1.3/cookbook/test_generation_by_coze_eval_by_chatglm_faithfulness.ipynb
+-rw-r--r--   0 everfly    (501) staff       (20)    29653 2024-05-12 09:05:53.000000 unionllm-0.1.3/cookbook/test_zeval.ipynb
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.273575 unionllm-0.1.3/docs/
+-rw-r--r--   0 everfly    (501) staff       (20)      926 2024-05-20 02:32:47.000000 unionllm-0.1.3/docs/baichuan.md
+-rw-r--r--   0 everfly    (501) staff       (20)      967 2024-05-20 02:19:02.000000 unionllm-0.1.3/docs/baidu.md
+-rw-r--r--   0 everfly    (501) staff       (20)      937 2024-05-20 02:47:22.000000 unionllm-0.1.3/docs/coze.md
+-rw-r--r--   0 everfly    (501) staff       (20)      828 2024-05-20 02:51:27.000000 unionllm-0.1.3/docs/dify.md
+-rw-r--r--   0 everfly    (501) staff       (20)      856 2024-05-20 02:48:50.000000 unionllm-0.1.3/docs/fastgpt.md
+-rw-r--r--   0 everfly    (501) staff       (20)     5951 2024-05-20 03:39:58.000000 unionllm-0.1.3/docs/litellm.md
+-rw-r--r--   0 everfly    (501) staff       (20)      872 2024-05-20 02:32:45.000000 unionllm-0.1.3/docs/minimax.md
+-rw-r--r--   0 everfly    (501) staff       (20)      944 2024-05-20 02:32:45.000000 unionllm-0.1.3/docs/moonshot.md
+-rw-r--r--   0 everfly    (501) staff       (20)      879 2024-05-20 02:32:45.000000 unionllm-0.1.3/docs/qwen.md
+-rw-r--r--   0 everfly    (501) staff       (20)      976 2024-05-20 02:41:46.000000 unionllm-0.1.3/docs/tiangong.md
+-rw-r--r--   0 everfly    (501) staff       (20)      816 2024-05-20 02:29:57.000000 unionllm-0.1.3/docs/xunfei.md
+-rw-r--r--   0 everfly    (501) staff       (20)      884 2024-05-20 02:32:45.000000 unionllm-0.1.3/docs/zhipuai.md
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.273696 unionllm-0.1.3/examples/
+-rw-r--r--   0 everfly    (501) staff       (20)       46 2024-05-08 02:19:48.000000 unionllm-0.1.3/examples/example_usage.py
+-rw-r--r--   0 everfly    (501) staff       (20)      427 2024-05-21 08:55:32.000000 unionllm-0.1.3/pyproject.toml
+-rw-r--r--   0 everfly    (501) staff       (20)      133 2024-05-12 14:58:23.000000 unionllm-0.1.3/pytest.ini
+-rw-r--r--   0 everfly    (501) staff       (20)       95 2024-05-16 03:33:55.000000 unionllm-0.1.3/requirements.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       38 2024-05-21 08:56:12.278693 unionllm-0.1.3/setup.cfg
+-rw-r--r--   0 everfly    (501) staff       (20)      563 2024-05-21 08:56:00.000000 unionllm-0.1.3/setup.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.275416 unionllm-0.1.3/tests/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.3/tests/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1409 2024-05-12 15:47:41.000000 unionllm-0.1.3/tests/test_baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1403 2024-05-13 00:05:32.000000 unionllm-0.1.3/tests/test_coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1423 2024-05-12 23:54:14.000000 unionllm-0.1.3/tests/test_dify.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1406 2024-05-12 23:47:08.000000 unionllm-0.1.3/tests/test_fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1137 2024-05-13 00:21:07.000000 unionllm-0.1.3/tests/test_litellm.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1422 2024-05-12 23:15:34.000000 unionllm-0.1.3/tests/test_minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1407 2024-05-12 15:50:43.000000 unionllm-0.1.3/tests/test_moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1377 2024-05-12 22:48:43.000000 unionllm-0.1.3/tests/test_qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1457 2024-05-12 15:56:14.000000 unionllm-0.1.3/tests/test_tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     4838 2024-05-20 05:46:21.000000 unionllm-0.1.3/tests/test_unionchat.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1444 2024-05-12 16:01:29.000000 unionllm-0.1.3/tests/test_wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1021 2024-05-12 16:19:20.000000 unionllm-0.1.3/tests/test_xunfei.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1371 2024-05-12 22:47:46.000000 unionllm-0.1.3/tests/test_zhipu.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.276084 unionllm-0.1.3/unionllm/
+-rw-r--r--   0 everfly    (501) staff       (20)       54 2024-05-20 14:04:18.000000 unionllm-0.1.3/unionllm/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5354 2024-05-19 08:13:23.000000 unionllm-0.1.3/unionllm/exceptions.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5104 2024-05-20 13:56:42.000000 unionllm-0.1.3/unionllm/main.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 unionllm-0.1.3/unionllm/models.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.278083 unionllm-0.1.3/unionllm/providers/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.3/unionllm/providers/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5579 2024-05-12 10:20:45.000000 unionllm-0.1.3/unionllm/providers/baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)     3484 2024-05-16 03:12:50.000000 unionllm-0.1.3/unionllm/providers/base_provider.py
+-rw-r--r--   0 everfly    (501) staff       (20)    10431 2024-05-14 02:35:52.000000 unionllm-0.1.3/unionllm/providers/coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7740 2024-05-12 23:53:57.000000 unionllm-0.1.3/unionllm/providers/dify.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7162 2024-05-14 02:35:50.000000 unionllm-0.1.3/unionllm/providers/fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2119 2024-05-13 16:15:14.000000 unionllm-0.1.3/unionllm/providers/litellm.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5247 2024-05-12 22:57:26.000000 unionllm-0.1.3/unionllm/providers/minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2832 2024-05-13 16:15:40.000000 unionllm-0.1.3/unionllm/providers/moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7055 2024-05-12 10:20:45.000000 unionllm-0.1.3/unionllm/providers/qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6425 2024-05-12 16:00:03.000000 unionllm-0.1.3/unionllm/providers/tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6891 2024-05-16 03:05:33.000000 unionllm-0.1.3/unionllm/providers/wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     9372 2024-05-12 10:04:56.000000 unionllm-0.1.3/unionllm/providers/xunfei.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2533 2024-05-16 03:04:34.000000 unionllm-0.1.3/unionllm/providers/zhipu.py
+-rw-r--r--   0 everfly    (501) staff       (20)    14331 2024-05-13 16:45:47.000000 unionllm-0.1.3/unionllm/utils.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.278254 unionllm-0.1.3/unionllm.egg-info/
+-rw-r--r--   0 everfly    (501) staff       (20)      491 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)     1440 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) staff       (20)        1 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       84 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       15 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/top_level.txt
```

### Comparing `unionllm-0.1.2/cookbook/chat_with_zhipu.ipynb` & `unionllm-0.1.3/cookbook/chat_with_zhipu.ipynb`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/cookbook/coze_non_stream.ipynb` & `unionllm-0.1.3/cookbook/coze_non_stream.ipynb`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/cookbook/coze_non_stream_func.ipynb` & `unionllm-0.1.3/cookbook/coze_non_stream_func.ipynb`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/cookbook/test_generation_by_coze_eval_by_chatglm_faithfulness.ipynb` & `unionllm-0.1.3/cookbook/test_generation_by_coze_eval_by_chatglm_faithfulness.ipynb`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/cookbook/test_zeval.ipynb` & `unionllm-0.1.3/cookbook/test_zeval.ipynb`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/setup.py` & `unionllm-0.1.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='unionllm',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     license='MIT',
     description='A Python library for unified access to Chinese domestic large language models.',
     author='everfly',
     author_email='tagriver@gmail.com',
     url='https://github.com/EvalsOne/UnionLLM',
     install_requires=[
```

### Comparing `unionllm-0.1.2/tests/test_baichuan.py` & `unionllm-0.1.3/tests/test_baichuan.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_coze.py` & `unionllm-0.1.3/tests/test_coze.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_dify.py` & `unionllm-0.1.3/tests/test_dify.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_fastgpt.py` & `unionllm-0.1.3/tests/test_fastgpt.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_litellm.py` & `unionllm-0.1.3/tests/test_litellm.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_minimax.py` & `unionllm-0.1.3/tests/test_minimax.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_moonshot.py` & `unionllm-0.1.3/tests/test_moonshot.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_qwen.py` & `unionllm-0.1.3/tests/test_qwen.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_tiangong.py` & `unionllm-0.1.3/tests/test_tiangong.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_unionchat.py` & `unionllm-0.1.3/tests/test_unionchat.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_wenxin.py` & `unionllm-0.1.3/tests/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_xunfei.py` & `unionllm-0.1.3/tests/test_xunfei.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/tests/test_zhipu.py` & `unionllm-0.1.3/tests/test_zhipu.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/main.py` & `unionllm-0.1.3/unionllm/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import logging
+import asyncio
+from functools import partial
+
 from typing import Any, List
 from .providers import zhipu, moonshot, minimax, qwen, tiangong, baichuan, wenxin, xunfei, dify, fastgpt, coze, litellm
 from .exceptions import ProviderError
 from litellm import completion as litellm_completion
 
 logger = logging.getLogger(__name__)
 
@@ -41,14 +44,16 @@
                 elif support_type == 2:
                     self.litellm_call_type = 2
             else:
                 raise ProviderError(f"Provider '{self.provider}' is not supported.")
         else:
             self.provider_instance = litellm.LiteLLMProvider(**kwargs)
 
+
+
     def completion(self, model: str, messages: List[str], **kwargs) -> Any:
         if not self.provider_instance:
             raise ProviderError(f"Provider '{self.provider}' is not initialized.")
         
         if self.litellm_call_type:
             if self.litellm_call_type == 1:
                 # Jugde whether the model starts with self.provider, if not, add it
@@ -56,20 +61,38 @@
                     model = f"{self.provider}/{model}"
                 return self.provider_instance.completion(model, messages, **kwargs)
             elif self.litellm_call_type == 2:
                 return self.provider_instance.completion(model, messages, **kwargs)
         else:
             return self.provider_instance.completion(model, messages, **kwargs)
         
+    async def acompletion(self, model: str, messages: List[str], **kwargs) -> Any:
+        loop = asyncio.get_event_loop()
+        if not self.provider_instance:
+            raise ProviderError(f"Provider '{self.provider}' is not initialized.")
+        
+        if self.litellm_call_type:
+            if self.litellm_call_type == 1:
+                if not model.startswith(self.provider + "/"):
+                    model = f"{self.provider}/{model}"
+                func = partial(self.provider_instance.completion, model, messages, **kwargs)
+                return await loop.run_in_executor(None, func)
+            elif self.litellm_call_type == 2:
+                func = partial(self.provider_instance.completion, model, messages, **kwargs)
+                return await loop.run_in_executor(None, func)
+        else:
+            func = partial(self.provider_instance.completion, model, messages, **kwargs)
+            return await loop.run_in_executor(None, func)
+
     def check_litellm_providers(self, provider: str) -> bool:
         # Judge whether the provider is supported by LiteLLM, and if provider name should be added to the model name
         if provider in ['azure', 'sagemaker', 'bedrock', 'vertex_ai', 'palm', 'gemini', 'mistral', 'cloudflare', 'huggingface', 'replicate', 'together_ai', 'openrouter', 'baseten', 'nlp_cloud', 'petals', 'ollama', 'perplexity', 'groq', 'anyscale', 'watsonx', 'voyage', 'xinference']:
             # provider name should be added to the model name
             return True, 1
-        elif provider in ['openai', 'claude', 'cohere', 'ai21', 'luminous']:
+        elif provider in ['openai', 'anthropic', 'cohere', 'ai21', 'deepseek', 'deepinfra', 'ai21', 'alpha_alpha']:
             # provider name should not be added to the model name
             return True, 2
         else:
             return False, 0
         
 # This is the new function to simplify calling
 def unionchat(model: str, messages: List[dict], **kwargs) -> Any:
```

### Comparing `unionllm-0.1.2/unionllm/models.py` & `unionllm-0.1.3/unionllm/models.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/baichuan.py` & `unionllm-0.1.3/unionllm/providers/baichuan.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/base_provider.py` & `unionllm-0.1.3/unionllm/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/coze.py` & `unionllm-0.1.3/unionllm/providers/coze.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/dify.py` & `unionllm-0.1.3/unionllm/providers/dify.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/fastgpt.py` & `unionllm-0.1.3/unionllm/providers/fastgpt.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/litellm.py` & `unionllm-0.1.3/unionllm/providers/litellm.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/minimax.py` & `unionllm-0.1.3/unionllm/providers/minimax.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/moonshot.py` & `unionllm-0.1.3/unionllm/providers/moonshot.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/qwen.py` & `unionllm-0.1.3/unionllm/providers/qwen.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/tiangong.py` & `unionllm-0.1.3/unionllm/providers/tiangong.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/wenxin.py` & `unionllm-0.1.3/unionllm/providers/wenxin.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/xunfei.py` & `unionllm-0.1.3/unionllm/providers/xunfei.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/providers/zhipu.py` & `unionllm-0.1.3/unionllm/providers/zhipu.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm/utils.py` & `unionllm-0.1.3/unionllm/utils.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.2/unionllm.egg-info/SOURCES.txt` & `unionllm-0.1.3/unionllm.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 requirements.txt
 setup.py
 cookbook/chat_with_zhipu.ipynb
 cookbook/coze_non_stream.ipynb
 cookbook/coze_non_stream_func.ipynb
 cookbook/test_generation_by_coze_eval_by_chatglm_faithfulness.ipynb
 cookbook/test_zeval.ipynb
+docs/baichuan.md
+docs/baidu.md
+docs/coze.md
+docs/dify.md
+docs/fastgpt.md
+docs/litellm.md
+docs/minimax.md
+docs/moonshot.md
+docs/qwen.md
+docs/tiangong.md
+docs/xunfei.md
+docs/zhipuai.md
 examples/example_usage.py
 tests/__init__.py
 tests/test_baichuan.py
 tests/test_coze.py
 tests/test_dify.py
 tests/test_fastgpt.py
 tests/test_litellm.py
```

