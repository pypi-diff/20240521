# Comparing `tmp/autorag-0.1.9.tar.gz` & `tmp/autorag-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autorag-0.1.9.tar", last modified: Wed May  1 06:27:49 2024, max compression
+gzip compressed data, was "autorag-0.2.0.tar", last modified: Tue May 21 07:42:28 2024, max compression
```

## Comparing `autorag-0.1.9.tar` & `autorag-0.2.0.tar`

### file list

```diff
@@ -1,518 +1,538 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.746204 autorag-0.1.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-01 06:27:38.000000 autorag-0.1.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.746204 autorag-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-01 06:27:38.000000 autorag-0.1.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-01 06:27:38.000000 autorag-0.1.9/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-01 06:27:38.000000 autorag-0.1.9/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-01 06:27:38.000000 autorag-0.1.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/AutoRAG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-01 06:27:38.000000 autorag-0.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-01 06:27:38.000000 autorag-0.1.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 06:27:38.000000 autorag-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-05-01 06:27:49.838204 autorag-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-01 06:27:38.000000 autorag-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.750204 autorag-0.1.9/autorag/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.750204 autorag-0.1.9/autorag/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.750204 autorag-0.1.9/autorag/data/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/corpus/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.750204 autorag-0.1.9/autorag/data/qacreation/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/ragas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/data/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/evaluate/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17379 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/node_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/openai_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.758204 autorag-0.1.9/autorag/nodes/passageaugmenter/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/prev_next_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.758204 autorag-0.1.9/autorag/nodes/passagecompressor/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.758204 autorag-0.1.9/autorag/nodes/passagefilter/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/pass_passage_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/recency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/threshold_cutoff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.762204 autorag-0.1.9/autorag/nodes/passagereranker/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/flag_embedding_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.762204 autorag-0.1.9/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/time_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.762204 autorag-0.1.9/autorag/nodes/promptmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.762204 autorag-0.1.9/autorag/nodes/queryexpansion/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.766204 autorag-0.1.9/autorag/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/hybrid_dbsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/hybrid_rsf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.766204 autorag-0.1.9/autorag/schema/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/schema/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/schema/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.766204 autorag-0.1.9/autorag/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/web.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 06:27:38.000000 autorag-0.1.9/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.766204 autorag-0.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.770204 autorag-0.1.9/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.774204 autorag-0.1.9/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    57124 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/data_creation.png
--rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/data_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_line_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    42589 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_line_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)    92939 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_lines.png
--rw-r--r--   0 runner    (1001) docker     (127)    95669 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/project_folder_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    19853 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/project_folders.png
--rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.774204 autorag-0.1.9/docs/source/_static/roadmap/
--rw-r--r--   0 runner    (1001) docker     (127)   159068 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 runner    (1001) docker     (127)    38568 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 runner    (1001) docker     (127)    62853 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 runner    (1001) docker     (127)    75826 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 runner    (1001) docker     (127)    82200 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 runner    (1001) docker     (127)    69999 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 runner    (1001) docker     (127)   567356 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/trial_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/trial_json.png
--rw-r--r--   0 runner    (1001) docker     (127)   177107 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/trial_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)   269046 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/web_interface.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.778204 autorag-0.1.9/docs/source/api_spec/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagefilter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.778204 autorag-0.1.9/docs/source/data_creation/
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/data_creation/data_format.md
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/data_creation/ragas.md
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/deploy/web.md
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/local_model.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/generator/generator.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/generator/openai_llm.md
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/passage_augmenter/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_augmenter/passage_augmenter.md
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_compressor/refine.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/passage_filter/
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_filter/passage_filter.md
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_filter/recency_filter.md
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/nodes/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/time_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/nodes/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/nodes/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/hybrid_dbsf.md
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/hybrid_rsf.md
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/optimization/custom_config.md
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/optimization/folder_structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/optimization/optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/optimization/sample_full_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/roadmap/
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/troubleshooting.md
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-01 06:27:38.000000 autorag-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-01 06:27:38.000000 autorag-0.1.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_config/
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/compact_local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/compact_openai.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/config_korean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/extracted_sample.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/simple_local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/simple_openai.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_dataset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_dataset/eli5/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_dataset/msmarco/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_dataset/triviaqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:27:49.838204 autorag-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/tests/autorag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.738204 autorag-0.1.9/tests/autorag/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/tests/autorag/data/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/data/qacreation/
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/qacreation/test_ragas_qa_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/evaluate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/evaluate/metric/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.742204 autorag-0.1.9/tests/autorag/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.798204 autorag-0.1.9/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.798204 autorag-0.1.9/tests/autorag/nodes/passagefilter/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_recency_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_time_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/autorag/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/utils/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.742204 autorag-0.1.9/tests/resources/data_creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/qa_gen_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/result_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/result_project/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    26448 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    41557 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.742204 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/2/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.746204 autorag-0.1.9/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.826204 autorag-0.1.9/tests/resources/result_project/3/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.826204 autorag-0.1.9/tests/resources/result_project/data/
--rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.826204 autorag-0.1.9/tests/resources/result_project/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   109454 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/bm25.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.826204 autorag-0.1.9/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 runner    (1001) docker     (127)  6284000 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 runner    (1001) docker     (127)   352256 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/trial.json
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.746204 autorag-0.1.9/tests/resources/sample_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/tests/resources/sample_project/data/
--rw-r--r--   0 runner    (1001) docker     (127)   115302 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/tests/resources/sample_project/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   109454 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/sample_project/resources/bm25.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/simple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.839811 autorag-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.751811 autorag-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-21 07:42:18.000000 autorag-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.751811 autorag-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-21 07:42:18.000000 autorag-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-21 07:42:18.000000 autorag-0.2.0/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-21 07:42:18.000000 autorag-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-21 07:42:18.000000 autorag-0.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.835811 autorag-0.2.0/AutoRAG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25104 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-21 07:42:18.000000 autorag-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-21 07:42:18.000000 autorag-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 07:42:18.000000 autorag-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25104 2024-05-21 07:42:28.839811 autorag-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-21 07:42:18.000000 autorag-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/corpus/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17782 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/node_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/openai_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.763811 autorag-0.2.0/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/recency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/similarity_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/similarity_threshold_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.763811 autorag-0.2.0/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/schema/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/schema/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.771811 autorag-0.2.0/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.771811 autorag-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.771811 autorag-0.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.775811 autorag-0.2.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    57124 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/data_creation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/data_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/dcg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/f1_score.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38900 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45576 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/mrr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81810 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/ndcg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/ndcg_formula.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42589 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92939 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_lines.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95669 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19853 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/project_folders.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.779811 autorag-0.2.0/docs/source/_static/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)   159068 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38568 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62853 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75826 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 runner    (1001) docker     (127)    82200 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69999 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 runner    (1001) docker     (127)   567356 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/trial_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/trial_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)   177107 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/trial_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)   269046 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/web_interface.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/api_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/data_creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/data_creation/data_format.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/data_creation/ragas.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/deploy/web.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/evaluate_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/evaluate_metrics/generation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/evaluate_metrics/retrieval.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/evaluate_metrics/retrieval_contents.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/local_model.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/generator/openai_llm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/nodes/passage_augmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_augmenter/passage_augmenter.md
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_compressor/refine.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.787811 autorag-0.2.0/docs/source/nodes/passage_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/percentile_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/recency_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/threshold_cutoff.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.787811 autorag-0.2.0/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.787811 autorag-0.2.0/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.787811 autorag-0.2.0/docs/source/nodes/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/docs/source/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/docs/source/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/custom_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/sample_full_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/strategies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/docs/source/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/troubleshooting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-21 07:42:18.000000 autorag-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-21 07:42:18.000000 autorag-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/compact_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/compact_openai.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/config_korean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/extracted_sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/simple_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/simple_openai.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_dataset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_dataset/eli5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_dataset/msmarco/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_dataset/triviaqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:42:28.839811 autorag-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.743811 autorag-0.2.0/tests/autorag/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/evaluate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.743811 autorag-0.2.0/tests/autorag/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.799811 autorag-0.2.0/tests/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.799811 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.799811 autorag-0.2.0/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.799811 autorag-0.2.0/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_recency_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.803811 autorag-0.2.0/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.803811 autorag-0.2.0/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.803811 autorag-0.2.0/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.807811 autorag-0.2.0/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.807811 autorag-0.2.0/tests/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.807811 autorag-0.2.0/tests/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/utils/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.807811 autorag-0.2.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.743811 autorag-0.2.0/tests/resources/data_creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    26448 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    41557 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.747811 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.747811 autorag-0.2.0/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/3/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.827811 autorag-0.2.0/tests/resources/result_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.827811 autorag-0.2.0/tests/resources/result_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/bm25_porter_stemmer.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.827811 autorag-0.2.0/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.835811 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 runner    (1001) docker     (127)  6284000 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 runner    (1001) docker     (127)   352256 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/trial.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.747811 autorag-0.2.0/tests/resources/sample_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.835811 autorag-0.2.0/tests/resources/sample_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   115302 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.835811 autorag-0.2.0/tests/resources/sample_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   109478 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_project/resources/bm25_gpt2.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_project/resources/bm25_porter_stemmer.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `autorag-0.1.9/.github/workflows/publish.yml` & `autorag-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/.github/workflows/sphinx.yml` & `autorag-0.2.0/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/.github/workflows/test.yml` & `autorag-0.2.0/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -3,22 +3,17 @@
 on:
   push:
     branches:
       - main
   pull_request:
     branches:
       - main
-  pull_request_target:
-    branches:
-      - main
 
 env:
   OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
-  COHERE_API_KEY: ${{ secrets.COHERE_API_KEY }}
-  JINAAI_API_KEY: ${{ secrets.JINAAI_API_KEY }}
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Upgrade pip
@@ -28,13 +23,13 @@
         run: |
           sudo apt-get install gcc
       - name: Install AutoRAG
         run: |
           pip install -e .
       - name: Install dependencies
         run: |
-          pip install pytest pytest-xdist pytest-asyncio
+          pip install -r tests/requirements.txt
       - name: delete tests package
         run: python3 tests/delete_tests.py
       - name: Run tests
         run: |
           python3 -m pytest -o log_cli=true --log-cli-level=INFO -n auto tests/
```

### Comparing `autorag-0.1.9/.gitignore` & `autorag-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/AutoRAG.egg-info/PKG-INFO` & `autorag-0.2.0/AutoRAG.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.9
+Version: 0.2.0
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,15 +218,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: tqdm
-Requires-Dist: tiktoken
+Requires-Dist: tiktoken>=0.7.0
 Requires-Dist: openai>=1.0.0
 Requires-Dist: rank_bm25
 Requires-Dist: transformers
 Requires-Dist: swifter
 Requires-Dist: pyyaml
 Requires-Dist: pyarrow
 Requires-Dist: fastparquet
@@ -245,23 +245,30 @@
 Requires-Dist: tokenlog>=0.0.2
 Requires-Dist: aiohttp
 Requires-Dist: bert_score
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding
 Requires-Dist: ragas
 Requires-Dist: ray
+Requires-Dist: kiwipiepy
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
+Requires-Dist: llama-index-retrievers-bm25
 Requires-Dist: streamlit
 Requires-Dist: langchain-core>=0.1.6
+Requires-Dist: panel
+Requires-Dist: seaborn
+Requires-Dist: ipykernel
+Requires-Dist: ipywidgets
+Requires-Dist: ipywidgets_bokeh
 
 # AutoRAG
 
 RAG AutoML tool for automatically finds an optimal RAG pipeline for your data.
 
 Explore our 📖 [Document](https://marker-inc-korea.github.io/AutoRAG/)!!
 
@@ -289,15 +296,16 @@
 - [Quick Install](#-quick-install)
 - [Index](#-index)
 - [Strengths](#-strengths)
 - [QuickStart](#-quickstart)
   - [1. Prepare your evaluation data](#1-prepare-your-evaluation-data)
   - [2. Evaluate your data to various RAG modules](#2-evaluate-your-data-to-various-rag-modules)
   - [3. Use a found optimal RAG pipeline](#3-use-a-found-optimal-rag-pipeline)
-  - [4. Share your RAG pipeline](#4-share-your-rag-pipeline)
+  - [4. Run Dashboard to see the result](#4-run-dashboard)
+  - [5. Share your RAG pipeline](#5-share-your-rag-pipeline)
   - [+ Config yaml file](#-create-your-own-config-yaml-file)
 - [Supporting RAG modules](#supporting-nodes--modules)
 - [Roadmap](#roadmap)
 - [Contribution](#contribution)
 
 # Introduction
 
@@ -419,15 +427,23 @@
 
 You can run api server with CLI command.
 
 ```bash
 autorag run_api --config_path your/path/to/pipeline.yaml --host 0.0.0.0 --port 8000
 ```
 
-### 4. Share your RAG pipeline
+### 4. Run Dashboard
+
+You can run dashboard to easily see the result.
+
+```bash
+autorag dashboard --trial_dir /your/path/to/trial_dir
+```
+
+### 5. Share your RAG pipeline
 
 You can use your RAG pipeline from extracted pipeline yaml file.
 This extracted pipeline is great for sharing your RAG pipeline to others.
 
 You must run this at project folder, which contains datas in data folder, and ingested corpus for retrieval at resources
 folder.
 
@@ -497,23 +513,32 @@
 ```
 
 # ❗Supporting Nodes & modules
 
 You can check our all supporting Nodes & modules
 at [here](https://edai.notion.site/Supporting-Nodes-modules-0ebc7810649f4e41aead472a92976be4?pvs=4)
 
+# ❗Supporting Evaluation Metrics
+
+You can check our all supporting Evaluation Metrics
+at [here](https://edai.notion.site/Supporting-metrics-867d71caefd7401c9264dd91ba406043?pvs=4)
+
+- [Retrieval Metrics](https://edai.notion.site/Retrieval-Metrics-dde3d9fa1d9547cdb8b31b94060d21e7?pvs=4)
+- [Retrieval Token Metrics](https://edai.notion.site/Retrieval-Token-Metrics-c3e2d83358e04510a34b80429ebb543f?pvs=4)
+- [Generation Metrics](https://edai.notion.site/Retrieval-Token-Metrics-c3e2d83358e04510a34b80429ebb543f?pvs=4)
+
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
-- [ ] Visualize evaluation result
+- [x] Visualize evaluation result
 - [ ] Visualize config yaml file
-- [ ] More RAG modules support
+- [x] More RAG modules support
 - [x] Token usage strategy
 - [ ] Multi-modal support
-- [ ] More evaluation metrics
+- [x] More evaluation metrics
 - [ ] Answer Filtering Module
 - [x] Restart optimization from previous trial
 
 # Contribution
 
 We are developing AutoRAG as open-source.
```

### Comparing `autorag-0.1.9/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.2.0/AutoRAG.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .gitignore
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.md
-dev_requirements.txt
 pyproject.toml
 requirements.txt
 .github/dependabot.yml
 .github/workflows/publish.yml
 .github/workflows/sphinx.yml
 .github/workflows/test.yml
 AutoRAG.egg-info/PKG-INFO
@@ -15,14 +14,15 @@
 AutoRAG.egg-info/dependency_links.txt
 AutoRAG.egg-info/entry_points.txt
 AutoRAG.egg-info/requires.txt
 AutoRAG.egg-info/top_level.txt
 autorag/VERSION
 autorag/__init__.py
 autorag/cli.py
+autorag/dashboard.py
 autorag/deploy.py
 autorag/evaluator.py
 autorag/node_line.py
 autorag/strategy.py
 autorag/support.py
 autorag/web.py
 autorag/data/__init__.py
@@ -71,14 +71,16 @@
 autorag/nodes/passagecompressor/tree_summarize.py
 autorag/nodes/passagefilter/__init__.py
 autorag/nodes/passagefilter/base.py
 autorag/nodes/passagefilter/pass_passage_filter.py
 autorag/nodes/passagefilter/percentile_cutoff.py
 autorag/nodes/passagefilter/recency.py
 autorag/nodes/passagefilter/run.py
+autorag/nodes/passagefilter/similarity_percentile_cutoff.py
+autorag/nodes/passagefilter/similarity_threshold_cutoff.py
 autorag/nodes/passagefilter/threshold_cutoff.py
 autorag/nodes/passagereranker/__init__.py
 autorag/nodes/passagereranker/base.py
 autorag/nodes/passagereranker/cohere.py
 autorag/nodes/passagereranker/colbert.py
 autorag/nodes/passagereranker/flag_embedding.py
 autorag/nodes/passagereranker/flag_embedding_llm.py
@@ -129,14 +131,20 @@
 docs/source/install.md
 docs/source/local_model.md
 docs/source/structure.md
 docs/source/troubleshooting.md
 docs/source/tutorial.md
 docs/source/_static/data_creation.png
 docs/source/_static/data_folder.png
+docs/source/_static/dcg.png
+docs/source/_static/f1_score.png
+docs/source/_static/map.png
+docs/source/_static/mrr.png
+docs/source/_static/ndcg.png
+docs/source/_static/ndcg_formula.png
 docs/source/_static/node_folder.png
 docs/source/_static/node_line_folder.png
 docs/source/_static/node_line_summary.png
 docs/source/_static/node_lines.png
 docs/source/_static/node_summary.png
 docs/source/_static/project_folder_example.png
 docs/source/_static/project_folders.png
@@ -173,28 +181,33 @@
 docs/source/api_spec/autorag.utils.rst
 docs/source/api_spec/modules.rst
 docs/source/data_creation/data_format.md
 docs/source/data_creation/ragas.md
 docs/source/data_creation/tutorial.md
 docs/source/deploy/api_endpoint.md
 docs/source/deploy/web.md
+docs/source/evaluate_metrics/generation.md
+docs/source/evaluate_metrics/retrieval.md
+docs/source/evaluate_metrics/retrieval_contents.md
 docs/source/nodes/index.md
 docs/source/nodes/generator/generator.md
 docs/source/nodes/generator/llama_index_llm.md
 docs/source/nodes/generator/openai_llm.md
 docs/source/nodes/generator/vllm.md
 docs/source/nodes/passage_augmenter/passage_augmenter.md
 docs/source/nodes/passage_augmenter/prev_next_augmenter.md
 docs/source/nodes/passage_compressor/passage_compressor.md
 docs/source/nodes/passage_compressor/refine.md
 docs/source/nodes/passage_compressor/tree_summarize.md
 docs/source/nodes/passage_filter/passage_filter.md
+docs/source/nodes/passage_filter/percentile_cutoff.md
 docs/source/nodes/passage_filter/recency_filter.md
 docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
 docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+docs/source/nodes/passage_filter/threshold_cutoff.md
 docs/source/nodes/passage_reranker/cohere.md
 docs/source/nodes/passage_reranker/colbert.md
 docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
 docs/source/nodes/passage_reranker/flag_embedding_reranker.md
 docs/source/nodes/passage_reranker/jina_reranker.md
 docs/source/nodes/passage_reranker/koreranker.md
 docs/source/nodes/passage_reranker/monot5.md
@@ -217,14 +230,15 @@
 docs/source/nodes/retrieval/hybrid_rsf.md
 docs/source/nodes/retrieval/retrieval.md
 docs/source/nodes/retrieval/vectordb.md
 docs/source/optimization/custom_config.md
 docs/source/optimization/folder_structure.md
 docs/source/optimization/optimization.md
 docs/source/optimization/sample_full_config.yaml
+docs/source/optimization/strategies.md
 docs/source/roadmap/modular_rag.md
 sample_config/compact_local.yaml
 sample_config/compact_openai.yaml
 sample_config/config_korean.yaml
 sample_config/extracted_sample.yaml
 sample_config/full.yaml
 sample_config/simple_local.yaml
@@ -232,15 +246,17 @@
 sample_dataset/README.md
 sample_dataset/eli5/load_eli5_dataset.py
 sample_dataset/msmarco/load_msmarco_dataset.py
 sample_dataset/triviaqa/load_triviaqa_dataset.py
 tests/conftest.py
 tests/delete_tests.py
 tests/mock.py
+tests/requirements.txt
 tests/autorag/test_cli.py
+tests/autorag/test_dashboard.py
 tests/autorag/test_deploy.py
 tests/autorag/test_evaluator.py
 tests/autorag/test_strategy.py
 tests/autorag/test_support.py
 tests/autorag/test_web.py
 tests/autorag/data/corpus/test_base.py
 tests/autorag/data/corpus/test_langchain.py
@@ -271,14 +287,16 @@
 tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
 tests/autorag/nodes/passagecompressor/test_tree_summarize.py
 tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
 tests/autorag/nodes/passagefilter/test_passage_filter_base.py
 tests/autorag/nodes/passagefilter/test_passage_filter_run.py
 tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
 tests/autorag/nodes/passagefilter/test_recency_filter.py
+tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py
+tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py
 tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
 tests/autorag/nodes/passagereranker/test_cohere_reranker.py
 tests/autorag/nodes/passagereranker/test_colbert_reranker.py
 tests/autorag/nodes/passagereranker/test_flag_embedding.py
 tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
 tests/autorag/nodes/passagereranker/test_jina_reranker.py
 tests/autorag/nodes/passagereranker/test_koreranker.py
@@ -365,15 +383,15 @@
 tests/resources/result_project/1/config.yaml
 tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
 tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
 tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
 tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
 tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
 tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
-tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
+tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet
 tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
 tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
 tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
 tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
 tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
 tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
 tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
@@ -397,16 +415,17 @@
 tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
 tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
 tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
 tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
 tests/resources/result_project/3/config.yaml
 tests/resources/result_project/data/corpus.parquet
 tests/resources/result_project/data/qa.parquet
-tests/resources/result_project/resources/bm25.pkl
+tests/resources/result_project/resources/bm25_porter_stemmer.pkl
 tests/resources/result_project/resources/chroma/chroma.sqlite3
 tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
 tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
 tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
 tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
 tests/resources/sample_project/data/corpus.parquet
 tests/resources/sample_project/data/qa.parquet
-tests/resources/sample_project/resources/bm25.pkl
+tests/resources/sample_project/resources/bm25_gpt2.pkl
+tests/resources/sample_project/resources/bm25_porter_stemmer.pkl
```

### Comparing `autorag-0.1.9/CODE_OF_CONDUCT.md` & `autorag-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/CONTRIBUTING.md` & `autorag-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/LICENSE` & `autorag-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/PKG-INFO` & `autorag-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.9
+Version: 0.2.0
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,15 +218,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: tqdm
-Requires-Dist: tiktoken
+Requires-Dist: tiktoken>=0.7.0
 Requires-Dist: openai>=1.0.0
 Requires-Dist: rank_bm25
 Requires-Dist: transformers
 Requires-Dist: swifter
 Requires-Dist: pyyaml
 Requires-Dist: pyarrow
 Requires-Dist: fastparquet
@@ -245,23 +245,30 @@
 Requires-Dist: tokenlog>=0.0.2
 Requires-Dist: aiohttp
 Requires-Dist: bert_score
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding
 Requires-Dist: ragas
 Requires-Dist: ray
+Requires-Dist: kiwipiepy
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
+Requires-Dist: llama-index-retrievers-bm25
 Requires-Dist: streamlit
 Requires-Dist: langchain-core>=0.1.6
+Requires-Dist: panel
+Requires-Dist: seaborn
+Requires-Dist: ipykernel
+Requires-Dist: ipywidgets
+Requires-Dist: ipywidgets_bokeh
 
 # AutoRAG
 
 RAG AutoML tool for automatically finds an optimal RAG pipeline for your data.
 
 Explore our 📖 [Document](https://marker-inc-korea.github.io/AutoRAG/)!!
 
@@ -289,15 +296,16 @@
 - [Quick Install](#-quick-install)
 - [Index](#-index)
 - [Strengths](#-strengths)
 - [QuickStart](#-quickstart)
   - [1. Prepare your evaluation data](#1-prepare-your-evaluation-data)
   - [2. Evaluate your data to various RAG modules](#2-evaluate-your-data-to-various-rag-modules)
   - [3. Use a found optimal RAG pipeline](#3-use-a-found-optimal-rag-pipeline)
-  - [4. Share your RAG pipeline](#4-share-your-rag-pipeline)
+  - [4. Run Dashboard to see the result](#4-run-dashboard)
+  - [5. Share your RAG pipeline](#5-share-your-rag-pipeline)
   - [+ Config yaml file](#-create-your-own-config-yaml-file)
 - [Supporting RAG modules](#supporting-nodes--modules)
 - [Roadmap](#roadmap)
 - [Contribution](#contribution)
 
 # Introduction
 
@@ -419,15 +427,23 @@
 
 You can run api server with CLI command.
 
 ```bash
 autorag run_api --config_path your/path/to/pipeline.yaml --host 0.0.0.0 --port 8000
 ```
 
-### 4. Share your RAG pipeline
+### 4. Run Dashboard
+
+You can run dashboard to easily see the result.
+
+```bash
+autorag dashboard --trial_dir /your/path/to/trial_dir
+```
+
+### 5. Share your RAG pipeline
 
 You can use your RAG pipeline from extracted pipeline yaml file.
 This extracted pipeline is great for sharing your RAG pipeline to others.
 
 You must run this at project folder, which contains datas in data folder, and ingested corpus for retrieval at resources
 folder.
 
@@ -497,23 +513,32 @@
 ```
 
 # ❗Supporting Nodes & modules
 
 You can check our all supporting Nodes & modules
 at [here](https://edai.notion.site/Supporting-Nodes-modules-0ebc7810649f4e41aead472a92976be4?pvs=4)
 
+# ❗Supporting Evaluation Metrics
+
+You can check our all supporting Evaluation Metrics
+at [here](https://edai.notion.site/Supporting-metrics-867d71caefd7401c9264dd91ba406043?pvs=4)
+
+- [Retrieval Metrics](https://edai.notion.site/Retrieval-Metrics-dde3d9fa1d9547cdb8b31b94060d21e7?pvs=4)
+- [Retrieval Token Metrics](https://edai.notion.site/Retrieval-Token-Metrics-c3e2d83358e04510a34b80429ebb543f?pvs=4)
+- [Generation Metrics](https://edai.notion.site/Retrieval-Token-Metrics-c3e2d83358e04510a34b80429ebb543f?pvs=4)
+
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
-- [ ] Visualize evaluation result
+- [x] Visualize evaluation result
 - [ ] Visualize config yaml file
-- [ ] More RAG modules support
+- [x] More RAG modules support
 - [x] Token usage strategy
 - [ ] Multi-modal support
-- [ ] More evaluation metrics
+- [x] More evaluation metrics
 - [ ] Answer Filtering Module
 - [x] Restart optimization from previous trial
 
 # Contribution
 
 We are developing AutoRAG as open-source.
```

### Comparing `autorag-0.1.9/README.md` & `autorag-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 - [Quick Install](#-quick-install)
 - [Index](#-index)
 - [Strengths](#-strengths)
 - [QuickStart](#-quickstart)
   - [1. Prepare your evaluation data](#1-prepare-your-evaluation-data)
   - [2. Evaluate your data to various RAG modules](#2-evaluate-your-data-to-various-rag-modules)
   - [3. Use a found optimal RAG pipeline](#3-use-a-found-optimal-rag-pipeline)
-  - [4. Share your RAG pipeline](#4-share-your-rag-pipeline)
+  - [4. Run Dashboard to see the result](#4-run-dashboard)
+  - [5. Share your RAG pipeline](#5-share-your-rag-pipeline)
   - [+ Config yaml file](#-create-your-own-config-yaml-file)
 - [Supporting RAG modules](#supporting-nodes--modules)
 - [Roadmap](#roadmap)
 - [Contribution](#contribution)
 
 # Introduction
 
@@ -158,15 +159,23 @@
 
 You can run api server with CLI command.
 
 ```bash
 autorag run_api --config_path your/path/to/pipeline.yaml --host 0.0.0.0 --port 8000
 ```
 
-### 4. Share your RAG pipeline
+### 4. Run Dashboard
+
+You can run dashboard to easily see the result.
+
+```bash
+autorag dashboard --trial_dir /your/path/to/trial_dir
+```
+
+### 5. Share your RAG pipeline
 
 You can use your RAG pipeline from extracted pipeline yaml file.
 This extracted pipeline is great for sharing your RAG pipeline to others.
 
 You must run this at project folder, which contains datas in data folder, and ingested corpus for retrieval at resources
 folder.
 
@@ -236,23 +245,32 @@
 ```
 
 # ❗Supporting Nodes & modules
 
 You can check our all supporting Nodes & modules
 at [here](https://edai.notion.site/Supporting-Nodes-modules-0ebc7810649f4e41aead472a92976be4?pvs=4)
 
+# ❗Supporting Evaluation Metrics
+
+You can check our all supporting Evaluation Metrics
+at [here](https://edai.notion.site/Supporting-metrics-867d71caefd7401c9264dd91ba406043?pvs=4)
+
+- [Retrieval Metrics](https://edai.notion.site/Retrieval-Metrics-dde3d9fa1d9547cdb8b31b94060d21e7?pvs=4)
+- [Retrieval Token Metrics](https://edai.notion.site/Retrieval-Token-Metrics-c3e2d83358e04510a34b80429ebb543f?pvs=4)
+- [Generation Metrics](https://edai.notion.site/Retrieval-Token-Metrics-c3e2d83358e04510a34b80429ebb543f?pvs=4)
+
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
-- [ ] Visualize evaluation result
+- [x] Visualize evaluation result
 - [ ] Visualize config yaml file
-- [ ] More RAG modules support
+- [x] More RAG modules support
 - [x] Token usage strategy
 - [ ] Multi-modal support
-- [ ] More evaluation metrics
+- [x] More evaluation metrics
 - [ ] Answer Filtering Module
 - [x] Restart optimization from previous trial
 
 # Contribution
 
 We are developing AutoRAG as open-source.
```

### Comparing `autorag-0.1.9/autorag/__init__.py` & `autorag-0.2.0/autorag/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import logging.config
 import os
 import sys
 
 import transformers
+from llama_index.core.llms.mock import MockLLM
 from llama_index.embeddings.huggingface import HuggingFaceEmbedding
 from llama_index.embeddings.openai import OpenAIEmbedding
 from llama_index.embeddings.openai import OpenAIEmbeddingModelType
 from llama_index.llms.huggingface import HuggingFaceLLM
 from llama_index.llms.openai import OpenAI
 from llama_index.llms.openai_like import OpenAILike
 from rich.logging import RichHandler
@@ -51,14 +52,15 @@
                                               max_length=512, )
 }
 
 generator_models = {
     'openai': OpenAI,
     'huggingfacellm': HuggingFaceLLM,
     'openailike': OpenAILike,
+    'mock': MockLLM,
 }
 
 rich_format = "[%(filename)s:%(lineno)s] >> %(message)s"
 logging.basicConfig(
     level="INFO",
     format=rich_format,
     handlers=[RichHandler(rich_tracebacks=True)]
```

### Comparing `autorag-0.1.9/autorag/cli.py` & `autorag-0.2.0/autorag/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pathlib
 import subprocess
 from pathlib import Path
 from typing import Optional
 
 import click
 
+from autorag import dashboard
 from autorag.deploy import Runner
 from autorag.deploy import extract_best_config as original_extract_best_config
 from autorag.evaluator import Evaluator
 
 logger = logging.getLogger("AutoRAG")
 
 
@@ -67,14 +68,20 @@
     elif yaml_path and project_dir:
         subprocess.run(['streamlit', 'run', web_py_path, '--', '--yaml_path', yaml_path, '--project_dir', project_dir])
     elif trial_path:
         subprocess.run(['streamlit', 'run', web_py_path, '--', '--trial_path', trial_path])
 
 
 @click.command()
+@click.option('--trial_dir', type=click.Path(dir_okay=True, file_okay=False, exists=True), required=True)
+def run_dashboard(trial_dir: str):
+    dashboard.run(trial_dir)
+
+
+@click.command()
 @click.option('--trial_path', type=click.Path(), help='Path to the trial directory.')
 @click.option('--output_path', type=click.Path(), help='Path to the output directory.'
                                                        ' Must be .yaml or .yml file.')
 def extract_best_config(trial_path: str, output_path: str):
     original_extract_best_config(trial_path, output_path)
 
 
@@ -90,12 +97,13 @@
     evaluator.restart_trial(trial_path)
     logger.info('Evaluation complete.')
 
 
 cli.add_command(evaluate, 'evaluate')
 cli.add_command(run_api, 'run_api')
 cli.add_command(run_web, 'run_web')
+cli.add_command(run_dashboard, 'dashboard')
 cli.add_command(extract_best_config, 'extract_best_config')
 cli.add_command(restart_evaluate, 'restart_evaluate')
 
 if __name__ == '__main__':
     cli()
```

### Comparing `autorag-0.1.9/autorag/data/corpus/langchain.py` & `autorag-0.2.0/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/data/corpus/llama_index.py` & `autorag-0.2.0/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/data/qacreation/base.py` & `autorag-0.2.0/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/data/qacreation/llama_index.py` & `autorag-0.2.0/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.2.0/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/data/qacreation/ragas.py` & `autorag-0.2.0/autorag/data/qacreation/ragas.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/data/qacreation/simple.py` & `autorag-0.2.0/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/data/utils/util.py` & `autorag-0.2.0/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/deploy.py` & `autorag-0.2.0/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluate/generation.py` & `autorag-0.2.0/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluate/metric/generation.py` & `autorag-0.2.0/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluate/metric/retrieval.py` & `autorag-0.2.0/autorag/evaluate/metric/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.2.0/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluate/retrieval.py` & `autorag-0.2.0/autorag/evaluate/retrieval_contents.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 import functools
-import warnings
 from typing import List, Callable, Any, Tuple
 
 import pandas as pd
 
-from autorag.evaluate.metric import (retrieval_recall, retrieval_precision, retrieval_f1, retrieval_ndcg, retrieval_mrr,
-                                     retrieval_map)
+from autorag.evaluate.metric import retrieval_token_f1, retrieval_token_precision, retrieval_token_recall
 
 
-def evaluate_retrieval(retrieval_gt: List[List[List[str]]], metrics: List[str]):
-    def decorator_evaluate_retrieval(
+def evaluate_retrieval_contents(retrieval_gt: List[List[str]], metrics: List[str]):
+    def decorator_evaluate_retireval_contents(
             func: Callable[[Any], Tuple[List[List[str]], List[List[str]], List[List[float]]]]):
         """
-        Decorator for evaluating retrieval results.
+        Decorator for evaluating retrieval contents.
         You can use this decorator to any method that returns (contents, scores, ids),
         which is the output of conventional retrieval modules.
 
         :param func: Must return (contents, scores, ids)
-        :return: wrapper function that returns pd.DataFrame, which is the evaluation result.
+        :return: pd.DataFrame, which is the evaluation result and function result.
         """
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs) -> pd.DataFrame:
             contents, pred_ids, scores = func(*args, **kwargs)
             metric_funcs = {
-                retrieval_recall.__name__: retrieval_recall,
-                retrieval_precision.__name__: retrieval_precision,
-                retrieval_f1.__name__: retrieval_f1,
-                retrieval_ndcg.__name__: retrieval_ndcg,
-                retrieval_mrr.__name__: retrieval_mrr,
-                retrieval_map.__name__: retrieval_map,
+                retrieval_token_recall.__name__: retrieval_token_recall,
+                retrieval_token_precision.__name__: retrieval_token_precision,
+                retrieval_token_f1.__name__: retrieval_token_f1,
             }
 
-            metric_scores = {}
+            metrics_scores = {}
             for metric in metrics:
                 if metric not in metric_funcs:
-                    warnings.warn(f"metric {metric} is not in supported metrics: {metric_funcs.keys()}"
-                                  f"{metric} will be ignored.")
+                    raise ValueError(f"metric {metric} is not in supported metrics: {metric_funcs.keys()}")
                 else:
                     metric_func = metric_funcs[metric]
-                    metric_scores[metric] = metric_func(retrieval_gt=retrieval_gt, pred_ids=pred_ids)
+                    metric_scores = metric_func(gt_contents=retrieval_gt, pred_contents=contents)
+                    metrics_scores[metric] = metric_scores
 
-            metric_result_df = pd.DataFrame(metric_scores)
+            metric_result_df = pd.DataFrame(metrics_scores)
             execution_result_df = pd.DataFrame({
                 'retrieved_contents': contents,
                 'retrieved_ids': pred_ids,
                 'retrieve_scores': scores,
             })
             result_df = pd.concat([execution_result_df, metric_result_df], axis=1)
             return result_df
 
         return wrapper
 
-    return decorator_evaluate_retrieval
+    return decorator_evaluate_retireval_contents
```

### Comparing `autorag-0.1.9/autorag/evaluate/util.py` & `autorag-0.2.0/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/evaluator.py` & `autorag-0.2.0/autorag/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import chromadb
 import pandas as pd
 import torch
 import yaml
 
 from autorag import embedding_models
 from autorag.node_line import run_node_line
+from autorag.nodes.retrieval.base import get_bm25_pkl_name
 from autorag.nodes.retrieval.bm25 import bm25_ingest
 from autorag.nodes.retrieval.vectordb import vectordb_ingest
 from autorag.schema import Node
 from autorag.schema.node import module_type_exists, extract_values_from_nodes
 from autorag.utils import cast_qa_dataset, cast_corpus_dataset, validate_qa_from_corpus_dataset
 from autorag.utils.util import load_summary_file, convert_string_to_tuple_in_dict, convert_env_in_dict, explode
 
@@ -100,21 +101,24 @@
 
         trial_summary_df.to_csv(os.path.join(self.project_dir, trial_name, 'summary.csv'), index=False)
 
     def __embed(self, node_lines: Dict[str, List[Node]]):
         if any(list(map(lambda nodes: module_type_exists(nodes, 'bm25'), node_lines.values()))):
             # ingest BM25 corpus
             logger.info('Embedding BM25 corpus...')
-            bm25_dir = os.path.join(self.project_dir, 'resources', 'bm25.pkl')
-            if not os.path.exists(os.path.dirname(bm25_dir)):
-                os.makedirs(os.path.dirname(bm25_dir))
-            if os.path.exists(bm25_dir):
-                logger.debug('BM25 corpus already exists.')
-            else:
-                bm25_ingest(bm25_dir, self.corpus_data)
+            bm25_tokenizer_list = list(chain.from_iterable(
+                map(lambda nodes: extract_values_from_nodes(nodes, 'bm25_tokenizer'), node_lines.values())))
+            if len(bm25_tokenizer_list) == 0:
+                bm25_tokenizer_list = ['porter_stemmer']
+            for bm25_tokenizer in bm25_tokenizer_list:
+                bm25_dir = os.path.join(self.project_dir, 'resources', get_bm25_pkl_name(bm25_tokenizer))
+                if not os.path.exists(os.path.dirname(bm25_dir)):
+                    os.makedirs(os.path.dirname(bm25_dir))
+                # ingest because bm25 supports update new corpus data
+                bm25_ingest(bm25_dir, self.corpus_data, bm25_tokenizer=bm25_tokenizer)
             logger.info('BM25 corpus embedding complete.')
         if any(list(map(lambda nodes: module_type_exists(nodes, 'vectordb'), node_lines.values()))):
             # load embedding_models in nodes
             embedding_models_list = list(chain.from_iterable(
                 map(lambda nodes: extract_values_from_nodes(nodes, 'embedding_model'), node_lines.values())))
 
             # duplicate check in embedding_models
```

### Comparing `autorag-0.1.9/autorag/node_line.py` & `autorag-0.2.0/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/generator/base.py` & `autorag-0.2.0/autorag/nodes/generator/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.2.0/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/generator/openai_llm.py` & `autorag-0.2.0/autorag/nodes/generator/openai_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from autorag.nodes.generator.base import generator_node
 from autorag.utils.util import process_batch
 
 logger = logging.getLogger("AutoRAG")
 
 MAX_TOKEN_DICT = {  # model name : token limit
+    'gpt-4o': 128_000,
+    'gpt-4o-2024-05-13': 128_000,
     'gpt-4-turbo': 128_000,
     'gpt-4-turbo-2024-04-09': 128_000,
     'gpt-4-turbo-preview': 128_000,
     'gpt-4-0125-preview': 128_000,
     'gpt-4-1106-preview': 128_000,
     'gpt-4-vision-preview': 128_000,
     'gpt-4-1106-vision-preview': 128_000,
```

### Comparing `autorag-0.1.9/autorag/nodes/generator/run.py` & `autorag-0.2.0/autorag/nodes/generator/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 from typing import Callable, List, Dict, Union
 
 import pandas as pd
 
 from autorag.evaluate import evaluate_generation
 from autorag.evaluate.util import cast_metrics
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average
+from autorag.strategy import measure_speed, filter_by_threshold, select_best
 
 
 def run_generator_node(modules: List[Callable],
                        module_params: List[Dict],
                        previous_result: pd.DataFrame,
                        node_line_dir: str,
                        strategies: Dict,
@@ -68,15 +68,16 @@
     })
 
     # filter by strategies
     if strategies.get('speed_threshold') is not None:
         results, filenames = filter_by_threshold(results, average_times, strategies['speed_threshold'], filenames)
     if strategies.get('token_threshold') is not None:
         results, filenames = filter_by_threshold(results, token_usages, strategies['token_threshold'], filenames)
-    selected_result, selected_filename = select_best_average(results, metric_names, filenames)
+    selected_result, selected_filename = select_best(results, metric_names, filenames,
+                                                     strategies.get('strategy', 'mean'))
     best_result = pd.concat([previous_result, selected_result], axis=1)
 
     # add 'is_best' column at summary file
     summary_df['is_best'] = summary_df['filename'] == selected_filename
 
     # save files
     summary_df.to_csv(os.path.join(node_dir, "summary.csv"), index=False)
```

### Comparing `autorag-0.1.9/autorag/nodes/generator/vllm.py` & `autorag-0.2.0/autorag/nodes/generator/vllm.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     generate_params = SamplingParams(**input_kwargs)
     results: List[RequestOutput] = vllm_model.generate(prompts, generate_params)
     generated_texts = list(map(lambda x: x.outputs[0].text, results))
     generated_token_ids = list(map(lambda x: x.outputs[0].token_ids, results))
     log_probs: List[SampleLogprobs] = list(map(lambda x: x.outputs[0].logprobs, results))
     generated_log_probs = list(map(lambda x: list(map(
-        lambda y: y[0][y[1]], zip(x[0], x[1])
+        lambda y: y[0][y[1]].logprob, zip(x[0], x[1])
     )), zip(log_probs, generated_token_ids)))
     destroy_vllm_instance(vllm_model)
     return generated_texts, generated_token_ids, generated_log_probs
 
 
 def make_vllm_instance(llm: str, input_args):
     from vllm import LLM
@@ -67,9 +67,10 @@
         from vllm.model_executor.parallel_utils.parallel_state import (
             destroy_model_parallel,
         )
 
         destroy_model_parallel()
         del vllm_instance
         torch.cuda.synchronize()
+        torch.cuda.empty_cache()
     else:
         del vllm_instance
```

### Comparing `autorag-0.1.9/autorag/nodes/passageaugmenter/base.py` & `autorag-0.2.0/autorag/nodes/passageaugmenter/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,14 @@
         ids = previous_result["retrieved_ids"].tolist()
 
         corpus_df = pd.read_parquet(os.path.join(data_dir, "corpus.parquet"))
         validate_corpus_dataset(corpus_df)
 
         # get top_k
         top_k = kwargs.pop("top_k")
-        assert top_k <= len(ids[0][0]), ("The number of top_k must be same or less than the number of retrieved "
-                                         "passages.")
 
         if func.__name__ == 'prev_next_augmenter':
             corpus_df = cast_corpus_dataset(corpus_df)
             slim_corpus_df = corpus_df[["doc_id", "metadata"]]
             slim_corpus_df['metadata'] = slim_corpus_df['metadata'].apply(filter_dict_keys, keys=['prev_id', 'next_id'])
 
             mode = kwargs.pop("mode", 'both')
```

### Comparing `autorag-0.1.9/autorag/nodes/passageaugmenter/prev_next_augmenter.py` & `autorag-0.2.0/autorag/nodes/passageaugmenter/prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passageaugmenter/run.py` & `autorag-0.2.0/autorag/nodes/passageaugmenter/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,43 @@
 import os
 import pathlib
 from typing import List, Callable, Dict
 
 import pandas as pd
 
 from autorag.nodes.retrieval.run import evaluate_retrieval_node
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average
+from autorag.strategy import measure_speed, filter_by_threshold, select_best
 
 logger = logging.getLogger("AutoRAG")
 
 
 def run_passage_augmenter_node(modules: List[Callable],
                                module_params: List[Dict],
                                previous_result: pd.DataFrame,
                                node_line_dir: str,
                                strategies: Dict,
                                ) -> pd.DataFrame:
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
-    retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
+    qa_df = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))
+    retrieval_gt = qa_df['retrieval_gt'].tolist()
     retrieval_gt = [[[str(uuid) for uuid in sub_array] if sub_array.size > 0 else [] for sub_array in inner_array]
                     for inner_array in retrieval_gt]
 
     results, execution_times = zip(*map(lambda task: measure_speed(
         task[0], project_dir=project_dir, previous_result=previous_result, **task[1]), zip(modules, module_params)))
     average_times = list(map(lambda x: x / len(results[0]), execution_times))
 
     # run metrics before filtering
     if strategies.get('metrics') is None:
         raise ValueError("You must at least one metrics for passage_augmenter evaluation.")
-    results = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, strategies.get('metrics')), results))
+    results = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, strategies.get('metrics'),
+                                                         qa_df['query'].tolist(),
+                                                         qa_df['generation_gt'].tolist()), results))
 
     # save results to folder
     save_dir = os.path.join(node_line_dir, "passage_augmenter")  # node name
     if not os.path.exists(save_dir):
         os.makedirs(save_dir)
     filepaths = list(map(lambda x: os.path.join(save_dir, f'{x}.parquet'), range(len(modules))))
     list(map(lambda x: x[0].to_parquet(x[1], index=False), zip(results, filepaths)))  # execute save to parquet
@@ -49,15 +52,16 @@
         **{f'passage_augmenter_{metric}': list(map(lambda result: result[metric].mean(), results)) for metric in
            strategies.get('metrics')},
     })
 
     # filter by strategies
     if strategies.get('speed_threshold') is not None:
         results, filenames = filter_by_threshold(results, average_times, strategies['speed_threshold'], filenames)
-    selected_result, selected_filename = select_best_average(results, strategies.get('metrics'), filenames)
+    selected_result, selected_filename = select_best(results, strategies.get('metrics'), filenames,
+                                                     strategies.get('strategy', 'mean'))
     # change metric name columns to passage_augmenter_metric_name
     selected_result = selected_result.rename(columns={
         metric_name: f'passage_augmenter_{metric_name}' for metric_name in strategies['metrics']})
     # drop retrieval result columns in previous_result
     previous_result = previous_result.drop(columns=['retrieved_contents', 'retrieved_ids', 'retrieve_scores'])
     best_result = pd.concat([previous_result, selected_result], axis=1)
```

### Comparing `autorag-0.1.9/autorag/nodes/passagecompressor/base.py` & `autorag-0.2.0/autorag/nodes/passagecompressor/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagecompressor/refine.py` & `autorag-0.2.0/autorag/nodes/passagecompressor/refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagecompressor/run.py` & `autorag-0.2.0/autorag/nodes/passagecompressor/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import os.path
 import pathlib
 from typing import Callable, List, Dict
 
 import pandas as pd
 
 from autorag.evaluate.metric import retrieval_token_recall, retrieval_token_precision, retrieval_token_f1
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average
-from autorag.utils import validate_qa_dataset, validate_corpus_dataset
+from autorag.strategy import measure_speed, filter_by_threshold, select_best
 from autorag.utils.util import fetch_contents
 
 
 def run_passage_compressor_node(modules: List[Callable],
                                 module_params: List[Dict],
                                 previous_result: pd.DataFrame,
                                 node_line_dir: str,
@@ -36,24 +35,29 @@
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     data_dir = os.path.join(project_dir, "data")
     save_dir = os.path.join(node_line_dir, "passage_compressor")
     if not os.path.exists(save_dir):
         os.makedirs(save_dir)
 
+    # make retrieval contents gt
+    qa_data = pd.read_parquet(os.path.join(data_dir, "qa.parquet"))
+    corpus_data = pd.read_parquet(os.path.join(data_dir, "corpus.parquet"))
+    # check qa_data have retrieval_gt
+    assert all(len(x[0]) > 0 for x in qa_data['retrieval_gt'].tolist()), \
+        "Can't use passage compressor if you don't have retrieval gt values in QA dataset."
+
     # run modules
     results, execution_times = zip(*map(lambda task: measure_speed(
         task[0], project_dir=project_dir, previous_result=previous_result, **task[1]), zip(modules, module_params)))
     results = list(results)
     average_times = list(map(lambda x: x / len(results[0]), execution_times))
 
-    # make retrieval contents gt
-    qa_data = pd.read_parquet(os.path.join(data_dir, "qa.parquet"))
-    corpus_data = pd.read_parquet(os.path.join(data_dir, "corpus.parquet"))
-    retrieval_contents_gt = make_contents_gt(qa_data, corpus_data)
+    retrieval_contents_gt = list(map(lambda x: fetch_contents(corpus_data, x), qa_data['retrieval_gt'].tolist()))
+    retrieval_contents_gt = list(map(lambda x: list(itertools.chain.from_iterable(x)), retrieval_contents_gt))
 
     # run metrics before filtering
     if strategies.get('metrics') is None:
         raise ValueError("You must at least one metrics for retrieval contents evaluation."
                          "It can be 'retrieval_token_f1', 'retrieval_token_precision', 'retrieval_token_recall'.")
     results = list(map(lambda x: evaluate_passage_compressor_node(x, retrieval_contents_gt,
                                                                   strategies.get('metrics')), results))
@@ -72,15 +76,16 @@
         **{f'passage_compressor_{metric}': list(map(lambda result: result[metric].mean(), results)) for metric in
            strategies.get('metrics')},
     })
 
     # filter by strategies
     if strategies.get('speed_threshold') is not None:
         results, filenames = filter_by_threshold(results, average_times, strategies['speed_threshold'], filenames)
-    selected_result, selected_filename = select_best_average(results, strategies.get('metrics'), filenames)
+    selected_result, selected_filename = select_best(results, strategies.get('metrics'), filenames,
+                                                     strategies.get('strategy', 'mean'))
     new_retrieved_contents = selected_result['retrieved_contents']
     previous_result['retrieved_contents'] = new_retrieved_contents
     selected_result = selected_result.drop(columns=['retrieved_contents'])
     best_result = pd.concat([previous_result, selected_result], axis=1)
 
     # add 'is_best' column to summary file
     summary_df['is_best'] = summary_df['filename'] == selected_filename
@@ -110,14 +115,7 @@
         raise ValueError(f"metrics must be one of {metric_funcs.keys()}")
     metrics_scores = dict(map(lambda metric: (metric, metric_funcs[metric](
         gt_contents=retrieval_contents_gt,
         pred_contents=result_df['retrieved_contents'].tolist()
     )), metrics))
     result_df = pd.concat([result_df, pd.DataFrame(metrics_scores)], axis=1)
     return result_df
-
-
-def make_contents_gt(qa_data: pd.DataFrame, corpus_data: pd.DataFrame) -> List[List[str]]:
-    validate_qa_dataset(qa_data)
-    validate_corpus_dataset(corpus_data)
-    retrieval_gt_ids = qa_data['retrieval_gt'].apply(lambda x: list(itertools.chain.from_iterable(x))).tolist()
-    return fetch_contents(corpus_data, retrieval_gt_ids)
```

### Comparing `autorag-0.1.9/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.2.0/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagefilter/base.py` & `autorag-0.2.0/autorag/nodes/passagefilter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagefilter/percentile_cutoff.py` & `autorag-0.2.0/autorag/nodes/passagefilter/similarity_percentile_cutoff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Tuple, Optional
 
 import numpy as np
 import torch.cuda
 
 from autorag.evaluate.metric.util import calculate_cosine_similarity
 from autorag.nodes.passagefilter.base import passage_filter_node
-from autorag.nodes.passagefilter.threshold_cutoff import embedding_query_content
+from autorag.nodes.passagefilter.similarity_threshold_cutoff import embedding_query_content
 
 
 @passage_filter_node
 def similarity_percentile_cutoff(queries: List[str], contents_list: List[List[str]],
                                  scores_list: List[List[float]], ids_list: List[List[str]],
                                  percentile: float, embedding_model: Optional[str] = None,
                                  batch: int = 128,
```

### Comparing `autorag-0.1.9/autorag/nodes/passagefilter/recency.py` & `autorag-0.2.0/autorag/nodes/passagefilter/recency.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagefilter/run.py` & `autorag-0.2.0/autorag/nodes/passagefilter/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pathlib
 from typing import List, Callable, Dict
 
 import pandas as pd
 
 from autorag.nodes.retrieval.run import evaluate_retrieval_node
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average
+from autorag.strategy import measure_speed, filter_by_threshold, select_best
 
 
 def run_passage_filter_node(modules: List[Callable],
                             module_params: List[Dict],
                             previous_result: pd.DataFrame,
                             node_line_dir: str,
                             strategies: Dict) -> pd.DataFrame:
@@ -26,26 +26,29 @@
         In this node, we use 'retrieval_f1', 'retrieval_recall' and 'retrieval_precision'.
         You can skip evaluation when you use only one module and a module parameter.
     :return: The best result dataframe with previous result columns.
     """
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
-    retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
+    qa_df = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))
+    retrieval_gt = qa_df['retrieval_gt'].tolist()
     retrieval_gt = [[[str(uuid) for uuid in sub_array] if sub_array.size > 0 else [] for sub_array in inner_array]
                     for inner_array in retrieval_gt]
 
     results, execution_times = zip(*map(lambda task: measure_speed(
         task[0], project_dir=project_dir, previous_result=previous_result, **task[1]), zip(modules, module_params)))
     average_times = list(map(lambda x: x / len(results[0]), execution_times))
 
     # run metrics before filtering
     if strategies.get('metrics') is None:
         raise ValueError("You must at least one metrics for passage_filter evaluation.")
-    results = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, strategies.get('metrics')), results))
+    results = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, strategies.get('metrics'),
+                                                         qa_df['query'].tolist(),
+                                                         qa_df['generation_gt'].tolist()), results))
 
     # save results to folder
     save_dir = os.path.join(node_line_dir, "passage_filter")  # node name
     if not os.path.exists(save_dir):
         os.makedirs(save_dir)
     filepaths = list(map(lambda x: os.path.join(save_dir, f'{x}.parquet'), range(len(modules))))
     list(map(lambda x: x[0].to_parquet(x[1], index=False), zip(results, filepaths)))  # execute save to parquet
@@ -59,15 +62,16 @@
         **{f'passage_filter_{metric}': list(map(lambda result: result[metric].mean(), results)) for metric in
            strategies.get('metrics')},
     })
 
     # filter by strategies
     if strategies.get('speed_threshold') is not None:
         results, filenames = filter_by_threshold(results, average_times, strategies['speed_threshold'], filenames)
-    selected_result, selected_filename = select_best_average(results, strategies.get('metrics'), filenames)
+    selected_result, selected_filename = select_best(results, strategies.get('metrics'), filenames,
+                                                     strategies.get('strategy', 'mean'))
     selected_result = selected_result.rename(columns={
         metric_name: f'passage_filter_{metric_name}' for metric_name in strategies['metrics']})
     previous_result = previous_result.drop(columns=['retrieved_contents', 'retrieved_ids', 'retrieve_scores'])
     best_result = pd.concat([previous_result, selected_result], axis=1)
 
     # add 'is_best' column to summary file
     summary_df['is_best'] = summary_df['filename'] == selected_filename
```

### Comparing `autorag-0.1.9/autorag/nodes/passagefilter/threshold_cutoff.py` & `autorag-0.2.0/autorag/nodes/passagefilter/similarity_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/base.py` & `autorag-0.2.0/autorag/nodes/passagereranker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/cohere.py` & `autorag-0.2.0/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/colbert.py` & `autorag-0.2.0/autorag/nodes/passagereranker/colbert.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,16 +65,17 @@
                                 model, tokenizer, batch_size: int) -> List[np.array]:
 
     encoding = tokenizer(input_strings, return_tensors="pt", padding=True, truncation=True,
                          max_length=model.config.max_position_embeddings)
 
     input_batches = slice_tokenizer_result(encoding, batch_size)
     result_embedding = []
-    for encoding_batch in tqdm(input_batches):
-        result_embedding.append(model(**encoding_batch).last_hidden_state)
+    with torch.no_grad():
+        for encoding_batch in tqdm(input_batches):
+            result_embedding.append(model(**encoding_batch).last_hidden_state)
     total_tensor = torch.cat(result_embedding, dim=0)  # shape [batch_size, token_length, embedding_dim]
     tensor_results = list(total_tensor.chunk(total_tensor.size()[0]))
 
     if torch.cuda.is_available():
         return list(map(lambda x: x.detach().cpu().numpy(), tensor_results))
     else:
         return list(map(lambda x: x.detach().numpy(), tensor_results))
@@ -104,14 +105,16 @@
     device = "cuda" if torch.cuda.is_available() else "cpu"
     tensor_list = list(map(lambda x: x.to(device), tensor_list))
 
     return tensor_list
 
 
 def get_colbert_score(query_embedding: np.array, content_embedding: np.array) -> float:
-    query_tensor = torch.tensor(query_embedding)
-    content_tensor = torch.tensor(content_embedding)
-    sim_matrix = torch.nn.functional.cosine_similarity(
-        query_tensor.unsqueeze(2), content_tensor.unsqueeze(1), dim=-1
+    if query_embedding.ndim == 3 and content_embedding.ndim == 3:
+        query_embedding = query_embedding.reshape(-1, query_embedding.shape[-1])
+        content_embedding = content_embedding.reshape(-1, content_embedding.shape[-1])
+
+    sim_matrix = np.dot(query_embedding, content_embedding.T) / (
+            np.linalg.norm(query_embedding, axis=1)[:, np.newaxis] * np.linalg.norm(content_embedding, axis=1)
     )
-    max_sim_scores, _ = torch.max(sim_matrix, dim=2)
-    return float(torch.mean(max_sim_scores, dim=1))
+    max_sim_scores = np.max(sim_matrix, axis=1)
+    return float(np.mean(max_sim_scores))
```

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.2.0/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/flag_embedding_llm.py` & `autorag-0.2.0/autorag/nodes/passagereranker/flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/jina.py` & `autorag-0.2.0/autorag/nodes/passagereranker/jina.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.2.0/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/monot5.py` & `autorag-0.2.0/autorag/nodes/passagereranker/monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.2.0/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.2.0/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/run.py` & `autorag-0.2.0/autorag/nodes/passagereranker/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pathlib
 from typing import List, Callable, Dict
 
 import pandas as pd
 
 from autorag.nodes.retrieval.run import evaluate_retrieval_node
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average
+from autorag.strategy import measure_speed, filter_by_threshold, select_best
 
 logger = logging.getLogger("AutoRAG")
 
 
 def run_passage_reranker_node(modules: List[Callable],
                               module_params: List[Dict],
                               previous_result: pd.DataFrame,
@@ -30,26 +30,29 @@
         In this node, we use 'retrieval_f1', 'retrieval_recall' and 'retrieval_precision'.
         You can skip evaluation when you use only one module and a module parameter.
     :return: The best result dataframe with previous result columns.
     """
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
-    retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
+    qa_df = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))
+    retrieval_gt = qa_df['retrieval_gt'].tolist()
     retrieval_gt = [[[str(uuid) for uuid in sub_array] if sub_array.size > 0 else [] for sub_array in inner_array]
                     for inner_array in retrieval_gt]
 
     results, execution_times = zip(*map(lambda task: measure_speed(
         task[0], project_dir=project_dir, previous_result=previous_result, **task[1]), zip(modules, module_params)))
     average_times = list(map(lambda x: x / len(results[0]), execution_times))
 
     # run metrics before filtering
     if strategies.get('metrics') is None:
         raise ValueError("You must at least one metrics for passage_reranker evaluation.")
-    results = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, strategies.get('metrics')), results))
+    results = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, strategies.get('metrics'),
+                                                         qa_df['query'].tolist(),
+                                                         qa_df['generation_gt'].tolist()), results))
 
     # save results to folder
     save_dir = os.path.join(node_line_dir, "passage_reranker")  # node name
     if not os.path.exists(save_dir):
         os.makedirs(save_dir)
     filepaths = list(map(lambda x: os.path.join(save_dir, f'{x}.parquet'), range(len(modules))))
     list(map(lambda x: x[0].to_parquet(x[1], index=False), zip(results, filepaths)))  # execute save to parquet
@@ -63,15 +66,16 @@
         **{f'passage_reranker_{metric}': list(map(lambda result: result[metric].mean(), results)) for metric in
            strategies.get('metrics')},
     })
 
     # filter by strategies
     if strategies.get('speed_threshold') is not None:
         results, filenames = filter_by_threshold(results, average_times, strategies['speed_threshold'], filenames)
-    selected_result, selected_filename = select_best_average(results, strategies.get('metrics'), filenames)
+    selected_result, selected_filename = select_best(results, strategies.get('metrics'), filenames,
+                                                     strategies.get('strategy', 'mean'))
     # change metric name columns to passage_reranker_metric_name
     selected_result = selected_result.rename(columns={
         metric_name: f'passage_reranker_{metric_name}' for metric_name in strategies['metrics']})
     # drop retrieval result columns in previous_result
     previous_result = previous_result.drop(columns=['retrieved_contents', 'retrieved_ids', 'retrieve_scores'])
     best_result = pd.concat([previous_result, selected_result], axis=1)
```

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.2.0/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.2.0/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/tart/tart.py` & `autorag-0.2.0/autorag/nodes/passagereranker/tart/tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.2.0/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/time_reranker.py` & `autorag-0.2.0/autorag/nodes/passagereranker/time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/passagereranker/upr.py` & `autorag-0.2.0/autorag/nodes/passagereranker/upr.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,17 +96,18 @@
                                               pad_to_multiple_of=8,
                                               truncation=True,
                                               return_tensors='pt')
 
         query_input_ids = torch.repeat_interleave(query_token['input_ids'], len(contents),
                                                   dim=0).to(self.device)
 
-        logits = self.model(input_ids=prompt_token_outputs['input_ids'].to(self.device),
-                            attention_mask=prompt_token_outputs['attention_mask'].to(self.device),
-                            labels=query_input_ids).logits
+        with torch.no_grad():
+            logits = self.model(input_ids=prompt_token_outputs['input_ids'].to(self.device),
+                                attention_mask=prompt_token_outputs['attention_mask'].to(self.device),
+                                labels=query_input_ids).logits
         log_softmax = torch.nn.functional.log_softmax(logits, dim=-1)
         nll = -log_softmax.gather(2, query_input_ids.unsqueeze(2)).squeeze(2)
         avg_nll = torch.sum(nll, dim=1)
         return {"output": avg_nll.tolist()}
 
     def __del__(self):
         del self.model
```

### Comparing `autorag-0.1.9/autorag/nodes/promptmaker/base.py` & `autorag-0.2.0/autorag/nodes/promptmaker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/promptmaker/fstring.py` & `autorag-0.2.0/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.2.0/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/promptmaker/run.py` & `autorag-0.2.0/autorag/nodes/promptmaker/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from typing import List, Callable, Dict, Optional, Union
 
 import pandas as pd
 import tokenlog
 
 from autorag.evaluate import evaluate_generation
 from autorag.evaluate.util import cast_metrics
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average
+from autorag.strategy import measure_speed, filter_by_threshold, select_best
 from autorag.support import get_support_modules
 from autorag.utils import validate_qa_dataset
-from autorag.utils.util import make_combinations, explode
+from autorag.utils.util import make_combinations, explode, split_dataframe
 
 
 def run_prompt_maker_node(modules: List[Callable],
                           module_params: List[Dict],
                           previous_result: pd.DataFrame,
                           node_line_dir: str,
                           strategies: Dict,
@@ -102,27 +102,33 @@
 
         # get generation_gt
         qa_data = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))
         validate_qa_dataset(qa_data)
         generation_gt = qa_data['generation_gt'].tolist()
         generation_gt = list(map(lambda x: x.tolist(), generation_gt))
 
-        # run evaluations
-        evaluation_results = list(map(lambda result: evaluate_one_prompt_maker_node(
-            generator_callables, generator_params, result['prompts'].tolist(),
-            generation_gt, general_strategy['metrics'], project_dir), results))
+        all_prompts = []
+        for result in results:
+            all_prompts.extend(result['prompts'].tolist())
+
+        evaluation_result_all = evaluate_one_prompt_maker_node(all_prompts, generator_callables, generator_params,
+                                                               generation_gt * len(results),
+                                                               general_strategy['metrics'], project_dir,
+                                                               strategy_name=strategies.get('strategy', 'mean'))
+        evaluation_results = split_dataframe(evaluation_result_all, chunk_size=len(results[0]))
 
         evaluation_df = pd.DataFrame({
             'filename': filenames,
             **{f'prompt_maker_{metric_name}': list(map(lambda x: x[metric_name].mean(), evaluation_results))
                for metric_name in metric_names}
         })
         summary_df = pd.merge(on='filename', left=summary_df, right=evaluation_df, how='left')
 
-        best_result, best_filename = select_best_average(evaluation_results, metric_names, filenames)
+        best_result, best_filename = select_best(evaluation_results, metric_names, filenames,
+                                                 strategies.get('strategy', 'mean'))
         # change metric name columns to prompt_maker_metric_name
         best_result = best_result.rename(columns={
             metric_name: f'prompt_maker_{metric_name}' for metric_name in metric_names})
         best_result = best_result.drop(columns=['generated_texts'])
     else:
         best_result, best_filename = results[0], filenames[0]
 
@@ -151,27 +157,28 @@
     modules = list(map(lambda module_dict: get_support_modules(module_dict.pop('module_type')),
                        generator_module_list))
     param_combinations = list(map(lambda module_dict: make_combinations({**module_dict, **node_params}),
                                   generator_module_list))
     return explode(modules, param_combinations)
 
 
-def evaluate_one_prompt_maker_node(generator_funcs: List[Callable],
+def evaluate_one_prompt_maker_node(prompts: List[str],
+                                   generator_funcs: List[Callable],
                                    generator_params: List[Dict],
-                                   prompts: List[str],
                                    generation_gt: List[List[str]],
                                    metrics: Union[List[str], List[Dict]],
-                                   project_dir) -> pd.DataFrame:
+                                   project_dir,
+                                   strategy_name: str) -> pd.DataFrame:
     input_df = pd.DataFrame({'prompts': prompts})
     generator_results = list(map(lambda x: x[0](project_dir=project_dir, previous_result=input_df, **x[1]),
                                  zip(generator_funcs, generator_params)))
     evaluation_results = list(map(lambda x: evaluate_generator_result(x[0], generation_gt, metrics),
                                   zip(generator_results, generator_funcs)))
     metric_names = list(map(lambda x: x['metric_name'], metrics)) if isinstance(metrics[0], dict) else metrics
-    best_result, _ = select_best_average(evaluation_results, metric_names)
+    best_result, _ = select_best(evaluation_results, metric_names, strategy_name=strategy_name)
     best_result = pd.concat([input_df, best_result], axis=1)
     return best_result  # it has 'generated_texts' column
 
 
 def evaluate_generator_result(result_df: pd.DataFrame,
                               generation_gt: List[List[str]],
                               metrics: Union[List[str], List[Dict]]) -> pd.DataFrame:
```

### Comparing `autorag-0.1.9/autorag/nodes/queryexpansion/base.py` & `autorag-0.2.0/autorag/nodes/queryexpansion/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.2.0/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.2.0/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/queryexpansion/run.py` & `autorag-0.2.0/autorag/nodes/queryexpansion/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 import os
 import pathlib
-from typing import List, Callable, Dict, Optional
 from copy import deepcopy
+from typing import List, Callable, Dict, Optional
 
 import pandas as pd
 
 from autorag.nodes.retrieval.run import evaluate_retrieval_node
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average
-from autorag.utils.util import make_combinations, explode
+from autorag.strategy import measure_speed, filter_by_threshold, select_best
 from autorag.support import get_support_modules
+from autorag.utils.util import make_combinations, explode
 
 logger = logging.getLogger("AutoRAG")
 
 
 def run_query_expansion_node(modules: List[Callable],
                              module_params: List[Dict],
                              previous_result: pd.DataFrame,
@@ -89,24 +89,25 @@
 
         # get retrieval_gt
         retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
 
         # run evaluation
         evaluation_results = list(map(lambda result: evaluate_one_query_expansion_node(
             retrieval_callables, retrieval_params, result['queries'].tolist(), retrieval_gt,
-            general_strategy['metrics'], project_dir, previous_result), results))
+            general_strategy['metrics'], project_dir, previous_result, strategies.get('strategy', 'mean')), results))
 
         evaluation_df = pd.DataFrame({
             'filename': filenames,
             **{f'query_expansion_{metric_name}': list(map(lambda x: x[metric_name].mean(), evaluation_results))
                for metric_name in general_strategy['metrics']}
         })
         summary_df = pd.merge(on='filename', left=summary_df, right=evaluation_df, how='left')
 
-        best_result, best_filename = select_best_average(evaluation_results, general_strategy['metrics'], filenames)
+        best_result, best_filename = select_best(evaluation_results, general_strategy['metrics'], filenames,
+                                                 strategies.get('strategy', 'mean'))
         # change metric name columns to query_expansion_metric_name
         best_result = best_result.rename(columns={
             metric_name: f'query_expansion_{metric_name}' for metric_name in strategies['metrics']})
         best_result = best_result.drop(columns=['retrieved_contents', 'retrieved_ids', 'retrieve_scores'])
     else:
         best_result, best_filename = results[0], filenames[0]
         best_result = pd.concat([previous_result, best_result], axis=1)
@@ -123,21 +124,24 @@
 
 def evaluate_one_query_expansion_node(retrieval_funcs: List[Callable],
                                       retrieval_params: List[Dict],
                                       expanded_queries: List[List[str]],
                                       retrieval_gt: List[List[str]],
                                       metrics: List[str],
                                       project_dir,
-                                      previous_result: pd.DataFrame) -> pd.DataFrame:
+                                      previous_result: pd.DataFrame,
+                                      strategy_name: str) -> pd.DataFrame:
     previous_result['queries'] = expanded_queries
     retrieval_results = list(map(lambda x: x[0](project_dir=project_dir, previous_result=previous_result, **x[1]),
                                  zip(retrieval_funcs, retrieval_params)))
-    evaluation_results = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, metrics),
+    evaluation_results = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, metrics,
+                                                                    previous_result['query'].tolist(),
+                                                                    previous_result['generation_gt'].tolist()),
                                   retrieval_results))
-    best_result, _ = select_best_average(evaluation_results, metrics)
+    best_result, _ = select_best(evaluation_results, metrics, strategy_name=strategy_name)
     best_result = pd.concat([previous_result, best_result], axis=1)
     return best_result
 
 
 def make_retrieval_callable_params(strategy_dict: Dict):
     """
         strategy_dict looks like this:
```

### Comparing `autorag-0.1.9/autorag/nodes/retrieval/base.py` & `autorag-0.2.0/autorag/nodes/retrieval/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,18 @@
         logger.info(f"Running retrieval node - {func.__name__} module...")
         validate_qa_dataset(previous_result)
         resources_dir = os.path.join(project_dir, "resources")
         data_dir = os.path.join(project_dir, "data")
 
         if func.__name__ == "bm25":
             # check if bm25_path and file exists
-            bm25_path = os.path.join(resources_dir, 'bm25.pkl')
+            bm25_tokenizer = kwargs.get('bm25_tokenizer', None)
+            if bm25_tokenizer is None:
+                bm25_tokenizer = "porter_stemmer"
+            bm25_path = os.path.join(resources_dir, get_bm25_pkl_name(bm25_tokenizer))
             assert bm25_path is not None, "bm25_path must be specified for using bm25 retrieval."
             assert os.path.exists(bm25_path), f"bm25_path {bm25_path} does not exist. Please ingest first."
         elif func.__name__ == "vectordb":
             # check if chroma_path and file exist
             chroma_path = os.path.join(resources_dir, 'chroma')
             embedding_model_str = kwargs.pop("embedding_model")
             assert chroma_path is not None, "chroma_path must be specified for using vectordb retrieval."
@@ -138,10 +141,10 @@
         else:
             new_ids.extend(ids[i][:avg_len])
             new_scores.extend(scores[i][:avg_len])
 
     return new_ids, new_scores
 
 
-def run_retrieval_modules(project_dir: str, previous_result: pd.DataFrame,
-                          module_name: str, module_params: Dict) -> pd.DataFrame:
-    return
+def get_bm25_pkl_name(bm25_tokenizer: str):
+    bm25_tokenizer = bm25_tokenizer.replace('/', '')
+    return f'bm25_{bm25_tokenizer}.pkl'
```

### Comparing `autorag-0.1.9/autorag/nodes/retrieval/bm25.py` & `autorag-0.2.0/autorag/nodes/retrieval/bm25.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,62 @@
 import asyncio
 import os
 import pickle
-from typing import List, Dict, Tuple
+import re
+from typing import List, Dict, Tuple, Callable, Union, Iterable
 
 import numpy as np
 import pandas as pd
+from kiwipiepy import Kiwi, Token
+from llama_index.core.indices.keyword_table.utils import simple_extract_keywords
+from nltk import PorterStemmer
 from rank_bm25 import BM25Okapi
-from transformers import AutoTokenizer
+from transformers import AutoTokenizer, PreTrainedTokenizerBase
 
 from autorag.nodes.retrieval.base import retrieval_node, evenly_distribute_passages
 from autorag.utils import validate_corpus_dataset
+from autorag.utils.util import normalize_string
+
+
+def tokenize_ko_kiwi(texts: List[str]) -> List[List[str]]:
+    texts = list(map(lambda x: x.strip().lower(), texts))
+    kiwi = Kiwi()
+    tokenized_list: Iterable[List[Token]] = kiwi.tokenize(texts)
+    return [list(map(lambda x: x.form, token_list)) for token_list in tokenized_list]
+
+
+def tokenize_porter_stemmer(texts: List[str]) -> List[List[str]]:
+    def tokenize_remove_stopword(text: str, stemmer) -> List[str]:
+        text = text.lower()
+        words = list(simple_extract_keywords(text))
+        return [stemmer.stem(word) for word in words]
+
+    stemmer = PorterStemmer()
+    tokenized_list: List[List[str]] = list(map(lambda x: tokenize_remove_stopword(x, stemmer), texts))
+    return tokenized_list
+
+
+def tokenize_space(texts: List[str]) -> List[List[str]]:
+    def tokenize_space_text(text: str) -> List[str]:
+        text = normalize_string(text)
+        return re.split(r'\s+', text.strip())
+
+    return list(map(tokenize_space_text, texts))
+
+
+BM25_TOKENIZER = {
+    'porter_stemmer': tokenize_porter_stemmer,
+    'ko_kiwi': tokenize_ko_kiwi,
+    'space': tokenize_space,
+}
 
 
 @retrieval_node
-def bm25(queries: List[List[str]], top_k: int, bm25_corpus: Dict) -> Tuple[List[List[str
-]], List[List[float]]]:
+def bm25(queries: List[List[str]], top_k: int, bm25_corpus: Dict, bm25_tokenizer: str = 'porter_stemmer') -> \
+        Tuple[List[List[str]], List[List[float]]]:
     """
     BM25 retrieval function.
     You have to load a pickle file that is already ingested.
 
     :param queries: 2-d list of query strings.
         Each element of the list is a query strings of each row.
     :param top_k: The number of passages to be retrieved.
@@ -28,33 +66,40 @@
         .. Code:: python
 
             {
                 "tokens": [], # 2d list of tokens
                 "passage_id": [], # 2d list of passage_id.
             }
 
+    :param bm25_tokenizer: The tokenizer name that uses to the BM25.
+        It supports 'porter_stemmer', 'ko_kiwi', and huggingface `AutoTokenizer`.
+        You can pass huggingface tokenizer name.
+        Default is porter_stemmer.
     :return: The 2-d list contains a list of passage ids that retrieved from bm25 and 2-d list of its scores.
         It will be a length of queries. And each element has a length of top_k.
     """
     # check if bm25_corpus is valid
     assert ("tokens" and "passage_id" in list(bm25_corpus.keys())), \
         "bm25_corpus must contain tokens and passage_id. Please check you ingested bm25 corpus correctly."
-    tokenizer = AutoTokenizer.from_pretrained("gpt2", use_fast=False)
+    tokenizer = select_bm25_tokenizer(bm25_tokenizer)
+    assert bm25_corpus['tokenizer_name'] == bm25_tokenizer, \
+        (f"The bm25 corpus tokenizer is {bm25_corpus['tokenizer_name']}, but your input is {bm25_tokenizer}. "
+         f"You need to ingest again. Delete bm25 pkl file and re-ingest it.")
     bm25_instance = BM25Okapi(bm25_corpus["tokens"])
     # run async bm25_pure function
     tasks = [bm25_pure(input_queries, top_k, tokenizer, bm25_instance, bm25_corpus) for input_queries in queries]
     loop = asyncio.get_event_loop()
     results = loop.run_until_complete(asyncio.gather(*tasks))
     id_result = list(map(lambda x: x[0], results))
     score_result = list(map(lambda x: x[1], results))
     return id_result, score_result
 
 
-async def bm25_pure(queries: List[str], top_k: int, tokenizer, bm25_api: BM25Okapi, bm25_corpus: Dict) -> Tuple[
-        List[str], List[float]]:
+async def bm25_pure(queries: List[str], top_k: int, tokenizer, bm25_api: BM25Okapi, bm25_corpus: Dict) -> \
+        Tuple[List[str], List[float]]:
     """
     Async BM25 retrieval function.
     Its usage is for async retrieval of bm25 row by row.
 
     :param queries: A list of query strings.
     :param top_k: The number of passages to be retrieved.
     :param tokenizer: A tokenizer that will be used to tokenize queries.
@@ -67,15 +112,18 @@
             {
                 "tokens": [], # 2d list of tokens
                 "passage_id": [], # 2d list of passage_id. Type must be str.
             }
     :return: The tuple contains a list of passage ids that retrieved from bm25 and its scores.
     """
     # I don't make queries operation to async, because queries length might be small, so it will occur overhead.
-    tokenized_queries = tokenizer(queries).input_ids
+    if isinstance(tokenizer, PreTrainedTokenizerBase):
+        tokenized_queries = tokenizer(queries).input_ids
+    else:
+        tokenized_queries = tokenizer(queries)
     id_result = []
     score_result = []
     for query in tokenized_queries:
         scores = bm25_api.get_scores(query)
         sorted_scores = sorted(scores, reverse=True)
         top_n_index = np.argsort(scores)[::-1][:top_k]
         ids = [bm25_corpus['passage_id'][i] for i in top_n_index]
@@ -87,15 +135,15 @@
     # sort id_result and score_result by score
     result = [(_id, score) for score, _id in
               sorted(zip(score_result, id_result), key=lambda pair: pair[0], reverse=True)]
     id_result, score_result = zip(*result)
     return list(id_result), list(score_result)
 
 
-def bm25_ingest(corpus_path: str, corpus_data: pd.DataFrame):
+def bm25_ingest(corpus_path: str, corpus_data: pd.DataFrame, bm25_tokenizer: str = 'porter_stemmer'):
     if not corpus_path.endswith('.pkl'):
         raise ValueError(f"Corpus path {corpus_path} is not a pickle file.")
     validate_corpus_dataset(corpus_data)
     ids = corpus_data['doc_id'].tolist()
 
     # Initialize bm25_corpus
     bm25_corpus = pd.DataFrame()
@@ -107,29 +155,35 @@
             bm25_corpus = pd.DataFrame.from_dict(corpus)
         duplicated_passage_rows = bm25_corpus[bm25_corpus['passage_id'].isin(ids)]
         new_passage = corpus_data[~corpus_data['doc_id'].isin(duplicated_passage_rows['passage_id'])]
     else:
         new_passage = corpus_data
 
     if not new_passage.empty:
-        tokenizer = AutoTokenizer.from_pretrained('gpt2', use_fast=False)
-        results = new_passage.swifter.apply(lambda x: bm25_tokenize(x['contents'], x['doc_id'], tokenizer), axis=1)
-        tokenized_corpus, passage_ids = zip(*results)
-
+        tokenizer = select_bm25_tokenizer(bm25_tokenizer)
+        if isinstance(tokenizer, PreTrainedTokenizerBase):
+            tokenized_corpus = tokenizer(new_passage['contents'].tolist()).input_ids
+        else:
+            tokenized_corpus = tokenizer(new_passage['contents'].tolist())
         new_bm25_corpus = pd.DataFrame({
-            'tokens': list(tokenized_corpus),
-            'passage_id': list(passage_ids),
+            'tokens': tokenized_corpus,
+            'passage_id': new_passage['doc_id'].tolist(),
         })
 
         if not bm25_corpus.empty:
             bm25_corpus_updated = pd.concat([bm25_corpus, new_bm25_corpus], ignore_index=True)
             bm25_dict = bm25_corpus_updated.to_dict('list')
         else:
             bm25_dict = new_bm25_corpus.to_dict('list')
 
+        # add tokenizer name to bm25_dict
+        bm25_dict['tokenizer_name'] = bm25_tokenizer
+
         with open(corpus_path, 'wb') as w:
             pickle.dump(bm25_dict, w)
 
 
-def bm25_tokenize(queries: List[str], passage_id: str, tokenizer) -> Tuple[List[int], str]:
-    tokenized_queries = tokenizer(queries).input_ids
-    return tokenized_queries, passage_id
+def select_bm25_tokenizer(bm25_tokenizer: str) -> Callable[[str], List[Union[int, str]]]:
+    if bm25_tokenizer in list(BM25_TOKENIZER.keys()):
+        return BM25_TOKENIZER[bm25_tokenizer]
+
+    return AutoTokenizer.from_pretrained(bm25_tokenizer, use_fast=False)
```

### Comparing `autorag-0.1.9/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.2.0/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/retrieval/hybrid_dbsf.py` & `autorag-0.2.0/autorag/nodes/retrieval/hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.2.0/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/retrieval/hybrid_rsf.py` & `autorag-0.2.0/autorag/nodes/retrieval/hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/nodes/retrieval/run.py` & `autorag-0.2.0/autorag/nodes/retrieval/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pathlib
 from typing import List, Callable, Dict, Tuple
 
 import pandas as pd
 
 from autorag.evaluate import evaluate_retrieval
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average
+from autorag.strategy import measure_speed, filter_by_threshold, select_best
 from autorag.utils.util import load_summary_file
 
 logger = logging.getLogger("AutoRAG")
 
 
 def run_retrieval_node(modules: List[Callable],
                        module_params: List[Dict],
@@ -29,15 +29,16 @@
     :param strategies: Strategies for retrieval node.
     :return: The best result dataframe.
         It contains previous result columns and retrieval node's result columns.
     """
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
-    retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
+    qa_df = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))
+    retrieval_gt = qa_df['retrieval_gt'].tolist()
     retrieval_gt = [[[str(uuid) for uuid in sub_array] if sub_array.size > 0 else [] for sub_array in inner_array]
                     for inner_array in retrieval_gt]
 
     save_dir = os.path.join(node_line_dir, "retrieval")  # node name
     if not os.path.exists(save_dir):
         os.makedirs(save_dir)
 
@@ -46,15 +47,17 @@
             task[0], project_dir=project_dir, previous_result=previous_result, **task[1]),
                                            zip(input_modules, input_module_params)))
         average_times = list(map(lambda x: x / len(result[0]), execution_times))
 
         # run metrics before filtering
         if strategies.get('metrics') is None:
             raise ValueError("You must at least one metrics for retrieval evaluation.")
-        result = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, strategies.get('metrics')), result))
+        result = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, strategies.get('metrics'),
+                                                            qa_df['query'].tolist(),
+                                                            qa_df['generation_gt'].tolist()), result))
 
         # save results to folder
         filepaths = list(map(lambda x: os.path.join(save_dir, f'{x}.parquet'),
                              range(filename_start, filename_start + len(input_modules))))
         list(map(lambda x: x[0].to_parquet(x[1], index=False), zip(result, filepaths)))  # execute save to parquet
         filename_list = list(map(lambda x: os.path.basename(x), filepaths))
 
@@ -109,39 +112,43 @@
     results = non_hybrid_results + hybrid_results
     average_times = non_hybrid_times + hybrid_times
     filenames = summary['filename'].tolist()
 
     # filter by strategies
     if strategies.get('speed_threshold') is not None:
         results, filenames = filter_by_threshold(results, average_times, strategies['speed_threshold'], filenames)
-    selected_result, selected_filename = select_best_average(results, strategies.get('metrics'), filenames)
+    selected_result, selected_filename = select_best(results, strategies.get('metrics'), filenames,
+                                                     strategies.get('strategy', 'mean'))
     best_result = pd.concat([previous_result, selected_result], axis=1)
 
     # add summary.csv 'is_best' column
     summary['is_best'] = summary['filename'] == selected_filename
 
     # save the result files
     best_result.to_parquet(os.path.join(save_dir, f'best_{os.path.splitext(selected_filename)[0]}.parquet'),
                            index=False)
     summary.to_csv(os.path.join(save_dir, 'summary.csv'), index=False)
     return best_result
 
 
-def evaluate_retrieval_node(result_df: pd.DataFrame, retrieval_gt, metrics) -> pd.DataFrame:
+def evaluate_retrieval_node(result_df: pd.DataFrame, retrieval_gt, metrics,
+                            queries: List[str], generation_gt: List[List[str]]) -> pd.DataFrame:
     """
     Evaluate retrieval node from retrieval node result dataframe.
 
     :param result_df: The result dataframe from a retrieval node.
     :param retrieval_gt: Ground truth for retrieval from qa dataset.
     :param metrics: Metric list from input strategies.
+    :param queries: Query list from input strategies.
+    :param generation_gt: Ground truth for generation from qa dataset.
     :return: Return result_df with metrics columns.
         The columns will be 'retrieved_contents', 'retrieved_ids', 'retrieve_scores', and metric names.
     """
 
-    @evaluate_retrieval(retrieval_gt=retrieval_gt, metrics=metrics)
+    @evaluate_retrieval(retrieval_gt=retrieval_gt, metrics=metrics, queries=queries, generation_gt=generation_gt)
     def evaluate_this_module(df: pd.DataFrame):
         return df['retrieved_contents'].tolist(), df['retrieved_ids'].tolist(), df['retrieve_scores'].tolist()
 
     return evaluate_this_module(result_df)
 
 
 def select_result_for_hybrid(node_dir: str, target_modules: Tuple) -> List[str]:
```

### Comparing `autorag-0.1.9/autorag/nodes/retrieval/vectordb.py` & `autorag-0.2.0/autorag/nodes/retrieval/vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/schema/module.py` & `autorag-0.2.0/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/schema/node.py` & `autorag-0.2.0/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/autorag/support.py` & `autorag-0.2.0/autorag/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         'flag_embedding_llm_reranker': ('autorag.nodes.passagereranker', 'flag_embedding_llm_reranker'),
         'time_reranker': ('autorag.nodes.passagereranker', 'time_reranker'),
         # passage_filter
         'pass_passage_filter': ('autorag.nodes.passagefilter', 'pass_passage_filter'),
         'similarity_threshold_cutoff': ('autorag.nodes.passagefilter', 'similarity_threshold_cutoff'),
         'similarity_percentile_cutoff': ('autorag.nodes.passagefilter', 'similarity_percentile_cutoff'),
         'recency_filter': ('autorag.nodes.passagefilter', 'recency_filter'),
+        'threshold_cutoff': ('autorag.nodes.passagefilter', 'threshold_cutoff'),
+        'percentile_cutoff': ('autorag.nodes.passagefilter', 'percentile_cutoff'),
         # passage_compressor
         'tree_summarize': ('autorag.nodes.passagecompressor', 'tree_summarize'),
         'pass_compressor': ('autorag.nodes.passagecompressor', 'pass_compressor'),
         'refine': ('autorag.nodes.passagecompressor', 'refine'),
         # prompt_maker
         'fstring': ('autorag.nodes.promptmaker', 'fstring'),
         'long_context_reorder': ('autorag.nodes.promptmaker', 'long_context_reorder'),
```

### Comparing `autorag-0.1.9/autorag/utils/preprocess.py` & `autorag-0.2.0/autorag/utils/preprocess.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
 
+from autorag.utils.util import normalize_unicode
+
 
 def validate_qa_dataset(df: pd.DataFrame):
     columns = ['qid', 'query', 'retrieval_gt', 'generation_gt']
     assert set(columns).issubset(df.columns), f"df must have columns {columns}, but got {df.columns}"
 
 
 def validate_corpus_dataset(df: pd.DataFrame):
@@ -45,14 +47,16 @@
     validate_qa_dataset(df)
     assert df['qid'].apply(lambda x: isinstance(x, str)).sum() == len(df), \
         "qid must be string type."
     assert df['query'].apply(lambda x: isinstance(x, str)).sum() == len(df), \
         "query must be string type."
     df['retrieval_gt'] = df['retrieval_gt'].apply(cast_retrieval_gt)
     df['generation_gt'] = df['generation_gt'].apply(cast_generation_gt)
+    df['query'] = df['query'].apply(normalize_unicode)
+    df['generation_gt'] = df['generation_gt'].apply(lambda x: list(map(normalize_unicode, x)))
     return df
 
 
 def cast_corpus_dataset(df: pd.DataFrame):
     validate_corpus_dataset(df)
 
     def make_datetime_metadata(x):
@@ -76,14 +80,27 @@
             return {**x, id_type: None}
         else:
             return x
 
     df['metadata'] = df['metadata'].apply(lambda x: make_prev_next_id_metadata(x, 'prev_id'))
     df['metadata'] = df['metadata'].apply(lambda x: make_prev_next_id_metadata(x, 'next_id'))
 
+    df['contents'] = df['contents'].apply(normalize_unicode)
+
+    def normalize_unicode_metadata(metadata: dict):
+        result = {}
+        for key, value in metadata.items():
+            if isinstance(value, str):
+                result[key] = normalize_unicode(value)
+            else:
+                result[key] = value
+        return result
+
+    df['metadata'] = df['metadata'].apply(normalize_unicode_metadata)
+
     # check every metadata have a prev_id, next_id key
     assert all('prev_id' in metadata for metadata in df['metadata']), "Every metadata must have a prev_id key."
     assert all('next_id' in metadata for metadata in df['metadata']), "Every metadata must have a next_id key."
 
     return df
```

### Comparing `autorag-0.1.9/autorag/utils/util.py` & `autorag-0.2.0/autorag/utils/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import ast
 import asyncio
 import datetime
 import functools
+import glob
 import itertools
 import logging
 import os
 import re
 import string
+import unicodedata
 from copy import deepcopy
 from typing import List, Callable, Dict, Optional, Any, Collection
 
 import pandas as pd
 import tiktoken
 
 logger = logging.getLogger("AutoRAG")
@@ -351,7 +353,80 @@
     result = {}
     for key in keys:
         if key in dict_:
             result[key] = dict_[key]
         else:
             raise KeyError(f"Key '{key}' not found in dictionary.")
     return result
+
+
+def split_dataframe(df, chunk_size):
+    num_chunks = len(df) // chunk_size + 1 if len(df) % chunk_size != 0 else len(df) // chunk_size
+    return list(map(lambda x: df[x * chunk_size:(x + 1) * chunk_size], range(num_chunks)))
+
+
+def find_trial_dir(project_dir: str) -> List[str]:
+    # Pattern to match directories named with numbers
+    pattern = os.path.join(project_dir, '[0-9]*')
+    all_entries = glob.glob(pattern)
+
+    # Filter out only directories
+    trial_dirs = [entry for entry in all_entries if os.path.isdir(entry) and entry.split(os.sep)[-1].isdigit()]
+
+    return trial_dirs
+
+
+def find_node_summary_files(trial_dir: str) -> List[str]:
+    # Find all summary.csv files recursively
+    all_summary_files = glob.glob(os.path.join(trial_dir, '**', 'summary.csv'), recursive=True)
+
+    # Filter out files that are at a lower directory level
+    filtered_files = [f for f in all_summary_files if f.count(os.sep) > trial_dir.count(os.sep) + 2]
+
+    return filtered_files
+
+
+def normalize_unicode(text: str) -> str:
+    return unicodedata.normalize('NFC', text)
+
+
+def dict_to_markdown(d, level=1):
+    """
+    Convert a dictionary to a Markdown formatted string.
+
+    :param d: Dictionary to convert
+    :param level: Current level of heading (used for nested dictionaries)
+    :return: Markdown formatted string
+    """
+    markdown = ""
+    for key, value in d.items():
+        if isinstance(value, dict):
+            markdown += f"{'#' * level} {key}\n"
+            markdown += dict_to_markdown(value, level + 1)
+        elif isinstance(value, list):
+            markdown += f"{'#' * level} {key}\n"
+            for item in value:
+                if isinstance(item, dict):
+                    markdown += dict_to_markdown(item, level + 1)
+                else:
+                    markdown += f"- {item}\n"
+        else:
+            markdown += f"{'#' * level} {key}\n{value}\n"
+    return markdown
+
+
+def dict_to_markdown_table(data, key_column_name: str, value_column_name: str):
+    # Check if the input is a dictionary
+    if not isinstance(data, dict):
+        raise ValueError("Input must be a dictionary")
+
+    # Create the header of the table
+    header = f"| {key_column_name} | {value_column_name} |\n| :---: | :-----: |\n"
+
+    # Create the rows of the table
+    rows = ""
+    for key, value in data.items():
+        rows += f"| {key} | {value} |\n"
+
+    # Combine header and rows
+    markdown_table = header + rows
+    return markdown_table
```

### Comparing `autorag-0.1.9/autorag/web.py` & `autorag-0.2.0/autorag/web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/Makefile` & `autorag-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/make.bat` & `autorag-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/data_creation.png` & `autorag-0.2.0/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/data_folder.png` & `autorag-0.2.0/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/node_folder.png` & `autorag-0.2.0/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/node_line_folder.png` & `autorag-0.2.0/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/node_line_summary.png` & `autorag-0.2.0/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/node_lines.png` & `autorag-0.2.0/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/node_summary.png` & `autorag-0.2.0/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/project_folder_example.png` & `autorag-0.2.0/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/project_folders.png` & `autorag-0.2.0/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/resources_folder.png` & `autorag-0.2.0/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.2.0/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.2.0/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/roadmap/cycle.png` & `autorag-0.2.0/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/roadmap/merger.png` & `autorag-0.2.0/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.2.0/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/roadmap/policy.png` & `autorag-0.2.0/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.2.0/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/trial_folder.png` & `autorag-0.2.0/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/trial_json.png` & `autorag-0.2.0/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/trial_summary.png` & `autorag-0.2.0/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/_static/web_interface.png` & `autorag-0.2.0/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.nodes.passageaugmenter.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.nodes.passageaugmenter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagefilter.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,133 @@
-autorag.nodes.passagefilter package
-===================================
+autorag.nodes.passagereranker package
+=====================================
+
+Subpackages
+-----------
+
+.. toctree::
+   :maxdepth: 4
+
+   autorag.nodes.passagereranker.tart
 
 Submodules
 ----------
 
-autorag.nodes.passagefilter.base module
----------------------------------------
+autorag.nodes.passagereranker.base module
+-----------------------------------------
 
-.. automodule:: autorag.nodes.passagefilter.base
+.. automodule:: autorag.nodes.passagereranker.base
    :members:
    :undoc-members:
    :show-inheritance:
 
-autorag.nodes.passagefilter.pass\_passage\_filter module
---------------------------------------------------------
+autorag.nodes.passagereranker.cohere module
+-------------------------------------------
 
-.. automodule:: autorag.nodes.passagefilter.pass_passage_filter
+.. automodule:: autorag.nodes.passagereranker.cohere
    :members:
    :undoc-members:
    :show-inheritance:
 
-autorag.nodes.passagefilter.percentile\_cutoff module
------------------------------------------------------
+autorag.nodes.passagereranker.colbert module
+--------------------------------------------
 
-.. automodule:: autorag.nodes.passagefilter.percentile_cutoff
+.. automodule:: autorag.nodes.passagereranker.colbert
    :members:
    :undoc-members:
    :show-inheritance:
 
-autorag.nodes.passagefilter.recency module
-------------------------------------------
+autorag.nodes.passagereranker.flag\_embedding module
+----------------------------------------------------
 
-.. automodule:: autorag.nodes.passagefilter.recency
+.. automodule:: autorag.nodes.passagereranker.flag_embedding
    :members:
    :undoc-members:
    :show-inheritance:
 
-autorag.nodes.passagefilter.run module
---------------------------------------
+autorag.nodes.passagereranker.flag\_embedding\_llm module
+---------------------------------------------------------
 
-.. automodule:: autorag.nodes.passagefilter.run
+.. automodule:: autorag.nodes.passagereranker.flag_embedding_llm
    :members:
    :undoc-members:
    :show-inheritance:
 
-autorag.nodes.passagefilter.threshold\_cutoff module
-----------------------------------------------------
+autorag.nodes.passagereranker.jina module
+-----------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.jina
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.koreranker module
+-----------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.koreranker
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.monot5 module
+-------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.monot5
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.pass\_reranker module
+---------------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.pass_reranker
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.rankgpt module
+--------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.rankgpt
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.run module
+----------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.run
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.sentence\_transformer module
+----------------------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.sentence_transformer
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.time\_reranker module
+---------------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.time_reranker
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.upr module
+----------------------------------------
 
-.. automodule:: autorag.nodes.passagefilter.threshold_cutoff
+.. automodule:: autorag.nodes.passagereranker.upr
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
 
-.. automodule:: autorag.nodes.passagefilter
+.. automodule:: autorag.nodes.passagereranker
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/api_spec/autorag.rst` & `autorag-0.2.0/docs/source/api_spec/autorag.rst`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 ------------------
 
 .. automodule:: autorag.cli
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.dashboard module
+------------------------
+
+.. automodule:: autorag.dashboard
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.deploy module
 ---------------------
 
 .. automodule:: autorag.deploy
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.9/docs/source/conf.py` & `autorag-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/data_creation/data_format.md` & `autorag-0.2.0/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/data_creation/ragas.md` & `autorag-0.2.0/docs/source/data_creation/ragas.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/data_creation/tutorial.md` & `autorag-0.2.0/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/deploy/api_endpoint.md` & `autorag-0.2.0/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/deploy/web.md` & `autorag-0.2.0/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/index.rst` & `autorag-0.2.0/docs/source/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -85,28 +85,41 @@
    :maxdepth: 2
    :caption: Optimization
    :hidden:
 
    optimization/optimization.md
    optimization/folder_structure.md
    optimization/custom_config.md
+   optimization/strategies.md
+
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Evaluation Metrics
+   :hidden:
+
+   evaluate_metrics/retrieval.md
+   evaluate_metrics/retrieval_contents.md
+   evaluate_metrics/generation.md
+
 
 .. toctree::
    :maxdepth: 3
    :caption: Nodes & Modules
    :hidden:
 
    nodes/index.md
    nodes/query_expansion/query_expansion.md
    nodes/retrieval/retrieval.md
+   nodes/passage_augmenter/passage_augmenter.md
    nodes/passage_reranker/passage_reranker.md
+   nodes/passage_filter/passage_filter.md
    nodes/passage_compressor/passage_compressor.md
    nodes/prompt_maker/prompt_maker.md
    nodes/generator/generator.md
-   nodes/passage_filter/passage_filter.md
 
 .. toctree::
    :maxdepth: 2
    :caption: Deploy
    :hidden:
 
    deploy/api_endpoint.md
```

### Comparing `autorag-0.1.9/docs/source/install.md` & `autorag-0.2.0/docs/source/install.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 cd AutoRAG
 pip install -e .
 ```
 
 And then, for testing and documentation build, you need to install some additional packages.
 
 ```bash
-pip install -r dev_requirements.txt
+pip install -r tests/requirements.txt
 pip install -r docs/requirements.txt
 ```
 
 For testing, you have to set env variable at pytest.ini.
 Make new pytest.ini file at the root of the project and write below.
 
 ```ini
```

### Comparing `autorag-0.1.9/docs/source/local_model.md` & `autorag-0.2.0/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/generator/generator.md` & `autorag-0.2.0/docs/source/nodes/generator/generator.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 6. Generator
+# 8. Generator
 
 ### 🔎 **Definition**
 A node that allows for experimentation with various Large Language Models (LLMs). This node is designed to facilitate the testing and evaluation of different LLMs to determine the most effective model for specific tasks or data sets.
 
 ## 🔢 **Parameters**
 
 ### **Overview**
```

### Comparing `autorag-0.1.9/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.2.0/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/generator/openai_llm.md` & `autorag-0.2.0/docs/source/nodes/generator/openai_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/generator/vllm.md` & `autorag-0.2.0/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_augmenter/passage_augmenter.md` & `autorag-0.2.0/docs/source/nodes/passage_augmenter/passage_augmenter.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Passage Augmenter
+# 3. Passage Augmenter
 
 ### 🔎 **Definition**
 
 Passage augmenter is a node that augments passages.
 As opposed to the passage filter node, this is a node that adds passages
 
 ### 🤸 **Benefits**
```

### Comparing `autorag-0.1.9/docs/source/nodes/passage_augmenter/prev_next_augmenter.md` & `autorag-0.2.0/docs/source/nodes/passage_augmenter/prev_next_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.2.0/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 4. Passage_Compressor
+# 6. Passage_Compressor
 
 ### 🔎 **Definition**
 Passage compressor module compresses the contents before they are input into a language model (LLM), reducing the amount of token usage.
 
 ### 🤸 **Benefits**
 - **Efficiency in Token Usage:** By compressing the contents prior to their entry into a language model, the Passage Compressor significantly reduces the number of tokens required. This efficiency is crucial for large-scale applications where token usage can quickly accumulate, potentially leading to higher computational costs and slower processing times.
 - **Cost Reduction:** Efficient token usage directly impacts the cost of running large language models. By reducing the number of tokens needed, the Passage Compressor can help lower operational costs associated with data processing and analysis.
```

### Comparing `autorag-0.1.9/docs/source/nodes/passage_compressor/refine.md` & `autorag-0.2.0/docs/source/nodes/passage_compressor/refine.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.2.0/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_filter/passage_filter.md` & `autorag-0.2.0/docs/source/nodes/passage_filter/passage_filter.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Passage Filter
+# 5. Passage Filter
 
 ### 🔎 **Definition**
 
 Passage filtering is a node that filters out passages.
 It does not compress passages, but it deletes passages that are not relatable enough to the query.
 
 ```{admonition} What is difference between Passage Filter and Passage Reranker?
@@ -48,8 +48,10 @@
 ```{toctree}
 ---
 maxdepth: 1
 ---
 similarity_threshold_cutoff.md
 similarity_percentile_cutoff.md
 recency_filter.md
+threshold_cutoff.md
+percentile_cutoff.md
 ```
```

### Comparing `autorag-0.1.9/docs/source/nodes/passage_filter/recency_filter.md` & `autorag-0.2.0/docs/source/nodes/passage_filter/recency_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md` & `autorag-0.2.0/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md` & `autorag-0.2.0/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Similarity Threshold Cutoff
 
 This module is inspired by
 LlamaIndex ['Sentence Embedding Optimizer'](https://docs.llamaindex.ai/en/stable/examples/node_postprocessor/OptimizerDemo/).
 Re-calculate each content's similarity with the query and filter out the contents that are below the threshold.
 
+📣 Keeps at least one item per query if all scores are below the threshold.
+
 ## **Module Parameters**
 
 - **threshold** : The threshold value to filter out the contents.
   If the similarity score is below the threshold, the content will be filtered out.
   This is essential to run the module, so you have to set this parameter.
 - **embedding_model** : The embedding model name.
 - **batch** : The batch size for embedding queries and contents.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 3. Passage_Reranker
+# 4. Passage_Reranker
 
 ### 🔎 **Definition**
 Reranking is a process applied after the initial retrieval of contents. It involves reassessing and reordering the contents based on their relevance to the query. This step is crucial in information retrieval systems to refine the results obtained from the first retrieval phase.
 
 
 ### 🤸 **Benefits**
 The primary benefit of reranking is the enhanced prioritization of high-relevance contents. By performing a subsequent evaluation, reranking ensures that the most pertinent information is more accessible, improving the overall quality and relevance of the retrieved data.
```

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/time_reranker.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/time_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.2.0/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.2.0/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.2.0/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.2.0/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,8 @@
-# 5. Prompt Maker
+# 7. Prompt Maker
 
 ### 🔎 **Definition**
 **Prompt Maker** is a module that makes a prompt from user query and retrieved contents.
 
 ## 🔢 **Parameters**
 ### **Overview**:
 This document serves as a guide for configuring parameters, strategies, and the config YAML file for various nodes within a system.
```

### Comparing `autorag-0.1.9/docs/source/nodes/query_expansion/hyde.md` & `autorag-0.2.0/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/query_expansion/query_decompose.md` & `autorag-0.2.0/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.2.0/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.2.0/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/retrieval/hybrid_dbsf.md` & `autorag-0.2.0/docs/source/nodes/retrieval/hybrid_dbsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.2.0/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/retrieval/hybrid_rsf.md` & `autorag-0.2.0/docs/source/nodes/retrieval/hybrid_rsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.2.0/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.2.0/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/optimization/custom_config.md` & `autorag-0.2.0/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/optimization/folder_structure.md` & `autorag-0.2.0/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/optimization/optimization.md` & `autorag-0.2.0/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/optimization/sample_full_config.yaml` & `autorag-0.2.0/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/roadmap/modular_rag.md` & `autorag-0.2.0/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/structure.md` & `autorag-0.2.0/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/troubleshooting.md` & `autorag-0.2.0/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/docs/source/tutorial.md` & `autorag-0.2.0/docs/source/tutorial.md`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,23 @@
 ```{admonition} What if Trial_Path didn't also create a First Node Line?
 If the First Node Line folder has not been created in the trial path you want to restart,
 start_trial function will be executed instead of restart_trial.
 
 Note that a new trial folder will be created, not a new restart result in that Trial Path.
 ```
 
+## Run Dashboard to see your trial result!
+
+Up to AutoRAG version 0.2.0, you can use dashboard feature for easily see the results of AutoRAG.
+You can run dashboard just running below command.
+
+```bash
+autorag dashboard --trial_dir /your/path/to/trial_dir
+```
+
 ## Extract pipeline and evaluate test dataset
 
 Now, it's time to evaluate test dataset with a found RAG pipeline. For this, you can extract the optimal pipeline and
 save it to new config yaml file.
 
 You can use the below code.
```

### Comparing `autorag-0.1.9/pyproject.toml` & `autorag-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/requirements.txt` & `autorag-0.2.0/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 numpy
 pandas
 tqdm
-tiktoken  # for counting token
+tiktoken>=0.7.0  # for counting token
 openai>=1.0.0
 rank_bm25  # for bm25 retrieval
 transformers
 swifter  # for parallel pandas apply
 pyyaml  # for yaml file
 pyarrow  # for pandas with parquet
 fastparquet  # for pandas with parquet
@@ -24,25 +24,35 @@
 tokenlog>=0.0.2 # for token logging
 aiohttp # for async http requests
 bert_score # for bert score
 sentence-transformers # for sentence transformer reranker
 FlagEmbedding # for flag embedding reranker
 ragas # evaluation data generation & evaluation
 ray # for parallel processing
+kiwipiepy  # for BM25 Korean tokenizer
 
 ### LlamaIndex ###
 llama-index>=0.10.1
 llama-index-core>=0.10.1
 # Embeddings
 llama-index-embeddings-openai
 llama-index-embeddings-huggingface
 # LLMs
 llama-index-llms-openai
 llama-index-llms-huggingface
 llama-index-llms-openai-like
+# Retriever
+llama-index-retrievers-bm25
 
 # WebUI
 streamlit
 
 
 ### Langchain ###
 langchain-core>=0.1.6
+
+# autorag dashboard    
+panel
+seaborn
+ipykernel
+ipywidgets
+ipywidgets_bokeh
```

### Comparing `autorag-0.1.9/sample_config/compact_local.yaml` & `autorag-0.2.0/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/sample_config/compact_openai.yaml` & `autorag-0.2.0/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/sample_config/config_korean.yaml` & `autorag-0.2.0/tests/resources/result_project/1/config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,66 @@
 node_lines:
-- node_line_name: retrieve_node_line
-  nodes:
-  - node_type: retrieval
-    modules:
-    - module_type: vectordb
-      embedding_model: openai
-    top_k: 3
-    strategy:
-      metrics:
-      - retrieval_f1
-      - retrieval_recall
-      - retrieval_precision
-  - node_type: passage_reranker
-    modules:
-    - module_type: koreranker
-    - module_type: pass_reranker
-    - module_type: cohere_reranker
-    strategy:
-      metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
-    top_k: 3
-- node_line_name: post_retrieve_node_line
-  nodes:
-  - modules:
-    - module_type: fstring
-      prompt: "주어진 passage만을 이용하여 question에 따라 답하시오 passage: {retrieved_contents} \n\n Question: {query} \n\n Answer:"
-    node_type: prompt_maker
-    strategy:
-      generator_modules:
-      - batch: 2
-        llm: openai
-        module_type: llama_index_llm
-      metrics:
-      - bleu
-      - meteor
-      - rouge
-  - modules:
-    - batch: 2
-      llm: openai
-      model: gpt-4
-      module_type: llama_index_llm
-    node_type: generator
-    strategy:
-      metrics:
-      - metric_name: bleu
-      - metric_name: meteor
-      - embedding_model: openai
-        metric_name: sem_score
+  - node_line_name: pre_retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: query_expansion
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
+          top_k: 10
+          retrieval_modules:
+            - module_type: bm25
+            - module_type: vectordb
+              embedding_model: openai
+        modules:
+          - module_type: query_decompose
+            llm: openai
+            temperature: [ 0.2, 1.0 ]
+          - module_type: hyde
+            llm: openai
+            max_token: 64
+  - node_line_name: retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: retrieval
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
+        top_k: 10
+        modules:
+          - module_type: bm25
+          - module_type: vectordb
+            embedding_model: openai
+      - node_type: passage_reranker
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
+        top_k: 5
+        modules:
+          - module_type: tart
+          - module_type: monot5
+      - node_type: passage_filter
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 5
+        modules:
+          - module_type: pass_passage_filter
+          - module_type: threshold_cutoff
+            threshold: 0.85
+  - node_line_name: post_retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: prompt_maker
+        strategy:
+          metrics: [ bleu, meteor, rouge ]
+          speed_threshold: 10
+          generator_modules:
+            - module_type: llama_index_llm
+              llm: mock
+        modules:
+          - module_type: fstring
+            prompt: [ "Tell me something about the question: {query} \n\n {retrieved_contents}",
+                      "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?" ]
+      - node_type: generator
+        strategy:
+          metrics: [ bleu, meteor, rouge ]
+          speed_threshold: 10
+        modules:
+          - module_type: llama_index_llm
+            llm: [ mock ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autorag-0.1.9/sample_config/extracted_sample.yaml` & `autorag-0.2.0/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/sample_config/full.yaml` & `autorag-0.2.0/sample_config/full.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,31 @@
     - node_type: query_expansion
       strategy:
         metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
         speed_threshold: 10
         top_k: 10
         retrieval_modules:
           - module_type: bm25
+            bm25_tokenizer: [ porter_stemmer, ko_kiwi, space, gpt2 ]
           - module_type: vectordb
             embedding_model: openai
       modules:
         - module_type: pass_query_expansion
         - module_type: query_decompose
           llm: openai
           temperature: [0.2, 1.0]
         - module_type: hyde
           llm: openai
           max_token: 64
 - node_line_name: retrieve_node_line  # Arbitrary node line name
   nodes:
     - node_type: retrieval
       strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
+        metrics: [ retrieval_f1, retrieval_recall, retrieval_precision,
+                   retrieval_ndcg, retrieval_map, retrieval_mrr ]
         speed_threshold: 10
       top_k: 10
       modules:
         - module_type: bm25
         - module_type: vectordb
           embedding_model: openai
         - module_type: hybrid_rrf
@@ -82,16 +84,22 @@
       strategy:
         metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
         speed_threshold: 5
       modules:
         - module_type: pass_passage_filter
         - module_type: similarity_threshold_cutoff
           threshold: 0.85
+        - module_type: similarity_percentile_cutoff
+          percentile: 0.6
         - module_type: recency_filter
           threshold: 2015-01-01
+        - module_type: threshold_cutoff
+          threshold: 0.85
+        - module_type: percentile_cutoff
+          percentile: 0.6
     - node_type: passage_compressor
       strategy:
         metrics: [retrieval_token_f1, retrieval_token_recall, retrieval_token_precision]
         speed_threshold: 10
       modules:
         - module_type: pass_compressor
         - module_type: tree_summarize
```

### Comparing `autorag-0.1.9/sample_config/simple_local.yaml` & `autorag-0.2.0/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/sample_config/simple_openai.yaml` & `autorag-0.2.0/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/sample_dataset/README.md` & `autorag-0.2.0/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.2.0/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.2.0/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.2.0/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/data/corpus/test_base.py` & `autorag-0.2.0/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/data/corpus/test_langchain.py` & `autorag-0.2.0/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.2.0/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/data/qacreation/test_base_qacreation.py` & `autorag-0.2.0/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.2.0/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/data/qacreation/test_ragas_qa_creation.py` & `autorag-0.2.0/tests/autorag/data/qacreation/test_ragas_qa_creation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.2.0/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.2.0/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.2.0/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `autorag-0.2.0/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.2.0/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/evaluate/test_generation_evaluate.py` & `autorag-0.2.0/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.2.0/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.2.0/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,36 +2,50 @@
 from typing import Tuple, List
 
 import pandas as pd
 
 from autorag.evaluate import evaluate_retrieval
 
 retrieval_gt = [[[f'test{i}-{j}'] for i in range(2)] for j in range(4)]
+queries_example = ["Query 1", "Query 2", "Query 3", "Query 4"]
+generation_gt_example = [['Jazz', 'Music'],
+                         ['Havertz'],
+                         ['William', 'Gamst'],
+                         ['Kia', 'Tigers', 'V12']]
+contents = [
+    ['a', 'b', 'c', 'd'],
+    ['better', 'bone', 'caleb', 'done'],
+    ['ate', 'better', 'cortex', 'dad'],
+    ['aim', 'bond', 'cane', 'dance'],
+]
+scores = [
+    [0.1, 0.2, 0.3, 0.4],
+    [0.4, 0.3, 0.2, 0.1],
+    [0.5, 0.4, 0.3, 0.2],
+    [0.6, 0.5, 0.4, 0.3],
+]
+ids = [
+    [retrieval_gt[0][0][0], retrieval_gt[0][1][0], 'pred-0', 'pred-1'],
+    ['pred-2', retrieval_gt[1][0][0], retrieval_gt[1][1][0], 'pred-3'],
+    [f'pred-{i}' for i in range(4, 8)],
+    [retrieval_gt[3][0][0], 'pred-8', 'pred-9', 'pred-10'],
+]
+
+
+@evaluate_retrieval(retrieval_gt=retrieval_gt,
+                    metrics=['retrieval_recall', 'retrieval_precision', 'retrieval_f1'],
+                    queries=queries_example, generation_gt=generation_gt_example)
+def pseudo_retrieval() -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
+    return contents, ids, scores
 
 
-@evaluate_retrieval(retrieval_gt=retrieval_gt, metrics=['retrieval_recall', 'retrieval_precision', 'retrieval_f1'])
-def pseudo_retrieval() -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
-    contents = [
-        ['a', 'b', 'c', 'd'],
-        ['better', 'bone', 'caleb', 'done'],
-        ['ate', 'better', 'cortex', 'dad'],
-        ['aim', 'bond', 'cane', 'dance'],
-    ]
-    scores = [
-        [0.1, 0.2, 0.3, 0.4],
-        [0.4, 0.3, 0.2, 0.1],
-        [0.5, 0.4, 0.3, 0.2],
-        [0.6, 0.5, 0.4, 0.3],
-    ]
-    ids = [
-        [retrieval_gt[0][0][0], retrieval_gt[0][1][0], 'pred-0', 'pred-1'],
-        ['pred-2', retrieval_gt[1][0][0], retrieval_gt[1][1][0], 'pred-3'],
-        [f'pred-{i}' for i in range(4, 8)],
-        [retrieval_gt[3][0][0], 'pred-8', 'pred-9', 'pred-10'],
-    ]
+@evaluate_retrieval(retrieval_gt=retrieval_gt,
+                    metrics=[{'metric_name': 'retrieval_recall'}, {'metric_name': 'retrieval_f1'}],
+                    queries=queries_example, generation_gt=generation_gt_example)
+def pseudo_retrieval_dict_metric() -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
     return contents, ids, scores
 
 
 def test_evaluate_retrieval():
     result_df = pseudo_retrieval()
     assert isinstance(result_df, pd.DataFrame)
     assert len(result_df) == 4
@@ -48,7 +62,21 @@
     for pred, sol in zip(precision, precision_solution):
         assert math.isclose(pred, sol, rel_tol=1e-4)
 
     f1 = result_df['retrieval_f1'].tolist()
     f1_solution = [1 / 1.5, 1 / 1.5, 0, 0.25 / 0.75]
     for pred, sol in zip(f1, f1_solution):
         assert math.isclose(pred, sol, rel_tol=1e-4)
+
+
+def test_evaluate_retrieval_dict():
+    result_df = pseudo_retrieval_dict_metric()
+    assert isinstance(result_df, pd.DataFrame)
+    assert len(result_df) == 4
+    assert len(result_df.columns) == 5
+    assert set(result_df.columns) == {'retrieved_contents', 'retrieved_ids', 'retrieve_scores', 'retrieval_recall',
+                                      'retrieval_f1'}
+
+    recall = result_df['retrieval_recall'].tolist()
+    recall_solution = [1, 1, 0, 0.5]
+    for pred, sol in zip(recall, recall_solution):
+        assert math.isclose(pred, sol, rel_tol=1e-4)
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.2.0/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.2.0/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/generator/test_openai.py` & `autorag-0.2.0/tests/autorag/nodes/generator/test_openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 @patch.object(openai.resources.chat.completions.AsyncCompletions, 'create', mock_openai_chat_create)
 def test_openai_llm_node():
     previous_result = pd.DataFrame(
         {
             'prompts': prompts,
             'qid': ['id-1', 'id-2', 'id-3']
         })
-    result_df = openai_llm(project_dir='.', previous_result=previous_result, llm='gpt-3.5-turbo-0125')
+    result_df = openai_llm(project_dir='.', previous_result=previous_result, llm='gpt-4o')
     check_generated_texts(result_df['generated_texts'].tolist())
     check_generated_tokens(result_df['generated_tokens'].tolist())
     check_generated_log_probs(result_df['generated_log_probs'].tolist())
 
 
 @patch.object(openai.resources.chat.completions.AsyncCompletions, 'create', mock_openai_chat_create)
 def test_openai_llm_truncate():
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.2.0/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 def test_run_generator_node(node_line_dir):
     generator_models['mock'] = MockLLM
     modules = [llama_index_llm, llama_index_llm]
     module_params = [{'llm': 'mock', 'temperature': 0.5, 'top_p': 0.9, 'max_tokens': 128, 'batch': 8},
                      {'llm': 'mock', 'temperature': 1.5, 'top_p': 0.9, 'max_tokens': 32, 'batch': 8}]
     strategies = {
+        'strategy': 'rank',
         'metrics': [{'metric_name': 'bleu'}, {'metric_name': 'meteor'}, {'metric_name': 'rouge'}],
         'speed_threshold': 5,
         'token_threshold': 64,
     }
     best_result = run_generator_node(modules, module_params, previous_df, node_line_dir, strategies)
     assert os.path.exists(os.path.join(node_line_dir, "generator"))
     expect_columns = {'qid', 'query', 'prompts', 'generated_texts', 'generated_tokens', 'generated_log_probs',
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.2.0/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py` & `autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py` & `autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py` & `autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py` & `autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py` & `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_refine.py` & `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 root_dir = pathlib.PurePath(os.path.dirname(os.path.realpath(__file__))).parent.parent.parent
 resources_dir = os.path.join(root_dir, "resources")
 qa_data = pd.DataFrame({
     'qid': ['id-1', 'id-2', 'id-3'],
     'query': ['query-1', 'query-2', 'query-3'],
     'retrieval_gt': [
-        [['doc-1'], ['doc-2']],
-        [[]],
+        [['doc-1', 'doc-2']],
+        [['doc-3']],
         [['doc-5'], ['doc-6']],
     ],
     'generation_gt': [['generation-1'], ['generation-2'], ['generation-3']],
 })
 corpus_data = pd.DataFrame({
     'doc_id': ['doc-1', 'doc-2', 'doc-3', 'doc-4', 'doc-5', 'doc-6'],
     'contents': [
@@ -98,17 +98,17 @@
     assert os.path.exists(summary_path)
     summary_df = load_summary_file(summary_path)
     assert set(summary_df.columns) == {'filename', 'passage_compressor_retrieval_token_f1',
                                        'passage_compressor_retrieval_token_precision',
                                        'module_name', 'module_params', 'execution_time', 'is_best'}
     assert len(summary_df) == 2
     assert summary_df['filename'][0] == "0.parquet"
-    assert summary_df['passage_compressor_retrieval_token_f1'][0] == pytest.approx(single_result_df[
-                                                                                       'retrieval_token_f1'].mean())
-    assert summary_df['passage_compressor_retrieval_token_precision'][0] == pytest.approx(single_result_df[
-                                                                                              'retrieval_token_precision'].mean())
+    assert summary_df['passage_compressor_retrieval_token_f1'][0] == pytest.approx(
+        single_result_df['retrieval_token_f1'].mean())
+    assert summary_df['passage_compressor_retrieval_token_precision'][0] == pytest.approx(
+        single_result_df['retrieval_token_precision'].mean())
     assert summary_df['module_name'][0] == "tree_summarize"
     assert summary_df['module_params'][0] == {'llm': 'mock', 'model': 'gpt-3.5-turbo-16k', 'batch': 4}
     assert summary_df['execution_time'][0] > 0
     # test the best file is saved properly
     best_path = summary_df[summary_df['is_best']]['filename'].values[0]
     assert os.path.exists(os.path.join(node_line_dir, "passage_compressor", f'best_{best_path}'))
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py` & `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_passage_filter_base.py` & `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_passage_filter_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_passage_filter_run.py` & `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_passage_filter_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py` & `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_recency_filter.py` & `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_recency_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py` & `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,52 @@
-from autorag.nodes.passagereranker import cohere_reranker
+import asyncio
 
+from llama_index.core import QueryBundle
+from llama_index.core.schema import NodeWithScore, TextNode
+from llama_index.llms.openai import OpenAI
+
+from autorag.nodes.passagereranker import rankgpt
+from autorag.nodes.passagereranker.rankgpt import AsyncRankGPTRerank
 from tests.autorag.nodes.passagereranker.test_passage_reranker_base import queries_example, contents_example, \
     scores_example, ids_example, base_reranker_test, project_dir, previous_result, base_reranker_node_test
 
 
-def test_cohere_reranker():
+def test_async_rankgpt_rerank():
+    query = queries_example[0]
+    query_bundle = QueryBundle(query_str=query)
+    nodes = list(map(lambda x: NodeWithScore(node=TextNode(text=x)), contents_example[0]))
+
+    reranker = AsyncRankGPTRerank(top_n=3, llm=OpenAI())
+    result, id_result = asyncio.run(reranker.async_postprocess_nodes(nodes, query_bundle))
+
+    assert len(result) == 3
+    assert all(isinstance(node, NodeWithScore) for node in result)
+
+
+def test_rankgpt_reranker():
     top_k = 3
-    original_cohere_reranker = cohere_reranker.__wrapped__
+    original_rankgpt_reranker = rankgpt.__wrapped__
     contents_result, id_result, score_result \
-        = original_cohere_reranker(queries_example, contents_example, scores_example, ids_example, top_k)
+        = original_rankgpt_reranker(queries_example, contents_example, scores_example, ids_example, top_k,
+                                    llm=OpenAI(model="gpt-3.5-turbo-16k"))
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
-def test_cohere_reranker_batch_one():
+def test_rankgpt_reranker_batch_one():
     top_k = 3
     batch = 1
-    original_cohere_reranker = cohere_reranker.__wrapped__
+    original_rankgpt_reranker = rankgpt.__wrapped__
     contents_result, id_result, score_result \
-        = original_cohere_reranker(queries_example, contents_example, scores_example, ids_example, top_k, batch=batch)
+        = original_rankgpt_reranker(queries_example, contents_example, scores_example, ids_example, top_k,
+                                    llm=OpenAI(model="gpt-3.5-turbo-16k"), batch=batch)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
-def test_cohere_node():
+def test_rankgpt_node():
     top_k = 1
-    result_df = cohere_reranker(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
+    result_df = rankgpt(project_dir=project_dir, previous_result=previous_result, top_k=top_k,
+                        llm='openai', model='gpt-3.5-turbo', temperature=0.5, batch=8, verbose=True)
+    base_reranker_node_test(result_df, top_k)
+
+    top_k = 2
+    result_df = rankgpt(project_dir=project_dir, previous_result=previous_result, top_k=top_k, batch=4)
     base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_flag_embedding.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,58 @@
-import asyncio
-import os
+from unittest.mock import patch
 
-from autorag.nodes.passagereranker import jina_reranker
-from autorag.nodes.passagereranker.jina import jina_reranker_pure
+import cohere.base_client
+from cohere import RerankResponse, RerankResponseResultsItem
+
+from autorag.nodes.passagereranker import cohere_reranker
 from tests.autorag.nodes.passagereranker.test_passage_reranker_base import queries_example, contents_example, \
     scores_example, ids_example, base_reranker_test, project_dir, previous_result, base_reranker_node_test
 
 
-def test_jina_reranker_pure():
-    api_key = os.environ['JINAAI_API_KEY']
-    assert bool(api_key) is True
-    content_result, id_result, score_result = asyncio.run(
-        jina_reranker_pure(queries_example[0], contents_example[0], scores_example[0], ids_example[0], top_k=2,
-                           api_key=api_key))
-    assert len(content_result) == 2
-    assert len(id_result) == 2
-    assert len(score_result) == 2
-
-    assert all([res in contents_example[0] for res in content_result])
-    assert all([res in ids_example[0] for res in id_result])
-
-    # check if the scores are sorted
-    assert score_result[0] >= score_result[1]
+async def mock_cohere_reranker(self, model, query, documents, top_n, **kwargs) -> RerankResponse:
+    if query == queries_example[0]:
+        return RerankResponse(
+            results=[
+                        RerankResponseResultsItem(index=1, relevance_score=0.8),
+                        RerankResponseResultsItem(index=2, relevance_score=0.2),
+                        RerankResponseResultsItem(index=0, relevance_score=0.1),
+                    ][:top_n]
+        )
+    elif query == queries_example[1]:
+        return RerankResponse(
+            results=[
+                        RerankResponseResultsItem(index=2, relevance_score=0.8),
+                        RerankResponseResultsItem(index=0, relevance_score=0.2),
+                        RerankResponseResultsItem(index=1, relevance_score=0.1),
+                    ][:top_n]
+        )
+    response_items = [
+        RerankResponseResultsItem(index=i, relevance_score=0.1 * i)
+        for i in range(len(documents) - 1, -1, -1)
+    ]
+    return RerankResponse(results=response_items[:top_n])
 
 
-def test_jina_reranker():
+@patch.object(cohere.base_client.AsyncBaseCohere, "rerank", mock_cohere_reranker)
+def test_cohere_reranker():
     top_k = 3
-    original_jina_reranker = jina_reranker.__wrapped__
+    original_cohere_reranker = cohere_reranker.__wrapped__
     contents_result, id_result, score_result \
-        = original_jina_reranker(queries_example, contents_example, scores_example, ids_example, top_k)
+        = original_cohere_reranker(queries_example, contents_example, scores_example, ids_example, top_k)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
-def test_jina_reranker_batch_one():
+@patch.object(cohere.base_client.AsyncBaseCohere, "rerank", mock_cohere_reranker)
+def test_cohere_reranker_batch_one():
     top_k = 3
     batch = 1
-    original_jina_reranker = jina_reranker.__wrapped__
+    original_cohere_reranker = cohere_reranker.__wrapped__
     contents_result, id_result, score_result \
-        = original_jina_reranker(queries_example, contents_example, scores_example, ids_example, top_k, batch=batch)
+        = original_cohere_reranker(queries_example, contents_example, scores_example, ids_example, top_k, batch=batch)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
-def test_jina_reranker_node():
+@patch.object(cohere.base_client.AsyncBaseCohere, "rerank", mock_cohere_reranker)
+def test_cohere_node():
     top_k = 1
-    result_df = jina_reranker(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
+    result_df = cohere_reranker(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
     base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_time_reranker.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_upr.py` & `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.2.0/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.2.0/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.2.0/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.2.0/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
 def test_evaluate_one_prompt_maker_node():
     generator_models['mock'] = MockLLM
     generator_funcs = [llama_index_llm, llama_index_llm]
     generator_params = [{'llm': 'mock', 'model': 'gpt-3.5-turbo'},
                         {'llm': 'mock', 'model': 'gpt-3.5-turbo-1106'}]
     project_dir = '_'
-    best_result = evaluate_one_prompt_maker_node(generator_funcs, generator_params, prompts, sample_generation_gt,
-                                                 metrics, project_dir)
+    best_result = evaluate_one_prompt_maker_node(prompts, generator_funcs, generator_params, sample_generation_gt,
+                                                 metrics, project_dir, 'rank')
     metric_names, _ = cast_metrics(metrics)
     assert isinstance(best_result, pd.DataFrame)
     assert all(metric_name in best_result.columns for metric_name in metric_names)
     assert len(best_result) == len(prompts)
 
 
 @pytest.fixture
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_hyde.py` & `autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,26 +39,26 @@
         test_trail_dir = os.path.join(project_dir, "test_trial")
         os.makedirs(test_trail_dir)
         node_line_dir = os.path.join(test_trail_dir, "test_node_line")
         os.makedirs(node_line_dir)
         yield node_line_dir
 
 
-def test_evaluate_one_prompt_maker_node(node_line_dir):
+def test_evaluate_one_query_expansion_node(node_line_dir):
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     qa_path = os.path.join(project_dir, "data", "qa.parquet")
     previous_result = pd.read_parquet(qa_path)
     sample_previous_result = previous_result.head(2)
     sample_retrieval_gt = sample_previous_result['retrieval_gt'].tolist()
 
     retrieval_funcs = [bm25, bm25]
-    retrieval_params = [{'top_k': 1}, {'top_k': 2}]
+    retrieval_params = [{'top_k': 1, 'bm25_tokenizer': 'gpt2'}, {'top_k': 2, 'bm25_tokenizer': 'gpt2'}]
     best_result = evaluate_one_query_expansion_node(retrieval_funcs, retrieval_params,
                                                     sample_expanded_queries, sample_retrieval_gt,
-                                                    metrics, project_dir, sample_previous_result)
+                                                    metrics, project_dir, sample_previous_result, 'rank')
     assert isinstance(best_result, pd.DataFrame)
     assert all(metric_name in best_result.columns for metric_name in metrics)
     assert len(best_result) == len(sample_expanded_queries)
 
 
 def base_query_expansion_test(best_result, node_line_dir):
     assert os.path.exists(os.path.join(node_line_dir, "query_expansion"))
@@ -95,15 +95,15 @@
 
     modules = [query_decompose, hyde]
     module_params = [{'llm': "mock", 'temperature': 0.2, 'batch': 7}, {'llm': "mock"}]
     strategies = {
         'metrics': metrics,
         'speed_threshold': 5,
         'top_k': 4,
-        'retrieval_modules': [{'module_type': 'bm25'}],
+        'retrieval_modules': [{'module_type': 'bm25', 'bm25_tokenizer': 'gpt2'}],
     }
     best_result = run_query_expansion_node(modules, module_params, previous_result, node_line_dir, strategies)
     base_query_expansion_test(best_result, node_line_dir)
 
 
 def test_run_query_expansion_node_default(node_line_dir):
     generator_models['mock'] = MockLLM
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_base.py` & `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             'contents': ['doc-1', 'doc-2', 'doc-3', 'doc-4', 'doc-5', 'doc-6', 'doc-7', 'doc-8', 'doc-9'],
             'metadata': [{'last_modified_date': datetime.now()} for _ in range(9)]
         })
         os.makedirs(os.path.join(project_dir, "data"))
         corpus_df.to_parquet(os.path.join(project_dir, "data", 'corpus.parquet'))
         resource_dir = os.path.join(project_dir, "resources")
         os.makedirs(resource_dir)
-        bm25_ingest(os.path.join(resource_dir, 'bm25.pkl'), corpus_df)
+        bm25_ingest(os.path.join(resource_dir, 'bm25_porter_stemmer.pkl'), corpus_df)
         chroma_path = os.path.join(resource_dir, 'chroma')
         db = chromadb.PersistentClient(path=chroma_path)
         collection = db.create_collection(name="openai", metadata={"hnsw:space": "cosine"})
         vectordb_ingest(collection, corpus_df, OpenAIEmbedding())
         yield project_dir
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py` & `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_rsf.py` & `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `autorag-0.2.0/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.2.0/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         os.makedirs(node_line_dir)
         yield node_line_dir
 
 
 def test_run_retrieval_node(node_line_dir):
     modules = [bm25, vectordb, hybrid_rrf, hybrid_cc, hybrid_cc]
     module_params = [
-        {'top_k': 4},
+        {'top_k': 4, 'bm25_tokenizer': 'gpt2'},
         {'top_k': 4, 'embedding_model': 'openai'},
         {'top_k': 4, 'rrf_k': 2, 'target_modules': ('bm25', 'vectordb')},
         {'top_k': 4, 'target_modules': ('bm25', 'vectordb'), 'weights': (0.3, 0.7)},
         {'top_k': 4, 'target_modules': ('bm25', 'vectordb'), 'weights': (0.5, 0.5)},
     ]
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     qa_path = os.path.join(project_dir, "data", "qa.parquet")
@@ -70,15 +70,15 @@
     assert set(summary_df.columns) == {'filename', 'retrieval_f1', 'retrieval_recall',
                                        'module_name', 'module_params', 'execution_time', 'is_best'}
     assert len(summary_df) == 5
     assert summary_df['filename'][0] == "0.parquet"
     assert summary_df['retrieval_f1'][0] == bm25_top_k_df['retrieval_f1'].mean()
     assert summary_df['retrieval_recall'][0] == bm25_top_k_df['retrieval_recall'].mean()
     assert summary_df['module_name'][0] == "bm25"
-    assert summary_df['module_params'][0] == {'top_k': 4}
+    assert summary_df['module_params'][0] == {'top_k': 4, 'bm25_tokenizer': 'gpt2'}
     assert summary_df['execution_time'][0] > 0
     # assert average times
     assert summary_df['execution_time'][0] + summary_df['execution_time'][1] == pytest.approx(
         summary_df['execution_time'][2])
     assert summary_df['execution_time'][0] + summary_df['execution_time'][1] == pytest.approx(
         summary_df['execution_time'][3])
 
@@ -89,15 +89,16 @@
     assert all(summary_df['module_params'].apply(lambda x: 'ids' not in x))
     assert all(summary_df['module_params'].apply(lambda x: 'scores' not in x))
     hybrid_summary_df = summary_df[summary_df['module_name'].str.contains('hybrid')]
     assert all(hybrid_summary_df['module_params'].apply(lambda x: 'target_modules' in x))
     assert all(hybrid_summary_df['module_params'].apply(lambda x: 'target_module_params' in x))
     assert all(hybrid_summary_df['module_params'].apply(lambda x: x['target_modules'] == ('bm25', 'vectordb')))
     assert all(hybrid_summary_df['module_params'].apply(
-        lambda x: x['target_module_params'] == ({'top_k': 4}, {'top_k': 4, 'embedding_model': 'openai'})))
+        lambda x: x['target_module_params'] == (
+        {'top_k': 4, 'bm25_tokenizer': 'gpt2'}, {'top_k': 4, 'embedding_model': 'openai'})))
 
     # test the best file is saved properly
     best_filename = summary_df[summary_df['is_best'] == True]['filename'].values[0]
     best_path = os.path.join(node_line_dir, "retrieval", f'best_{best_filename}')
     assert os.path.exists(best_path)
     best_df = pd.read_parquet(best_path)
     assert all([expect_column in best_df.columns for expect_column in expect_columns])
```

### Comparing `autorag-0.1.9/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.2.0/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/schema/test_module_schema.py` & `autorag-0.2.0/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/schema/test_node_schema.py` & `autorag-0.2.0/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/test_cli.py` & `autorag-0.2.0/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/test_deploy.py` & `autorag-0.2.0/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/test_evaluator.py` & `autorag-0.2.0/tests/autorag/test_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     assert node.strategy['metrics'] == ['retrieval_f1', 'retrieval_recall']
     assert node.modules[0].module_type == 'bm25'
     assert node.modules[1].module_type == 'vectordb'
     assert node.modules[2].module_type == 'hybrid_rrf'
     assert node.modules[0].module == bm25
     assert node.modules[1].module == vectordb
     assert node.modules[2].module == hybrid_rrf
-    assert node.modules[0].module_param == {}
+    assert node.modules[0].module_param == {'bm25_tokenizer': ['facebook/opt-125m', 'porter_stemmer']}
     assert node.modules[1].module_param == {'embedding_model': ['openai', 'openai']}
     assert node.modules[2].module_param == {
         'rrf_k': 5, 'target_modules': ('bm25', 'vectordb')
     }
     assert nodes[1].node_type == 'passage_filter'
 
 
@@ -109,29 +109,35 @@
     node_line_summary_df = load_summary_file(node_line_summary_path, ["best_module_params"])
     assert len(node_line_summary_df) == 2
     assert set(node_line_summary_df.columns) == {'node_type', 'best_module_filename',
                                                  'best_module_name', 'best_module_params', 'best_execution_time'}
     assert node_line_summary_df['node_type'][0] == 'retrieval'
     assert node_line_summary_df['best_module_filename'][0] == '0.parquet'
     assert node_line_summary_df['best_module_name'][0] == 'bm25'
-    assert node_line_summary_df['best_module_params'][0] == {'top_k': 10}
+    assert node_line_summary_df['best_module_params'][0] == {'top_k': 10,
+                                                             'bm25_tokenizer': 'porter_stemmer'} or \
+           node_line_summary_df['best_module_params'][0] == {'top_k': 10,
+                                                             'bm25_tokenizer': 'facebook/opt-125m'}
     assert node_line_summary_df['best_execution_time'][0] > 0
 
     # test trial summary
     trial_summary_path = os.path.join(project_dir, '0', 'summary.csv')
     assert os.path.exists(trial_summary_path)
     trial_summary_df = load_summary_file(trial_summary_path, ["best_module_params"])
     assert len(trial_summary_df) == 2
     assert set(trial_summary_df.columns) == {'node_line_name', 'node_type', 'best_module_filename',
                                              'best_module_name', 'best_module_params', 'best_execution_time'}
     assert trial_summary_df['node_line_name'][0] == 'retrieve_node_line'
     assert trial_summary_df['node_type'][0] == 'retrieval'
     assert trial_summary_df['best_module_filename'][0] == '0.parquet'
     assert trial_summary_df['best_module_name'][0] == 'bm25'
-    assert trial_summary_df['best_module_params'][0] == {'top_k': 10}
+    assert trial_summary_df['best_module_params'][0] == {'top_k': 10,
+                                                         'bm25_tokenizer': 'facebook/opt-125m'} or \
+           trial_summary_df['best_module_params'][0] == {'top_k': 10,
+                                                         'bm25_tokenizer': 'porter_stemmer'}
     assert trial_summary_df['best_execution_time'][0] > 0
 
 
 @pytest.mark.skip(reason="This test is too slow")
 def test_start_trial_full(evaluator):
     evaluator.start_trial(os.path.join(resource_dir, 'full.yaml'))
     project_dir = evaluator.project_dir
@@ -224,16 +230,14 @@
     return CompletionResponse(text=messages)
 
 
 async def mock_apredict(self, prompt, **kwargs):
     return prompt.format(**kwargs)
 
 
-@patch.object(OpenAI, "acomplete", mock_acomplete)
-@patch.object(OpenAI, "apredict", mock_apredict)
 def test_restart_last_node(evaluator):
     compressor_error_folder_path = os.path.join(resource_dir, 'result_project', '1')
     base_restart_trial(evaluator, compressor_error_folder_path)
 
 
 @patch.object(OpenAI, "acomplete", mock_acomplete)
 def test_restart_first_node(evaluator):
```

### Comparing `autorag-0.1.9/tests/autorag/test_strategy.py` & `autorag-0.2.0/tests/autorag/test_strategy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import time
 
 import pandas as pd
 import pytest
 
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average
+from autorag.strategy import measure_speed, filter_by_threshold, select_best_average, select_best_rr
+
+sample_dfs = [
+    pd.DataFrame(
+        {'content': ['a', 'b', 'c'], 'retrieval_f1': [0.1, 0.2, 0.3], 'retrieval_recall': [0.1, 0.2, 0.3]}),
+    pd.DataFrame(
+        {'content': ['d', 'e', 'f'], 'retrieval_f1': [0.2, 0.3, 0.4], 'retrieval_recall': [0.2, 0.3, 0.4]}),
+    pd.DataFrame(
+        {'content': ['g', 'h', 'i'], 'retrieval_f1': [0.3, 0.4, 0.5], 'retrieval_recall': [0.3, 0.4, 0.5]}),
+]
+sample_metadatas = ['a', 'b', 'c']
 
 
 def test_measure_speed():
     empty_result, five_seconds = measure_speed(time.sleep, 2)
     assert empty_result is None
     assert pytest.approx(2, 0.1) == five_seconds
 
@@ -32,24 +42,26 @@
     filenames = ['a', 'b', 'c', 'd']
     filtered_results, filtered_filenames = filter_by_threshold(results, values, threshold, filenames)
     assert filtered_results == [1, 2, 3, 4]
     assert filtered_filenames == ['a', 'b', 'c', 'd']
 
 
 def test_select_best_average():
-    sample_dfs = [
-        pd.DataFrame(
-            {'content': ['a', 'b', 'c'], 'retrieval_f1': [0.1, 0.2, 0.3], 'retrieval_recall': [0.1, 0.2, 0.3]}),
-        pd.DataFrame(
-            {'content': ['d', 'e', 'f'], 'retrieval_f1': [0.2, 0.3, 0.4], 'retrieval_recall': [0.2, 0.3, 0.4]}),
-        pd.DataFrame(
-            {'content': ['g', 'h', 'i'], 'retrieval_f1': [0.3, 0.4, 0.5], 'retrieval_recall': [0.3, 0.4, 0.5]}),
-    ]
-    sample_metadatas = ['a', 'b', 'c']
     best_df, best_filename = select_best_average(sample_dfs, ['retrieval_f1', 'retrieval_recall'], sample_metadatas)
     assert best_df['content'].tolist() == ['g', 'h', 'i']
     assert best_df['retrieval_f1'].tolist() == [0.3, 0.4, 0.5]
     assert best_df['retrieval_recall'].tolist() == [0.3, 0.4, 0.5]
     assert best_filename == 'c'
 
     best_df, _ = select_best_average(sample_dfs, ['retrieval_f1', 'retrieval_recall'])
     assert best_df['content'].tolist() == ['g', 'h', 'i']
+
+
+def test_select_best_rr():
+    best_df, best_filename = select_best_rr(sample_dfs, ['retrieval_f1', 'retrieval_recall'], sample_metadatas)
+    assert best_df['content'].tolist() == ['g', 'h', 'i']
+    assert best_df['retrieval_f1'].tolist() == [0.3, 0.4, 0.5]
+    assert best_df['retrieval_recall'].tolist() == [0.3, 0.4, 0.5]
+    assert best_filename == 'c'
+
+    best_df, _ = select_best_average(sample_dfs, ['retrieval_f1', 'retrieval_recall'])
+    assert best_df['content'].tolist() == ['g', 'h', 'i']
```

### Comparing `autorag-0.1.9/tests/autorag/test_web.py` & `autorag-0.2.0/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/autorag/utils/test_preprocess.py` & `autorag-0.2.0/tests/autorag/utils/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/delete_tests.py` & `autorag-0.2.0/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/mock.py` & `autorag-0.2.0/tests/mock.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/README.md` & `autorag-0.2.0/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/corpus_data_sample.parquet` & `autorag-0.2.0/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.2.0/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.2.0/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.2.0/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/full.yaml` & `autorag-0.2.0/tests/resources/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/qa_data_sample.parquet` & `autorag-0.2.0/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/qa_test_data_sample.parquet` & `autorag-0.2.0/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/config.yaml` & `autorag-0.2.0/tests/resources/result_project/2/config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 node_lines:
-- node_line_name: pre_retrieve_node_line  # Arbitrary node line name
-  nodes:
-    - node_type: query_expansion
-      strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
-        speed_threshold: 10
+  - node_line_name: pre_retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: query_expansion
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
+          top_k: 10
+          retrieval_modules:
+            - module_type: bm25
+            - module_type: vectordb
+              embedding_model: openai
+        modules:
+          - module_type: query_decompose
+            llm: openai
+            temperature: [ 0.2, 1.0 ]
+          - module_type: hyde
+            llm: openai
+            max_token: 64
+  - node_line_name: retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: retrieval
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
         top_k: 10
-        retrieval_modules:
+        modules:
           - module_type: bm25
           - module_type: vectordb
             embedding_model: openai
-      modules:
-        - module_type: query_decompose
-          llm: openai
-          temperature: [0.2, 1.0]
-        - module_type: hyde
-          llm: openai
-          max_token: 64
-- node_line_name: retrieve_node_line  # Arbitrary node line name
-  nodes:
-    - node_type: retrieval
-      strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
-        speed_threshold: 10
-      top_k: 10
-      modules:
-        - module_type: bm25
-        - module_type: vectordb
-          embedding_model: openai
-    - node_type: passage_reranker
-      strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
-        speed_threshold: 10
-      top_k: 5
-      modules:
-        - module_type: tart
-        - module_type: monot5
-    - node_type: passage_compressor
-      strategy:
-        metrics: [retrieval_token_f1, retrieval_token_recall, retrieval_token_precision]
-        speed_threshold: 10
-      modules:
-        - module_type: tree_summarize
-          llm: openai
-          model: gpt-3.5-turbo-16k
-- node_line_name: post_retrieve_node_line  # Arbitrary node line name
-  nodes:
-    - node_type: prompt_maker
-      strategy:
-        metrics: [bleu, meteor, rouge]
-        speed_threshold: 10
-        generator_modules:
-          - module_type: llama_index_llm
+      - node_type: passage_reranker
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
+        top_k: 5
+        modules:
+          - module_type: tart
+          - module_type: monot5
+      - node_type: passage_compressor
+        strategy:
+          metrics: [ retrieval_token_f1, retrieval_token_recall, retrieval_token_precision ]
+          speed_threshold: 10
+        modules:
+          - module_type: tree_summarize
             llm: openai
-            model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
-      modules:
-        - module_type: fstring
-          prompt: ["Tell me something about the question: {query} \n\n {retrieved_contents}",
-                   "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?"]
-    - node_type: generator
-      strategy:
-        metrics: [bleu, meteor, rouge]
-        speed_threshold: 10
-      modules:
-        - module_type: llama_index_llm
-          llm: [openai]
-          model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
-          temperature: [0.5, 1.0, 1.5]
+            model: gpt-3.5-turbo-16k
+  - node_line_name: post_retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: prompt_maker
+        strategy:
+          metrics: [ bleu, meteor, rouge ]
+          speed_threshold: 10
+          generator_modules:
+            - module_type: llama_index_llm
+              llm: mock
+        modules:
+          - module_type: fstring
+            prompt: [ "Tell me something about the question: {query} \n\n {retrieved_contents}",
+                      "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?" ]
+      - node_type: generator
+        strategy:
+          metrics: [ bleu, meteor, rouge ]
+          speed_threshold: 10
+        modules:
+          - module_type: llama_index_llm
+            llm: [ mock ]
```

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/0/summary.csv` & `autorag-0.2.0/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.2.0/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/3/config.yaml` & `autorag-0.2.0/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/best.yaml` & `autorag-0.2.0/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/data/corpus.parquet` & `autorag-0.2.0/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/data/qa.parquet` & `autorag-0.2.0/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/resources/bm25.pkl` & `autorag-0.2.0/tests/resources/sample_project/resources/bm25_gpt2.pkl`

 * *Files 0% similar despite different names*

```diff
@@ -4090,15 +4090,15 @@
 0000ff90: 4dae 354d 3a01 4d4d 5d4d f354 4da7 4d4d  M.5M:.MM]M.TM.MM
 0000ffa0: da03 4d17 034d b458 4d22 014d da14 4d4d  ..M..M.XM".M..MM
 0000ffb0: 5d4d 2805 4b1e 4d37 0f4d 88c3 4b1a 4ddb  ]M(.K.M7.M..K.M.
 0000ffc0: 074d ce25 4b00 4d3a 234d 2506 4ddf 064b  .M.%K.M:#M%.M..K
 0000ffd0: 1a4d 3a01 4d1d 044d 4d2e 4d01 014d 670f  .M:.M..MM.M..Mg.
 0000ffe0: 4d3e 014d 2202 4d55 334b 1a4d 8b06 4dca  M>.M".MU3K.M..M.
 0000fff0: 364d 7f01 4de8 364d 2201 4db0 2a4d 3a01  6M..M.6M".M.*M:.
-00010000: 4d1c 2f4d 1c01 4d99 034b 1e95 7aab 0000  M./M..M..K..z...
+00010000: 4d1c 2f4d 1c01 4d99 034b 1e95 92ab 0000  M./M..M..K......
 00010010: 0000 0000 4dc2 064d 5f01 4dc3 1c4b 1a4d  ....M..M_.M..K.M
 00010020: 2201 4d78 024b dc65 5d94 284d 7b06 4d01  ".Mx.K.e].(M{.M.
 00010030: 014d 300e 4d19 014d 455b 4d7d 034b 4c4b  .M0.M..ME[M}.KLK
 00010040: 0d4b c64b 334d 3c01 4dae 014d 8204 4b46  .K.K3M<.M..M..KF
 00010050: 4d23 014d 6112 4d5c 3b4d 2501 4d43 0a4d  M#.Ma.M\;M%.MC.M
 00010060: 0601 4dcd 024d 1804 4d1c 014d 5e06 4d19  ..M..M..M..M^.M.
 00010070: 014d 922d 4dfd 034d ee04 4d01 014d 432e  .M.-M..M..M..MC.
@@ -6834,8 +6834,10 @@
 0001ab10: 3763 3732 3894 8c24 3536 3836 6234 6237  7c728..$5686b4b7
 0001ab20: 2d31 3837 302d 3434 3731 2d62 3766 622d  -1870-4471-b7fb-
 0001ab30: 6664 6266 3331 6633 6166 3734 948c 2439  fdbf31f3af74..$9
 0001ab40: 3966 3065 3664 662d 3366 3033 2d34 6264  9f0e6df-3f03-4bd
 0001ab50: 622d 6261 3234 2d38 6633 3837 6137 3833  b-ba24-8f387a783
 0001ab60: 6335 3594 8c24 3139 3530 6335 6536 2d65  c55..$1950c5e6-e
 0001ab70: 6535 332d 3462 3066 2d39 6233 322d 6530  e53-4b0f-9b32-e0
-0001ab80: 3164 3931 6436 6365 3963 9465 752e       1d91d6ce9c.eu.
+0001ab80: 3164 3931 6436 6365 3963 9465 8c0e 746f  1d91d6ce9c.e..to
+0001ab90: 6b65 6e69 7a65 725f 6e61 6d65 948c 0467  kenizer_name...g
+0001aba0: 7074 3294 752e                           pt2.u.
```

### Comparing `autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.2.0/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/sample_contents_nqa.csv` & `autorag-0.2.0/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.2.0/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/sample_project/data/qa.parquet` & `autorag-0.2.0/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.9/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.2.0/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

