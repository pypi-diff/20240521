# Comparing `tmp/ragas-0.1.6.tar.gz` & `tmp/ragas-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.1.6.tar", last modified: Tue Apr  2 00:11:56 2024, max compression
+gzip compressed data, was "ragas-0.1.7.tar", last modified: Mon Apr  8 19:47:12 2024, max compression
```

## Comparing `ragas-0.1.6.tar` & `ragas-0.1.7.tar`

### file list

```diff
@@ -1,211 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.176890 ragas-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 00:11:50.000000 ragas-0.1.6/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:50.000000 ragas-0.1.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.136891 ragas-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.140890 ragas-0.1.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/ISSUE_TEMPLATE/question.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.140890 ragas-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-02 00:11:50.000000 ragas-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-02 00:11:50.000000 ragas-0.1.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-02 00:11:50.000000 ragas-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-02 00:11:50.000000 ragas-0.1.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-02 00:11:56.176890 ragas-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-02 00:11:50.000000 ragas-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.140890 ragas-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.144890 ragas-0.1.6/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.144890 ragas-0.1.6/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_ipython3.css
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_ipython3_dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_ipython3_light.css
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_python.css
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_python_dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_python_light.css
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/ragas.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.152890 ragas-0.1.6/docs/_static/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/bar-graph.svg
--rw-r--r--   0 runner    (1001) docker     (127)   164494 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-emb-results.png
--rw-r--r--   0 runner    (1001) docker     (127)    35659 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-embeddings.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)   526410 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-llm-result.png
--rw-r--r--   0 runner    (1001) docker     (127)    75530 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-llms-front.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)    54409 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-llms-testset.png
--rw-r--r--   0 runner    (1001) docker     (127)    85475 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/component-wise-metrics.png
--rw-r--r--   0 runner    (1001) docker     (127)   166767 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/eval-evolve.png
--rw-r--r--   0 runner    (1001) docker     (127)   246223 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/langsmith-tracing-faithfullness.png
--rw-r--r--   0 runner    (1001) docker     (127)   119984 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/langsmith-tracing-overview.png
--rw-r--r--   0 runner    (1001) docker     (127)    33956 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/question_types.png
--rw-r--r--   0 runner    (1001) docker     (127)   251574 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/quickstart-output.png
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/ragas-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   415043 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/ragas_workflow_white.png
--rw-r--r--   0 runner    (1001) docker     (127)   139460 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/testset_output.png
--rw-r--r--   0 runner    (1001) docker     (127)   734563 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/trace-langsmith.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.152890 ragas-0.1.6/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/js/mendable_chat_bubble.js
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/js/octolane.js
--rw-r--r--   0 runner    (1001) docker     (127)    62458 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/langsmith-dataset.png
--rw-r--r--   0 runner    (1001) docker     (127)   127732 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/langsmith-evaluation.png
--rw-r--r--   0 runner    (1001) docker     (127)   100406 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/langsmith-feedback.png
--rw-r--r--   0 runner    (1001) docker     (127)   282402 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/langsmith-ragas-chain-trace.png
--rw-r--r--   0 runner    (1001) docker     (127)   209039 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/list-score-traces-ragas.png
--rw-r--r--   0 runner    (1001) docker     (127)   310073 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/traces-score-ragas.png
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/alfred.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.152890 ragas-0.1.6/docs/community/
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/community/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.152890 ragas-0.1.6/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/feedback.md
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.156890 ragas-0.1.6/docs/concepts/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/answer_correctness.md
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/answer_relevance.md
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/context_entities_recall.md
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/context_precision.md
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/context_recall.md
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/context_relevancy.md
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/critique.md
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/faithfulness.md
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/semantic_similarity.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics_driven.md
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/prompt_adaptation.md
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/prompts.md
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/testset_generation.md
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.156890 ragas-0.1.6/docs/getstarted/
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/evaluation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/monitoring.md
--rw-r--r--   0 runner    (1001) docker     (127)    18719 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/prepare_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/testset_generation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.156890 ragas-0.1.6/docs/howtos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.156890 ragas-0.1.6/docs/howtos/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/compare_embeddings.md
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/compare_llms.md
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/custom_prompts.md
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/data_preparation.md
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/tracing.md
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/use_prompt_adaptation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/howtos/customisations/
--rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/aws-bedrock.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16912 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/azure-openai.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/bring-your-own-llm-or-embs.md
--rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/gcp-vertexai.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/howtos/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/athina.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/langchain.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24965 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/langfuse.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/langsmith.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/llamaindex.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/howtos/integrations/nyc_wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)   130296 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/nyc_wikipedia/nyc_text.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/openlayer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23009 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/ragas-arize.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/ragas_haystack.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/tonic-validate.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/zeno.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/references/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/references/evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/references/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/references/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/references/integrations/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/references/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 00:11:50.000000 ragas-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 00:11:50.000000 ragas-0.1.6/references.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.164890 ragas-0.1.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 00:11:50.000000 ragas-0.1.6/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 00:11:50.000000 ragas-0.1.6/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 00:11:50.000000 ragas-0.1.6/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:11:56.176890 ragas-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.136891 ragas-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.164890 ragas-0.1.6/src/ragas/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.164890 ragas-0.1.6/src/ragas/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.164890 ragas-0.1.6/src/ragas/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/integrations/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/integrations/langsmith.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.168890 ragas-0.1.6/src/ragas/llms/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.168890 ragas-0.1.6/src/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_answer_correctness.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_answer_relevance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_answer_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_context_entities_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_context_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_context_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_context_relevancy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_faithfulness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/critique.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/run_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.168890 ragas-0.1.6/src/ragas/testset/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/docstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    22732 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/evolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    28992 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/src/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/benchmarks/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/benchmarks/benchmark_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/benchmarks/benchmark_testsetgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/benchmarks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/e2e/test_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/e2e/test_fullflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/unit/llms/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/llms/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/llms/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/unit/testset_generator/
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/testset_generator/test_docstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/testset_generator/test_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    41535 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/testset_generator/test_embs.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.209253 ragas-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 19:47:03.000000 ragas-0.1.7/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:03.000000 ragas-0.1.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.169253 ragas-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.177253 ragas-0.1.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 19:47:03.000000 ragas-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 19:47:03.000000 ragas-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-08 19:47:03.000000 ragas-0.1.7/.github/ISSUE_TEMPLATE/question.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.177253 ragas-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-08 19:47:03.000000 ragas-0.1.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-08 19:47:03.000000 ragas-0.1.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-08 19:47:03.000000 ragas-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-08 19:47:03.000000 ragas-0.1.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-08 19:47:03.000000 ragas-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-08 19:47:03.000000 ragas-0.1.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-08 19:47:12.209253 ragas-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-08 19:47:03.000000 ragas-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.177253 ragas-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.177253 ragas-0.1.7/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.181253 ragas-0.1.7/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/css/highlight_ipython3.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/css/highlight_ipython3_dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/css/highlight_ipython3_light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/css/highlight_python.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/css/highlight_python_dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/css/highlight_python_light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/css/ragas.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.185253 ragas-0.1.7/docs/_static/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/bar-graph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   164494 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/compare-emb-results.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35659 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/compare-embeddings.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)   526410 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/compare-llm-result.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75530 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/compare-llms-front.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)    54409 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/compare-llms-testset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    85475 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/component-wise-metrics.png
+-rw-r--r--   0 runner    (1001) docker     (127)   166767 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/eval-evolve.png
+-rw-r--r--   0 runner    (1001) docker     (127)   246223 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/langsmith-tracing-faithfullness.png
+-rw-r--r--   0 runner    (1001) docker     (127)   119984 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/langsmith-tracing-overview.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33956 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/question_types.png
+-rw-r--r--   0 runner    (1001) docker     (127)   251574 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/quickstart-output.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/ragas-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   415043 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/ragas_workflow_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)   139460 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/testset_output.png
+-rw-r--r--   0 runner    (1001) docker     (127)   734563 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/imgs/trace-langsmith.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.185253 ragas-0.1.7/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/js/mendable_chat_bubble.js
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/js/octolane.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62458 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/langsmith-dataset.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127732 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/langsmith-evaluation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100406 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/langsmith-feedback.png
+-rw-r--r--   0 runner    (1001) docker     (127)   282402 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/langsmith-ragas-chain-trace.png
+-rw-r--r--   0 runner    (1001) docker     (127)   209039 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/list-score-traces-ragas.png
+-rw-r--r--   0 runner    (1001) docker     (127)   310073 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/_static/traces-score-ragas.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/alfred.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.185253 ragas-0.1.7/docs/community/
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/community/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.189253 ragas-0.1.7/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/feedback.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.189253 ragas-0.1.7/docs/concepts/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/answer_correctness.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/answer_relevance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/context_entities_recall.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/context_precision.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/context_recall.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/context_relevancy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/critique.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/faithfulness.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics/semantic_similarity.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/metrics_driven.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/prompt_adaptation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/prompts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/concepts/testset_generation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.189253 ragas-0.1.7/docs/getstarted/
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/getstarted/evaluation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/getstarted/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/getstarted/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/getstarted/monitoring.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18719 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/getstarted/prepare_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/getstarted/testset_generation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.189253 ragas-0.1.7/docs/howtos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.193253 ragas-0.1.7/docs/howtos/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/applications/compare_embeddings.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/applications/compare_llms.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/applications/custom_prompts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/applications/data_preparation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/applications/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/applications/tracing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/applications/use_prompt_adaptation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.193253 ragas-0.1.7/docs/howtos/customisations/
+-rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/customisations/aws-bedrock.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16912 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/customisations/azure-openai.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/customisations/bring-your-own-llm-or-embs.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/customisations/gcp-vertexai.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/customisations/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/customisations/ragas_custom_model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.193253 ragas-0.1.7/docs/howtos/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/athina.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/langchain.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24965 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/langfuse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/langsmith.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/llamaindex.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.193253 ragas-0.1.7/docs/howtos/integrations/nyc_wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)   130296 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/nyc_wikipedia/nyc_text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/openlayer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23009 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/ragas-arize.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/ragas_haystack.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/tonic-validate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/howtos/integrations/zeno.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.197253 ragas-0.1.7/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/references/evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/references/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.197253 ragas-0.1.7/docs/references/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/references/integrations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 19:47:03.000000 ragas-0.1.7/docs/references/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 19:47:03.000000 ragas-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-08 19:47:03.000000 ragas-0.1.7/references.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.197253 ragas-0.1.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 19:47:03.000000 ragas-0.1.7/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 19:47:03.000000 ragas-0.1.7/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 19:47:03.000000 ragas-0.1.7/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:47:12.209253 ragas-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.173253 ragas-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.197253 ragas-0.1.7/src/ragas/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 19:47:12.000000 ragas-0.1.7/src/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.197253 ragas-0.1.7/src/ragas/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.201253 ragas-0.1.7/src/ragas/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/integrations/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/integrations/langsmith.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.201253 ragas-0.1.7/src/ragas/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/llms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/llms/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/llms/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/llms/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.201253 ragas-0.1.7/src/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/_answer_correctness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/_answer_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/_answer_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/_context_entities_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/_context_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/_context_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/_context_relevancy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/_faithfulness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/metrics/critique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/run_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.205253 ragas-0.1.7/src/ragas/testset/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/testset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/testset/docstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22732 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/testset/evolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/testset/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/testset/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/testset/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31411 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/testset/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/testset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-08 19:47:03.000000 ragas-0.1.7/src/ragas/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.209253 ragas-0.1.7/src/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-08 19:47:12.000000 ragas-0.1.7/src/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-08 19:47:12.000000 ragas-0.1.7/src/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:47:12.000000 ragas-0.1.7/src/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-08 19:47:12.000000 ragas-0.1.7/src/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 19:47:12.000000 ragas-0.1.7/src/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.205253 ragas-0.1.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.205253 ragas-0.1.7/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/benchmarks/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/benchmarks/benchmark_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/benchmarks/benchmark_testsetgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/benchmarks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.205253 ragas-0.1.7/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/e2e/test_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/e2e/test_fullflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.205253 ragas-0.1.7/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.205253 ragas-0.1.7/tests/unit/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/llms/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/llms/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:47:12.209253 ragas-0.1.7/tests/unit/testset_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/testset_generator/test_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/testset_generator/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41535 2024-04-08 19:47:03.000000 ragas-0.1.7/tests/unit/testset_generator/test_embs.pkl
```

### Comparing `ragas-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md` & `ragas-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md` & `ragas-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/.github/workflows/ci.yaml` & `ragas-0.1.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/.github/workflows/python-publish.yml` & `ragas-0.1.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/.gitignore` & `ragas-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/.readthedocs.yml` & `ragas-0.1.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/LICENSE` & `ragas-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/Makefile` & `ragas-0.1.7/Makefile`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/PKG-INFO` & `ragas-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.1.6
+Version: 0.1.7
 Description-Content-Type: text/plain
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: datasets
 Requires-Dist: tiktoken
 Requires-Dist: langchain
 Requires-Dist: langchain-core
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.1.6 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.1.7 Description-Content-Type:
 text/plain License-File: LICENSE Requires-Dist: numpy Requires-Dist: datasets
 Requires-Dist: tiktoken Requires-Dist: langchain Requires-Dist: langchain-core
 Requires-Dist: langchain-community Requires-Dist: langchain_openai Requires-
 Dist: openai>1 Requires-Dist: pysbd>=0.3.4 Requires-Dist: nest-asyncio
 Requires-Dist: appdirs Provides-Extra: all Requires-Dist: sentence-
 transformers; extra == "all"
                  ************ [[..//ddooccss//__ssttaattiicc//iimmggss//llooggoo..ppnngg]] ************
```

### Comparing `ragas-0.1.6/README.md` & `ragas-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/Makefile` & `ragas-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/css/highlight_ipython3.css` & `ragas-0.1.7/docs/_static/css/highlight_ipython3.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/css/highlight_ipython3_dark.css` & `ragas-0.1.7/docs/_static/css/highlight_ipython3_dark.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/css/highlight_ipython3_light.css` & `ragas-0.1.7/docs/_static/css/highlight_ipython3_light.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/css/highlight_python.css` & `ragas-0.1.7/docs/_static/css/highlight_python.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/css/highlight_python_dark.css` & `ragas-0.1.7/docs/_static/css/highlight_python_dark.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/css/highlight_python_light.css` & `ragas-0.1.7/docs/_static/css/highlight_python_light.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/css/ragas.css` & `ragas-0.1.7/docs/_static/css/ragas.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/favicon.ico` & `ragas-0.1.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/bar-graph.svg` & `ragas-0.1.7/docs/_static/imgs/bar-graph.svg`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/compare-emb-results.png` & `ragas-0.1.7/docs/_static/imgs/compare-emb-results.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/compare-embeddings.jpeg` & `ragas-0.1.7/docs/_static/imgs/compare-embeddings.jpeg`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/compare-llm-result.png` & `ragas-0.1.7/docs/_static/imgs/compare-llm-result.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/compare-llms-front.jpeg` & `ragas-0.1.7/docs/_static/imgs/compare-llms-front.jpeg`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/compare-llms-testset.png` & `ragas-0.1.7/docs/_static/imgs/compare-llms-testset.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/component-wise-metrics.png` & `ragas-0.1.7/docs/_static/imgs/component-wise-metrics.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/eval-evolve.png` & `ragas-0.1.7/docs/_static/imgs/eval-evolve.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/langsmith-tracing-faithfullness.png` & `ragas-0.1.7/docs/_static/imgs/langsmith-tracing-faithfullness.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/langsmith-tracing-overview.png` & `ragas-0.1.7/docs/_static/imgs/langsmith-tracing-overview.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/logo.png` & `ragas-0.1.7/docs/_static/imgs/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/question_types.png` & `ragas-0.1.7/docs/_static/imgs/question_types.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/quickstart-output.png` & `ragas-0.1.7/docs/_static/imgs/quickstart-output.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/ragas-logo.png` & `ragas-0.1.7/docs/_static/imgs/ragas-logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/ragas_workflow_white.png` & `ragas-0.1.7/docs/_static/imgs/ragas_workflow_white.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/testset_output.png` & `ragas-0.1.7/docs/_static/imgs/testset_output.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/imgs/trace-langsmith.png` & `ragas-0.1.7/docs/_static/imgs/trace-langsmith.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/js/mendable_chat_bubble.js` & `ragas-0.1.7/docs/_static/js/mendable_chat_bubble.js`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/langsmith-dataset.png` & `ragas-0.1.7/docs/_static/langsmith-dataset.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/langsmith-evaluation.png` & `ragas-0.1.7/docs/_static/langsmith-evaluation.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/langsmith-feedback.png` & `ragas-0.1.7/docs/_static/langsmith-feedback.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/langsmith-ragas-chain-trace.png` & `ragas-0.1.7/docs/_static/langsmith-ragas-chain-trace.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/list-score-traces-ragas.png` & `ragas-0.1.7/docs/_static/list-score-traces-ragas.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/_static/traces-score-ragas.png` & `ragas-0.1.7/docs/_static/traces-score-ragas.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/alfred.py` & `ragas-0.1.7/docs/alfred.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/community/index.md` & `ragas-0.1.7/docs/community/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/feedback.md` & `ragas-0.1.7/docs/concepts/feedback.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/index.md` & `ragas-0.1.7/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics/answer_correctness.md` & `ragas-0.1.7/docs/concepts/metrics/answer_correctness.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics/answer_relevance.md` & `ragas-0.1.7/docs/concepts/metrics/answer_relevance.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Answer Relevance
 
 The evaluation metric, Answer Relevancy, focuses on assessing how pertinent the generated answer is to the given prompt. A lower score is assigned to answers that are incomplete or contain redundant information and higher scores indicate better relevancy. This metric is computed using the `question`, the `context` and the `answer`. 
 
-The Answer Relevancy is defined as the mean cosine similartiy of the orginal `question` to a number of artifical questions, which where generated (reverse engineered) based on the `answer`: 
+The Answer Relevancy is defined as the mean cosine similartiy of the original `question` to a number of artifical questions, which where generated (reverse engineered) based on the `answer`: 
 
 ```{math}
 \text{answer relevancy} = \frac{1}{N} \sum_{i=1}^{N} cos(E_{g_i}, E_o)
 ````
 ```{math}
 \text{answer relevancy} = \frac{1}{N} \sum_{i=1}^{N} \frac{E_{g_i} \cdot E_o}{\|E_{g_i}\|\|E_o\|}
 ````
@@ -62,8 +62,8 @@
   For instance, for the first answer, the LLM might generate the following possible questions:
     - *Question 1:* "In which part of Europe is France located?"
     - *Question 2:* "What is the geographical location of France within Europe?"
     - *Question 3:* "Can you identify the region of Europe where France is situated?"
 
 - **Step 2:** Calculate the mean cosine similarity between the generated questions and the actual question.
 
-The underlying concept is that if the answer correctly addresses the question, it is highly probable that the original question can be reconstructed solely from the answer.
+The underlying concept is that if the answer correctly addresses the question, it is highly probable that the original question can be reconstructed solely from the answer.
```

### Comparing `ragas-0.1.6/docs/concepts/metrics/context_entities_recall.md` & `ragas-0.1.7/docs/concepts/metrics/context_entities_recall.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics/context_precision.md` & `ragas-0.1.7/docs/concepts/metrics/context_precision.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics/context_recall.md` & `ragas-0.1.7/docs/concepts/metrics/context_recall.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics/context_relevancy.md` & `ragas-0.1.7/docs/concepts/metrics/context_relevancy.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics/critique.md` & `ragas-0.1.7/docs/concepts/metrics/critique.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics/faithfulness.md` & `ragas-0.1.7/docs/concepts/metrics/faithfulness.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics/index.md` & `ragas-0.1.7/docs/concepts/metrics/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics/semantic_similarity.md` & `ragas-0.1.7/docs/concepts/metrics/semantic_similarity.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/metrics_driven.md` & `ragas-0.1.7/docs/concepts/metrics_driven.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/prompt_adaptation.md` & `ragas-0.1.7/docs/concepts/prompt_adaptation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/prompts.md` & `ragas-0.1.7/docs/concepts/prompts.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/concepts/testset_generation.md` & `ragas-0.1.7/docs/concepts/testset_generation.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 <p align="center">
 <img src="../_static/imgs/eval-evolve.png" alt="evol-generate" width="600" height="400" />
 </p>
 
 
 ### In-Depth Evolution
 
-Language Language Models (LLMs) possess the capability to transform simple questions into more complex ones effectively. To generate medium to hard samples from the provided documents, we employ the following methods:
+Large Language Models (LLMs) possess the capability to transform simple questions into more complex ones effectively. To generate medium to hard samples from the provided documents, we employ the following methods:
 
 - **Reasoning:** Rewrite the question in a way that enhances the need for reasoning to answer it effectively.
 
 - **Conditioning:** Modify the question to introduce a conditional element, which adds complexity to the question.
 
 - **Multi-Context:** Rephrase the question in a manner that necessitates information from multiple related sections or chunks to formulate an answer.
```

### Comparing `ragas-0.1.6/docs/conf.py` & `ragas-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/getstarted/evaluation.md` & `ragas-0.1.7/docs/getstarted/evaluation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/getstarted/index.md` & `ragas-0.1.7/docs/getstarted/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/getstarted/install.md` & `ragas-0.1.7/docs/getstarted/install.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/getstarted/monitoring.md` & `ragas-0.1.7/docs/getstarted/monitoring.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/getstarted/prepare_data.ipynb` & `ragas-0.1.7/docs/getstarted/prepare_data.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/getstarted/testset_generation.md` & `ragas-0.1.7/docs/getstarted/testset_generation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/applications/compare_embeddings.md` & `ragas-0.1.7/docs/howtos/applications/compare_embeddings.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 distributions = {
     simple: 0.5,
     multi_context: 0.4,
     reasoning: 0.1
 }
 
 # generate testset
-testset = generator.generate_with_llama_index_docs(documents, 100,distributions)
+testset = generator.generate_with_llamaindex_docs(documents, 100,distributions)
 testset.to_pandas()
 ```
 
 <p align="left">
 <img src="../../_static/imgs/testset_output.png" alt="test-outputs" width="800" height="600" />
 </p>
 
@@ -77,16 +77,16 @@
 ```{note}
 refer to [langchain-tutorial](../integrations/langchain.ipynb) see how to evaluate using langchain
 ```
 
 ```{code-block} python
 
 import nest_asyncio
-from llama_index import VectorStoreIndex, SimpleDirectoryReader, ServiceContext,OpenAIEmbedding
-from langchain.embeddings import HuggingFaceEmbeddings
+from llama_index.core import VectorStoreIndex, SimpleDirectoryReader, ServiceContext
+from langchain.embeddings import HuggingFaceEmbeddings, OpenAIEmbeddings
 import pandas as pd
 
 nest_asyncio.apply()
 
 
 def build_query_engine(embed_model):
     vector_index = VectorStoreIndex.from_documents(
@@ -154,8 +154,8 @@
 ```{code-block} python
 result_df = result.to_pandas()
 result_df.head()
 ```
 
 <p align="left">
 <img src="../../_static/imgs/compare-emb-results.png" alt="results" width="800" height="600" />
-</p>
+</p>
```

### Comparing `ragas-0.1.6/docs/howtos/applications/compare_llms.md` & `ragas-0.1.7/docs/howtos/applications/compare_llms.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/applications/custom_prompts.md` & `ragas-0.1.7/docs/howtos/applications/custom_prompts.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/applications/data_preparation.md` & `ragas-0.1.7/docs/howtos/applications/data_preparation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/applications/tracing.md` & `ragas-0.1.7/docs/howtos/applications/tracing.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/applications/use_prompt_adaptation.md` & `ragas-0.1.7/docs/howtos/applications/use_prompt_adaptation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/customisations/aws-bedrock.ipynb` & `ragas-0.1.7/docs/howtos/customisations/aws-bedrock.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/customisations/azure-openai.ipynb` & `ragas-0.1.7/docs/howtos/customisations/azure-openai.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/customisations/bring-your-own-llm-or-embs.md` & `ragas-0.1.7/docs/howtos/customisations/bring-your-own-llm-or-embs.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/customisations/gcp-vertexai.ipynb` & `ragas-0.1.7/docs/howtos/customisations/gcp-vertexai.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/index.md` & `ragas-0.1.7/docs/howtos/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/athina.ipynb` & `ragas-0.1.7/docs/howtos/integrations/athina.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/langchain.ipynb` & `ragas-0.1.7/docs/howtos/integrations/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/langfuse.ipynb` & `ragas-0.1.7/docs/howtos/integrations/langfuse.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/langsmith.ipynb` & `ragas-0.1.7/docs/howtos/integrations/langsmith.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/llamaindex.ipynb` & `ragas-0.1.7/docs/howtos/integrations/llamaindex.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/nyc_wikipedia/nyc_text.txt` & `ragas-0.1.7/docs/howtos/integrations/nyc_wikipedia/nyc_text.txt`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/openlayer.ipynb` & `ragas-0.1.7/docs/howtos/integrations/openlayer.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/ragas-arize.ipynb` & `ragas-0.1.7/docs/howtos/integrations/ragas-arize.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/ragas_haystack.ipynb` & `ragas-0.1.7/docs/howtos/integrations/ragas_haystack.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/tonic-validate.ipynb` & `ragas-0.1.7/docs/howtos/integrations/tonic-validate.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/howtos/integrations/zeno.ipynb` & `ragas-0.1.7/docs/howtos/integrations/zeno.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/index.md` & `ragas-0.1.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/docs/make.bat` & `ragas-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/pyproject.toml` & `ragas-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/references.md` & `ragas-0.1.7/references.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/_analytics.py` & `ragas-0.1.7/src/ragas/_analytics.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/adaptation.py` & `ragas-0.1.7/src/ragas/adaptation.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/async_utils.py` & `ragas-0.1.7/src/ragas/async_utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/callbacks.py` & `ragas-0.1.7/src/ragas/callbacks.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/embeddings/base.py` & `ragas-0.1.7/src/ragas/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/evaluation.py` & `ragas-0.1.7/src/ragas/evaluation.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/exceptions.py` & `ragas-0.1.7/src/ragas/exceptions.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/executor.py` & `ragas-0.1.7/src/ragas/executor.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/integrations/langchain.py` & `ragas-0.1.7/src/ragas/integrations/langchain.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/integrations/langsmith.py` & `ragas-0.1.7/src/ragas/integrations/langsmith.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/llms/base.py` & `ragas-0.1.7/src/ragas/llms/base.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/llms/json_load.py` & `ragas-0.1.7/src/ragas/llms/json_load.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/llms/output_parser.py` & `ragas-0.1.7/src/ragas/llms/output_parser.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/llms/prompt.py` & `ragas-0.1.7/src/ragas/llms/prompt.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/__init__.py` & `ragas-0.1.7/src/ragas/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/_answer_correctness.py` & `ragas-0.1.7/src/ragas/metrics/_answer_correctness.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/_answer_relevance.py` & `ragas-0.1.7/src/ragas/metrics/_answer_relevance.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/_answer_similarity.py` & `ragas-0.1.7/src/ragas/metrics/_answer_similarity.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/_context_entities_recall.py` & `ragas-0.1.7/src/ragas/metrics/_context_entities_recall.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/_context_precision.py` & `ragas-0.1.7/src/ragas/metrics/_context_precision.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/_context_recall.py` & `ragas-0.1.7/src/ragas/metrics/_context_recall.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/_context_relevancy.py` & `ragas-0.1.7/src/ragas/metrics/_context_relevancy.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/_faithfulness.py` & `ragas-0.1.7/src/ragas/metrics/_faithfulness.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/metrics/base.py` & `ragas-0.1.7/src/ragas/metrics/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,21 @@
     return [k for k in keys if k not in ignore_columns]
 
 
 @dataclass
 class Metric(ABC):
     @property
     @abstractmethod
-    def name(self) -> str: ...
+    def name(self) -> str:
+        ...
 
     @property
     @abstractmethod
-    def evaluation_mode(self) -> EvaluationMode: ...
+    def evaluation_mode(self) -> EvaluationMode:
+        ...
 
     @abstractmethod
     def init(self, run_config: RunConfig):
         """
         This method will lazy initialize the model.
         """
         ...
@@ -114,17 +116,16 @@
             raise e
         else:
             if not group_cm.ended:
                 rm.on_chain_end({"output": score})
         return score
 
     @abstractmethod
-    async def _ascore(
-        self, row: t.Dict, callbacks: Callbacks, is_async: bool
-    ) -> float: ...
+    async def _ascore(self, row: t.Dict, callbacks: Callbacks, is_async: bool) -> float:
+        ...
 
 
 @dataclass
 class MetricWithLLM(Metric):
     llm: t.Optional[BaseRagasLLM] = None
 
     def init(self, run_config: RunConfig):
```

### Comparing `ragas-0.1.6/src/ragas/metrics/critique.py` & `ragas-0.1.7/src/ragas/metrics/critique.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/run_config.py` & `ragas-0.1.7/src/ragas/run_config.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/testset/docstore.py` & `ragas-0.1.7/src/ragas/testset/docstore.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/testset/evolutions.py` & `ragas-0.1.7/src/ragas/testset/evolutions.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/testset/extractor.py` & `ragas-0.1.7/src/ragas/testset/extractor.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/testset/filters.py` & `ragas-0.1.7/src/ragas/testset/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import logging
 import typing as t
 from abc import ABC
 from dataclasses import dataclass, field
 
-from ragas.llms.json_load import json_loader
 from ragas.run_config import RunConfig
 from ragas.testset.prompts import (
+    context_scoring_parser,
     context_scoring_prompt,
+    evolution_elimination_parser,
     evolution_elimination_prompt,
     filter_question_prompt,
+    question_filter_parser,
 )
 
 if t.TYPE_CHECKING:
     from ragas.llms.base import BaseRagasLLM
     from ragas.llms.prompt import Prompt
     from ragas.testset.docstore import Node
 
@@ -40,33 +42,29 @@
         Save the filter prompts to a path.
         """
         raise NotImplementedError("save() is not implemented for {} Filter")
 
 
 @dataclass
 class NodeFilter(Filter):
-    threshold: float = 7.5
+    threshold: float = 1.5
     context_scoring_prompt: Prompt = field(
         default_factory=lambda: context_scoring_prompt
     )
 
     async def filter(self, node: Node) -> t.Dict:
         prompt = self.context_scoring_prompt.format(context=node.page_content)
         results = await self.llm.generate(prompt=prompt)
         output = results.generations[0][0].text.strip()
-        score = await json_loader.safe_load(output, llm=self.llm)
-        score_dict = score if isinstance(score, dict) else {}
-        logger.debug("node filter: %s", score)
-        score = score_dict.get("score", 0)
-        try:
-            score = float(score)
-        except Exception as _:
-            score = 0
-        score_dict.update({"score": score >= self.threshold})
-        return score_dict
+        output = await context_scoring_parser.aparse(output, prompt, self.llm)
+        output = output.dict() if output is not None else {}
+        output["score"] = sum(output.values()) / len(output.values())
+        logger.debug("context scoring: %s", output)
+        output.update({"score": output.get("score", 0) >= self.threshold})
+        return output
 
     def adapt(self, language: str, cache_dir: t.Optional[str] = None) -> None:
         """
         Adapt the filter to a different language.
         """
         self.context_scoring_prompt = self.context_scoring_prompt.adapt(
             language, self.llm, cache_dir
@@ -86,18 +84,18 @@
         default_factory=lambda: filter_question_prompt
     )
 
     async def filter(self, question: str) -> t.Tuple[bool, str]:
         prompt = self.filter_question_prompt.format(question=question)
         results = await self.llm.generate(prompt=prompt)
         results = results.generations[0][0].text.strip()
-        json_results = await json_loader.safe_load(results, llm=self.llm)
-        json_results = json_results if isinstance(json_results, dict) else {}
-        logger.debug("filtered question: %s", json_results)
-        return json_results.get("verdict") == "1", json_results.get("feedback", "")
+        results = await question_filter_parser.aparse(results, prompt, self.llm)
+        results = results.dict() if results is not None else {}
+        logger.debug("filtered question: %s", results)
+        return results.get("verdict") == 1, results.get("feedback", "")
 
     def adapt(self, language: str, cache_dir: t.Optional[str] = None) -> None:
         """
         Adapt the filter to a different language.
         """
         self.filter_question_prompt = self.filter_question_prompt.adapt(
             language, self.llm, cache_dir
@@ -119,18 +117,18 @@
 
     async def filter(self, simple_question: str, compressed_question: str) -> bool:
         prompt = self.evolution_elimination_prompt.format(
             question1=simple_question, question2=compressed_question
         )
         results = await self.llm.generate(prompt=prompt)
         results = results.generations[0][0].text.strip()
-        json_results = await json_loader.safe_load(results, llm=self.llm)
-        json_results = json_results if isinstance(json_results, dict) else {}
-        logger.debug("evolution filter: %s", json_results)
-        return json_results.get("verdict") == "1"
+        results = await evolution_elimination_parser.aparse(results, prompt, self.llm)
+        results = results.dict() if results is not None else {}
+        logger.debug("evolution filter: %s", results)
+        return results.get("verdict") == 1
 
     def adapt(self, language: str, cache_dir: t.Optional[str] = None) -> None:
         """
         Adapt the filter to a different language.
         """
         self.evolution_elimination_prompt = self.evolution_elimination_prompt.adapt(
             language, self.llm, cache_dir
```

### Comparing `ragas-0.1.6/src/ragas/testset/generator.py` & `ragas-0.1.7/src/ragas/testset/generator.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/testset/prompts.py` & `ragas-0.1.7/src/ragas/testset/prompts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from langchain_core.pydantic_v1 import BaseModel
+
+from ragas.llms.output_parser import RagasoutputParser, get_json_format_instructions
 from ragas.llms.prompt import Prompt
 
 reasoning_question_prompt = Prompt(
     name="reasoning_question",
     instruction="""Complicate the given question by rewriting question into a multi-hop reasoning question based on the provided context.
     Answering the question should require the reader to make multiple logical connections or inferences using the information available in given context.
     Rules to follow when rewriting question:
@@ -126,156 +129,14 @@
     ],
     input_keys=["question"],
     output_key="output",
     output_type="json",
     language="english",
 )
 
-context_scoring_prompt = Prompt(
-    name="score_context",
-    instruction="""Given a context, perform the following task and output the answer in VALID JSON format:
-    Evaluate the provided context and assign a numerical score between 0 and 10 based on the following criteria:
-      - Clarity and Accuracy: Award a high score to the context that provides accurate and non-misleading information with clarity.
-      - Depth and Innovation: Give extra points to the context that thoroughly delves into the concepts or includes new perspectives and unique insights.
-      - Structure: Award a high score to the context with clear structure and logical flow.
-      - Relevance: Assign a lower score to the context that contains excessive references, acknowledgments, personal information, or other non-essential elements.
-    """,
-    examples=[
-        {
-            "context": "The Pythagorean theorem is a fundamental principle in geometry. It states that in a right-angled triangle, the square of the length of the hypotenuse (the side opposite the right angle) is equal to the sum of the squares of the lengths of the other two sides. This can be written as a^2 + b^2 = c^2 where c represents the length of the hypotenuse, and a and b represent the lengths of the other two sides.",
-            "output": {"score": 8.5},
-        },
-        {
-            "context": "Albert Einstein (14 March 1879 - 18 April 1955) was a German-born theoretical physicist who is widely held to be one of the greatest and most influential scientists of all time.",
-            "output": {"score": 6.0},
-        },
-        {
-            "context": "I love chocolate. It's really tasty. Oh, and by the way, the earth orbits the sun, not the other way around. Also, my favorite color is blue.",
-            "output": {"score": 2.0},
-        },
-    ],
-    input_keys=["context"],
-    output_key="output",
-    output_type="json",
-    language="english",
-)
-
-question_rewrite_prompt = Prompt(
-    name="rewrite_question",
-    instruction="""Given a context, question and feedback, rewrite the question to improve its clarity and answerability based on the feedback provided.""",
-    examples=[
-        {
-            "context": "The Eiffel Tower was constructed using iron and was originally intended as a temporary exhibit for the 1889 World's Fair held in Paris. Despite its initial temporary purpose, the Eiffel Tower quickly became a symbol of Parisian ingenuity and an iconic landmark of the city, attracting millions of visitors each year. The tower's design, created by Gustave Eiffel, was initially met with criticism from some French artists and intellectuals, but it has since been celebrated as a masterpiece of structural engineering and architectural design.",
-            "question": "Who created the design for the Tower?",
-            "feedback": "The question asks about the creator of the design for 'the Tower', but it does not specify which tower it refers to. There are many towers worldwide, and without specifying the exact tower, the question is unclear and unanswerable. To improve the question, it should include the name or a clear description of the specific tower in question.",
-            "output": "Who created the design for the Eiffel Tower?",
-        },
-        {
-            "context": "'Exploring Zero-Shot Learning in Neural Networks' was published by Smith and Lee in 2021, focusing on the application of zero-shot learning techniques in artificial intelligence.",
-            "question": "What datasets were used for the zero-shot evaluations in this study?",
-            "feedback": "The question asks about the datasets used for zero-shot evaluations in 'this study', without specifying or providing any details about the study in question. This makes the question unclear for those who do not have access to or knowledge of the specific study. To improve clarity and answerability, the question should specify the study it refers to, or provide enough context about the study for the question to be understood and answered independently.",
-            "output": "What datasets were used for the zero-shot evaluations Exploring Zero-Shot Learning in Neural Networks paper?",
-        },
-    ],
-    input_keys=["context", "question", "feedback"],
-    output_key="output",
-    output_type="str",
-    language="english",
-)
-
-
-filter_question_prompt = Prompt(
-    name="filter_question",
-    instruction="""
-Asses the given question for clarity and answerability given enough domain knowledge, consider the following criteria:
-1.Independence: Can the question be understood and answered without needing additional context or access to external references not provided within the question itself? Questions should be self-contained, meaning they do not rely on specific documents, tables, or prior knowledge not shared within the question.
-2.Clear Intent: Is it clear what type of answer or information the question seeks? The question should convey its purpose without ambiguity, allowing for a direct and relevant response.
-Based on these criteria, assign a verdict of "1" if a question is specific, independent, and has a clear intent, making it understandable and answerable based on the details provided. Assign "0" if it fails to meet one or more of these criteria due to vagueness, reliance on external references, or ambiguity in intent.
-Provide feedback and a verdict in JSON format, including suggestions for improvement if the question is deemed unclear. Highlight aspects of the question that contribute to its clarity or lack thereof, and offer advice on how it could be reframed or detailed for better understanding and answerability.
-""",
-    examples=[
-        {
-            "question": "What is the discovery about space?",
-            "output": {
-                "feedback": "The question is too vague and broad, asking for a 'discovery about space' without specifying any particular aspect, time frame, or context of interest. This could refer to a wide range of topics, from the discovery of new celestial bodies to advancements in space travel technology. To improve clarity and answerability, the question could specify the type of discovery (e.g., astronomical, technological), the time frame (e.g., recent, historical), or the context (e.g., within a specific research study or space mission).",
-                "verdict": "0",
-            },
-        },
-        {
-            "question": "How does ALMA-13B-R perform compared to other translation models in the WMT'23 study, based on the results in context1 and context2?",
-            "output": {
-                "feedback": "This question asks for a comparison of the ALMA-13B-R model's performance against other translation models within the WMT'23 study, specifically referring to results in 'context1' and 'context2'. While it clearly specifies the model of interest (ALMA-13B-R) and the study (WMT'23), it assumes access to and understanding of 'context1' and 'context2' without explaining what these contexts entail. This makes the question unclear for those not familiar with the WMT'23 study or these specific contexts. To improve clarity and answerability for a broader audience, the question could benefit from defining or describing 'context1' and 'context2' or explaining the criteria used for comparison in these contexts.",
-                "verdict": "0",
-            },
-        },
-        {
-            "question": "How do KIWI-XXL and XCOMET compare to the gold standard references in Table 1 in terms of evaluation scores, translation model performance, and success rate in surpassing the references?",
-            "output": {
-                "feedback": "The question requests a comparison between KIWI-XXL and XCOMET models and gold standard references in 'Table 1', focusing on evaluation scores, translation model performance, and success rates in surpassing the references. It specifies the models and criteria for comparison, making the intent clear. However, the question assumes access to 'Table 1' without providing its content or context, making it unclear for those without direct access to the source material. To be clearer and more answerable for a general audience, the question could include a brief description of the content or key findings of 'Table 1', or alternatively, frame the question in a way that does not rely on specific, unpublished documents.",
-                "verdict": "0",
-            },
-        },
-        {
-            "question": "What is the configuration of UL2 training objective in OpenMoE and why is it a better choice for pre-training?",
-            "output": {
-                "feedback": "The question asks for the configuration of the UL2 training objective within the OpenMoE framework and the rationale behind its suitability for pre-training. It is clear in specifying the topic of interest (UL2 training objective, OpenMoE) and seeks detailed information on both the configuration and the reasons for its effectiveness in pre-training. However, the question might be challenging for those unfamiliar with the specific terminology or the context of OpenMoE and UL2. For broader clarity and answerability, it would be helpful if the question included a brief explanation or context about OpenMoE and the UL2 training objective, or clarified the aspects of pre-training effectiveness it refers to (e.g., efficiency, accuracy, generalization).",
-                "verdict": "1",
-            },
-        },
-        {
-            "question": "What is the detailed configuration of the UL2 training objective in OpenMoE, based on the provided context?",
-            "output": {
-                "feedback": "The question seeks detailed information on the UL2 training objective's configuration within the OpenMoE framework, mentioning 'the provided context' without actually including or describing this context within the query. This makes the question unclear for those who do not have access to the unspecified context. For the question to be clear and answerable, it needs to either include the relevant context directly within the question or be framed in a way that does not require external information. Detailing the specific aspects of the configuration of interest (e.g., loss functions, data augmentation techniques) could also help clarify the query.",
-                "verdict": "0",
-            },
-        },
-    ],
-    input_keys=["question"],
-    output_key="output",
-    output_type="json",
-    language="english",
-)
-
-evolution_elimination_prompt = Prompt(
-    name="evolution_elimination",
-    instruction="""Check if the given two questions are equal based on following requirements:
-    1. They have same constraints and requirements.
-    2. They have same depth and breadth of the inquiry.
-    Output verdict as 1 if they are equal and 0 if they are not""",
-    examples=[
-        {
-            "question1": "What are the primary causes of climate change?",
-            "question2": "What factors contribute to global warming?",
-            "output": {
-                "reason": "While both questions deal with environmental issues, 'climate change' encompasses broader changes than 'global warming', leading to different depths of inquiry.",
-                "verdict": "0",
-            },
-        },
-        {
-            "question1": "How does photosynthesis work in plants?",
-            "question2": "Can you explain the process of photosynthesis in plants?",
-            "output": {
-                "reason": "Both questions ask for an explanation of the photosynthesis process in plants, sharing the same depth, breadth, and requirements for the answer.",
-                "verdict": "1",
-            },
-        },
-        {
-            "question1": "What are the health benefits of regular exercise?",
-            "question2": "Can you list the advantages of exercising regularly for health?",
-            "output": {
-                "reason": "Both questions seek information about the positive effects of regular exercise on health. They require a similar level of detail in listing the health benefits.",
-                "verdict": "1",
-            },
-        },
-    ],
-    input_keys=["question1", "question2"],
-    output_key="output",
-    output_type="json",
-    language="english",
-)
 
 question_answer_prompt = Prompt(
     name="answer_formulate",
     instruction="""Answer the question using the information from the given context. Output verdict as '1' if answer is present '-1' if answer is not present in the context.""",
     examples=[
         {
             "context": """Climate change is significantly influenced by human activities, notably the emission of greenhouse gases from burning fossil fuels. The increased greenhouse gas concentration in the atmosphere traps more heat, leading to global warming and changes in weather patterns.""",
@@ -421,7 +282,202 @@
         },
     ],
     input_keys=["question", "contexts"],
     output_key="output",
     output_type="json",
     language="english",
 )
+
+
+question_rewrite_prompt = Prompt(
+    name="rewrite_question",
+    instruction="""Given a context, question and feedback, rewrite the question to improve its clarity and answerability based on the feedback provided.""",
+    examples=[
+        {
+            "context": "The Eiffel Tower was constructed using iron and was originally intended as a temporary exhibit for the 1889 World's Fair held in Paris. Despite its initial temporary purpose, the Eiffel Tower quickly became a symbol of Parisian ingenuity and an iconic landmark of the city, attracting millions of visitors each year. The tower's design, created by Gustave Eiffel, was initially met with criticism from some French artists and intellectuals, but it has since been celebrated as a masterpiece of structural engineering and architectural design.",
+            "question": "Who created the design for the Tower?",
+            "feedback": "The question asks about the creator of the design for 'the Tower', but it does not specify which tower it refers to. There are many towers worldwide, and without specifying the exact tower, the question is unclear and unanswerable. To improve the question, it should include the name or a clear description of the specific tower in question.",
+            "output": "Who created the design for the Eiffel Tower?",
+        },
+        {
+            "context": "'Exploring Zero-Shot Learning in Neural Networks' was published by Smith and Lee in 2021, focusing on the application of zero-shot learning techniques in artificial intelligence.",
+            "question": "What datasets were used for the zero-shot evaluations in this study?",
+            "feedback": "The question asks about the datasets used for zero-shot evaluations in 'this study', without specifying or providing any details about the study in question. This makes the question unclear for those who do not have access to or knowledge of the specific study. To improve clarity and answerability, the question should specify the study it refers to, or provide enough context about the study for the question to be understood and answered independently.",
+            "output": "What datasets were used for the zero-shot evaluations Exploring Zero-Shot Learning in Neural Networks paper?",
+        },
+    ],
+    input_keys=["context", "question", "feedback"],
+    output_key="output",
+    output_type="str",
+    language="english",
+)
+
+### Filters
+
+
+class ContextScoring(BaseModel):
+    clarity: int
+    depth: int
+    structure: int
+    relevance: int
+
+
+class QuestionFilter(BaseModel):
+    feedback: str
+    verdict: int
+
+
+class EvolutionElimination(BaseModel):
+    reason: str
+    verdict: int
+
+
+context_scoring_parser = RagasoutputParser(pydantic_object=ContextScoring)
+question_filter_parser = RagasoutputParser(pydantic_object=QuestionFilter)
+evolution_elimination_parser = RagasoutputParser(pydantic_object=EvolutionElimination)
+
+context_scoring_prompt = Prompt(
+    name="score_context",
+    instruction="""
+    Given a context, perform the following task and output the answer in VALID JSON format: Assess the provided context and assign a numerical score of 1 (Low), 2 (Medium), or 3 (High) for each of the following criteria in your JSON response:
+
+clarity: Evaluate the precision and understandability of the information presented. High scores (3) are reserved for contexts that are both precise in their information and easy to understand. Low scores (1) are for contexts where the information is vague or hard to comprehend.
+depth: Determine the level of detailed examination and the inclusion of innovative insights within the context. A high score indicates a comprehensive and insightful analysis, while a low score suggests a superficial treatment of the topic.
+structure: Assess how well the content is organized and whether it flows logically. High scores are awarded to contexts that demonstrate coherent organization and logical progression, whereas low scores indicate a lack of structure or clarity in progression.
+relevance: Judge the pertinence of the content to the main topic, awarding high scores to contexts tightly focused on the subject without unnecessary digressions, and low scores to those that are cluttered with irrelevant information.
+Structure your JSON output to reflect these criteria as keys with their corresponding scores as values
+    """,
+    output_format_instruction=get_json_format_instructions(ContextScoring),
+    examples=[
+        {
+            "context": "The Pythagorean theorem is a fundamental principle in geometry. It states that in a right-angled triangle, the square of the length of the hypotenuse (the side opposite the right angle) is equal to the sum of the squares of the lengths of the other two sides. This can be written as a^2 + b^2 = c^2 where c represents the length of the hypotenuse, and a and b represent the lengths of the other two sides.",
+            "output": ContextScoring.parse_obj(
+                {"clarity": 3, "depth": 1, "structure": 3, "relevance": 3}
+            ).dict(),
+        },
+        {
+            "context": "Albert Einstein (14 March 1879 - 18 April 1955) was a German-born theoretical physicist who is widely held to be one of the greatest and most influential scientists of all time.",
+            "output": ContextScoring.parse_obj(
+                {"clarity": 3, "depth": 2, "structure": 3, "relevance": 3}
+            ).dict(),
+        },
+        {
+            "context": "I love chocolate. It's really tasty. Oh, and by the way, the earth orbits the sun, not the other way around. Also, my favorite color is blue.",
+            "output": ContextScoring.parse_obj(
+                {"clarity": 2, "depth": 1, "structure": 1, "relevance": 1}
+            ).dict(),
+        },
+    ],
+    input_keys=["context"],
+    output_key="output",
+    output_type="json",
+    language="english",
+)
+
+
+filter_question_prompt = Prompt(
+    name="filter_question",
+    instruction="""
+Asses the given question for clarity and answerability given enough domain knowledge, consider the following criteria:
+1.Independence: Can the question be understood and answered without needing additional context or access to external references not provided within the question itself? Questions should be self-contained, meaning they do not rely on specific documents, tables, or prior knowledge not shared within the question.
+2.Clear Intent: Is it clear what type of answer or information the question seeks? The question should convey its purpose without ambiguity, allowing for a direct and relevant response.
+Based on these criteria, assign a verdict of "1" if a question is specific, independent, and has a clear intent, making it understandable and answerable based on the details provided. Assign "0" if it fails to meet one or more of these criteria due to vagueness, reliance on external references, or ambiguity in intent.
+Provide feedback and a verdict in JSON format, including suggestions for improvement if the question is deemed unclear. Highlight aspects of the question that contribute to its clarity or lack thereof, and offer advice on how it could be reframed or detailed for better understanding and answerability.
+""",
+    output_format_instruction=get_json_format_instructions(QuestionFilter),
+    examples=[
+        {
+            "question": "What is the discovery about space?",
+            "output": QuestionFilter.parse_obj(
+                {
+                    "feedback": "The question is too vague and broad, asking for a 'discovery about space' without specifying any particular aspect, time frame, or context of interest. This could refer to a wide range of topics, from the discovery of new celestial bodies to advancements in space travel technology. To improve clarity and answerability, the question could specify the type of discovery (e.g., astronomical, technological), the time frame (e.g., recent, historical), or the context (e.g., within a specific research study or space mission).",
+                    "verdict": "0",
+                }
+            ).dict(),
+        },
+        {
+            "question": "How does ALMA-13B-R perform compared to other translation models in the WMT'23 study, based on the results in context1 and context2?",
+            "output": QuestionFilter.parse_obj(
+                {
+                    "feedback": "This question asks for a comparison of the ALMA-13B-R model's performance against other translation models within the WMT'23 study, specifically referring to results in 'context1' and 'context2'. While it clearly specifies the model of interest (ALMA-13B-R) and the study (WMT'23), it assumes access to and understanding of 'context1' and 'context2' without explaining what these contexts entail. This makes the question unclear for those not familiar with the WMT'23 study or these specific contexts. To improve clarity and answerability for a broader audience, the question could benefit from defining or describing 'context1' and 'context2' or explaining the criteria used for comparison in these contexts.",
+                    "verdict": "0",
+                }
+            ).dict(),
+        },
+        {
+            "question": "How do KIWI-XXL and XCOMET compare to the gold standard references in Table 1 in terms of evaluation scores, translation model performance, and success rate in surpassing the references?",
+            "output": QuestionFilter.parse_obj(
+                {
+                    "feedback": "The question requests a comparison between KIWI-XXL and XCOMET models and gold standard references in 'Table 1', focusing on evaluation scores, translation model performance, and success rates in surpassing the references. It specifies the models and criteria for comparison, making the intent clear. However, the question assumes access to 'Table 1' without providing its content or context, making it unclear for those without direct access to the source material. To be clearer and more answerable for a general audience, the question could include a brief description of the content or key findings of 'Table 1', or alternatively, frame the question in a way that does not rely on specific, unpublished documents.",
+                    "verdict": 0,
+                }
+            ).dict(),
+        },
+        {
+            "question": "What is the configuration of UL2 training objective in OpenMoE and why is it a better choice for pre-training?",
+            "output": QuestionFilter.parse_obj(
+                {
+                    "feedback": "The question asks for the configuration of the UL2 training objective within the OpenMoE framework and the rationale behind its suitability for pre-training. It is clear in specifying the topic of interest (UL2 training objective, OpenMoE) and seeks detailed information on both the configuration and the reasons for its effectiveness in pre-training. However, the question might be challenging for those unfamiliar with the specific terminology or the context of OpenMoE and UL2. For broader clarity and answerability, it would be helpful if the question included a brief explanation or context about OpenMoE and the UL2 training objective, or clarified the aspects of pre-training effectiveness it refers to (e.g., efficiency, accuracy, generalization).",
+                    "verdict": 1,
+                }
+            ).dict(),
+        },
+        {
+            "question": "What is the detailed configuration of the UL2 training objective in OpenMoE, based on the provided context?",
+            "output": QuestionFilter.parse_obj(
+                {
+                    "feedback": "The question seeks detailed information on the UL2 training objective's configuration within the OpenMoE framework, mentioning 'the provided context' without actually including or describing this context within the query. This makes the question unclear for those who do not have access to the unspecified context. For the question to be clear and answerable, it needs to either include the relevant context directly within the question or be framed in a way that does not require external information. Detailing the specific aspects of the configuration of interest (e.g., loss functions, data augmentation techniques) could also help clarify the query.",
+                    "verdict": 0,
+                }
+            ).dict(),
+        },
+    ],
+    input_keys=["question"],
+    output_key="output",
+    output_type="json",
+    language="english",
+)
+
+evolution_elimination_prompt = Prompt(
+    name="evolution_elimination",
+    instruction="""Check if the given two questions are equal based on following requirements:
+    1. They have same constraints and requirements.
+    2. They have same depth and breadth of the inquiry.
+    Output verdict as 1 if they are equal and 0 if they are not""",
+    output_format_instruction=get_json_format_instructions(EvolutionElimination),
+    examples=[
+        {
+            "question1": "What are the primary causes of climate change?",
+            "question2": "What factors contribute to global warming?",
+            "output": EvolutionElimination.parse_obj(
+                {
+                    "reason": "While both questions deal with environmental issues, 'climate change' encompasses broader changes than 'global warming', leading to different depths of inquiry.",
+                    "verdict": 0,
+                }
+            ).dict(),
+        },
+        {
+            "question1": "How does photosynthesis work in plants?",
+            "question2": "Can you explain the process of photosynthesis in plants?",
+            "output": EvolutionElimination.parse_obj(
+                {
+                    "reason": "Both questions ask for an explanation of the photosynthesis process in plants, sharing the same depth, breadth, and requirements for the answer.",
+                    "verdict": 1,
+                }
+            ).dict(),
+        },
+        {
+            "question1": "What are the health benefits of regular exercise?",
+            "question2": "Can you list the advantages of exercising regularly for health?",
+            "output": EvolutionElimination.parse_obj(
+                {
+                    "reason": "Both questions seek information about the positive effects of regular exercise on health. They require a similar level of detail in listing the health benefits.",
+                    "verdict": 1,
+                }
+            ).dict(),
+        },
+    ],
+    input_keys=["question1", "question2"],
+    output_key="output",
+    output_type="json",
+    language="english",
+)
```

### Comparing `ragas-0.1.6/src/ragas/utils.py` & `ragas-0.1.7/src/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas/validation.py` & `ragas-0.1.7/src/ragas/validation.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/src/ragas.egg-info/PKG-INFO` & `ragas-0.1.7/src/ragas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.1.6
+Version: 0.1.7
 Description-Content-Type: text/plain
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: datasets
 Requires-Dist: tiktoken
 Requires-Dist: langchain
 Requires-Dist: langchain-core
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.1.6 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.1.7 Description-Content-Type:
 text/plain License-File: LICENSE Requires-Dist: numpy Requires-Dist: datasets
 Requires-Dist: tiktoken Requires-Dist: langchain Requires-Dist: langchain-core
 Requires-Dist: langchain-community Requires-Dist: langchain_openai Requires-
 Dist: openai>1 Requires-Dist: pysbd>=0.3.4 Requires-Dist: nest-asyncio
 Requires-Dist: appdirs Provides-Extra: all Requires-Dist: sentence-
 transformers; extra == "all"
                  ************ [[..//ddooccss//__ssttaattiicc//iimmggss//llooggoo..ppnngg]] ************
```

### Comparing `ragas-0.1.6/src/ragas.egg-info/SOURCES.txt` & `ragas-0.1.7/src/ragas.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 docs/howtos/applications/tracing.md
 docs/howtos/applications/use_prompt_adaptation.md
 docs/howtos/customisations/aws-bedrock.ipynb
 docs/howtos/customisations/azure-openai.ipynb
 docs/howtos/customisations/bring-your-own-llm-or-embs.md
 docs/howtos/customisations/gcp-vertexai.ipynb
 docs/howtos/customisations/index.md
+docs/howtos/customisations/ragas_custom_model.ipynb
 docs/howtos/integrations/athina.ipynb
 docs/howtos/integrations/index.md
 docs/howtos/integrations/langchain.ipynb
 docs/howtos/integrations/langfuse.ipynb
 docs/howtos/integrations/langsmith.ipynb
 docs/howtos/integrations/llamaindex.ipynb
 docs/howtos/integrations/openlayer.ipynb
```

### Comparing `ragas-0.1.6/tests/benchmarks/benchmark_eval.py` & `ragas-0.1.7/tests/benchmarks/benchmark_eval.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/benchmarks/benchmark_testsetgen.py` & `ragas-0.1.7/tests/benchmarks/benchmark_testsetgen.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/benchmarks/utils.py` & `ragas-0.1.7/tests/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/conftest.py` & `ragas-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/unit/llms/test_llm.py` & `ragas-0.1.7/tests/unit/llms/test_llm.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/unit/llms/test_prompt.py` & `ragas-0.1.7/tests/unit/llms/test_prompt.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/unit/test_analytics.py` & `ragas-0.1.7/tests/unit/test_analytics.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/unit/test_import.py` & `ragas-0.1.7/tests/unit/test_import.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/unit/test_validation.py` & `ragas-0.1.7/tests/unit/test_validation.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/unit/testset_generator/test_docstore.py` & `ragas-0.1.7/tests/unit/testset_generator/test_docstore.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/unit/testset_generator/test_document.py` & `ragas-0.1.7/tests/unit/testset_generator/test_document.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.6/tests/unit/testset_generator/test_embs.pkl` & `ragas-0.1.7/tests/unit/testset_generator/test_embs.pkl`

 * *Files identical despite different names*

