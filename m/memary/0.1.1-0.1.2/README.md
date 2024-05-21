# Comparing `tmp/memary-0.1.1.tar.gz` & `tmp/memary-0.1.2.tar.gz`

## Comparing `memary-0.1.1.tar` & `memary-0.1.2.tar`

### file list

```diff
@@ -1,108 +1,109 @@
--rw-r--r--   0        0        0    16518 2020-02-02 00:00:00.000000 memary-0.1.1/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 memary-0.1.1/requirements.txt
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/openrc
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/data/past_chat.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/data/system_persona.txt
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/data/user_persona.txt
--rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/data/chapter/1.txt
--rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/data/chapter/2.txt
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/data/chapter/3.txt
--rw-r--r--   0        0        0    20428 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/data/chapter/4.txt
--rw-r--r--   0        0        0    37700 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/data/chapter/5.txt
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/update_021924.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/update_022024.md
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/update_022524.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/update_022924.md
--rw-r--r--   0        0        0    81673 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/src/0225_chapter1and2.png
--rw-r--r--   0        0        0   126281 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/src/0225_update_with_chapter3.png
--rw-r--r--   0        0        0   180800 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/src/GraphRAG.png
--rw-r--r--   0        0        0   161852 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/src/chapter1_2.png
--rw-r--r--   0        0        0   197194 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/src/chapter1_2_3.png
--rw-r--r--   0        0        0   106885 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/src/memory_stream_Q1.png
--rw-r--r--   0        0        0   110531 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/docs/src/memory_stream_Q2.png
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2/default__vector_store.json
--rw-r--r--   0        0        0   152568 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2/docstore.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2/image__vector_store.json
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2/index_store.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3/default__vector_store.json
--rw-r--r--   0        0        0   450485 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3/docstore.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3/image__vector_store.json
--rw-r--r--   0        0        0    24222 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3/index_store.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3_4/default__vector_store.json
--rw-r--r--   0        0        0   521199 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3_4/docstore.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3_4/image__vector_store.json
--rw-r--r--   0        0        0    24667 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3_4/index_store.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/tests/memory/test_entity_knowledge_store.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/tests/memory/test_memory.json
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 memary-0.1.1/dev/KG_memory_stream/tests/memory/test_memory_stream.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 memary-0.1.1/dev/legacy_routing_agent/get_location.ipynb
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 memary-0.1.1/dev/legacy_routing_agent/main.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 memary-0.1.1/dev/legacy_routing_agent/ml.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 memary-0.1.1/dev/legacy_routing_agent/readme.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 memary-0.1.1/dev/legacy_routing_agent/tool_spec.ipynb
--rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 memary-0.1.1/dev/legacy_routing_agent/utils.py
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 memary-0.1.1/dev/query_decomposition/MS-SQ.ipynb
--rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 memary-0.1.1/dev/query_decomposition/MS_finetuning.ipynb
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 memary-0.1.1/dev/query_decomposition/SQ-MS.ipynb
--rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 memary-0.1.1/dev/query_decomposition/langchain_ms.ipynb
--rw-r--r--   0        0        0    12581 2020-02-02 00:00:00.000000 memary-0.1.1/dev/query_decomposition/routing_and_multistep.ipynb
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/external_perplexity.ipynb
--rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/recurse.ipynb
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/requirements.txt
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/benchmarking/benchmark.py
--rw-r--r--   0        0        0   109937 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/benchmarking/get_results.ipynb
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/benchmarking/judge.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/benchmarking/ollama_quality.ipynb
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/benchmarking/ollama_test.ipynb
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/benchmarking/output.py
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/benchmarking/perplexity_quality.ipynb
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/benchmarking/perplexity_test.ipynb
--rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/data/external_response.txt
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/docs/cypher.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/docs/implementation.md
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/docs/updates.md
--rw-r--r--   0        0        0   265458 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/docs/images/harry_subgraph.png
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/entity_extraction/entity_extraction.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/entity_extraction/output.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/langchain_retrieval/retrieve.ipynb
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/langchain_retrieval/retrieve.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/synonym_expand/output.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 memary-0.1.1/dev/recursive_retrieval/synonym_expand/synonym.py
--rw-r--r--   0        0        0    73358 2020-02-02 00:00:00.000000 memary-0.1.1/dev/reranking/Reranking.ipynb
--rw-r--r--   0        0        0   262686 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/final.png
--rw-r--r--   0        0        0   135432 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/kg.png
--rw-r--r--   0        0        0    52143 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/memary_logo.png
--rw-r--r--   0        0        0    94297 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/memory.png
--rw-r--r--   0        0        0    55143 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/memory_compression.png
--rw-r--r--   0        0        0    62869 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/memory_module.png
--rw-r--r--   0        0        0    26496 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/query_decomposition.png
--rw-r--r--   0        0        0    41373 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/reranking_diagram.png
--rw-r--r--   0        0        0    16029 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/routing_agent.png
--rw-r--r--   0        0        0   216730 2020-02-02 00:00:00.000000 memary-0.1.1/diagrams/system.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/agent/__init__.py
--rw-r--r--   0        0        0    14636 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/agent/base_agent.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/agent/chat_agent.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/agent/data_types.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/agent/llm_api/tools.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/memory/__init__.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/memory/base_memory.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/memory/entity_knowledge_store.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/memory/memory_stream.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/memory/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/synonym_expand/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/synonym_expand/output.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 memary-0.1.1/src/memary/synonym_expand/synonym.py
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 memary-0.1.1/streamlit_app/app.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 memary-0.1.1/streamlit_app/data/entity_knowledge_store.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 memary-0.1.1/streamlit_app/data/external_response.txt
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 memary-0.1.1/streamlit_app/data/memory_stream.json
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 memary-0.1.1/streamlit_app/data/past_chat.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 memary-0.1.1/streamlit_app/data/routing_response.txt
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 memary-0.1.1/streamlit_app/data/system_persona.txt
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 memary-0.1.1/streamlit_app/data/user_persona.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 memary-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 memary-0.1.1/LICENSE
--rw-r--r--   0        0        0    15581 2020-02-02 00:00:00.000000 memary-0.1.1/README_hidden.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 memary-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    17044 2020-02-02 00:00:00.000000 memary-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 memary-0.1.2/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 memary-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/openrc
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/past_chat.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/system_persona.txt
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/user_persona.txt
+-rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/1.txt
+-rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/2.txt
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/3.txt
+-rw-r--r--   0        0        0    20428 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/4.txt
+-rw-r--r--   0        0        0    37700 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/5.txt
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/update_021924.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/update_022024.md
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/update_022524.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/update_022924.md
+-rw-r--r--   0        0        0    81673 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/0225_chapter1and2.png
+-rw-r--r--   0        0        0   126281 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/0225_update_with_chapter3.png
+-rw-r--r--   0        0        0   180800 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/GraphRAG.png
+-rw-r--r--   0        0        0   161852 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/chapter1_2.png
+-rw-r--r--   0        0        0   197194 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/chapter1_2_3.png
+-rw-r--r--   0        0        0   106885 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/memory_stream_Q1.png
+-rw-r--r--   0        0        0   110531 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/memory_stream_Q2.png
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/default__vector_store.json
+-rw-r--r--   0        0        0   152568 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/docstore.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/image__vector_store.json
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/index_store.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/default__vector_store.json
+-rw-r--r--   0        0        0   450485 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/docstore.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/image__vector_store.json
+-rw-r--r--   0        0        0    24222 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/index_store.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/default__vector_store.json
+-rw-r--r--   0        0        0   521199 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/docstore.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/image__vector_store.json
+-rw-r--r--   0        0        0    24667 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/index_store.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/tests/memory/test_entity_knowledge_store.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/tests/memory/test_memory.json
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/tests/memory/test_memory_stream.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/get_location.ipynb
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/main.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/ml.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/readme.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/tool_spec.ipynb
+-rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/utils.py
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/MS-SQ.ipynb
+-rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/MS_finetuning.ipynb
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/SQ-MS.ipynb
+-rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/langchain_ms.ipynb
+-rw-r--r--   0        0        0    12581 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/routing_and_multistep.ipynb
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/external_perplexity.ipynb
+-rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/recurse.ipynb
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/requirements.txt
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/benchmark.py
+-rw-r--r--   0        0        0   109937 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/get_results.ipynb
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/judge.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/ollama_quality.ipynb
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/ollama_test.ipynb
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/output.py
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/perplexity_quality.ipynb
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/perplexity_test.ipynb
+-rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/data/external_response.txt
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/docs/cypher.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/docs/implementation.md
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/docs/updates.md
+-rw-r--r--   0        0        0   265458 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/docs/images/harry_subgraph.png
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/entity_extraction/entity_extraction.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/entity_extraction/output.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/langchain_retrieval/retrieve.ipynb
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/langchain_retrieval/retrieve.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/synonym_expand/output.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/synonym_expand/synonym.py
+-rw-r--r--   0        0        0    73358 2020-02-02 00:00:00.000000 memary-0.1.2/dev/reranking/Reranking.ipynb
+-rw-r--r--   0        0        0   262686 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/final.png
+-rw-r--r--   0        0        0   135432 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/kg.png
+-rw-r--r--   0        0        0   123706 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/memary_logo.png
+-rw-r--r--   0        0        0    94297 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/memory.png
+-rw-r--r--   0        0        0    55143 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/memory_compression.png
+-rw-r--r--   0        0        0    62869 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/memory_module.png
+-rw-r--r--   0        0        0    26496 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/query_decomposition.png
+-rw-r--r--   0        0        0    41373 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/reranking_diagram.png
+-rw-r--r--   0        0        0    16029 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/routing_agent.png
+-rw-r--r--   0        0        0   216730 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/system.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/__init__.py
+-rw-r--r--   0        0        0    16844 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/base_agent.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/chat_agent.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/data_types.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/llm_api/tools.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/__init__.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/base_memory.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/entity_knowledge_store.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/memory_stream.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/synonym_expand/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/synonym_expand/output.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/synonym_expand/synonym.py
+-rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/app.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/entity_knowledge_store.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/external_response.txt
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/memory_stream.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/past_chat.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/routing_response.txt
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/system_persona.txt
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/user_persona.txt
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/user_persona_template.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 memary-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 memary-0.1.2/LICENSE
+-rw-r--r--   0        0        0    15882 2020-02-02 00:00:00.000000 memary-0.1.2/README_hidden.md
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 memary-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    17449 2020-02-02 00:00:00.000000 memary-0.1.2/PKG-INFO
```

### Comparing `memary-0.1.1/README.md` & `memary-0.1.2/README_hidden.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,41 @@
 # memary: Open-Source Longterm Memory for Autonomous Agents
 
-<img width="1410" alt="memary logo" src="diagrams/memary_logo.png">
-
-[memary demo](https://youtu.be/GnUU3_xK6bg)
-
 ## Why use memary?
 
 Agents use LLMs that are currently constrained to finite context windows. memary overcomes this limitation by allowing your agents to store a large corpus of information in knowledge graphs, infer user knowledge through our memory modules, and only retrieve relevant information for meaningful responses.
 
 ## Features
 
 - **Routing Agent:** Leverage a ReAct agent to route a query for execution amongst many tools.
 - **Knowledge Graph Creation & Retrieval:** Leverage Neo4j to create knowledge graphs storing agent responses for later retrieval.
 - **Memory Stream:** Track all entities stored in the knowledge graph using entity extraction. This stream reflects the user's breadth of knowledge.
 - **Entity Knowledge Store:** Group and order all the entities in the memory stream and pass the top N entities into the context window. This knowledge store reflects the user's depth of knowledge.
 
-## How it works
-
-The current structure of memary is detailed in the diagram below.
-
-<img width="1410" alt="memary overview" src="diagrams/system.png">
-
-The above process includes the routing agent, knoweldge graph and memory module are all integrated into the `ChatAgent` class located in the `src/agent` directory.
-
-Raw source code for these components can also be found in their respective directories including benchmarks, notebooks, and updates.
-
-## Installation
-
-1. Create your [virtual environment](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#create-and-use-virtual-environments) and activate it. Note that Python versions 3.12 or greater are not supported by a key dependancy, llama-index and reccomended to run of python versions <= 3.11.9.
-
-2. Install Python dependencies:
-   ```
-   pip install -r requirements.txt
-   ```
-
 ## Demo
+**Notes:** memary currently assumes the local installation method and currently supports any models available through Ollama:
+- LLM running locally using Ollama **OR** `gpt-3.5-turbo`
+- Vision model running locally using Ollama **OR** `gpt-4-vision-preview`
+
+memary will default to the locally run models unless explicitly specified.
 
-To run the Streamlit app:
+**To run the Streamlit app:**
+1. [Optional] If running models locally using Ollama, follow this the instructions in this [repo](https://github.com/ollama/ollama).
 
-1. Ensure that a `.env` exists with necessary API keys and Neo4j credentials.
+2. Ensure that a `.env` exists with any necessary API keys and Neo4j credentials.
 
 ```
 OPENAI_API_KEY="YOUR_API_KEY"
 NEO4J_PW="YOUR_NEO4J_PW"
 NEO4J_URL="YOUR_NEO4J_URL"
 PERPLEXITY_API_KEY="YOUR_API_KEY"
 GOOGLEMAPS_API_KEY="YOUR_API_KEY"
 ALPHA_VANTAGE_API_KEY="YOUR_API_KEY"
 ```
 
-2. Remove the quotations "" because python may read escape characters '\' and skip characters
-
-```
-CORRECT:
-OPENAI_API_KEY=SKxxxxxxxx
-
-INCORRECT:
-OPENAI_API_KEY="SKxxxxxxxx"
-```
-
 3. How to get API keys:
 
 ```
 OpenAI key: https://openai.com/index/openai-api
 
 Neo4j: https://neo4j.com/cloud/platform/aura-graph-database/?ref=nav-get-started-cta
    Click 'Start for free'
@@ -75,27 +48,28 @@
    Keys are generated in the 'Credentials' page of the 'APIs & Services' tab of Google Cloud Console https://console.cloud.google.com/apis/credentials
 
 Alpha Vantage: (this key is for getting real time stock data)
   https://www.alphavantage.co/support/#api-key
   Reccomend use https://10minutemail.com/ to generate a temporary email to use
 ```
 
-4. Run:
+4.  Update user persona which can be found in `streamlit_app/data/user_persona.txt` using the user persona template which can be found in `streamlit_app/data/user_persona_template.txt`. Instructions have been provided - replace the curly brackets with relevant information. 
+
+5. . [Optional] Update system persona, if needed, which can be found in `streamlit_app/data/system_persona.txt`. 
+6. Run:
 
 ```
 cd streamlit_app
 streamlit run app.py
 ```
 
 ## Detailed Component Breakdown
 
 ### Routing Agent
 
-![agent diagram](diagrams/routing_agent.png)
-
 - Uses the [ReAct agent](https://react-lm.github.io/) to plan and execute a query given the tools provided. This type of agent can reason over which of the tools to use next to further the response, feed inputs into the selected tool, and repeat the process with the output until it determines that the answer is satisfactory.
 - Current tool suite:
   While we didn't emphasize equipping the agent with many tools, we hope to see memary help agents in the community equipped with a vast array of tools covering multi-modalities.
   - **Location** - determines the user's current location and nearby surroundings using geocoder and googlemaps.
   - **CV** - answers a query based on a provided image using gpt-4-vision-preview.
   - **Search** - queries the knowledge graph for a response based on existing nodes and executes an external search if no related entities exist.
 - How does it work?
@@ -105,16 +79,14 @@
 - Future contributions
   - Make your own agent and add as many tools as possible! Each tool expands the agent's ability to answer a wide variety of queries.
   - Create an LLM Judge that scores the routing agent and provides feedback.
   - Integrate multiprocessing so that the agent can process multiple sub-queries simultaneously. We have open-sourced the query decomposition and reranking code to help with this!
 
 ### Knowledge Graph
 
-![KG diagram](diagrams/kg.png)
-
 - What are knowledge graphs (KG)?
   - KGs are databases that store information in the form of entities, which can be anything from objects to more abstract concepts and their relationships with one another.
 - KGs vs other knowledge stores
   - KGs provide more depth of essential context that can be easily retrieved.
   - The knowledge store's graph structure allows information to be centered around certain entities and their relationships with other entities, thus ensuring that the context of the information is relevant.
   - KGs are more adept at handling complex queries, as the varying relationships between different entities in the query can provide insight into how to join multiple subgraphs together.
 - Knowledge graphs &harr; LLMs
@@ -130,16 +102,14 @@
   - Continuously update the memory module with each node insertion.
 - Future contributions
   - Expand the graph’s capabilities to support multiple modalities, i.e., images.
   - Graph optimizations to reduce latency of search times.
 
 ### Memory Module
 
-![Memory Module](diagrams/memory_module.png)
-
 - What is the memory module?
 
 The memory module comprises the Memory Stream and Entity Knowledge Store. The memory module was influenced by the design of [K-LaMP](https://arxiv.org/pdf/2311.06318.pdf) proposed by Microsoft Research.
 
 1. The Memory Stream captures all entities inserted into the KG and their associated timestamps. This stream reflects the breadth of the users' knowledge, i.e., concepts users have had exposure to but no depth of exposure is inferred.
    - Timeline Analysis: Map out a timeline of interactions, highlighting moments of high engagement or shifts in topic focus. This helps in understanding the evolution of the user's interests over time.
    - Extract Themes: Look for recurring themes or topics within the interactions. This thematic analysis can help anticipate user interests or questions even before they are explicitly stated.
@@ -152,34 +122,28 @@
 - Purpose in larger system
   - Compress/summarize the top N ranked entities in the entity knowledge store and pass to the LLM’s finite context window alongside the agent's response and chat history for inference.
   - Personalize Responses: Use the key categorized entities and themes associated with the user to tailor agent responses more closely to the user's current interests and knowledge level/expertise.
   - Anticipate Needs: Leverage trends and shifts identified in the summaries to anticipate users' future questions or needs.
 - Future contributions
   - We currently extract the top N entities from the entitiy knowledge store and pass these entities into the context window for inference. memary can future benefit from more advanced memory compression techniques such as passing only entities that are in the agent's response to the context window. We look forward to related community contributions.
 
-![Memory Compression](diagrams/memory_compression.png)
-
 ## Future Integrations
 
 As mentioned above, memary will benefit from the following integrations:
 
 - Create an LLM Judge that scores the ReACT agent forming a feedback loop. See [Zooter](https://arxiv.org/abs/2311.08692) for insights.
 - Expand the knowledge graph’s capabilities to support multiple modalities, i.e., images.
 - Optimize the graph to reduce latency of search times.
 - Instead of extracting the top N entities from the entity knowledge store deploy more advanced memory compression techniques such as extracting only the entities included in the agent’s response.
 - Create an intuitive UI to switch between models easily. We aim to setup memary so that users can use it for free without any costly API integrations.
 
 Currently memary is structured so that the ReAct agent can only process one query at a time. We hope to see **multiprocessing** integrated so that the agent can process many subqueries simultaneously. We expect this to improve the relevancy and accuracy of responses. The source code for both decomposing the query and reranking the many agent responses has been provided, and once multiprocessing has been added to the system, these components can easily be integrated into the main `ChatAgent` class. The diagram below shows how the newly integrated system would work.
 
-![Future Integrations](diagrams/final.png)
-
 ### Query Decomposition
 
-![QD Diagram](diagrams/query_decomposition.png)
-
 - What is query decomposition?
   - A preprocessing technique that breaks down complex queries into simpler queries to expedite the LLM’s ability to answer the prompt. It is important to note that this process leaves simple queries unchanged.
 - Why decompose?
   - User queries are complex and multifaceted, and base-model LLMs are often unable to fully understand all aspects of the query in order to create a succinct and accurate response.
   - Allows an LLM of similar capabilities to answer easier questions and synthesize those answers to provide an improved response.
 - How it works
 
@@ -195,16 +159,14 @@
   - Simultaneously, QD will pass the original query to the reranking module to rerank the agent responses based on their relevance to the pre-decomposed query.
 - Future contributions
   - Once agent multiprocessing is integrated, QD will be valuable to leverage. All user queries will be passed to QD, and the (sub)queries wil be passed to the routing agent for parallel processing.
   - Self-Learning: Whenever queries are decomposed, those examples will be appended to the engine’s example store as a feedback loop for improved future performance.
 
 ### Reranking
 
-![Reranking Diagram](diagrams/reranking_diagram.png)
-
 - What is reranking?
   - Reranking is the process of scoring nodes based on their relevancy.
 - Why rerank agent responses?
   - Ensure that the various responses to subqueries, when merged, are relevant to the original query prior to decomposition.
 - Our Approach
   - We benchmarked three models to determine which one would best work for reranking: BM25 Reranking Fusion, Cohere Rerank, and ColBERT Rerank. After testing BM25, it was clear that the model was not able to classify the different responses and provide a simple merged answer. Instead of answering the question, it combined all the information on the page, introducing irrelevant information.
   - Next, when testing out Cohere, the model performed better than BM25 but was still not classifying the paragraphs well. The reranking was not always accurate, as it performed well for some questions but was not able to rank others. Furthermore, the ranking was still pretty inaccurate, performing between 0.25 - 0.5 out of 1.
```

### Comparing `memary-0.1.1/requirements.txt` & `memary-0.1.2/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,12 +13,15 @@
 llama-index-multi-modal-llms-openai==0.1.3
 llama-index-program-openai==0.1.3
 llama-index-question-gen-openai==0.1.2
 llama-index-readers-file==0.1.4
 langchain==0.1.12
 langchain-openai==0.0.8
 llama-index-llms-perplexity==0.1.3
+llama-index-multi-modal-llms-ollama==0.1.3
+llama-index-llms-ollama==0.1.2
 pandas
 geocoder
 googlemaps
 ansistrip
-numpy
+numpy
+ollama
```

### Comparing `memary-0.1.1/dev/KG_memory_stream/data/system_persona.txt` & `memary-0.1.2/dev/KG_memory_stream/data/system_persona.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/data/user_persona.txt` & `memary-0.1.2/dev/KG_memory_stream/data/user_persona.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/data/chapter/1.txt` & `memary-0.1.2/dev/KG_memory_stream/data/chapter/1.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/data/chapter/2.txt` & `memary-0.1.2/dev/KG_memory_stream/data/chapter/2.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/data/chapter/3.txt` & `memary-0.1.2/dev/KG_memory_stream/data/chapter/3.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/data/chapter/4.txt` & `memary-0.1.2/dev/KG_memory_stream/data/chapter/4.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/data/chapter/5.txt` & `memary-0.1.2/dev/KG_memory_stream/data/chapter/5.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/update_021924.md` & `memary-0.1.2/dev/KG_memory_stream/docs/update_021924.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/update_022024.md` & `memary-0.1.2/dev/KG_memory_stream/docs/update_022024.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/update_022524.md` & `memary-0.1.2/dev/KG_memory_stream/docs/update_022524.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/update_022924.md` & `memary-0.1.2/dev/KG_memory_stream/docs/update_022924.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/src/0225_chapter1and2.png` & `memary-0.1.2/dev/KG_memory_stream/docs/src/0225_chapter1and2.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/src/0225_update_with_chapter3.png` & `memary-0.1.2/dev/KG_memory_stream/docs/src/0225_update_with_chapter3.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/src/GraphRAG.png` & `memary-0.1.2/dev/KG_memory_stream/docs/src/GraphRAG.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/src/chapter1_2.png` & `memary-0.1.2/dev/KG_memory_stream/docs/src/chapter1_2.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/src/chapter1_2_3.png` & `memary-0.1.2/dev/KG_memory_stream/docs/src/chapter1_2_3.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/src/memory_stream_Q1.png` & `memary-0.1.2/dev/KG_memory_stream/docs/src/memory_stream_Q1.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/docs/src/memory_stream_Q2.png` & `memary-0.1.2/dev/KG_memory_stream/docs/src/memory_stream_Q2.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2/docstore.json` & `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/docstore.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2/index_store.json` & `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/index_store.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3/docstore.json` & `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/docstore.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3/index_store.json` & `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/index_store.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3_4/docstore.json` & `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/docstore.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/storage_graph/ch1_2_3_4/index_store.json` & `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/index_store.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/tests/memory/test_entity_knowledge_store.py` & `memary-0.1.2/dev/KG_memory_stream/tests/memory/test_entity_knowledge_store.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/KG_memory_stream/tests/memory/test_memory_stream.py` & `memary-0.1.2/dev/KG_memory_stream/tests/memory/test_memory_stream.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/legacy_routing_agent/get_location.ipynb` & `memary-0.1.2/dev/legacy_routing_agent/get_location.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/legacy_routing_agent/main.py` & `memary-0.1.2/dev/legacy_routing_agent/main.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/legacy_routing_agent/ml.py` & `memary-0.1.2/dev/legacy_routing_agent/ml.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/legacy_routing_agent/readme.md` & `memary-0.1.2/dev/legacy_routing_agent/readme.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/legacy_routing_agent/tool_spec.ipynb` & `memary-0.1.2/dev/legacy_routing_agent/tool_spec.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/legacy_routing_agent/utils.py` & `memary-0.1.2/dev/legacy_routing_agent/utils.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/query_decomposition/MS-SQ.ipynb` & `memary-0.1.2/dev/query_decomposition/MS-SQ.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/query_decomposition/MS_finetuning.ipynb` & `memary-0.1.2/dev/query_decomposition/MS_finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/query_decomposition/SQ-MS.ipynb` & `memary-0.1.2/dev/query_decomposition/SQ-MS.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/query_decomposition/langchain_ms.ipynb` & `memary-0.1.2/dev/query_decomposition/langchain_ms.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/query_decomposition/routing_and_multistep.ipynb` & `memary-0.1.2/dev/query_decomposition/routing_and_multistep.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/external_perplexity.ipynb` & `memary-0.1.2/dev/recursive_retrieval/external_perplexity.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/recurse.ipynb` & `memary-0.1.2/dev/recursive_retrieval/recurse.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/requirements.txt` & `memary-0.1.2/dev/recursive_retrieval/requirements.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/benchmarking/benchmark.py` & `memary-0.1.2/dev/recursive_retrieval/benchmarking/benchmark.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/benchmarking/get_results.ipynb` & `memary-0.1.2/dev/recursive_retrieval/benchmarking/get_results.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/benchmarking/judge.py` & `memary-0.1.2/dev/recursive_retrieval/benchmarking/judge.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/benchmarking/ollama_quality.ipynb` & `memary-0.1.2/dev/recursive_retrieval/benchmarking/ollama_quality.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/benchmarking/ollama_test.ipynb` & `memary-0.1.2/dev/recursive_retrieval/benchmarking/ollama_test.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/benchmarking/output.py` & `memary-0.1.2/dev/recursive_retrieval/benchmarking/output.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/benchmarking/perplexity_quality.ipynb` & `memary-0.1.2/dev/recursive_retrieval/benchmarking/perplexity_quality.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/benchmarking/perplexity_test.ipynb` & `memary-0.1.2/dev/recursive_retrieval/benchmarking/perplexity_test.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/data/external_response.txt` & `memary-0.1.2/dev/recursive_retrieval/data/external_response.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/docs/updates.md` & `memary-0.1.2/dev/recursive_retrieval/docs/updates.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/docs/images/harry_subgraph.png` & `memary-0.1.2/dev/recursive_retrieval/docs/images/harry_subgraph.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/entity_extraction/entity_extraction.py` & `memary-0.1.2/dev/recursive_retrieval/entity_extraction/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/langchain_retrieval/retrieve.ipynb` & `memary-0.1.2/dev/recursive_retrieval/langchain_retrieval/retrieve.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/langchain_retrieval/retrieve.py` & `memary-0.1.2/dev/recursive_retrieval/langchain_retrieval/retrieve.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/recursive_retrieval/synonym_expand/synonym.py` & `memary-0.1.2/dev/recursive_retrieval/synonym_expand/synonym.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/dev/reranking/Reranking.ipynb` & `memary-0.1.2/dev/reranking/Reranking.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/diagrams/final.png` & `memary-0.1.2/diagrams/final.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/diagrams/kg.png` & `memary-0.1.2/diagrams/kg.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/diagrams/memory.png` & `memary-0.1.2/diagrams/memory.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/diagrams/memory_compression.png` & `memary-0.1.2/diagrams/memory_compression.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/diagrams/memory_module.png` & `memary-0.1.2/diagrams/memory_module.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/diagrams/query_decomposition.png` & `memary-0.1.2/diagrams/query_decomposition.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/diagrams/reranking_diagram.png` & `memary-0.1.2/diagrams/reranking_diagram.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/diagrams/routing_agent.png` & `memary-0.1.2/diagrams/routing_agent.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/diagrams/system.png` & `memary-0.1.2/diagrams/system.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/src/memary/agent/base_agent.py` & `memary-0.1.2/src/memary/agent/base_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 import logging
 import os
 import sys
-import numpy as np
+from pathlib import Path
 
 import geocoder
 import googlemaps
+import numpy as np
+import requests
 from ansistrip import ansi_strip
 from dotenv import load_dotenv
 from llama_index.core import (
     KnowledgeGraphIndex,
     Settings,
     SimpleDirectoryReader,
     StorageContext,
 )
 from llama_index.core.agent import ReActAgent
 from llama_index.core.llms import ChatMessage
-from llama_index.core.multi_modal_llms.generic_utils import load_image_urls
 from llama_index.core.query_engine import RetrieverQueryEngine
 from llama_index.core.retrievers import KnowledgeGraphRAGRetriever
 from llama_index.core.tools import FunctionTool
 from llama_index.graph_stores.neo4j import Neo4jGraphStore
+from llama_index.llms.ollama import Ollama
 from llama_index.llms.openai import OpenAI
 from llama_index.llms.perplexity import Perplexity
+from llama_index.multi_modal_llms.ollama import OllamaMultiModal
 from llama_index.multi_modal_llms.openai import OpenAIMultiModal
-import requests
 
-from memary.agent.data_types import Message
-from memary.agent.llm_api.tools import openai_chat_completions_request
+from memary.agent.data_types import Context, Message
+from memary.agent.llm_api.tools import (
+    ollama_chat_completions_request,
+    openai_chat_completions_request,
+)
 from memary.memory import EntityKnowledgeStore, MemoryStream
 from memary.synonym_expand.synonym import custom_synonym_expand_fn
 
 MAX_ENTITIES_FROM_KG = 5
 ENTITY_EXCEPTIONS = ["Unknown relation"]
-# ChatGPT token limits
+# LLM token limits
 CONTEXT_LENGTH = 4096
 EVICTION_RATE = 0.7
 NONEVICTION_LENGTH = 5
 TOP_ENTITIES = 20
 
 
 def generate_string(entities):
@@ -54,39 +59,34 @@
         self,
         name,
         memory_stream_json,
         entity_knowledge_store_json,
         system_persona_txt,
         user_persona_txt,
         past_chat_json,
+        llm_model_name="llama3",
+        vision_model_name="llava",
         debug=True,
     ):
         load_dotenv()
-        # getting necessary API keys
-        os.environ["OPENAI_API_KEY"] = os.getenv("OPENAI_API_KEY")
+        self.name = name
+        self.model = llm_model_name
+
         googlemaps_api_key = os.getenv("GOOGLEMAPS_API_KEY")
         pplx_api_key = os.getenv("PERPLEXITY_API_KEY")
 
         # Neo4j credentials
         self.neo4j_username = "neo4j"
         self.neo4j_password = os.getenv("NEO4J_PW")
         self.neo4j_url = os.getenv("NEO4J_URL")
         database = "neo4j"
 
         # initialize APIs
-        # OpenAI API
-        self.model = "gpt-3.5-turbo"
-        self.openai_api_key = os.environ["OPENAI_API_KEY"]
-        self.model_endpoint = "https://api.openai.com/v1"
-        self.openai_mm_llm = OpenAIMultiModal(
-            model="gpt-4-vision-preview",
-            api_key=os.getenv("OPENAI_KEY"),
-            max_new_tokens=300,
-        )
-        self.llm = OpenAI(model="gpt-3.5-turbo-instruct")
+        self.load_llm_model(llm_model_name)
+        self.load_vision_model(vision_model_name)
         self.query_llm = Perplexity(
             api_key=pplx_api_key, model="mistral-7b-instruct", temperature=0.5
         )
         self.gmaps = googlemaps.Client(key=googlemaps_api_key)
         Settings.llm = self.llm
         Settings.chunk_size = 512
 
@@ -95,17 +95,19 @@
             username=self.neo4j_username,
             password=self.neo4j_password,
             url=self.neo4j_url,
             database=database,
         )
 
         self.vantage_key = os.getenv("ALPHA_VANTAGE_API_KEY")
-        #self.news_data_key = os.getenv("NEWS_DATA_API_KEY")
+        # self.news_data_key = os.getenv("NEWS_DATA_API_KEY")
 
-        self.storage_context = StorageContext.from_defaults(graph_store=self.graph_store)
+        self.storage_context = StorageContext.from_defaults(
+            graph_store=self.graph_store
+        )
         graph_rag_retriever = KnowledgeGraphRAGRetriever(
             storage_context=self.storage_context,
             verbose=True,
             llm=self.llm,
             retriever_mode="keyword",
             synonym_expand_fn=custom_synonym_expand_fn,
         )
@@ -118,37 +120,65 @@
         locate_tool = FunctionTool.from_defaults(fn=self.locate)
         vision_tool = FunctionTool.from_defaults(fn=self.vision)
         stock_tool = FunctionTool.from_defaults(fn=self.stock_price)
         # news_tool = FunctionTool.from_defaults(fn=self.get_news)
 
         self.debug = debug
         self.routing_agent = ReActAgent.from_tools(
-            [search_tool, locate_tool, vision_tool, stock_tool], llm=self.llm, verbose=True
+            [search_tool, locate_tool, vision_tool, stock_tool],
+            llm=self.llm,
+            verbose=True,
         )
 
         self.memory_stream = MemoryStream(memory_stream_json)
         self.entity_knowledge_store = EntityKnowledgeStore(entity_knowledge_store_json)
 
         self.message = Message(
             system_persona_txt, user_persona_txt, past_chat_json, self.model
         )
 
     def __str__(self):
         return f"Agent {self.name}"
 
+    def load_llm_model(self, llm_model_name):
+        if llm_model_name == "gpt-3.5-turbo":
+            os.environ["OPENAI_API_KEY"] = os.getenv("OPENAI_API_KEY")
+            self.openai_api_key = os.environ["OPENAI_API_KEY"]
+            self.model_endpoint = "https://api.openai.com/v1"
+            self.llm = OpenAI(model="gpt-3.5-turbo-instruct")
+        else:
+            try:
+                self.llm = Ollama(model=llm_model_name, request_timeout=60.0)
+            except:
+                raise ("Please provide a proper llm_model_name.")
+
+    def load_vision_model(self, vision_model_name):
+        if vision_model_name == "gpt-4-vision-preview":
+            os.environ["OPENAI_API_KEY"] = os.getenv("OPENAI_API_KEY")
+            self.openai_api_key = os.environ["OPENAI_API_KEY"]
+            self.mm_model = OpenAIMultiModal(
+                model="gpt-4-vision-preview",
+                api_key=os.getenv("OPENAI_KEY"),
+                max_new_tokens=300,
+            )
+        else:
+            try:
+                self.mm_model = OllamaMultiModal(model=vision_model_name)
+            except:
+                raise ("Please provide a proper vision_model_name.")
+
     def external_query(self, query: str):
         messages_dict = [
             {"role": "system", "content": "Be precise and concise."},
             {"role": "user", "content": query},
         ]
         messages = [ChatMessage(**msg) for msg in messages_dict]
         external_response = self.query_llm.chat(messages)
 
         return str(external_response)
-            
 
     def search(self, query: str) -> str:
         """Search the knowledge graph or perform search on the web if information is not present in the knowledge graph"""
         response = self.query_engine.query(query)
 
         if response.metadata is None:
             return self.external_query(query)
@@ -162,29 +192,44 @@
 
         reverse_geocode_result = self.gmaps.reverse_geocode((lattitude, longitude))
         formatted_address = reverse_geocode_result[0]["formatted_address"]
         return "Your address is" + formatted_address
 
     def vision(self, query: str, img_url: str) -> str:
         """Uses computer vision to process the image specified by the image url and answers the question based on the CV results"""
-        img_docs = load_image_urls([img_url])
-        response = self.openai_mm_llm.complete(prompt=query, image_documents=img_docs)
+        query_image_dir_path = Path("query_images")
+        if not query_image_dir_path.exists():
+            Path.mkdir(query_image_dir_path)
+
+        data = requests.get(img_url).content
+        query_image_path = os.path.join(query_image_dir_path, "query.jpg")
+        with open(query_image_path, "wb") as f:
+            f.write(data)
+        image_documents = SimpleDirectoryReader(query_image_dir_path).load_data()
+
+        response = self.mm_model.complete(prompt=query, image_documents=image_documents)
+
+        os.remove(query_image_path)  # delete image after use
         return response
-    
+
     def stock_price(self, query: str) -> str:
         """Get the stock price of the company given the ticker"""
-        request_api = requests.get(r'https://www.alphavantage.co/query?function=GLOBAL_QUOTE&symbol=' + query + r'&apikey=' + self.vantage_key)
-        return(request_api.json())
+        request_api = requests.get(
+            r"https://www.alphavantage.co/query?function=GLOBAL_QUOTE&symbol="
+            + query
+            + r"&apikey="
+            + self.vantage_key
+        )
+        return request_api.json()
 
     # def get_news(self, query: str) -> str:
     #     """Given a keyword, search for news articles related to the keyword"""
     #     request_api = requests.get(r'https://newsdata.io/api/1/news?apikey=' + self.news_data_key + r'&q=' + query)
     #     return request_api.json()
 
-
     def query(self, query: str) -> str:
         # get the response from react agent
         response = self.routing_agent.chat(query)
         self.routing_agent.reset()
         # write response to file for KG writeback
         with open("data/external_response.txt", "w") as f:
             print(response, file=f)
@@ -217,43 +262,49 @@
         if response.metadata is None:
             return False
         return generate_string(
             list(list(response.metadata.values())[0]["kg_rel_map"].keys())
         )
 
     def _select_top_entities(self):
-        entity_knowledge_store = self.message.llm_message['knowledge_entity_store']
+        entity_knowledge_store = self.message.llm_message["knowledge_entity_store"]
         entities = [entity.to_dict() for entity in entity_knowledge_store]
-        entity_counts = [entity['count'] for entity in entities]
+        entity_counts = [entity["count"] for entity in entities]
         top_indexes = np.argsort(entity_counts)[:TOP_ENTITIES]
         return [entities[index] for index in top_indexes]
 
-    def _change_llm_message_chatgpt(self) -> dict:
-        """Change the llm_message to chatgpt format.
+    def _add_contexts_to_llm_message(self, role, content, index=None):
+        """Add contexts to the llm_message."""
+        if index:
+            self.message.llm_message["messages"].insert(index, Context(role, content))
+        else:
+            self.message.llm_message["messages"].append(Context(role, content))
+
+    def _change_llm_message_chat(self) -> dict:
+        """Change the llm_message to chat format.
 
         Returns:
-            dict: llm_message in chatgpt format
+            dict: llm_message in chat format
         """
-        llm_message_chatgpt = self.message.llm_message.copy()
-        llm_message_chatgpt["messages"] = []
+        llm_message_chat = self.message.llm_message.copy()
+        llm_message_chat["messages"] = []
         top_entities = self._select_top_entities()
-        logging.info(f"top_eneities: {top_entities}")
-        llm_message_chatgpt["messages"].append(
+        logging.info(f"top_entities: {top_entities}")
+        llm_message_chat["messages"].append(
             {
                 "role": "user",
-                "content": "Knowledge Entity Store:"
-                + str(top_entities),
+                "content": "Knowledge Entity Store:" + str(top_entities),
             }
         )
-        llm_message_chatgpt["messages"].extend(
+        llm_message_chat["messages"].extend(
             [context.to_dict() for context in self.message.llm_message["messages"]]
         )
-        llm_message_chatgpt.pop("knowledge_entity_store")
-        llm_message_chatgpt.pop("memory_stream")
-        return llm_message_chatgpt
+        llm_message_chat.pop("knowledge_entity_store")
+        llm_message_chat.pop("memory_stream")
+        return llm_message_chat
 
     def _summarize_contexts(self, total_tokens: int):
         """Summarize the contexts.
 
         Args:
             total_tokens (int): total tokens in the response
         """
@@ -265,54 +316,63 @@
             del self.message.llm_message["messages"][2:-NONEVICTION_LENGTH]
         else:
             messages = messages[2:]
             del self.message.llm_message["messages"][2:]
 
         message_contents = [message.to_dict()["content"] for message in messages]
 
-        llm_message_chatgpt = {
+        llm_message_chat = {
             "model": self.model,
             "messages": [
                 {
                     "role": "user",
                     "content": "Summarize these previous conversations into 50 words:"
                     + str(message_contents),
                 }
             ],
         }
-        response, _ = self._get_gpt_response(llm_message_chatgpt)
+        response, _ = self._get_chat_response(llm_message_chat)
         content = "Summarized past conversation:" + response
         self._add_contexts_to_llm_message("assistant", content, index=2)
         logging.info(f"Contexts summarized successfully. \n summary: {response}")
         logging.info(f"Total tokens after eviction: {total_tokens*EVICTION_RATE}")
 
-    def _get_gpt_response(self, llm_message_chatgpt: str) -> str:
-        """Get response from the GPT model.
+    def _get_chat_response(self, llm_message_chat: str) -> str:
+        """Get response from the LLM chat model.
 
         Args:
-            llm_message_chatgpt (str): query to get response for
+            llm_message_chat (str): query to get response for
 
         Returns:
-            str: response from the GPT model
+            str: response from the LLM chat model
         """
-        response = openai_chat_completions_request(
-            self.model_endpoint, self.openai_api_key, llm_message_chatgpt
-        )
-        total_tokens = response["usage"]["total_tokens"]
-        response = str(response["choices"][0]["message"]["content"])
+        if self.model == "gpt-3.5-turbo":
+            response = openai_chat_completions_request(
+                self.model_endpoint, self.openai_api_key, llm_message_chat
+            )
+            total_tokens = response["usage"]["total_tokens"]
+            response = str(response["choices"][0]["message"]["content"])
+        else:  # default to Ollama model
+            response = ollama_chat_completions_request(
+                llm_message_chat["messages"], self.model
+            )
+            total_tokens = response.get(
+                "prompt_eval_count", 0
+            )  # if 'prompt_eval_count' not present then query is cached
+            response = str(response["message"]["content"])
         return response, total_tokens
 
     def get_response(self) -> str:
         """Get response from the RAG model.
 
         Returns:
             str: response from the RAG model
         """
-        llm_message_chatgpt = self._change_llm_message_chatgpt()
-        response, total_tokens = self._get_gpt_response(llm_message_chatgpt)
+        llm_message_chat = self._change_llm_message_chat()
+        response, total_tokens = self._get_chat_response(llm_message_chat)
         if total_tokens > CONTEXT_LENGTH * EVICTION_RATE:
             logging.info("Evicting and summarizing contexts")
             self._summarize_contexts(total_tokens)
 
         self.message.save_contexts_to_json()
 
         return response
@@ -370,15 +430,14 @@
             if len(entities) > MAX_ENTITIES_FROM_KG:
                 break
         entities = list(set(entities))
         for exceptions in ENTITY_EXCEPTIONS:
             if exceptions in entities:
                 entities.remove(exceptions)
         return entities
-    
 
     def update_tools(self, updatedTools):
         print("recieved update tools")
         tools = []
         for tool in updatedTools:
             if tool == "Search":
                 tools.append(FunctionTool.from_defaults(fn=self.search))
@@ -386,10 +445,9 @@
                 tools.append(FunctionTool.from_defaults(fn=self.locate))
             elif tool == "Vision":
                 tools.append(FunctionTool.from_defaults(fn=self.vision))
             elif tool == "Stocks":
                 tools.append(FunctionTool.from_defaults(fn=self.stock_price))
             # elif tool == "News":
             #     tools.append(FunctionTool.from_defaults(fn=self.get_news))
-        
+
         self.routing_agent = ReActAgent.from_tools(tools, llm=self.llm, verbose=True)
-
```

### Comparing `memary-0.1.1/src/memary/agent/chat_agent.py` & `memary-0.1.2/src/memary/agent/chat_agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import tiktoken
 from typing import Optional, List
 
 from memary.agent.base_agent import Agent
-from memary.agent.data_types import Context
 
 
 class ChatAgent(Agent):
-
+    """ChatAgent currently able to support Llama3 running on Ollama (default) and gpt-3.5-turbo for llm models,
+    and LLaVA running on Ollama (default) and gpt-4-vision-preview for the vision tool.
+    """
     def __init__(self, name, memory_stream_json, entity_knowledge_store_json,
-                 system_persona_txt, user_persona_txt, past_chat_json):
+                 system_persona_txt, user_persona_txt, past_chat_json, llm_model_name="llama3", vision_model_name="llava"):
         super().__init__(name, memory_stream_json, entity_knowledge_store_json,
-                         system_persona_txt, user_persona_txt, past_chat_json)
+                         system_persona_txt, user_persona_txt, past_chat_json, llm_model_name, vision_model_name)
         
 
     def add_chat(self,
                  role: str,
                  content: str,
                  entities: Optional[List[str]] = None):
         """Add a chat to the agent's memory.
@@ -50,24 +50,14 @@
         print("Deleting nodes from Neo4j...")
         try:
             self.graph_store.query("MATCH (n) DETACH DELETE n")
         except Exception as e:
             print(f"Error deleting nodes: {e}")
         print("Nodes deleted from Neo4j.")
 
-
-
-    def _add_contexts_to_llm_message(self, role, content, index=None):
-        """Add contexts to the llm_message."""
-        if index:
-            self.message.llm_message["messages"].insert(index, Context(
-                role, content))
-        else:
-            self.message.llm_message["messages"].append(Context(role, content))
-
     def _replace_memory_from_llm_message(self):
         """Replace the memory_stream from the llm_message."""
         self.message.llm_message[
             "memory_stream"] = self.memory_stream.get_memory()
 
     def _replace_eks_to_from_message(self):
         """Replace the entity knowledge store from the llm_message.
```

### Comparing `memary-0.1.1/src/memary/agent/data_types.py` & `memary-0.1.2/src/memary/agent/data_types.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/src/memary/memory/base_memory.py` & `memary-0.1.2/src/memary/memory/base_memory.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/src/memary/memory/entity_knowledge_store.py` & `memary-0.1.2/src/memary/memory/entity_knowledge_store.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/src/memary/memory/memory_stream.py` & `memary-0.1.2/src/memary/memory/memory_stream.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/src/memary/memory/types.py` & `memary-0.1.2/src/memary/memory/types.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/src/memary/synonym_expand/synonym.py` & `memary-0.1.2/src/memary/synonym_expand/synonym.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/streamlit_app/app.py` & `memary-0.1.2/streamlit_app/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 import random
 import sys
 import textwrap
 
+import ollama
 import pandas as pd
 import streamlit as st
 import streamlit.components.v1 as components
 from dotenv import load_dotenv
 from neo4j import GraphDatabase
 from pyvis.network import Network
 
 # src should sit in the same level as /streamlit_app
 curr_dir = os.getcwd()
 
 parent_dir = os.path.dirname(curr_dir)
-#parent_dir = os.path.dirname(curr_dir) + '/memary' #Use this if error: src not found. Also move the '/streamlit_app/data' folder to the 'memary' folder, outside the 'src' folder.
+# parent_dir = os.path.dirname(curr_dir) + '/memary' #Use this if error: src not found. Also move the '/streamlit_app/data' folder to the 'memary' folder, outside the 'src' folder.
 
-sys.path.append(parent_dir + '/src')
+sys.path.append(parent_dir + "/src")
 
 from memary.agent.chat_agent import ChatAgent
 
 load_dotenv()
 
 system_persona_txt = "data/system_persona.txt"
 user_persona_txt = "data/user_persona.txt"
@@ -78,123 +79,161 @@
                 n2_id = record["p"].nodes[1]["id"]
                 nodes.add(n1_id)
                 nodes.add(n2_id)
                 edges.append((n1_id, n2_id, rels))
                 entities.extend([n1_id, n2_id])
 
 
+def get_models(llm_models, vision_models):
+    models = set()
+    try:
+        ollama_info = ollama.list()
+        for e in ollama_info["models"]:
+            models.add(e["model"])
+        if "llava:latest" in models:
+            vision_models.append("llava:latest")
+            models.remove("llava:latest")
+        llm_models.extend(list(models))
+    except:
+        print("No Ollama instance detected.")
+
 cypher_query = "MATCH p = (:Entity)-[r]-()  RETURN p, r LIMIT 1000;"
 answer = ""
 external_response = ""
-st.title("memary Demo")
-clear_memory = st.button("Clear Memory DB")
-query = st.text_input("Ask a question")
-
-
-
-tools = st.multiselect( 
-    "Select tools to include:",
-    # ["Search", "Location", "Vision", "Stocks", "News"], #all options available
-    # ["Search", "Location", "Vision", "Stocks", "News"],) #options that are selected by default
-
-
-    ["Search", "Location", "Vision", "Stocks"], #all options available
-    ["Search", "Location", "Vision", "Stocks"],) #options that are selected by default
-
-if 'Vision' in tools:
-    img_url = st.text_input("URL of image, leave blank if no image to provide")
-    if img_url:
-        st.image(img_url, caption="Uploaded Image", use_column_width=True)
-
-
-generate_clicked = st.button("Generate")
-st.write("")
+st.title("memary")
 
+llm_models = ["gpt-3.5-turbo"]
+vision_models = ["gpt-4-vision-preview"]
+get_models(llm_models, vision_models)
+
+selected_llm_model = st.selectbox(
+    "Select an LLM model to use.",
+    (model for model in llm_models),
+    index=None,
+    placeholder="Select LLM Model...",
+)
+selected_vision_model = st.selectbox(
+    "Select a vision model to use.",
+    (model for model in vision_models),
+    index=None,
+    placeholder="Select Vision Model...",
+)
 
-if clear_memory:
-    #print("Front end recieved request to clear memory")
-    chat_agent.clearMemory()
-    st.write("Memory DB cleared")
-
-if generate_clicked:
-
-    if(query == ""):
-        st.write("Please enter a question")
-        st.stop()
-
-    #get tools
-    print("tools enabled: ", tools)
-    if(len(tools) == 0):
-        st.write("Please select at least one tool")
-        st.stop()
-
-    print("start update tools")
-    chat_agent.update_tools(tools)
-
-    if img_url:
-        query += "Image URL: " + img_url
-    react_response = ""
-    rag_response = (
-        "There was no information in knowledge_graph to answer your question."
+if selected_llm_model and selected_vision_model:
+    chat_agent = ChatAgent(
+        "Personal Agent",
+        memory_stream_json,
+        entity_knowledge_store_json,
+        system_persona_txt,
+        user_persona_txt,
+        past_chat_json,
+        selected_llm_model,
+        selected_vision_model,
     )
-    chat_agent.add_chat("user", query)
-    cypher_query = chat_agent.check_KG(query)
-    if cypher_query:
-        rag_response, entities = chat_agent.get_routing_agent_response(
-            query, return_entity=True
-        )
-        chat_agent.add_chat("user", "rag: " + rag_response, entities)
-    else:
-        # get response
-        react_response = chat_agent.get_routing_agent_response(query)
-        chat_agent.add_chat("user", "ReAct agent: " + react_response)
-
-    answer = chat_agent.get_response()
-    st.subheader("Routing Agent Response")
-    routing_response = ""
-    with open("data/routing_response.txt", "r") as f:
-        routing_response = f.read()
-    st.text(str(routing_response))
-
-    if cypher_query:
-        nodes = set()
-        edges = []  # (node1, node2, [relationships])
-        fill_graph(nodes, edges, cypher_query)
-
-        st.subheader("Knoweldge Graph")
-        st.code("# Current Cypher Used\n" + cypher_query)
-        st.write("")
-        st.text("Subgraph:")
-        graph = create_graph(nodes, edges)
-        graph_html = graph.generate_html(f"graph_{random.randint(0, 1000)}.html")
-        components.html(graph_html, height=500, scrolling=True)
-    else:
-        st.subheader("Knowledge Graph")
-        st.text("No information found in the knowledge graph")
-
-    st.subheader("Final Response")
-    wrapped_text = textwrap.fill(answer, width=80)
-    st.text(wrapped_text)
-
-    if len(chat_agent.memory_stream) > 0:
-        # Memory Stream
-        memory_items = chat_agent.memory_stream.get_memory()
-        memory_items_dicts = [item.to_dict() for item in memory_items]
-        df = pd.DataFrame(memory_items_dicts)
-        st.write("Memory Stream")
-        st.dataframe(df)
-
-        # Entity Knowledge Store
-        knowledge_memory_items = chat_agent.entity_knowledge_store.get_memory()
-        knowledge_memory_items_dicts = [
-            item.to_dict() for item in knowledge_memory_items
-        ]
-        df_knowledge = pd.DataFrame(knowledge_memory_items_dicts)
-        st.write("Entity Knowledge Store")
-        st.dataframe(df_knowledge)
-
-        # top entities
-        top_entities = chat_agent._select_top_entities()
-        df_top = pd.DataFrame(top_entities)
-        st.write("Top 20 Entities")
-        st.dataframe(df_top)
 
+    st.write(" ")
+    clear_memory = st.button("Clear Memory DB")
+    query = st.text_input("Ask a question")
+
+    tools = st.multiselect(
+        "Select tools to include:",
+        # ["Search", "Location", "Vision", "Stocks", "News"], #all options available
+        # ["Search", "Location", "Vision", "Stocks", "News"],) #options that are selected by default
+        ["Search", "Location", "Vision", "Stocks"],  # all options available
+        ["Search", "Location", "Vision", "Stocks"],
+    )  # options that are selected by default
+
+    if "Vision" in tools:
+        img_url = st.text_input("URL of image, leave blank if no image to provide")
+        if img_url:
+            st.image(img_url, caption="Uploaded Image", use_column_width=True)
+
+    generate_clicked = st.button("Generate")
+    st.write("")
+
+    if clear_memory:
+        # print("Front end recieved request to clear memory")
+        chat_agent.clearMemory()
+        st.write("Memory DB cleared")
+
+    if generate_clicked:
+
+        if query == "":
+            st.write("Please enter a question")
+            st.stop()
+
+        # get tools
+        print("tools enabled: ", tools)
+        if len(tools) == 0:
+            st.write("Please select at least one tool")
+            st.stop()
+
+        print("start update tools")
+        chat_agent.update_tools(tools)
+
+        if img_url:
+            query += "Image URL: " + img_url
+        react_response = ""
+        rag_response = (
+            "There was no information in knowledge_graph to answer your question."
+        )
+        chat_agent.add_chat("user", query)
+        cypher_query = chat_agent.check_KG(query)
+        if cypher_query:
+            rag_response, entities = chat_agent.get_routing_agent_response(
+                query, return_entity=True
+            )
+            chat_agent.add_chat("system", "ReAct agent: " + rag_response, entities)
+        else:
+            # get response
+            react_response = chat_agent.get_routing_agent_response(query)
+            chat_agent.add_chat("system", "ReAct agent: " + react_response)
+
+        answer = chat_agent.get_response()
+        st.subheader("Routing Agent Response")
+        routing_response = ""
+        with open("data/routing_response.txt", "r") as f:
+            routing_response = f.read()
+        st.text(str(routing_response))
+
+        if cypher_query:
+            nodes = set()
+            edges = []  # (node1, node2, [relationships])
+            fill_graph(nodes, edges, cypher_query)
+
+            st.subheader("Knoweldge Graph")
+            st.code("# Current Cypher Used\n" + cypher_query)
+            st.write("")
+            st.text("Subgraph:")
+            graph = create_graph(nodes, edges)
+            graph_html = graph.generate_html(f"graph_{random.randint(0, 1000)}.html")
+            components.html(graph_html, height=500, scrolling=True)
+        else:
+            st.subheader("Knowledge Graph")
+            st.text("No information found in the knowledge graph")
+
+        st.subheader("Final Response")
+        wrapped_text = textwrap.fill(answer, width=80)
+        st.text(wrapped_text)
+
+        if len(chat_agent.memory_stream) > 0:
+            # Memory Stream
+            memory_items = chat_agent.memory_stream.get_memory()
+            memory_items_dicts = [item.to_dict() for item in memory_items]
+            df = pd.DataFrame(memory_items_dicts)
+            st.write("Memory Stream")
+            st.dataframe(df)
+
+            # Entity Knowledge Store
+            knowledge_memory_items = chat_agent.entity_knowledge_store.get_memory()
+            knowledge_memory_items_dicts = [
+                item.to_dict() for item in knowledge_memory_items
+            ]
+            df_knowledge = pd.DataFrame(knowledge_memory_items_dicts)
+            st.write("Entity Knowledge Store")
+            st.dataframe(df_knowledge)
+
+            # top entities
+            top_entities = chat_agent._select_top_entities()
+            df_top = pd.DataFrame(top_entities)
+            st.write("Top 20 Entities")
+            st.dataframe(df_top)
```

### Comparing `memary-0.1.1/streamlit_app/data/user_persona.txt` & `memary-0.1.2/streamlit_app/data/user_persona.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/LICENSE` & `memary-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `memary-0.1.1/README_hidden.md` & `memary-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# memary: Open-Source Longterm Memory for Autonomous Agents
+# memary: Open-Source Longterm Memory for Autonomous Agents <img alt="memary logo" src="diagrams/memary_logo.png">
+
+[![Documentation](https://img.shields.io/badge/Documentation-memary-428BCA?style=flat&logo=open-book)](https://kingjulio8238.github.io/memarydocs/)
+[![Demo](https://img.shields.io/badge/Watch-Demo-red?logo=youtube)](https://youtu.be/GnUU3_xK6bg)
 
 ## Why use memary?
 
 Agents use LLMs that are currently constrained to finite context windows. memary overcomes this limitation by allowing your agents to store a large corpus of information in knowledge graphs, infer user knowledge through our memory modules, and only retrieve relevant information for meaningful responses.
 
 ## Features
 
@@ -11,43 +14,55 @@
 - **Memory Stream:** Track all entities stored in the knowledge graph using entity extraction. This stream reflects the user's breadth of knowledge.
 - **Entity Knowledge Store:** Group and order all the entities in the memory stream and pass the top N entities into the context window. This knowledge store reflects the user's depth of knowledge.
 
 ## How it works
 
 The current structure of memary is detailed in the diagram below.
 
+<img width="1410" alt="memary overview" src="diagrams/system.png">
+
 The above process includes the routing agent, knoweldge graph and memory module are all integrated into the `ChatAgent` class located in the `src/agent` directory.
 
 Raw source code for these components can also be found in their respective directories including benchmarks, notebooks, and updates.
 
+## Installation
+1. With pip:
+```
+pip install memary
+```
+
+2. Locally:
+   1. Create your [virtual environment](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#create-and-use-virtual-environments) and activate it. Note that Python versions 3.12 or greater are not supported by a key dependancy, llama-index and reccomended to run of python versions <= 3.11.9.
+
+   2. Install Python dependencies:
+   ```
+   pip install -r requirements.txt
+   ```
+
 ## Demo
+**Notes:** memary currently assumes the local installation method and currently supports any models available through Ollama:
+- LLM running locally using Ollama **OR** `gpt-3.5-turbo`
+- Vision model running locally using Ollama **OR** `gpt-4-vision-preview`
+
+memary will default to the locally run models unless explicitly specified.
 
-To run the Streamlit app:
+**To run the Streamlit app:**
+1. [Optional] If running models locally using Ollama, follow this the instructions in this [repo](https://github.com/ollama/ollama).
 
-1. Ensure that a `.env` exists with necessary API keys and Neo4j credentials.
+2. Ensure that a `.env` exists with any necessary API keys and Neo4j credentials.
 
 ```
 OPENAI_API_KEY="YOUR_API_KEY"
 NEO4J_PW="YOUR_NEO4J_PW"
 NEO4J_URL="YOUR_NEO4J_URL"
 PERPLEXITY_API_KEY="YOUR_API_KEY"
 GOOGLEMAPS_API_KEY="YOUR_API_KEY"
 ALPHA_VANTAGE_API_KEY="YOUR_API_KEY"
 ```
 
-2. Remove the quotations "" because python may read escape characters '\' and skip characters
-
-```
-CORRECT:
-OPENAI_API_KEY=SKxxxxxxxx
-
-INCORRECT:
-OPENAI_API_KEY="SKxxxxxxxx"
-```
-
 3. How to get API keys:
 
 ```
 OpenAI key: https://openai.com/index/openai-api
 
 Neo4j: https://neo4j.com/cloud/platform/aura-graph-database/?ref=nav-get-started-cta
    Click 'Start for free'
@@ -60,25 +75,30 @@
    Keys are generated in the 'Credentials' page of the 'APIs & Services' tab of Google Cloud Console https://console.cloud.google.com/apis/credentials
 
 Alpha Vantage: (this key is for getting real time stock data)
   https://www.alphavantage.co/support/#api-key
   Reccomend use https://10minutemail.com/ to generate a temporary email to use
 ```
 
-4. Run:
+4.  Update user persona which can be found in `streamlit_app/data/user_persona.txt` using the user persona template which can be found in `streamlit_app/data/user_persona_template.txt`. Instructions have been provided - replace the curly brackets with relevant information. 
+
+5. . [Optional] Update system persona, if needed, which can be found in `streamlit_app/data/system_persona.txt`. 
+6. Run:
 
 ```
 cd streamlit_app
 streamlit run app.py
 ```
 
 ## Detailed Component Breakdown
 
 ### Routing Agent
 
+![agent diagram](diagrams/routing_agent.png)
+
 - Uses the [ReAct agent](https://react-lm.github.io/) to plan and execute a query given the tools provided. This type of agent can reason over which of the tools to use next to further the response, feed inputs into the selected tool, and repeat the process with the output until it determines that the answer is satisfactory.
 - Current tool suite:
   While we didn't emphasize equipping the agent with many tools, we hope to see memary help agents in the community equipped with a vast array of tools covering multi-modalities.
   - **Location** - determines the user's current location and nearby surroundings using geocoder and googlemaps.
   - **CV** - answers a query based on a provided image using gpt-4-vision-preview.
   - **Search** - queries the knowledge graph for a response based on existing nodes and executes an external search if no related entities exist.
 - How does it work?
@@ -88,14 +108,16 @@
 - Future contributions
   - Make your own agent and add as many tools as possible! Each tool expands the agent's ability to answer a wide variety of queries.
   - Create an LLM Judge that scores the routing agent and provides feedback.
   - Integrate multiprocessing so that the agent can process multiple sub-queries simultaneously. We have open-sourced the query decomposition and reranking code to help with this!
 
 ### Knowledge Graph
 
+![KG diagram](diagrams/kg.png)
+
 - What are knowledge graphs (KG)?
   - KGs are databases that store information in the form of entities, which can be anything from objects to more abstract concepts and their relationships with one another.
 - KGs vs other knowledge stores
   - KGs provide more depth of essential context that can be easily retrieved.
   - The knowledge store's graph structure allows information to be centered around certain entities and their relationships with other entities, thus ensuring that the context of the information is relevant.
   - KGs are more adept at handling complex queries, as the varying relationships between different entities in the query can provide insight into how to join multiple subgraphs together.
 - Knowledge graphs &harr; LLMs
@@ -111,14 +133,16 @@
   - Continuously update the memory module with each node insertion.
 - Future contributions
   - Expand the graph’s capabilities to support multiple modalities, i.e., images.
   - Graph optimizations to reduce latency of search times.
 
 ### Memory Module
 
+![Memory Module](diagrams/memory_module.png)
+
 - What is the memory module?
 
 The memory module comprises the Memory Stream and Entity Knowledge Store. The memory module was influenced by the design of [K-LaMP](https://arxiv.org/pdf/2311.06318.pdf) proposed by Microsoft Research.
 
 1. The Memory Stream captures all entities inserted into the KG and their associated timestamps. This stream reflects the breadth of the users' knowledge, i.e., concepts users have had exposure to but no depth of exposure is inferred.
    - Timeline Analysis: Map out a timeline of interactions, highlighting moments of high engagement or shifts in topic focus. This helps in understanding the evolution of the user's interests over time.
    - Extract Themes: Look for recurring themes or topics within the interactions. This thematic analysis can help anticipate user interests or questions even before they are explicitly stated.
@@ -131,29 +155,33 @@
 - Purpose in larger system
   - Compress/summarize the top N ranked entities in the entity knowledge store and pass to the LLM’s finite context window alongside the agent's response and chat history for inference.
   - Personalize Responses: Use the key categorized entities and themes associated with the user to tailor agent responses more closely to the user's current interests and knowledge level/expertise.
   - Anticipate Needs: Leverage trends and shifts identified in the summaries to anticipate users' future questions or needs.
 - Future contributions
   - We currently extract the top N entities from the entitiy knowledge store and pass these entities into the context window for inference. memary can future benefit from more advanced memory compression techniques such as passing only entities that are in the agent's response to the context window. We look forward to related community contributions.
 
+![Memory Compression](diagrams/memory_compression.png)
+
 ## Future Integrations
 
 As mentioned above, memary will benefit from the following integrations:
 
 - Create an LLM Judge that scores the ReACT agent forming a feedback loop. See [Zooter](https://arxiv.org/abs/2311.08692) for insights.
 - Expand the knowledge graph’s capabilities to support multiple modalities, i.e., images.
 - Optimize the graph to reduce latency of search times.
 - Instead of extracting the top N entities from the entity knowledge store deploy more advanced memory compression techniques such as extracting only the entities included in the agent’s response.
 - Create an intuitive UI to switch between models easily. We aim to setup memary so that users can use it for free without any costly API integrations.
 
 Currently memary is structured so that the ReAct agent can only process one query at a time. We hope to see **multiprocessing** integrated so that the agent can process many subqueries simultaneously. We expect this to improve the relevancy and accuracy of responses. The source code for both decomposing the query and reranking the many agent responses has been provided, and once multiprocessing has been added to the system, these components can easily be integrated into the main `ChatAgent` class. The diagram below shows how the newly integrated system would work.
 
+![Future Integrations](diagrams/final.png)
 
 ### Query Decomposition
 
+![QD Diagram](diagrams/query_decomposition.png)
 
 - What is query decomposition?
   - A preprocessing technique that breaks down complex queries into simpler queries to expedite the LLM’s ability to answer the prompt. It is important to note that this process leaves simple queries unchanged.
 - Why decompose?
   - User queries are complex and multifaceted, and base-model LLMs are often unable to fully understand all aspects of the query in order to create a succinct and accurate response.
   - Allows an LLM of similar capabilities to answer easier questions and synthesize those answers to provide an improved response.
 - How it works
@@ -170,14 +198,16 @@
   - Simultaneously, QD will pass the original query to the reranking module to rerank the agent responses based on their relevance to the pre-decomposed query.
 - Future contributions
   - Once agent multiprocessing is integrated, QD will be valuable to leverage. All user queries will be passed to QD, and the (sub)queries wil be passed to the routing agent for parallel processing.
   - Self-Learning: Whenever queries are decomposed, those examples will be appended to the engine’s example store as a feedback loop for improved future performance.
 
 ### Reranking
 
+![Reranking Diagram](diagrams/reranking_diagram.png)
+
 - What is reranking?
   - Reranking is the process of scoring nodes based on their relevancy.
 - Why rerank agent responses?
   - Ensure that the various responses to subqueries, when merged, are relevant to the original query prior to decomposition.
 - Our Approach
   - We benchmarked three models to determine which one would best work for reranking: BM25 Reranking Fusion, Cohere Rerank, and ColBERT Rerank. After testing BM25, it was clear that the model was not able to classify the different responses and provide a simple merged answer. Instead of answering the question, it combined all the information on the page, introducing irrelevant information.
   - Next, when testing out Cohere, the model performed better than BM25 but was still not classifying the paragraphs well. The reranking was not always accurate, as it performed well for some questions but was not able to rank others. Furthermore, the ranking was still pretty inaccurate, performing between 0.25 - 0.5 out of 1.
```

### Comparing `memary-0.1.1/pyproject.toml` & `memary-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "memary"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="memary Labs", email="hello@memarylabs.com" },
 ]
 description = "Longterm Memory for Autonomous Agents"
 readme = "README_hidden.md"
 requires-python = ">=3.8, <=3.11.9"
 classifiers = [
@@ -34,14 +34,16 @@
     "llama-index-multi-modal-llms-openai==0.1.3",
     "llama-index-program-openai==0.1.3",
     "llama-index-question-gen-openai==0.1.2",
     "llama-index-readers-file==0.1.4",
     "langchain==0.1.12",
     "langchain-openai==0.0.8",
     "llama-index-llms-perplexity==0.1.3",
+    "llama-index-multi-modal-llms-ollama==0.1.3",
+    "llama-index-llms-ollama==0.1.2",
     "pandas",
     "geocoder",
     "googlemaps",
     "ansistrip",
     "numpy",
 ]
```

### Comparing `memary-0.1.1/PKG-INFO` & `memary-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: memary
-Version: 0.1.1
+Version: 0.1.2
 Summary: Longterm Memory for Autonomous Agents
 Project-URL: Homepage, https://github.com/kingjulio8238/memary
 Project-URL: Issues, https://github.com/kingjulio8238/memary/issues
 Author-email: memary Labs <hello@memarylabs.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,16 +17,18 @@
 Requires-Dist: langchain==0.1.12
 Requires-Dist: llama-index-agent-openai==0.1.5
 Requires-Dist: llama-index-core==0.10.12
 Requires-Dist: llama-index-embeddings-openai==0.1.5
 Requires-Dist: llama-index-graph-stores-nebula==0.1.2
 Requires-Dist: llama-index-graph-stores-neo4j==0.1.1
 Requires-Dist: llama-index-legacy==0.9.48
+Requires-Dist: llama-index-llms-ollama==0.1.2
 Requires-Dist: llama-index-llms-openai==0.1.5
 Requires-Dist: llama-index-llms-perplexity==0.1.3
+Requires-Dist: llama-index-multi-modal-llms-ollama==0.1.3
 Requires-Dist: llama-index-multi-modal-llms-openai==0.1.3
 Requires-Dist: llama-index-program-openai==0.1.3
 Requires-Dist: llama-index-question-gen-openai==0.1.2
 Requires-Dist: llama-index-readers-file==0.1.4
 Requires-Dist: llama-index==0.10.11
 Requires-Dist: neo4j==5.17.0
 Requires-Dist: numpy
@@ -45,47 +47,35 @@
 ## Features
 
 - **Routing Agent:** Leverage a ReAct agent to route a query for execution amongst many tools.
 - **Knowledge Graph Creation & Retrieval:** Leverage Neo4j to create knowledge graphs storing agent responses for later retrieval.
 - **Memory Stream:** Track all entities stored in the knowledge graph using entity extraction. This stream reflects the user's breadth of knowledge.
 - **Entity Knowledge Store:** Group and order all the entities in the memory stream and pass the top N entities into the context window. This knowledge store reflects the user's depth of knowledge.
 
-## How it works
-
-The current structure of memary is detailed in the diagram below.
-
-The above process includes the routing agent, knoweldge graph and memory module are all integrated into the `ChatAgent` class located in the `src/agent` directory.
-
-Raw source code for these components can also be found in their respective directories including benchmarks, notebooks, and updates.
-
 ## Demo
+**Notes:** memary currently assumes the local installation method and currently supports any models available through Ollama:
+- LLM running locally using Ollama **OR** `gpt-3.5-turbo`
+- Vision model running locally using Ollama **OR** `gpt-4-vision-preview`
 
-To run the Streamlit app:
+memary will default to the locally run models unless explicitly specified.
 
-1. Ensure that a `.env` exists with necessary API keys and Neo4j credentials.
+**To run the Streamlit app:**
+1. [Optional] If running models locally using Ollama, follow this the instructions in this [repo](https://github.com/ollama/ollama).
+
+2. Ensure that a `.env` exists with any necessary API keys and Neo4j credentials.
 
 ```
 OPENAI_API_KEY="YOUR_API_KEY"
 NEO4J_PW="YOUR_NEO4J_PW"
 NEO4J_URL="YOUR_NEO4J_URL"
 PERPLEXITY_API_KEY="YOUR_API_KEY"
 GOOGLEMAPS_API_KEY="YOUR_API_KEY"
 ALPHA_VANTAGE_API_KEY="YOUR_API_KEY"
 ```
 
-2. Remove the quotations "" because python may read escape characters '\' and skip characters
-
-```
-CORRECT:
-OPENAI_API_KEY=SKxxxxxxxx
-
-INCORRECT:
-OPENAI_API_KEY="SKxxxxxxxx"
-```
-
 3. How to get API keys:
 
 ```
 OpenAI key: https://openai.com/index/openai-api
 
 Neo4j: https://neo4j.com/cloud/platform/aura-graph-database/?ref=nav-get-started-cta
    Click 'Start for free'
@@ -98,15 +88,18 @@
    Keys are generated in the 'Credentials' page of the 'APIs & Services' tab of Google Cloud Console https://console.cloud.google.com/apis/credentials
 
 Alpha Vantage: (this key is for getting real time stock data)
   https://www.alphavantage.co/support/#api-key
   Reccomend use https://10minutemail.com/ to generate a temporary email to use
 ```
 
-4. Run:
+4.  Update user persona which can be found in `streamlit_app/data/user_persona.txt` using the user persona template which can be found in `streamlit_app/data/user_persona_template.txt`. Instructions have been provided - replace the curly brackets with relevant information. 
+
+5. . [Optional] Update system persona, if needed, which can be found in `streamlit_app/data/system_persona.txt`. 
+6. Run:
 
 ```
 cd streamlit_app
 streamlit run app.py
 ```
 
 ## Detailed Component Breakdown
@@ -181,18 +174,16 @@
 - Expand the knowledge graph’s capabilities to support multiple modalities, i.e., images.
 - Optimize the graph to reduce latency of search times.
 - Instead of extracting the top N entities from the entity knowledge store deploy more advanced memory compression techniques such as extracting only the entities included in the agent’s response.
 - Create an intuitive UI to switch between models easily. We aim to setup memary so that users can use it for free without any costly API integrations.
 
 Currently memary is structured so that the ReAct agent can only process one query at a time. We hope to see **multiprocessing** integrated so that the agent can process many subqueries simultaneously. We expect this to improve the relevancy and accuracy of responses. The source code for both decomposing the query and reranking the many agent responses has been provided, and once multiprocessing has been added to the system, these components can easily be integrated into the main `ChatAgent` class. The diagram below shows how the newly integrated system would work.
 
-
 ### Query Decomposition
 
-
 - What is query decomposition?
   - A preprocessing technique that breaks down complex queries into simpler queries to expedite the LLM’s ability to answer the prompt. It is important to note that this process leaves simple queries unchanged.
 - Why decompose?
   - User queries are complex and multifaceted, and base-model LLMs are often unable to fully understand all aspects of the query in order to create a succinct and accurate response.
   - Allows an LLM of similar capabilities to answer easier questions and synthesize those answers to provide an improved response.
 - How it works
```

