# Comparing `tmp/zhipuai-2.1.0.tar.gz` & `tmp/zhipuai-2.1.0.20240521.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhipuai-2.1.0.tar", max compression
+gzip compressed data, was "zhipuai-2.1.0.20240521.tar", max compression
```

## Comparing `zhipuai-2.1.0.tar` & `zhipuai-2.1.0.20240521.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     8583 2024-05-17 12:31:23.820003 zhipuai-2.1.0/README.md
--rw-r--r--   0        0        0     3275 2024-05-17 12:31:23.820003 zhipuai-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      359 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/__init__.py
--rw-r--r--   0        0        0       23 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/__version__.py
--rw-r--r--   0        0        0     2822 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/_client.py
--rw-r--r--   0        0        0      412 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/__init__.py
--rw-r--r--   0        0        0     5055 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/batches.py
--rw-r--r--   0        0        0      200 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/chat/__init__.py
--rw-r--r--   0        0        0     3285 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/chat/async_completions.py
--rw-r--r--   0        0        0      464 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/chat/chat.py
--rw-r--r--   0        0        0     4503 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/chat/completions.py
--rw-r--r--   0        0        0     1757 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/embeddings.py
--rw-r--r--   0        0        0     4868 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/files.py
--rw-r--r--   0        0        0      188 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/__init__.py
--rw-r--r--   0        0        0      413 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0       48 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/jobs/__init__.py
--rw-r--r--   0        0        0     5537 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/jobs/jobs.py
--rw-r--r--   0        0        0       77 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/models/__init__.py
--rw-r--r--   0        0        0     1309 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/models/fine_tuned_models.py
--rw-r--r--   0        0        0     1948 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/api_resource/images.py
--rw-r--r--   0        0        0     2134 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/__init__.py
--rw-r--r--   0        0        0      455 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_base_api.py
--rw-r--r--   0        0        0     6405 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_base_compat.py
--rw-r--r--   0        0        0    13647 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_base_models.py
--rw-r--r--   0        0        0     4901 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_base_type.py
--rw-r--r--   0        0        0      583 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_constants.py
--rw-r--r--   0        0        0     2256 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_errors.py
--rw-r--r--   0        0        0     1586 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_files.py
--rw-r--r--   0        0        0    30519 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_http_client.py
--rw-r--r--   0        0        0      774 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_jwt_token.py
--rw-r--r--   0        0        0    14681 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_legacy_response.py
--rw-r--r--   0        0        0     3443 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_request_opt.py
--rw-r--r--   0        0        0    14044 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_response.py
--rw-r--r--   0        0        0     6582 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_sse_client.py
--rw-r--r--   0        0        0     1675 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_utils/__init__.py
--rw-r--r--   0        0        0    13099 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_utils/_transform.py
--rw-r--r--   0        0        0     3858 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_utils/_typing.py
--rw-r--r--   0        0        0    11363 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_utils/_utils.py
--rw-r--r--   0        0        0     2618 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/logs.py
--rw-r--r--   0        0        0     1562 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/pagination.py
--rw-r--r--   0        0        0        0 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/__init__.py
--rw-r--r--   0        0        0     2427 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch.py
--rw-r--r--   0        0        0     1096 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch_create_params.py
--rw-r--r--   0        0        0      488 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch_error.py
--rw-r--r--   0        0        0      536 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch_list_params.py
--rw-r--r--   0        0        0      298 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch_request_counts.py
--rw-r--r--   0        0        0        0 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/__init__.py
--rw-r--r--   0        0        0      568 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/async_chat_completion.py
--rw-r--r--   0        0        0      859 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1272 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      171 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/chat_completions_create_param.py
--rw-r--r--   0        0        0      426 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/embeddings.py
--rw-r--r--   0        0        0      550 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/file_object.py
--rw-r--r--   0        0        0      244 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     1005 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0     1064 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0      339 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0       53 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/models/__init__.py
--rw-r--r--   0        0        0      456 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/models/fine_tuned_models.py
--rw-r--r--   0        0        0      374 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/image.py
--rw-r--r--   0        0        0     9311 1970-01-01 00:00:00.000000 zhipuai-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     8793 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/README.md
+-rw-r--r--   0        0        0     2731 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/pyproject.toml
+-rw-r--r--   0        0        0      359 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/__version__.py
+-rw-r--r--   0        0        0     2822 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/_client.py
+-rw-r--r--   0        0        0      412 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/__init__.py
+-rw-r--r--   0        0        0     5055 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/batches.py
+-rw-r--r--   0        0        0      200 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/chat/__init__.py
+-rw-r--r--   0        0        0     3285 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/chat/async_completions.py
+-rw-r--r--   0        0        0      464 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/chat/chat.py
+-rw-r--r--   0        0        0     4503 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/chat/completions.py
+-rw-r--r--   0        0        0     1757 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/embeddings.py
+-rw-r--r--   0        0        0     4868 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/files.py
+-rw-r--r--   0        0        0      188 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/fine_tuning/__init__.py
+-rw-r--r--   0        0        0      413 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/fine_tuning/fine_tuning.py
+-rw-r--r--   0        0        0       48 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/fine_tuning/jobs/__init__.py
+-rw-r--r--   0        0        0     5537 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/fine_tuning/jobs/jobs.py
+-rw-r--r--   0        0        0       77 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/fine_tuning/models/__init__.py
+-rw-r--r--   0        0        0     1309 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/fine_tuning/models/fine_tuned_models.py
+-rw-r--r--   0        0        0     1948 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/api_resource/images.py
+-rw-r--r--   0        0        0     2134 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/__init__.py
+-rw-r--r--   0        0        0      455 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_base_api.py
+-rw-r--r--   0        0        0     6405 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_base_compat.py
+-rw-r--r--   0        0        0    13647 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_base_models.py
+-rw-r--r--   0        0        0     4901 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_base_type.py
+-rw-r--r--   0        0        0      583 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_constants.py
+-rw-r--r--   0        0        0     2256 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_errors.py
+-rw-r--r--   0        0        0     1586 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_files.py
+-rw-r--r--   0        0        0    30519 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_http_client.py
+-rw-r--r--   0        0        0      774 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_jwt_token.py
+-rw-r--r--   0        0        0    14681 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_legacy_response.py
+-rw-r--r--   0        0        0     3443 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_request_opt.py
+-rw-r--r--   0        0        0    14044 2024-05-21 07:04:31.949920 zhipuai-2.1.0.20240521/zhipuai/core/_response.py
+-rw-r--r--   0        0        0     6582 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/core/_sse_client.py
+-rw-r--r--   0        0        0     1675 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/core/_utils/__init__.py
+-rw-r--r--   0        0        0    13099 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/core/_utils/_transform.py
+-rw-r--r--   0        0        0     3858 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/core/_utils/_typing.py
+-rw-r--r--   0        0        0    11363 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/core/_utils/_utils.py
+-rw-r--r--   0        0        0     2618 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/core/logs.py
+-rw-r--r--   0        0        0     1562 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/core/pagination.py
+-rw-r--r--   0        0        0        0 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/__init__.py
+-rw-r--r--   0        0        0     2427 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/batch.py
+-rw-r--r--   0        0        0     1096 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/batch_create_params.py
+-rw-r--r--   0        0        0      488 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/batch_error.py
+-rw-r--r--   0        0        0      536 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/batch_list_params.py
+-rw-r--r--   0        0        0      298 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/batch_request_counts.py
+-rw-r--r--   0        0        0        0 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/chat/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/chat/async_chat_completion.py
+-rw-r--r--   0        0        0      859 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     1272 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      171 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/chat/chat_completions_create_param.py
+-rw-r--r--   0        0        0      426 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/embeddings.py
+-rw-r--r--   0        0        0      550 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/file_object.py
+-rw-r--r--   0        0        0      244 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0        0        0     1064 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0        0        0      339 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0        0        0       53 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/fine_tuning/models/__init__.py
+-rw-r--r--   0        0        0      456 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/fine_tuning/models/fine_tuned_models.py
+-rw-r--r--   0        0        0      374 2024-05-21 07:04:31.953920 zhipuai-2.1.0.20240521/zhipuai/types/image.py
+-rw-r--r--   0        0        0     9571 1970-01-01 00:00:00.000000 zhipuai-2.1.0.20240521/PKG-INFO
```

### Comparing `zhipuai-2.1.0/README.md` & `zhipuai-2.1.0.20240521/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -225,14 +225,21 @@
 | 503         | `APIServerFlowExceedError`      |
 | N/A         | `APIStatusError`       |
 
 
 
 ### 更新日志
 
+`2024-5-20` 
+- 一些 `python3.12` 的依赖问题， 
+- 增加分页处理代码，重写部分相应类的实例化规则
+- 增加类型转换校验
+- 批处理任务相关api 
+- 文件流响应包装器   
+
 `2024-4-29` 
 - 一些 `python3.7` 的代码适配问题， 
 - 接口失败重试机制，通过 `retry` 参数控制重试次数，默认为3次
 - 接口超时策略调整，通过 `Timeout` 控制接口`connect` 和 `read` 超时时间，默认为`timeout=300.0, connect=8.0`
 - 对话模块增加超拟人大模型参数支持，`model="charglm-3"`, `meta`参数支持
   
 `2024-4-23`
```

### Comparing `zhipuai-2.1.0/pyproject.toml` & `zhipuai-2.1.0.20240521/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "zhipuai"
-version = "2.1.0"
+version = "2.1.0.20240521"
 description = "A SDK library for accessing big model apis from ZhipuAI"
 authors = ["Zhipu AI"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.12,!=3.9.7 "
+python = ">=3.7.1,<4.0,!=3.9.7 "
 httpx = ">=0.23.0"
 pydantic = ">=1.9.0,<3.0"
 cachetools = ">=4.2.2"
 pyjwt = "~=2.8.0"
 
 
 [tool.poetry.group.test.dependencies]
@@ -22,38 +22,20 @@
 pytest-dotenv = "^0.5.2"
 duckdb-engine = "^0.9.2"
 pytest-watcher = "^0.2.6"
 freezegun = "^1.2.2"
 responses = "^0.22.0"
 pytest-asyncio = { version = "^0.23.2", python = "^3.8" }
 lark = "^1.1.5"
-pandas = { version = "^2.0.0", python = "^3.8" }
 pytest-mock = "^3.10.0"
-pytest-socket = "^0.6.0"
-syrupy = { version = "^4.0.2", python = ">=3.8.1,<3.9.7 || >3.9.7,<3.12" }
+pytest-socket = { version = "^0.6.0", python = ">=3.8.1,<3.9.7 || >3.9.7,<4.0" }
+syrupy = { version = "^4.0.2", python = ">=3.8.1,<3.9.7 || >3.9.7,<4.0" }
 requests-mock = "^1.11.0"
 respx = "0.21.1"
 
-[tool.poetry.group.test_langchain.dependencies]
-pytest = "^7.3.0"
-pytest-cov = "^4.0.0"
-pytest-dotenv = "^0.5.2"
-duckdb-engine = "^0.9.2"
-pytest-watcher = "^0.2.6"
-freezegun = "^1.2.2"
-responses = "^0.22.0"
-pytest-asyncio = { version = "^0.23.2", python = "^3.8" }
-lark = "^1.1.5"
-pandas = { version = "^2.0.0", python = "^3.8" }
-pytest-mock = "^3.10.0"
-pytest-socket = "^0.6.0"
-syrupy = { version = "^4.0.2", python = ">=3.8.1,<3.9.7 || >3.9.7,<3.12" }
-requests-mock = "^1.11.0"
-langchain = { version = "0.1.5", python = ">=3.8.1,<3.9.7 || >3.9.7,<3.12" }
-
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
```

### Comparing `zhipuai-2.1.0/zhipuai/_client.py` & `zhipuai-2.1.0.20240521/zhipuai/_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/api_resource/batches.py` & `zhipuai-2.1.0.20240521/zhipuai/api_resource/batches.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/api_resource/chat/async_completions.py` & `zhipuai-2.1.0.20240521/zhipuai/api_resource/chat/async_completions.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/api_resource/chat/completions.py` & `zhipuai-2.1.0.20240521/zhipuai/api_resource/chat/completions.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/api_resource/embeddings.py` & `zhipuai-2.1.0.20240521/zhipuai/api_resource/embeddings.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/api_resource/files.py` & `zhipuai-2.1.0.20240521/zhipuai/api_resource/files.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/jobs/jobs.py` & `zhipuai-2.1.0.20240521/zhipuai/api_resource/fine_tuning/jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/models/fine_tuned_models.py` & `zhipuai-2.1.0.20240521/zhipuai/api_resource/fine_tuning/models/fine_tuned_models.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/api_resource/images.py` & `zhipuai-2.1.0.20240521/zhipuai/api_resource/images.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/__init__.py` & `zhipuai-2.1.0.20240521/zhipuai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_base_compat.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_base_compat.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_base_models.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_base_models.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_base_type.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_base_type.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_constants.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_constants.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_errors.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_errors.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_files.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_files.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_http_client.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_http_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_jwt_token.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_jwt_token.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_legacy_response.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_legacy_response.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_request_opt.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_request_opt.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_response.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_response.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_sse_client.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_sse_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_utils/__init__.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_utils/_transform.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_utils/_typing.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/_utils/_utils.py` & `zhipuai-2.1.0.20240521/zhipuai/core/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/logs.py` & `zhipuai-2.1.0.20240521/zhipuai/core/logs.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/core/pagination.py` & `zhipuai-2.1.0.20240521/zhipuai/core/pagination.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/types/batch.py` & `zhipuai-2.1.0.20240521/zhipuai/types/batch.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/types/batch_create_params.py` & `zhipuai-2.1.0.20240521/zhipuai/types/batch_create_params.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/types/batch_list_params.py` & `zhipuai-2.1.0.20240521/zhipuai/types/batch_list_params.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/types/chat/async_chat_completion.py` & `zhipuai-2.1.0.20240521/zhipuai/types/chat/async_chat_completion.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/types/chat/chat_completion.py` & `zhipuai-2.1.0.20240521/zhipuai/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/types/chat/chat_completion_chunk.py` & `zhipuai-2.1.0.20240521/zhipuai/types/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/types/file_object.py` & `zhipuai-2.1.0.20240521/zhipuai/types/file_object.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/types/fine_tuning/fine_tuning_job.py` & `zhipuai-2.1.0.20240521/zhipuai/types/fine_tuning/fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/zhipuai/types/fine_tuning/fine_tuning_job_event.py` & `zhipuai-2.1.0.20240521/zhipuai/types/fine_tuning/fine_tuning_job_event.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.1.0/PKG-INFO` & `zhipuai-2.1.0.20240521/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: zhipuai
-Version: 2.1.0
+Version: 2.1.0.20240521
 Summary: A SDK library for accessing big model apis from ZhipuAI
 Author: Zhipu AI
-Requires-Python: >=3.7, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.12.*
+Requires-Python: >=3.7, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: cli
 Provides-Extra: extended-testing
 Requires-Dist: cachetools (>=4.2.2)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: pydantic (>=1.9.0,<3.0)
 Requires-Dist: pyjwt (>=2.8.0,<2.9.0)
 Description-Content-Type: text/markdown
@@ -244,14 +245,21 @@
 | 503         | `APIServerFlowExceedError`      |
 | N/A         | `APIStatusError`       |
 
 
 
 ### 更新日志
 
+`2024-5-20` 
+- 一些 `python3.12` 的依赖问题， 
+- 增加分页处理代码，重写部分相应类的实例化规则
+- 增加类型转换校验
+- 批处理任务相关api 
+- 文件流响应包装器   
+
 `2024-4-29` 
 - 一些 `python3.7` 的代码适配问题， 
 - 接口失败重试机制，通过 `retry` 参数控制重试次数，默认为3次
 - 接口超时策略调整，通过 `Timeout` 控制接口`connect` 和 `read` 超时时间，默认为`timeout=300.0, connect=8.0`
 - 对话模块增加超拟人大模型参数支持，`model="charglm-3"`, `meta`参数支持
   
 `2024-4-23`
```

