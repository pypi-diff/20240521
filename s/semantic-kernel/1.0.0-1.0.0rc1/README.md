# Comparing `tmp/semantic_kernel-1.0.0.tar.gz` & `tmp/semantic_kernel-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-1.0.0.tar", max compression
+gzip compressed data, was "semantic_kernel-1.0.0rc1.tar", max compression
```

## Comparing `semantic_kernel-1.0.0.tar` & `semantic_kernel-1.0.0rc1.tar`

### file list

```diff
@@ -1,237 +1,233 @@
--rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0/pip/README.md
--rw-r--r--   0        0        0     5542 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     3250 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0      533 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0     7538 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/function_call_behavior.py
--rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
--rw-r--r--   0        0        0    10535 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0        0        0     4676 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0        0        0     3214 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
--rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
--rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
--rw-r--r--   0        0        0     6683 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2215 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
--rw-r--r--   0        0        0     8451 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0        0        0     3983 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0        0        0     1901 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/utils.py
--rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/const.py
--rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
--rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
--rw-r--r--   0        0        0     4147 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
--rw-r--r--   0        0        0    11081 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     5356 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0        0        0     6087 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     6171 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     3614 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0    24013 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
--rw-r--r--   0        0        0     3737 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0        0        0     3823 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     6363 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0        0        0     3759 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     2003 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0        0        0     2871 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/utils.py
--rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
--rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
--rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/prompt_execution_settings.py
--rw-r--r--   0        0        0     1741 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/__init__.py
--rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/astradb/__init__.py
--rw-r--r--   0        0        0     6814 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/astradb/astra_client.py
--rw-r--r--   0        0        0    13443 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
--rw-r--r--   0        0        0      831 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/astradb/astradb_settings.py
--rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/astradb/utils.py
--rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0     1256 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
--rw-r--r--   0        0        0    17059 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0        0        0    11214 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0        0        0     2326 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0        0        0      634 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
--rw-r--r--   0        0        0     1740 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0        0        0    13116 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
--rw-r--r--   0        0        0      236 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/__init__.py
--rw-r--r--   0        0        0     7733 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14373 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      657 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/memory_settings_base.py
--rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16786 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    13227 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0        0        0      614 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
--rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
--rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    15714 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0      556 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
--rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    21241 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      590 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/postgres/postgres_settings.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11799 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0        0        0    15976 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0        0        0      582 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/redis/redis_settings.py
--rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/redis/utils.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0        0        0    23353 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
--rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0        0        0    12592 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0     1004 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
--rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/connectors/openai_plugin/__init__.py
--rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
--rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
--rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/connectors/openai_plugin/openai_utils.py
--rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/connectors/openapi_plugin/__init__.py
--rw-r--r--   0        0        0     1364 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
--rw-r--r--   0        0        0    29334 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
--rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     3425 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/connectors/search_engine/bing_connector_settings.py
--rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-1.0.0/semantic_kernel/connectors/telemetry.py
--rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0/semantic_kernel/connectors/utils/__init__.py
--rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0/semantic_kernel/connectors/utils/document_loader.py
--rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/const.py
--rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/contents/__init__.py
--rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/contents/author_role.py
--rw-r--r--   0        0        0    14167 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/contents/chat_history.py
--rw-r--r--   0        0        0    12590 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0/semantic_kernel/contents/chat_message_content.py
--rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/contents/const.py
--rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/contents/finish_reason.py
--rw-r--r--   0        0        0     4032 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/contents/function_call_content.py
--rw-r--r--   0        0        0     4556 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0/semantic_kernel/contents/function_result_content.py
--rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/contents/kernel_content.py
--rw-r--r--   0        0        0    10964 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/contents/streaming_chat_message_content.py
--rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/contents/streaming_content_mixin.py
--rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/contents/streaming_text_content.py
--rw-r--r--   0        0        0     2011 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/contents/text_content.py
--rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/contents/types.py
--rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0/semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0/semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0/semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/core_plugins/sessions_python_tool/README.md
--rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
--rw-r--r--   0        0        0     9954 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
--rw-r--r--   0        0        0     1919 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
--rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
--rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0/semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0/semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0/semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0/semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0/semantic_kernel/core_plugins/web_search_engine_plugin.py
--rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/exceptions/__init__.py
--rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/exceptions/content_exceptions.py
--rw-r--r--   0        0        0     1270 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0/semantic_kernel/exceptions/function_exceptions.py
--rw-r--r--   0        0        0     1417 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0/semantic_kernel/exceptions/kernel_exceptions.py
--rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/exceptions/memory_connector_exceptions.py
--rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0/semantic_kernel/exceptions/planner_exceptions.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/exceptions/service_exceptions.py
--rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0/semantic_kernel/exceptions/template_engine_exceptions.py
--rw-r--r--   0        0        0      655 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py
--rw-r--r--   0        0        0      631 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/filters/filter_context_base.py
--rw-r--r--   0        0        0      386 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/filters/filter_types.py
--rw-r--r--   0        0        0      396 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/filters/functions/function_invocation_context.py
--rw-r--r--   0        0        0      437 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/filters/prompts/prompt_render_context.py
--rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/functions/__init__.py
--rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0/semantic_kernel/functions/function_result.py
--rw-r--r--   0        0        0     1750 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/functions/kernel_arguments.py
--rw-r--r--   0        0        0    10657 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function.py
--rw-r--r--   0        0        0     6170 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function_decorator.py
--rw-r--r--   0        0        0     8171 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function_from_method.py
--rw-r--r--   0        0        0    16893 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function_from_prompt.py
--rw-r--r--   0        0        0     1991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function_metadata.py
--rw-r--r--   0        0        0     2198 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/functions/kernel_parameter_metadata.py
--rw-r--r--   0        0        0    24196 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/functions/kernel_plugin.py
--rw-r--r--   0        0        0      974 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/functions/prompt_rendering_result.py
--rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0/semantic_kernel/functions/types.py
--rw-r--r--   0        0        0    37173 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     6346 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/kernel_extensions/kernel_filters_extension.py
--rw-r--r--   0        0        0      509 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/kernel_pydantic.py
--rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2640 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     4364 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7242 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1688 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6617 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3715 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12161 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0/semantic_kernel/planners/__init__.py
--rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
--rw-r--r--   0        0        0    12756 2024-05-21 00:02:54.747516 semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
--rw-r--r--   0        0        0     1675 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
--rw-r--r--   0        0        0      928 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
--rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
--rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
--rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0/semantic_kernel/planners/plan.py
--rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/planners/planner_extensions.py
--rw-r--r--   0        0        0      592 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0/semantic_kernel/planners/planner_options.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5978 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     4720 2024-05-09 23:07:37.275180 semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0/semantic_kernel/prompt_template/__init__.py
--rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0/semantic_kernel/prompt_template/const.py
--rw-r--r--   0        0        0     4760 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/prompt_template/handlebars_prompt_template.py
--rw-r--r--   0        0        0      893 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/prompt_template/input_variable.py
--rw-r--r--   0        0        0     4945 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/prompt_template/jinja2_prompt_template.py
--rw-r--r--   0        0        0     6744 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/prompt_template/kernel_prompt_template.py
--rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/prompt_template/prompt_template_base.py
--rw-r--r--   0        0        0     5586 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/prompt_template/prompt_template_config.py
--rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0/semantic_kernel/prompt_template/utils/__init__.py
--rw-r--r--   0        0        0     4592 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
--rw-r--r--   0        0        0     2483 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
--rw-r--r--   0        0        0     2069 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0/semantic_kernel/prompt_template/utils/template_function_helpers.py
--rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0/semantic_kernel/py.typed
--rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     1594 2024-05-21 00:02:54.757516 semantic_kernel-1.0.0/semantic_kernel/schema/kernel_json_schema.py
--rw-r--r--   0        0        0     2870 2024-05-21 00:02:54.757516 semantic_kernel-1.0.0/semantic_kernel/schema/kernel_json_schema_builder.py
--rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0/semantic_kernel/services/__init__.py
--rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/services/ai_service_client_base.py
--rw-r--r--   0        0        0     2648 2024-05-09 23:07:37.275180 semantic_kernel-1.0.0/semantic_kernel/services/ai_service_selector.py
--rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     7474 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/named_arg_block.py
--rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/utils/chat.py
--rw-r--r--   0        0        0      838 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0/semantic_kernel/utils/experimental_decorator.py
--rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/utils/logging.py
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/utils/naming.py
--rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5184 1970-01-01 00:00:00.000000 semantic_kernel-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0rc1/pip/README.md
+-rw-r--r--   0        0        0     5411 2024-05-17 22:45:44.178248 semantic_kernel-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     3250 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0      437 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0     7538 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/function_call_behavior.py
+-rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
+-rw-r--r--   0        0        0    10535 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0        0        0     4676 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0        0        0     3118 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+-rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
+-rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
+-rw-r--r--   0        0        0     6683 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2119 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
+-rw-r--r--   0        0        0     8451 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0        0        0     3983 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0        0        0     1805 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/utils.py
+-rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/const.py
+-rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+-rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
+-rw-r--r--   0        0        0     4147 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
+-rw-r--r--   0        0        0    11081 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     5356 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0        0        0     6087 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     6075 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     3614 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0    23919 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
+-rw-r--r--   0        0        0     3737 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0        0        0     3823 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     6363 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0        0        0     3663 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0        0        0     2908 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/utils.py
+-rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
+-rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
+-rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/prompt_execution_settings.py
+-rw-r--r--   0        0        0     1741 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/__init__.py
+-rw-r--r--   0        0        0     6718 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astra_client.py
+-rw-r--r--   0        0        0    13347 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
+-rw-r--r--   0        0        0      735 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_settings.py
+-rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/utils.py
+-rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0     1160 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
+-rw-r--r--   0        0        0    16963 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0        0        0    11118 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0        0        0      538 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
+-rw-r--r--   0        0        0     1592 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0        0        0    13020 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      560 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/memory_settings_base.py
+-rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    13131 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0        0        0      518 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
+-rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+-rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    15618 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0      460 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
+-rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    21145 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      494 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/postgres_settings.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0        0        0    15880 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0        0        0      486 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/redis_settings.py
+-rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/utils.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+-rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0        0        0    12496 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      908 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
+-rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
+-rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
+-rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_utils.py
+-rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/__init__.py
+-rw-r--r--   0        0        0     1268 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
+-rw-r--r--   0        0        0    28989 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
+-rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     3425 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector_settings.py
+-rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/telemetry.py
+-rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/utils/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/utils/document_loader.py
+-rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/const.py
+-rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/author_role.py
+-rw-r--r--   0        0        0    14167 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_history.py
+-rw-r--r--   0        0        0    12590 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_message_content.py
+-rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/const.py
+-rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/contents/finish_reason.py
+-rw-r--r--   0        0        0     4032 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_call_content.py
+-rw-r--r--   0        0        0     4556 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_result_content.py
+-rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/kernel_content.py
+-rw-r--r--   0        0        0    10964 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_chat_message_content.py
+-rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_content_mixin.py
+-rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_text_content.py
+-rw-r--r--   0        0        0     2011 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/text_content.py
+-rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/types.py
+-rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/README.md
+-rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
+-rw-r--r--   0        0        0     9954 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
+-rw-r--r--   0        0        0     1919 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
+-rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
+-rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/web_search_engine_plugin.py
+-rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/__init__.py
+-rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/content_exceptions.py
+-rw-r--r--   0        0        0     1270 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/function_exceptions.py
+-rw-r--r--   0        0        0     1417 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/kernel_exceptions.py
+-rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/memory_connector_exceptions.py
+-rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/planner_exceptions.py
+-rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/service_exceptions.py
+-rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/template_engine_exceptions.py
+-rw-r--r--   0        0        0      655 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py
+-rw-r--r--   0        0        0      631 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/filter_context_base.py
+-rw-r--r--   0        0        0      386 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/filter_types.py
+-rw-r--r--   0        0        0      396 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/functions/function_invocation_context.py
+-rw-r--r--   0        0        0      437 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/prompts/prompt_render_context.py
+-rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/functions/__init__.py
+-rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/functions/function_result.py
+-rw-r--r--   0        0        0     1750 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_arguments.py
+-rw-r--r--   0        0        0    10657 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function.py
+-rw-r--r--   0        0        0     6170 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_decorator.py
+-rw-r--r--   0        0        0     7843 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_method.py
+-rw-r--r--   0        0        0    16893 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_prompt.py
+-rw-r--r--   0        0        0     1991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_metadata.py
+-rw-r--r--   0        0        0      559 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_parameter_metadata.py
+-rw-r--r--   0        0        0    24196 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_plugin.py
+-rw-r--r--   0        0        0      974 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/prompt_rendering_result.py
+-rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/functions/types.py
+-rw-r--r--   0        0        0    37221 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     6346 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/kernel_extensions/kernel_filters_extension.py
+-rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/kernel_pydantic.py
+-rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6521 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3619 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/__init__.py
+-rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    12815 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
+-rw-r--r--   0        0        0     1675 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
+-rw-r--r--   0        0        0      928 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
+-rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
+-rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
+-rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/planners/plan.py
+-rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_extensions.py
+-rw-r--r--   0        0        0      592 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_options.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5978 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     4720 2024-05-09 23:07:37.275180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/const.py
+-rw-r--r--   0        0        0     4760 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/handlebars_prompt_template.py
+-rw-r--r--   0        0        0      893 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/input_variable.py
+-rw-r--r--   0        0        0     4945 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/jinja2_prompt_template.py
+-rw-r--r--   0        0        0     6744 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/kernel_prompt_template.py
+-rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_base.py
+-rw-r--r--   0        0        0     5586 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_config.py
+-rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/__init__.py
+-rw-r--r--   0        0        0     4592 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
+-rw-r--r--   0        0        0     2483 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
+-rw-r--r--   0        0        0     2069 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/template_function_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/py.typed
+-rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/services/__init__.py
+-rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_client_base.py
+-rw-r--r--   0        0        0     2648 2024-05-09 23:07:37.275180 semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_selector.py
+-rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     7474 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/named_arg_block.py
+-rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/chat.py
+-rw-r--r--   0        0        0      838 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/utils/experimental_decorator.py
+-rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/logging.py
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/naming.py
+-rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5105 1970-01-01 00:00:00.000000 semantic_kernel-1.0.0rc1/PKG-INFO
```

### Comparing `semantic_kernel-1.0.0/pip/README.md` & `semantic_kernel-1.0.0rc1/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/pyproject.toml` & `semantic_kernel-1.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "1.0.0"
+version = "1.0.0rc1"
 description = "Semantic Kernel Python SDK"
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
@@ -59,15 +59,14 @@
 weaviate-client = { version = ">=3.18,<5.0", optional = true}
 pinecone-client = { version = ">=3.0.0", optional = true}
 psycopg = { version="^3.1.9", extras=["binary","pool"], optional = true}
 redis = { version = "^4.6.0", optional = true}
 azure-search-documents = {version = "11.6.0b1", allow-prereleases = true, optional = true}
 azure-core = { version = "^1.28.0", optional = true}
 azure-identity = { version = "^1.13.0", optional = true}
-azure-cosmos = { version = "^4.7.0", optional = true}
 usearch = { version = "^2.9", optional = true}
 pyarrow = { version = ">=12.0.1,<16.0.0", optional = true}
 
 # Groups are for development only (installed through Poetry)
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.5"
 black = "^24.2.0"
@@ -83,15 +82,14 @@
 [tool.poetry.group.unit-tests]
 optional = true
 
 [tool.poetry.group.unit-tests.dependencies]
 google-generativeai = { version = ">=0.1,<0.4", markers = "python_version >= '3.9'"}
 azure-search-documents = {version = "11.6.0b1", allow-prereleases = true}
 azure-core = "^1.28.0"
-azure-cosmos = "^4.7.0"
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "^2.2.0"
 
 [tool.poetry.group.tests]
 optional = true
 
@@ -114,15 +112,14 @@
 weaviate-client = ">=3.18,<5.0"
 pinecone-client = ">=3.0.0"
 psycopg = { version="^3.1.9", extras=["binary","pool"]}
 redis = "^4.6.0"
 azure-search-documents = {version = "11.6.0b1", allow-prereleases = true}
 azure-core = "^1.28.0"
 azure-identity = "^1.13.0"
-azure-cosmos = "^4.7.0"
 usearch = "^2.9"
 pyarrow = ">=12.0.1,<16.0.0"
 msgraph-sdk = "^1.2.0"
 
 # Extras are exposed to pip, this allows a user to easily add the right dependencies to their environment
 [tool.poetry.extras]
 google = ["google-generativeai", "grpcio-status"]
@@ -130,18 +127,18 @@
 qdrant = ["qdrant-client"]
 chromadb = ["chromadb"]
 milvus = ["pymilvus", "milvus"]
 weaviate = ["weaviate-client"]
 pinecone = ["pinecone-client"]
 postgres = ["psycopg"]
 redis = ["redis"]
-azure = ["azure-search-documents", "azure-core", "azure-identity", "azure-cosmos", "msgraph-sdk"]
+azure = ["azure-search-documents", "azure-core", "azure-identity", "msgraph-sdk"]
 usearch = ["usearch", "pyarrow"]
 notebooks = ["ipykernel"]
-all = ["google-generativeai", "grpcio-status", "transformers", "sentence-transformers", "torch", "qdrant-client", "chromadb", "pymilvus", "milvus", "weaviate-client", "pinecone-client", "psycopg", "redis", "azure-search-documents", "azure-core", "azure-identity", "azure-cosmos", "usearch", "pyarrow", "ipykernel"]
+all = ["google-generativeai", "grpcio-status", "transformers", "sentence-transformers", "torch", "qdrant-client", "chromadb", "pymilvus", "milvus", "weaviate-client", "pinecone-client", "psycopg", "redis", "azure-search-documents", "azure-core", "azure-identity", "usearch", "pyarrow", "ipykernel"]
 
 [tool.ruff]
 lint.select = ["E", "F", "I"]
 line-length = 120
 
 [tool.black]
 line-length = 120
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/function_call_behavior.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/function_call_behavior.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 import google.generativeai as palm
 from numpy import array, ndarray
 from pydantic import StringConstraints, ValidationError
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.connectors.ai.google_palm.settings.google_palm_settings import GooglePalmSettings
 from semantic_kernel.exceptions import ServiceInvalidAuthError, ServiceResponseException
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class GooglePalmTextEmbedding(EmbeddingGeneratorBase):
     api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
 
     def __init__(self, ai_model_id: str, api_key: str | None = None, env_file_path: str | None = None) -> None:
         """
         Initializes a new instance of the GooglePalmTextEmbedding class.
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/hugging_face/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 
 import sentence_transformers
 import torch
 from numpy import array, ndarray
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.exceptions import ServiceResponseException
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class HuggingFaceTextEmbedding(EmbeddingGeneratorBase):
     device: str
     generator: Any
 
     def __init__(
         self,
         ai_model_id: str,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 
 import aiohttp
 from numpy import array, ndarray
 from pydantic import HttpUrl
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.connectors.ai.ollama.utils import AsyncSession
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class OllamaTextEmbedding(EmbeddingGeneratorBase):
     """Ollama embeddings client.
 
     Make sure to have the ollama service running either locally or remotely.
 
     Arguments:
         ai_model_id {str} -- Ollama model name, see https://ollama.ai/library
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,18 @@
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import (
     OpenAITextEmbeddingBase,
 )
 from semantic_kernel.connectors.ai.open_ai.settings.azure_open_ai_settings import AzureOpenAISettings
 from semantic_kernel.exceptions.service_exceptions import ServiceInitializationError
 from semantic_kernel.kernel_pydantic import HttpsUrl
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class AzureTextEmbedding(AzureOpenAIConfigBase, OpenAITextEmbeddingBase):
     """Azure Text Embedding class."""
 
     def __init__(
         self,
         service_id: str | None = None,
         api_key: str | None = None,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,20 +204,20 @@
                 # no need to process function calls
                 # note that we don't check the FinishReason and instead check whether there are any tool calls,
                 # as the service may return a FinishReason of "stop" even if there are tool calls to be made,
                 # in particular if a required tool is specified.
                 return
 
             # there is one response stream in the messages, combining now to create the full completion
-            # depending on the prompt, the message may contain both function call content and others
             full_completion: StreamingChatMessageContent = reduce(lambda x, y: x + y, all_messages)
-            function_calls = [item for item in full_completion.items if isinstance(item, FunctionCallContent)]
             chat_history.add_message(message=full_completion)
 
+            function_calls = [item for item in chat_history.messages[-1].items if isinstance(item, FunctionCallContent)]
             fc_count = len(function_calls)
+
             logger.info(f"processing {fc_count} tool calls in parallel.")
 
             # this function either updates the chat history with the function call results
             # or returns the context, with terminate set to True
             # in which case the loop will break and the function calls are returned.
             # Exceptions are not caught, that is up to the developer, can be done with a filter
             results = await asyncio.gather(
@@ -411,15 +411,15 @@
             settings.function_call_behavior.configure(
                 kernel=kernel,
                 update_settings_callback=update_settings_from_function_call_configuration,
                 settings=settings,
             )
 
     # endregion
-    # region function calling
+    # region tool calling
 
     async def _process_function_call(
         self,
         function_call: FunctionCallContent,
         chat_history: ChatHistory,
         kernel: "Kernel",
         arguments: "KernelArguments",
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
     OpenAIModelTypes,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import (
     OpenAITextEmbeddingBase,
 )
 from semantic_kernel.connectors.ai.open_ai.settings.open_ai_settings import OpenAISettings
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class OpenAITextEmbedding(OpenAIConfigBase, OpenAITextEmbeddingBase):
     """OpenAI Text Embedding class."""
 
     def __init__(
         self,
         ai_model_id: str,
         api_key: str | None = None,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIEmbeddingPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
 class OpenAITextEmbeddingBase(OpenAIHandler, EmbeddingGeneratorBase):
     async def generate_embeddings(self, texts: List[str], batch_size: Optional[int] = None, **kwargs: Any) -> ndarray:
         """Generates embeddings for the given texts.
 
         Arguments:
             texts {List[str]} -- The texts to generate embeddings for.
             batch_size {Optional[int]} -- The batch size to use for the request.
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/services/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,24 @@
     from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
         OpenAIChatPromptExecutionSettings,
     )
 
 logger = logging.getLogger(__name__)
 
 
+TYPE_MAPPER = {
+    "str": "string",
+    "int": "number",
+    "float": "number",
+    "bool": "boolean",
+    "list": "array",
+    "dict": "object",
+}
+
+
 def update_settings_from_function_call_configuration(
     function_call_configuration: "FunctionCallConfiguration", settings: "OpenAIChatPromptExecutionSettings"
 ) -> None:
     """Update the settings from a FunctionCallConfiguration."""
     if function_call_configuration.required_functions:
         if len(function_call_configuration.required_functions) > 1:
             logger.warning("Multiple required functions are not supported. Using the first required function.")
@@ -30,35 +40,35 @@
         settings.tools = [
             kernel_function_metadata_to_openai_tool_format(f) for f in function_call_configuration.available_functions
         ]
 
 
 def kernel_function_metadata_to_openai_tool_format(metadata: KernelFunctionMetadata) -> dict[str, Any]:
     """Convert the kernel function metadata to OpenAI format."""
-
-    def parse_schema(schema_data):
-        """Recursively parse the schema data to include nested properties."""
-        if schema_data.get("type") == "object":
-            return {
-                "type": "object",
-                "properties": {key: parse_schema(value) for key, value in schema_data.get("properties", {}).items()},
-                "description": schema_data.get("description", ""),
-            }
-        else:
-            return {
-                "type": schema_data.get("type", "string"),
-                "description": schema_data.get("description", ""),
-                **({"enum": schema_data.get("enum")} if "enum" in schema_data else {}),
-            }
-
     return {
         "type": "function",
         "function": {
             "name": metadata.fully_qualified_name,
             "description": metadata.description or "",
             "parameters": {
                 "type": "object",
-                "properties": {param.name: parse_schema(param.schema_data) for param in metadata.parameters},
+                "properties": {
+                    param.name: {
+                        "description": param.description or "",
+                        "type": parse_parameter_type(param.type_),
+                        **({"enum": param.enum} if hasattr(param, "enum") else {}),  # Added support for enum
+                    }
+                    for param in metadata.parameters
+                },
                 "required": [p.name for p in metadata.parameters if p.is_required],
             },
         },
     }
+
+
+def parse_parameter_type(param_type: str | None) -> str:
+    """Parse the parameter type."""
+    if not param_type:
+        return "string"
+    if "," in param_type:
+        param_type = param_type.split(",", maxsplit=1)[0]
+    return TYPE_MAPPER.get(param_type, "string")
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/astradb/astra_client.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astra_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 from typing import Dict, List, Optional
 
 import aiohttp
 
 from semantic_kernel.connectors.memory.astradb.utils import AsyncSession
 from semantic_kernel.connectors.telemetry import APP_INFO
 from semantic_kernel.exceptions import ServiceResponseException
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 ASTRA_CALLER_IDENTITY: str
 SEMANTIC_KERNEL_VERSION = APP_INFO.get("Semantic-Kernel-Version")
 if SEMANTIC_KERNEL_VERSION:
     ASTRA_CALLER_IDENTITY = f"semantic-kernel/{SEMANTIC_KERNEL_VERSION}"
 else:
     ASTRA_CALLER_IDENTITY = "semantic-kernel"
 
 
-@experimental_class
 class AstraClient:
     def __init__(
         self,
         astra_id: str,
         astra_region: str,
         astra_application_token: str,
         keyspace_name: str,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,27 +13,25 @@
 from semantic_kernel.connectors.memory.astradb.utils import (
     build_payload,
     parse_payload,
 )
 from semantic_kernel.exceptions import MemoryConnectorInitializationError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 MAX_DIMENSIONALITY = 20000
 MAX_UPSERT_BATCH_SIZE = 100
 MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
 MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
 MAX_FETCH_BATCH_SIZE = 1000
 MAX_DELETE_BATCH_SIZE = 1000
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class AstraDBMemoryStore(MemoryStoreBase):
     """A memory store that uses Astra database as the backend."""
 
     def __init__(
         self,
         astra_application_token: str,
         astra_id: str,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/astradb/astradb_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
 class AstraDBSettings(BaseModelSettings):
     """AstraDB model settings
 
     Optional:
     - app_token: SecretStr | None - AstraDB token
         (Env var ASTRADB_APP_TOKEN)
     - db_id: str | None - AstraDB database ID
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/astradb/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.kernel_pydantic import HttpsUrl
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
 class AzureAISearchSettings(BaseModelSettings):
     """Azure AI Search model settings currently used by the AzureCognitiveSearchMemoryStore connector
 
     Optional:
     - api_key: SecretStr - Azure AI Search API key (Env var AZURE_AI_SEARCH_API_KEY)
     - endpoint: HttpsUrl - Azure AI Search endpoint (Env var AZURE_AI_SEARCH_ENDPOINT)
     - index_name: str - Azure AI Search index name (Env var AZURE_AI_SEARCH_INDEX_NAME)
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,18 @@
     get_index_schema,
     get_search_index_async_client,
     memory_record_to_search_record,
 )
 from semantic_kernel.exceptions import MemoryConnectorInitializationError, MemoryConnectorResourceNotFound
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class AzureCognitiveSearchMemoryStore(MemoryStoreBase):
     _search_index_client: SearchIndexClient = None
     _vector_size: int = None
 
     def __init__(
         self,
         vector_size: int,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,18 @@
     CosmosDBVectorSearchType,
     get_mongodb_search_client,
 )
 from semantic_kernel.connectors.memory.azure_cosmosdb.mongo_vcore_store_api import MongoStoreApi
 from semantic_kernel.exceptions import MemoryConnectorInitializationError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class AzureCosmosDBMemoryStore(MemoryStoreBase):
     """A memory store that uses AzureCosmosDB for MongoDB vCore, to perform vector similarity search on a fully
     managed MongoDB compatible database service.
     https://learn.microsoft.com/en-us/azure/cosmos-db/mongodb/vcore/vector-search"""
 
     # Right now this only supports Mongo, but set up to support more later.
     apiStore: AzureCosmosDBStoreApi = None
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 
 from abc import ABC, abstractmethod
 from typing import List, Tuple
 
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 # Abstract class similar to the original data store that allows API level abstraction
-@experimental_class
 class AzureCosmosDBStoreApi(ABC):
     @abstractmethod
     async def create_collection(self, collection_name: str) -> None:
         raise NotImplementedError
 
     @abstractmethod
     async def get_collections(self) -> List[str]:
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
-class AzureCosmosDBSettings(BaseModelSettings):
-    """Azure CosmosDB model settings
+class MongoDBAtlasSettings(BaseModelSettings):
+    """MongoDB Atlas model settings
 
     Optional:
-    - connection_string: str - Azure CosmosDB connection string
-        (Env var COSMOSDB_CONNECTION_STRING)
+    - connection_string: str - MongoDB Atlas connection string
+        (Env var MONGODB_ATLAS_CONNECTION_STRING)
     """
 
-    api: str | None = None
     connection_string: SecretStr | None = None
 
     class Config(BaseModelSettings.Config):
-        env_prefix = "COSMOSDB_"
+        env_prefix = "MONGODB_ATLAS_"
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,40 +3,36 @@
 from enum import Enum
 
 from dotenv import load_dotenv
 from pymongo import MongoClient
 
 from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT
 from semantic_kernel.exceptions import ServiceInitializationError
-from semantic_kernel.utils.experimental_decorator import experimental_function
 
 
-@experimental_function
 class CosmosDBSimilarityType(str, Enum):
     """Cosmos DB Similarity Type as enumerator."""
 
     COS = "COS"
     """CosineSimilarity"""
     IP = "IP"
     """inner - product"""
     L2 = "L2"
     """Euclidean distance"""
 
 
-@experimental_function
 class CosmosDBVectorSearchType(str, Enum):
     """Cosmos DB Vector Search Type as enumerator."""
 
     VECTOR_IVF = "vector-ivf"
     """IVF vector index"""
     VECTOR_HNSW = "vector-hnsw"
     """HNSW vector index"""
 
 
-@experimental_function
 def get_mongodb_search_client(connection_string: str, application_name: str):
     """
     Returns a client for Azure Cosmos Mongo vCore Vector DB
 
     Arguments:
         connection_string {str}
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,16 @@
     AzureCosmosDBStoreApi,
 )
 from semantic_kernel.connectors.memory.azure_cosmosdb.cosmosdb_utils import (
     CosmosDBSimilarityType,
     CosmosDBVectorSearchType,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
 class MongoStoreApi(AzureCosmosDBStoreApi):
     database = None
     collection_name: str
     index_name = None
     vector_dimensions = None
     num_lists = None
     similarity = None
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 
 from numpy import array, ndarray
 
 from semantic_kernel.connectors.memory.chroma.utils import chroma_compute_similarity_scores, query_results_to_records
 from semantic_kernel.exceptions import ServiceInitializationError, ServiceResourceNotFoundError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 if TYPE_CHECKING:
     import chromadb
     import chromadb.config
     from chromadb.api.models.Collection import Collection
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class ChromaMemoryStore(MemoryStoreBase):
     _client: "chromadb.Client"
 
     def __init__(
         self,
         persist_directory: Optional[str] = None,
         client_settings: Optional["chromadb.config.Settings"] = None,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from numpy import array, expand_dims, ndarray
 from pymilvus import Collection, CollectionSchema, DataType, FieldSchema, connections, utility
 
 from semantic_kernel.exceptions import ServiceResourceNotFoundError, ServiceResponseException
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class, experimental_function
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 # Index parameters
 _INDEX_TYPE = "IVF_FLAT"
 _NLIST = 1024
 
@@ -44,15 +43,14 @@
     SEARCH_FIELD_DESC,
     SEARCH_FIELD_METADATA,
     SEARCH_FIELD_IS_REF,
     SEARCH_FIELD_TIMESTAMP,
 ]
 
 
-@experimental_function
 def memoryrecord_to_milvus_dict(mem: MemoryRecord) -> Dict[str, Any]:
     """Convert a memoryrecord into a dict.
     Args:
         mem (MemoryRecord): MemoryRecord to convert.
 
     Returns:
         dict: Dict result.
@@ -64,15 +62,14 @@
             # Remove underscore
             if isinstance(val, datetime):
                 val = val.isoformat()
             ret_dict[key[1:]] = val
     return ret_dict
 
 
-@experimental_function
 def milvus_dict_to_memoryrecord(milvus_dict: Dict[str, Any]) -> MemoryRecord:
     """Convert Milvus search result dict into MemoryRecord.
 
     Args:
         milvus_dict (dict): Search hit
 
     Returns:
@@ -91,15 +88,14 @@
         additional_metadata=milvus_dict.get(SEARCH_FIELD_METADATA, None),
         embedding=embedding,
         key=milvus_dict.get("key", None),
         timestamp=milvus_dict.get(SEARCH_FIELD_TIMESTAMP, None),
     )
 
 
-@experimental_function
 def create_fields(dimensions: int) -> List[FieldSchema]:
     return [
         FieldSchema(
             name=SEARCH_FIELD_ID,
             dtype=DataType.VARCHAR,
             is_primary=True,
             auto_id=False,
@@ -138,15 +134,14 @@
             name=SEARCH_FIELD_TIMESTAMP,
             dtype=DataType.VARCHAR,
             max_length=100,
         ),
     ]
 
 
-@experimental_class
 class MilvusMemoryStore(MemoryStoreBase):
     def __init__(
         self,
         uri: str = "http://localhost:19530",
         token: Optional[str] = None,
         **kwargs,
     ) -> None:
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,18 @@
     NUM_CANDIDATES_SCALAR,
     document_to_memory_record,
     memory_record_to_mongo_document,
 )
 from semantic_kernel.exceptions import ServiceResourceNotFoundError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class MongoDBAtlasMemoryStore(MemoryStoreBase):
     """Memory Store for MongoDB Atlas Vector Search Connections"""
 
     __slots__ = ("_mongo_client", "__database_name")
 
     _mongo_client: motor_asyncio.AsyncIOMotorClient
     __database_name: str
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,26 @@
     ServiceInitializationError,
     ServiceInvalidRequestError,
     ServiceResourceNotFoundError,
     ServiceResponseException,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 # Limitations set by Pinecone at https://docs.pinecone.io/reference/known-limitations
 MAX_DIMENSIONALITY = 20000
 MAX_UPSERT_BATCH_SIZE = 100
 MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
 MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
 MAX_FETCH_BATCH_SIZE = 1000
 MAX_DELETE_BATCH_SIZE = 1000
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class PineconeMemoryStore(MemoryStoreBase):
     """A memory store that uses Pinecone as the backend."""
 
     _pinecone_api_key: str
     _default_dimensionality: int
 
     DEFAULT_INDEX_SPEC: ServerlessSpec = ServerlessSpec(
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,22 @@
 from semantic_kernel.exceptions import (
     ServiceInitializationError,
     ServiceResourceNotFoundError,
     ServiceResponseException,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 # Limitation based on pgvector documentation https://github.com/pgvector/pgvector#what-if-i-want-to-index-vectors-with-more-than-2000-dimensions
 MAX_DIMENSIONALITY = 2000
 DEFAULT_SCHEMA = "public"
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class PostgresMemoryStore(MemoryStoreBase):
     """A memory store that uses Postgres with pgvector as the backend."""
 
     _connection_string: str
     _connection_pool: ConnectionPool
     _default_dimensionality: int
     _schema: str
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 from numpy import ndarray
 from qdrant_client import QdrantClient
 from qdrant_client import models as qdrant_models
 
 from semantic_kernel.exceptions import ServiceResponseException
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class QdrantMemoryStore(MemoryStoreBase):
     _qdrantclient: QdrantClient
 
     def __init__(
         self,
         vector_size: int,
         url: Optional[str] = None,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/redis/README.md` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,20 +22,18 @@
 from semantic_kernel.exceptions import (
     ServiceInitializationError,
     ServiceResourceNotFoundError,
     ServiceResponseException,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class RedisMemoryStore(MemoryStoreBase):
     """A memory store implementation using Redis"""
 
     _database: "redis.Redis"
     _ft: "redis.Redis.ft"
     # Without RedisAI, it is currently not possible to retrieve index-specific vector attributes to have
     # fully independent collections.
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/redis/redis_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
-class RedisSettings(BaseModelSettings):
-    """Redis model settings
+class AzureCosmosDBSettings(BaseModelSettings):
+    """Azure CosmosDB model settings
 
     Optional:
-    - connection_string: str | None - Redis connection string
-        (Env var REDIS_CONNECTION_STRING)
+    - connection_string: str - Azure CosmosDB connection string
+        (Env var COSMOSDB_CONNECTION_STRING)
     """
 
+    api: str | None = None
     connection_string: SecretStr | None = None
 
     class Config(BaseModelSettings.Config):
-        env_prefix = "REDIS_"
+        env_prefix = "COSMOSDB_"
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/redis/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from semantic_kernel.exceptions import (
     ServiceInitializationError,
     ServiceInvalidRequestError,
     ServiceResourceNotFoundError,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @dataclass
 class _USearchCollection:
     """Represents a collection for USearch with embeddings and related data.
@@ -113,15 +112,14 @@
         MemoryRecord(**row.to_dict(), embedding=vectors[index] if vectors is not None else None)
         for index, row in table.to_pandas().iterrows()
     ]
 
     return result_memory_records
 
 
-@experimental_class
 class USearchMemoryStore(MemoryStoreBase):
     def __init__(
         self,
         persist_directory: Optional[os.PathLike] = None,
     ) -> None:
         """
         Create a USearchMemoryStore instance.
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import numpy as np
 import weaviate
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.memory.weaviate.weaviate_settings import WeaviateSettings
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 SCHEMA = {
     "class": "MemoryRecord",
     "description": "A document from semantic kernel.",
     "properties": [
@@ -69,15 +68,14 @@
 @dataclass
 class WeaviateConfig:
     use_embed: bool = False
     url: str = None
     api_key: str = None
 
 
-@experimental_class
 class WeaviateMemoryStore(MemoryStoreBase):
     class FieldMapper:
         """
         This inner class is responsible for mapping attribute names between
         the SK's memory record and weaviate's schema. It provides methods
         for converting between the two naming conventions.
         """
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.kernel_pydantic import HttpsUrl
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
 class WeaviateSettings(BaseModelSettings):
     """Weaviate model settings
 
     Optional:
     - url: HttpsUrl | None - Weaviate URL (Env var WEAVIATE_URL)
     - api_key: SecretStr | None - Weaviate token (Env var WEAVIATE_API_KEY)
     - use_embed: bool - Whether to use the client embedding options
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/openai_plugin/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/openai_plugin/openai_utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 from typing import Any, Awaitable, Callable, List
 from urllib.parse import urlparse
 
 import httpx
 from pydantic import Field
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 AuthCallbackType = Callable[..., Awaitable[Any]]
 
 
-@experimental_class
 class OpenAPIFunctionExecutionParameters(KernelBaseModel):
     """OpenAPI function execution parameters."""
 
     http_client: httpx.AsyncClient | None = None
     auth_callback: AuthCallbackType | None = None
     server_url_override: str | None = None
     ignore_non_compliant_errors: bool = False
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/openapi_plugin/openapi_manager.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,30 @@
 
 from semantic_kernel.connectors.ai.open_ai.const import USER_AGENT
 from semantic_kernel.exceptions.function_exceptions import FunctionExecutionException, PluginInitializationError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.functions.kernel_function_from_method import KernelFunctionFromMethod
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
-from semantic_kernel.utils.experimental_decorator import experimental_class, experimental_function
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.openai_plugin.openai_function_execution_parameters import (
         OpenAIFunctionExecutionParameters,
     )
     from semantic_kernel.connectors.openapi_plugin.openapi_function_execution_parameters import (
         OpenAPIFunctionExecutionParameters,
     )
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class RestApiOperationParameterStyle(Enum):
     SIMPLE = "simple"
 
 
-@experimental_class
 class RestApiOperationPayloadProperty:
     def __init__(
         self,
         name: str,
         type: str,
         properties: RestApiOperationPayloadProperty,
         description: str | None = None,
@@ -54,30 +51,28 @@
         self.properties = properties
         self.description = description
         self.is_required = is_required
         self.default_value = default_value
         self.schema = schema
 
 
-@experimental_class
 class RestApiOperationPayload:
     def __init__(
         self,
         media_type: str,
         properties: list[RestApiOperationPayloadProperty],
         description: str | None = None,
         schema: str | None = None,
     ):
         self.media_type = media_type
         self.properties = properties
         self.description = description
         self.schema = schema
 
 
-@experimental_class
 class RestApiOperation:
     MEDIA_TYPE_TEXT_PLAIN = "text/plain"
     PAYLOAD_ARGUMENT_NAME = "payload"
     CONTENT_TYPE_ARGUMENT_NAME = "content-type"
     INVALID_SYMBOLS_REGEX = re.compile(r"[^0-9A-Za-z_]+")
 
     def __init__(
@@ -279,26 +274,24 @@
 
         return [
             self.create_payload_artificial_parameter(operation),
             self.create_content_type_artificial_parameter(operation),
         ]
 
 
-@experimental_class
 class RestApiOperationParameterLocation(Enum):
     """The location of the REST API operation parameter."""
 
     PATH = "path"
     QUERY = "query"
     HEADER = "header"
     COOKIE = "cookie"
     BODY = "body"
 
 
-@experimental_class
 class RestApiOperationParameter:
     def __init__(
         self,
         name: str,
         type: str,
         location: RestApiOperationParameterLocation,
         style: RestApiOperationParameterStyle | None = None,
@@ -316,15 +309,14 @@
         self.alternative_name = alternative_name
         self.description = description
         self.is_required = is_required
         self.default_value = default_value
         self.schema = schema
 
 
-@experimental_class
 class OpenApiParser:
     """
     NOTE: SK Python only supports the OpenAPI Spec >=3.0
 
     Import an OpenAPI file.
 
     Args:
@@ -467,36 +459,33 @@
                     description=description,
                 )
 
                 request_objects[operationId] = rest_api_operation
         return request_objects
 
 
-@experimental_class
 class Uri:
     """The Uri class that represents the URI."""
 
     def __init__(self, uri):
         self.uri = uri
 
     def get_left_part(self):
         parsed_uri = urlparse(self.uri)
         return f"{parsed_uri.scheme}://{parsed_uri.netloc}"
 
 
-@experimental_class
 class RestApiOperationRunOptions:
     """The options for running the REST API operation."""
 
     def __init__(self, server_url_override=None, api_host_url=None):
         self.server_url_override: str = server_url_override
         self.api_host_url: str = api_host_url
 
 
-@experimental_class
 class OpenApiRunner:
     """The OpenApiRunner that runs the operations defined in the OpenAPI manifest"""
 
     payload_argument_name = "payload"
     media_type_application_json = "application/json"
 
     def __init__(
@@ -624,15 +613,14 @@
             else:
                 async with httpx.AsyncClient() as client:
                     return await make_request(client)
 
         return await fetch()
 
 
-@experimental_function
 def create_functions_from_openapi(
     plugin_name: str,
     openapi_document_path: str,
     execution_settings: "OpenAIFunctionExecutionParameters | OpenAPIFunctionExecutionParameters | None" = None,
 ) -> list[KernelFunctionFromMethod]:
     """Creates the functions from OpenAPI document.
 
@@ -661,15 +649,14 @@
 
     return [
         _create_function_from_operation(openapi_runner, operation, plugin_name, execution_parameters=execution_settings)
         for operation in operations.values()
     ]
 
 
-@experimental_function
 def _create_function_from_operation(
     runner: OpenApiRunner,
     operation: RestApiOperation,
     plugin_name: str | None = None,
     execution_parameters: "OpenAIFunctionExecutionParameters | OpenAPIFunctionExecutionParameters | None" = None,
     document_uri: str | None = None,
 ) -> KernelFunctionFromMethod:
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/search_engine/bing_connector_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/telemetry.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/telemetry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/connectors/utils/document_loader.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/utils/document_loader.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/chat_history.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_history.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/chat_message_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_message_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/function_call_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_call_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/function_result_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_result_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/kernel_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/kernel_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/streaming_chat_message_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/streaming_content_mixin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_content_mixin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/streaming_text_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/text_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/contents/types.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/conversation_summary_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/http_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/http_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/math_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/math_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/sessions_python_tool/README.md` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/text_memory_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/text_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/time_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/time_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/wait_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/wait_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/core_plugins/web_search_engine_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/web_search_engine_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/exceptions/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/exceptions/content_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/content_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/exceptions/function_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/function_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/exceptions/kernel_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/kernel_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/exceptions/planner_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/planner_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/exceptions/service_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/service_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/exceptions/template_engine_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/template_engine_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/filters/filter_context_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/filters/filter_context_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/function_result.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/function_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/kernel_arguments.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_arguments.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function_decorator.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function_from_method.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         if parameters is None:
             parameters = [KernelParameterMetadata(**param) for param in method.__kernel_function_parameters__]  # type: ignore
         if return_parameter is None:
             return_param = KernelParameterMetadata(
                 name="return",
                 description=method.__kernel_function_return_description__,  # type: ignore
                 default_value=None,
-                type_=method.__kernel_function_return_type__,  # type: ignore
+                type=method.__kernel_function_return_type__,  # type: ignore
                 is_required=method.__kernel_function_return_required__,  # type: ignore
             )
 
         try:
             metadata = KernelFunctionMetadata(
                 name=function_name,
                 description=description,
@@ -120,16 +120,14 @@
         function_arguments = self.gather_function_parameters(context)
         context.result = FunctionResult(function=self.metadata, value=self.stream_method(**function_arguments))
 
     def gather_function_parameters(self, context: FunctionInvocationContext) -> dict[str, Any]:
         """Gathers the function parameters from the arguments."""
         function_arguments: dict[str, Any] = {}
         for param in self.parameters:
-            if param.name is None:
-                raise FunctionExecutionException("Parameter name cannot be None")
             if param.name == "kernel":
                 function_arguments[param.name] = context.kernel
                 continue
             if param.name == "service":
                 function_arguments[param.name] = context.kernel.select_ai_service(self, context.arguments)[0]
                 continue
             if param.name == "execution_settings":
@@ -146,21 +144,18 @@
                             value = param.type_object.model_validate(value)
                         except Exception as exc:
                             raise FunctionExecutionException(
                                 f"Parameter {param.name} is expected to be parsed to {param.type_} but is not."
                             ) from exc
                     else:
                         try:
-                            if isinstance(value, dict) and hasattr(param.type_object, "__init__"):
-                                value = param.type_object(**value)
-                            else:
-                                value = param.type_object(value)
+                            value = param.type_object(value)
                         except Exception as exc:
                             raise FunctionExecutionException(
-                                f"Parameter {param.name} is expected to be parsed to {param.type_object} but is not."
+                                f"Parameter {param.name} is expected to be parsed to {param.type_} but is not."
                             ) from exc
                 function_arguments[param.name] = value
                 continue
             if param.is_required:
                 raise FunctionExecutionException(
                     f"Parameter {param.name} is required but not provided in the arguments."
                 )
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function_from_prompt.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_prompt.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/kernel_function_metadata.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/kernel_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/functions/prompt_rendering_result.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/prompt_rendering_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/kernel.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,17 @@
     """
     The Kernel class is the main entry point for the Semantic Kernel. It provides the ability to run
     semantic/native functions, and manage plugins, memory, and AI services.
 
     Attributes:
         plugins (dict[str, KernelPlugin] | None): The plugins to be used by the kernel
         services (dict[str, AIServiceClientBase]): The services to be used by the kernel
-        ai_service_selector (AIServiceSelector): The AI service selector to be used by the kernel
         retry_mechanism (RetryMechanismBase): The retry mechanism to be used by the kernel
+        function_invoking_handlers (dict): The function invoking handlers
+        function_invoked_handlers (dict): The function invoked handlers
     """
 
     # region Init
 
     plugins: dict[str, KernelPlugin] = Field(default_factory=dict)
     services: dict[str, AIServiceClientBase] = Field(default_factory=dict)
     ai_service_selector: AIServiceSelector = Field(default_factory=AIServiceSelector)
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/kernel_extensions/kernel_filters_extension.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/kernel_extensions/kernel_filters_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_query_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from typing import Optional
 
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
 class MemoryQueryResult:
     is_reference: bool
     external_source_name: Optional[str]
     id: str
     description: Optional[str]
     text: Optional[str]
     additional_metadata: Optional[str]
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from datetime import datetime
 from typing import Optional
 
 from numpy import ndarray
 
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
-
-@experimental_class
 class MemoryRecord:
     _key: str
     _timestamp: Optional[datetime]
     _is_reference: bool
     _external_source_name: Optional[str]
     _id: str
     _description: Optional[str]
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_store_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 
 from abc import ABC, abstractmethod
 from typing import List, Tuple
 
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
 class MemoryStoreBase(ABC):
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *args):
         await self.close()
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/null_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from typing import List, Optional
 
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
 class NullMemory(SemanticTextMemoryBase):
     async def save_information(
         self,
         collection: str,
         text: str,
         id: str,
         description: Optional[str] = None,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 from pydantic import PrivateAttr
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-@experimental_class
 class SemanticTextMemory(SemanticTextMemoryBase):
     _storage: MemoryStoreBase = PrivateAttr()
     # TODO: replace with kernel and service_selector pattern
     _embeddings_generator: EmbeddingGeneratorBase = PrivateAttr()
 
     def __init__(self, storage: MemoryStoreBase, embeddings_generator: EmbeddingGeneratorBase) -> None:
         """Initialize a new instance of SemanticTextMemory.
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from abc import abstractmethod
 from typing import Any, Dict, List, Optional, TypeVar
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 SemanticTextMemoryT = TypeVar("SemanticTextMemoryT", bound="SemanticTextMemoryBase")
 
 
-@experimental_class
 class SemanticTextMemoryBase(KernelBaseModel):
     @abstractmethod
     async def save_information(
         self,
         collection: str,
         text: str,
         id: str,
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/volatile_memory_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 from typing import Dict, List, Tuple
 
 from numpy import array, linalg, ndarray
 
 from semantic_kernel.exceptions import ServiceResourceNotFoundError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
 class VolatileMemoryStore(MemoryStoreBase):
     _store: Dict[str, Dict[str, MemoryRecord]]
 
     def __init__(self) -> None:
         """Initializes a new instance of the VolatileMemoryStore class."""
         self._store = {}
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,34 +180,35 @@
                 args = function_call_content.parse_arguments()
                 return FunctionCallingStepwisePlannerResult(
                     final_answer=args.get("answer", ""),
                     chat_history=chat_history_for_steps,
                     iterations=i + 1,
                 )
 
-            for item in chat_result.items:
-                if not isinstance(item, FunctionCallContent):
+            for content in chat_result.items:
+                if not isinstance(content, FunctionCallContent):
                     continue
                 try:
                     context = await chat_completion._process_function_call(
-                        function_call=item,
+                        function_call=content,
+                        result=chat_result,
                         kernel=cloned_kernel,
                         chat_history=chat_history_for_steps,
                         arguments=arguments,
                         function_call_count=1,
                         request_index=0,
                         function_call_behavior=prompt_execution_settings.function_call_behavior,
                     )
                     frc = FunctionResultContent.from_function_call_content_and_result(
-                        function_call_content=item, result=context.function_result
+                        function_call_content=content, result=context.function_result
                     )
                     chat_history_for_steps.add_message(message=frc.to_chat_message_content())
                 except Exception as exc:
                     frc = FunctionResultContent.from_function_call_content_and_result(
-                        function_call_content=item,
+                        function_call_content=content,
                         result=TextContent(text=f"An error occurred during planner invocation: {exc}"),
                     )
                     chat_history_for_steps.add_message(message=frc.to_chat_message_content())
                     continue
 
         # We're done, but the model hasn't returned a final answer.
         return FunctionCallingStepwisePlannerResult(
```

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/plan.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/plan.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/planner_extensions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/planner_options.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/sequential_planner.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/sequential_planner_config.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/const.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/const.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/handlebars_prompt_template.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/handlebars_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/input_variable.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/input_variable.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/jinja2_prompt_template.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/jinja2_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/kernel_prompt_template.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/kernel_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/prompt_template_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/prompt_template_config.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/prompt_template/utils/template_function_helpers.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/template_function_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/services/ai_service_client_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/services/ai_service_selector.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_selector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/README.md` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/named_arg_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/named_arg_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/text/function_extension.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/utils/experimental_decorator.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/utils/experimental_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/utils/naming.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/utils/naming.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/utils/null_logger.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/utils/null_logger.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/semantic_kernel/utils/validation.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0/PKG-INFO` & `semantic_kernel-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Semantic Kernel Python SDK
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,15 +20,14 @@
 Provides-Extra: postgres
 Provides-Extra: qdrant
 Provides-Extra: redis
 Provides-Extra: usearch
 Provides-Extra: weaviate
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: azure-core (>=1.28.0,<2.0.0) ; extra == "azure" or extra == "all"
-Requires-Dist: azure-cosmos (>=4.7.0,<5.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: azure-identity (>=1.13.0,<2.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: azure-search-documents (==11.6.0b1) ; extra == "azure" or extra == "all"
 Requires-Dist: chromadb (>=0.4.13,<0.5.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: eval_type_backport (>=0.1.3,<0.2.0) ; python_version < "3.10"
 Requires-Dist: google-generativeai (>=0.1) ; (python_version >= "3.9") and (extra == "google" or extra == "all")
 Requires-Dist: grpcio (>=1.40.0) ; python_version == "3.8"
```

