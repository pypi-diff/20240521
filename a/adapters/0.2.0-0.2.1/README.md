# Comparing `tmp/adapters-0.2.0.tar.gz` & `tmp/adapters-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapters-0.2.0.tar", last modified: Thu Apr 25 13:46:39 2024, max compression
+gzip compressed data, was "adapters-0.2.1.tar", last modified: Tue May 21 19:15:27 2024, max compression
```

## Comparing `adapters-0.2.0.tar` & `adapters-0.2.1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.923250 adapters-0.2.0/
--rw-rw-rw-   0        0        0    11623 2024-01-27 12:24:34.000000 adapters-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       17 2023-08-25 14:36:57.000000 adapters-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11450 2024-04-25 13:46:39.923250 adapters-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10020 2024-04-25 13:45:33.000000 adapters-0.2.0/README.md
--rw-rw-rw-   0        0        0       60 2023-09-09 08:43:00.000000 adapters-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      875 2024-04-25 13:46:39.925251 adapters-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     4960 2024-04-25 13:45:33.000000 adapters-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.010967 adapters-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.170973 adapters-0.2.0/src/adapters/
--rw-rw-rw-   0        0        0     7343 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/__init__.py
--rw-rw-rw-   0        0        0     9546 2024-02-04 15:11:48.000000 adapters-0.2.0/src/adapters/composition.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.309251 adapters-0.2.0/src/adapters/configuration/
--rw-rw-rw-   0        0        0      156 2023-08-25 14:37:02.000000 adapters-0.2.0/src/adapters/configuration/__init__.py
--rw-rw-rw-   0        0        0    27171 2024-04-24 20:20:10.000000 adapters-0.2.0/src/adapters/configuration/adapter_config.py
--rw-rw-rw-   0        0        0     2743 2023-11-19 13:39:54.000000 adapters-0.2.0/src/adapters/configuration/adapter_fusion_config.py
--rw-rw-rw-   0        0        0     9999 2023-11-19 13:39:54.000000 adapters-0.2.0/src/adapters/configuration/model_adapters_config.py
--rw-rw-rw-   0        0        0     5038 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/context.py
--rw-rw-rw-   0        0        0    21553 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/head_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.359250 adapters-0.2.0/src/adapters/heads/
--rw-rw-rw-   0        0        0      212 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/heads/__init__.py
--rw-rw-rw-   0        0        0    19702 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/heads/base.py
--rw-rw-rw-   0        0        0     6341 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/heads/dependency_parsing.py
--rw-rw-rw-   0        0        0     7658 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/heads/language_modeling.py
--rw-rw-rw-   0        0        0    31796 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/heads/model_mixin.py
--rw-rw-rw-   0        0        0     9657 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/hub_mixin.py
--rw-rw-rw-   0        0        0    40478 2024-02-04 15:11:48.000000 adapters-0.2.0/src/adapters/loading.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.433251 adapters-0.2.0/src/adapters/methods/
--rw-rw-rw-   0        0        0        0 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/methods/__init__.py
--rw-rw-rw-   0        0        0    20866 2024-04-24 20:20:10.000000 adapters-0.2.0/src/adapters/methods/adapter_layer_base.py
--rw-rw-rw-   0        0        0    17156 2024-04-24 20:20:10.000000 adapters-0.2.0/src/adapters/methods/bottleneck.py
--rw-rw-rw-   0        0        0    30112 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/methods/lora.py
--rw-rw-rw-   0        0        0    31696 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/methods/modeling.py
--rw-rw-rw-   0        0        0    24359 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/methods/prefix_tuning.py
--rw-rw-rw-   0        0        0     9516 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/methods/prompt_tuning.py
--rw-rw-rw-   0        0        0     1878 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/methods/utils.py
--rw-rw-rw-   0        0        0    69255 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/model_mixin.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.442249 adapters-0.2.0/src/adapters/models/
--rw-rw-rw-   0        0        0     3969 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.483251 adapters-0.2.0/src/adapters/models/albert/
--rw-rw-rw-   0        0        0     1142 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/albert/__init__.py
--rw-rw-rw-   0        0        0     3921 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/albert/adapter_model.py
--rw-rw-rw-   0        0        0     2760 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/albert/mixin_albert.py
--rw-rw-rw-   0        0        0     6063 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/albert/modeling_albert.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.508249 adapters-0.2.0/src/adapters/models/auto/
--rw-rw-rw-   0        0        0     1251 2024-04-24 20:33:19.000000 adapters-0.2.0/src/adapters/models/auto/__init__.py
--rw-rw-rw-   0        0        0     1542 2024-04-24 20:33:19.000000 adapters-0.2.0/src/adapters/models/auto/adapter_model.py
--rw-rw-rw-   0        0        0      543 2024-04-24 20:33:19.000000 adapters-0.2.0/src/adapters/models/auto/auto_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.546249 adapters-0.2.0/src/adapters/models/bart/
--rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/bart/__init__.py
--rw-rw-rw-   0        0        0     5848 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/bart/adapter_model.py
--rw-rw-rw-   0        0        0     4500 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/bart/mixin_bart.py
--rw-rw-rw-   0        0        0    26766 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/bart/modeling_bart.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.583253 adapters-0.2.0/src/adapters/models/beit/
--rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/beit/__init__.py
--rw-rw-rw-   0        0        0     3121 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/beit/adapter_model.py
--rw-rw-rw-   0        0        0     2424 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/beit/mixin_beit.py
--rw-rw-rw-   0        0        0     5036 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/models/beit/modeling_beit.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.625250 adapters-0.2.0/src/adapters/models/bert/
--rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/bert/__init__.py
--rw-rw-rw-   0        0        0     4663 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/bert/adapter_model.py
--rw-rw-rw-   0        0        0     3608 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/bert/mixin_bert.py
--rw-rw-rw-   0        0        0     8251 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/bert/modeling_bert.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.655253 adapters-0.2.0/src/adapters/models/bert_generation/
--rw-rw-rw-   0        0        0     1547 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/bert_generation/__init__.py
--rw-rw-rw-   0        0        0     4734 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/bert_generation/adapter_model.py
--rw-rw-rw-   0        0        0     8635 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/bert_generation/modeling_bert_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.745252 adapters-0.2.0/src/adapters/models/clip/
--rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/clip/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/clip/adapter_model.py
--rw-rw-rw-   0        0        0     4593 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/clip/mixin_clip.py
--rw-rw-rw-   0        0        0     6843 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/clip/modeling_clip.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.826252 adapters-0.2.0/src/adapters/models/deberta/
--rw-rw-rw-   0        0        0     1144 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/deberta/__init__.py
--rw-rw-rw-   0        0        0     3673 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/deberta/adapter_model.py
--rw-rw-rw-   0        0        0      620 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/deberta/mixin_deberta.py
--rw-rw-rw-   0        0        0     7288 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/deberta/modeling_deberta.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.861251 adapters-0.2.0/src/adapters/models/deberta_v2/
--rw-rw-rw-   0        0        0     1148 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/deberta_v2/__init__.py
--rw-rw-rw-   0        0        0     3698 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/deberta_v2/adapter_model.py
--rw-rw-rw-   0        0        0      858 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/deberta_v2/mixin_deberta_v2.py
--rw-rw-rw-   0        0        0     7388 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/deberta_v2/modeling_deberta_v2.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.899253 adapters-0.2.0/src/adapters/models/distilbert/
--rw-rw-rw-   0        0        0     1150 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/distilbert/__init__.py
--rw-rw-rw-   0        0        0     4876 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/distilbert/adapter_model.py
--rw-rw-rw-   0        0        0     2455 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/distilbert/mixin_distilbert.py
--rw-rw-rw-   0        0        0     6356 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/distilbert/modeling_distilbert.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.925250 adapters-0.2.0/src/adapters/models/electra/
--rw-rw-rw-   0        0        0     1144 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/models/electra/__init__.py
--rw-rw-rw-   0        0        0     4429 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/electra/adapter_model.py
--rw-rw-rw-   0        0        0     7523 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/electra/modeling_electra.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.010251 adapters-0.2.0/src/adapters/models/gpt2/
--rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/gpt2/__init__.py
--rw-rw-rw-   0        0        0     5832 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/gpt2/adapter_model.py
--rw-rw-rw-   0        0        0     2597 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/gpt2/mixin_gpt2.py
--rw-rw-rw-   0        0        0     6480 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/models/gpt2/modeling_gpt2.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.049253 adapters-0.2.0/src/adapters/models/gptj/
--rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/gptj/__init__.py
--rw-rw-rw-   0        0        0     5645 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/gptj/adapter_model.py
--rw-rw-rw-   0        0        0     2394 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/gptj/mixin_gptj.py
--rw-rw-rw-   0        0        0     6291 2023-11-19 13:40:10.000000 adapters-0.2.0/src/adapters/models/gptj/modeling_gptj.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.092251 adapters-0.2.0/src/adapters/models/llama/
--rw-rw-rw-   0        0        0     1140 2023-08-25 14:37:02.000000 adapters-0.2.0/src/adapters/models/llama/__init__.py
--rw-rw-rw-   0        0        0     5922 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/llama/adapter_model.py
--rw-rw-rw-   0        0        0     2493 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/llama/mixin_llama.py
--rw-rw-rw-   0        0        0    18419 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/llama/modeling_llama.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.122249 adapters-0.2.0/src/adapters/models/mbart/
--rw-rw-rw-   0        0        0     1140 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/mbart/__init__.py
--rw-rw-rw-   0        0        0     6319 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/mbart/adapter_model.py
--rw-rw-rw-   0        0        0    15256 2023-11-19 13:40:10.000000 adapters-0.2.0/src/adapters/models/mbart/modeling_mbart.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.154252 adapters-0.2.0/src/adapters/models/mt5/
--rw-rw-rw-   0        0        0     1136 2024-02-04 15:11:48.000000 adapters-0.2.0/src/adapters/models/mt5/__init__.py
--rw-rw-rw-   0        0        0     7911 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/mt5/adapter_model.py
--rw-rw-rw-   0        0        0    21626 2024-02-04 15:11:48.000000 adapters-0.2.0/src/adapters/models/mt5/modeling_mt5.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.300252 adapters-0.2.0/src/adapters/models/roberta/
--rw-rw-rw-   0        0        0     1144 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/roberta/__init__.py
--rw-rw-rw-   0        0        0     4710 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/roberta/adapter_model.py
--rw-rw-rw-   0        0        0     8512 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/roberta/modeling_roberta.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.360253 adapters-0.2.0/src/adapters/models/t5/
--rw-rw-rw-   0        0        0     1134 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/t5/__init__.py
--rw-rw-rw-   0        0        0     7872 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/t5/adapter_model.py
--rw-rw-rw-   0        0        0     5158 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/t5/mixin_t5.py
--rw-rw-rw-   0        0        0    22273 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/t5/modeling_t5.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.428254 adapters-0.2.0/src/adapters/models/vit/
--rw-rw-rw-   0        0        0     1136 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/vit/__init__.py
--rw-rw-rw-   0        0        0     2984 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/vit/adapter_model.py
--rw-rw-rw-   0        0        0     2347 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/vit/mixin_vit.py
--rw-rw-rw-   0        0        0     4697 2023-11-19 13:40:10.000000 adapters-0.2.0/src/adapters/models/vit/modeling_vit.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.460251 adapters-0.2.0/src/adapters/models/xlm_roberta/
--rw-rw-rw-   0        0        0     1150 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/xlm_roberta/__init__.py
--rw-rw-rw-   0        0        0     4760 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/xlm_roberta/adapter_model.py
--rw-rw-rw-   0        0        0     8644 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/xlm_roberta/modeling_xlm_roberta.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.500250 adapters-0.2.0/src/adapters/models/xmod/
--rw-rw-rw-   0        0        0     1138 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/models/xmod/__init__.py
--rw-rw-rw-   0        0        0     5218 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/xmod/adapter_model.py
--rw-rw-rw-   0        0        0     2687 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/xmod/mixin_xmod.py
--rw-rw-rw-   0        0        0     8460 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/xmod/modeling_xmod.py
--rw-rw-rw-   0        0        0    11982 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/trainer.py
--rw-rw-rw-   0        0        0     4193 2023-11-19 13:39:55.000000 adapters-0.2.0/src/adapters/training.py
--rw-rw-rw-   0        0        0    35223 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.544251 adapters-0.2.0/src/adapters/wrappers/
--rw-rw-rw-   0        0        0     1212 2023-08-25 14:37:02.000000 adapters-0.2.0/src/adapters/wrappers/__init__.py
--rw-rw-rw-   0        0        0     3962 2024-01-05 22:29:03.000000 adapters-0.2.0/src/adapters/wrappers/configuration.py
--rw-rw-rw-   0        0        0     5279 2023-09-09 08:42:47.000000 adapters-0.2.0/src/adapters/wrappers/model.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.260967 adapters-0.2.0/src/adapters.egg-info/
--rw-rw-rw-   0        0        0    11450 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5412 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-04 20:36:09.000000 adapters-0.2.0/src/adapters.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1534 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.922255 adapters-0.2.0/tests/
--rw-rw-rw-   0        0        0     4871 2024-04-20 14:48:45.000000 adapters-0.2.0/tests/test_adapter.py
--rw-rw-rw-   0        0        0     1847 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_backward_compability.py
--rw-rw-rw-   0        0        0     5523 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_config.py
--rw-rw-rw-   0        0        0    10792 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_conversion.py
--rw-rw-rw-   0        0        0     3425 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_custom_head.py
--rw-rw-rw-   0        0        0     6882 2024-04-06 16:40:46.000000 adapters-0.2.0/tests/test_adapter_embeddings.py
--rw-rw-rw-   0        0        0     9165 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_fusion_common.py
--rw-rw-rw-   0        0        0     1249 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_fusion_config.py
--rw-rw-rw-   0        0        0    19179 2024-02-17 10:34:53.000000 adapters-0.2.0/tests/test_adapter_heads.py
--rw-rw-rw-   0        0        0     7249 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_hub.py
--rw-rw-rw-   0        0        0     4133 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_save_id2label.py
--rw-rw-rw-   0        0        0    21978 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_trainer.py
--rw-rw-rw-   0        0        0     2012 2023-12-02 11:06:43.000000 adapters-0.2.0/tests/test_albert.py
--rw-rw-rw-   0        0        0     1774 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_bart.py
--rw-rw-rw-   0        0        0     1472 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_beit.py
--rw-rw-rw-   0        0        0     1745 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_bert.py
--rw-rw-rw-   0        0        0     3535 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_bert_generation.py
--rw-rw-rw-   0        0        0     6026 2024-04-20 14:48:45.000000 adapters-0.2.0/tests/test_clip.py
--rw-rw-rw-   0        0        0     1866 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_deberta.py
--rw-rw-rw-   0        0        0     1885 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_debertaV2.py
--rw-rw-rw-   0        0        0     1763 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_distilbert.py
--rw-rw-rw-   0        0        0     1806 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_electra.py
--rw-rw-rw-   0        0        0     3216 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_encoder_decoder.py
--rw-rw-rw-   0        0        0     1685 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_gpt2.py
--rw-rw-rw-   0        0        0     1747 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_gptj.py
--rw-rw-rw-   0        0        0     1816 2024-04-25 13:45:33.000000 adapters-0.2.0/tests/test_llama.py
--rw-rw-rw-   0        0        0     1497 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_mbart.py
--rw-rw-rw-   0        0        0     1687 2024-02-04 15:11:48.000000 adapters-0.2.0/tests/test_mt5.py
--rw-rw-rw-   0        0        0     1660 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_roberta.py
--rw-rw-rw-   0        0        0     1671 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_t5.py
--rw-rw-rw-   0        0        0     1622 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_vit.py
--rw-rw-rw-   0        0        0     1293 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_xlm_roberta.py
--rw-rw-rw-   0        0        0     1617 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_xmod.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.319029 adapters-0.2.1/
+-rw-rw-rw-   0        0        0    11623 2024-01-27 12:24:34.000000 adapters-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-08-25 14:36:57.000000 adapters-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11450 2024-05-21 19:15:27.319029 adapters-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10020 2024-04-25 13:45:33.000000 adapters-0.2.1/README.md
+-rw-rw-rw-   0        0        0       60 2023-09-09 08:43:00.000000 adapters-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      875 2024-05-21 19:15:27.326030 adapters-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     4960 2024-05-21 19:08:12.000000 adapters-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.541516 adapters-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.768028 adapters-0.2.1/src/adapters/
+-rw-rw-rw-   0        0        0     7343 2024-05-21 19:08:40.000000 adapters-0.2.1/src/adapters/__init__.py
+-rw-rw-rw-   0        0        0     9546 2024-02-04 15:11:48.000000 adapters-0.2.1/src/adapters/composition.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.810031 adapters-0.2.1/src/adapters/configuration/
+-rw-rw-rw-   0        0        0      156 2023-08-25 14:37:02.000000 adapters-0.2.1/src/adapters/configuration/__init__.py
+-rw-rw-rw-   0        0        0    27171 2024-05-11 21:05:01.000000 adapters-0.2.1/src/adapters/configuration/adapter_config.py
+-rw-rw-rw-   0        0        0     2743 2023-11-19 13:39:54.000000 adapters-0.2.1/src/adapters/configuration/adapter_fusion_config.py
+-rw-rw-rw-   0        0        0     9999 2023-11-19 13:39:54.000000 adapters-0.2.1/src/adapters/configuration/model_adapters_config.py
+-rw-rw-rw-   0        0        0     5038 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/context.py
+-rw-rw-rw-   0        0        0    21553 2024-04-20 14:48:45.000000 adapters-0.2.1/src/adapters/head_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.819029 adapters-0.2.1/src/adapters/heads/
+-rw-rw-rw-   0        0        0      212 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/heads/__init__.py
+-rw-rw-rw-   0        0        0    19702 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/heads/base.py
+-rw-rw-rw-   0        0        0     6341 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/heads/dependency_parsing.py
+-rw-rw-rw-   0        0        0     7658 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/heads/language_modeling.py
+-rw-rw-rw-   0        0        0    31796 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/heads/model_mixin.py
+-rw-rw-rw-   0        0        0     9657 2024-04-20 14:48:45.000000 adapters-0.2.1/src/adapters/hub_mixin.py
+-rw-rw-rw-   0        0        0    42652 2024-05-11 21:07:29.000000 adapters-0.2.1/src/adapters/loading.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.835029 adapters-0.2.1/src/adapters/methods/
+-rw-rw-rw-   0        0        0        0 2023-11-14 20:50:28.000000 adapters-0.2.1/src/adapters/methods/__init__.py
+-rw-rw-rw-   0        0        0    20866 2024-05-11 21:05:01.000000 adapters-0.2.1/src/adapters/methods/adapter_layer_base.py
+-rw-rw-rw-   0        0        0    17478 2024-05-11 21:07:29.000000 adapters-0.2.1/src/adapters/methods/bottleneck.py
+-rw-rw-rw-   0        0        0    30112 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/methods/lora.py
+-rw-rw-rw-   0        0        0    31696 2024-05-11 21:05:01.000000 adapters-0.2.1/src/adapters/methods/modeling.py
+-rw-rw-rw-   0        0        0    24359 2024-04-20 14:48:45.000000 adapters-0.2.1/src/adapters/methods/prefix_tuning.py
+-rw-rw-rw-   0        0        0     9516 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/methods/prompt_tuning.py
+-rw-rw-rw-   0        0        0     1878 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/methods/utils.py
+-rw-rw-rw-   0        0        0    75265 2024-05-11 21:07:29.000000 adapters-0.2.1/src/adapters/model_mixin.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.836030 adapters-0.2.1/src/adapters/models/
+-rw-rw-rw-   0        0        0     3969 2024-04-20 14:48:45.000000 adapters-0.2.1/src/adapters/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.841029 adapters-0.2.1/src/adapters/models/albert/
+-rw-rw-rw-   0        0        0     1142 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/albert/__init__.py
+-rw-rw-rw-   0        0        0     3921 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/albert/adapter_model.py
+-rw-rw-rw-   0        0        0     2760 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/albert/mixin_albert.py
+-rw-rw-rw-   0        0        0     6063 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/albert/modeling_albert.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.847031 adapters-0.2.1/src/adapters/models/auto/
+-rw-rw-rw-   0        0        0     1251 2024-05-10 10:06:00.000000 adapters-0.2.1/src/adapters/models/auto/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-05-10 10:06:00.000000 adapters-0.2.1/src/adapters/models/auto/adapter_model.py
+-rw-rw-rw-   0        0        0      543 2024-05-10 10:06:00.000000 adapters-0.2.1/src/adapters/models/auto/auto_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.852030 adapters-0.2.1/src/adapters/models/bart/
+-rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.2.1/src/adapters/models/bart/__init__.py
+-rw-rw-rw-   0        0        0     5848 2024-04-20 14:48:45.000000 adapters-0.2.1/src/adapters/models/bart/adapter_model.py
+-rw-rw-rw-   0        0        0     4500 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/bart/mixin_bart.py
+-rw-rw-rw-   0        0        0    26766 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/bart/modeling_bart.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.858029 adapters-0.2.1/src/adapters/models/beit/
+-rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/beit/__init__.py
+-rw-rw-rw-   0        0        0     3121 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/beit/adapter_model.py
+-rw-rw-rw-   0        0        0     2424 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/beit/mixin_beit.py
+-rw-rw-rw-   0        0        0     5036 2023-11-14 20:50:28.000000 adapters-0.2.1/src/adapters/models/beit/modeling_beit.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.886030 adapters-0.2.1/src/adapters/models/bert/
+-rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.2.1/src/adapters/models/bert/__init__.py
+-rw-rw-rw-   0        0        0     4663 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/bert/adapter_model.py
+-rw-rw-rw-   0        0        0     3608 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/bert/mixin_bert.py
+-rw-rw-rw-   0        0        0     8251 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/bert/modeling_bert.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.892031 adapters-0.2.1/src/adapters/models/bert_generation/
+-rw-rw-rw-   0        0        0     1547 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/bert_generation/__init__.py
+-rw-rw-rw-   0        0        0     4734 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/bert_generation/adapter_model.py
+-rw-rw-rw-   0        0        0     8635 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/bert_generation/modeling_bert_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.900030 adapters-0.2.1/src/adapters/models/clip/
+-rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/clip/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/clip/adapter_model.py
+-rw-rw-rw-   0        0        0     4593 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/clip/mixin_clip.py
+-rw-rw-rw-   0        0        0     6843 2024-04-20 14:48:45.000000 adapters-0.2.1/src/adapters/models/clip/modeling_clip.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.905029 adapters-0.2.1/src/adapters/models/deberta/
+-rw-rw-rw-   0        0        0     1144 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/deberta/__init__.py
+-rw-rw-rw-   0        0        0     3673 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/deberta/adapter_model.py
+-rw-rw-rw-   0        0        0      620 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/deberta/mixin_deberta.py
+-rw-rw-rw-   0        0        0     7288 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/deberta/modeling_deberta.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.910031 adapters-0.2.1/src/adapters/models/deberta_v2/
+-rw-rw-rw-   0        0        0     1148 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/deberta_v2/__init__.py
+-rw-rw-rw-   0        0        0     3698 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/deberta_v2/adapter_model.py
+-rw-rw-rw-   0        0        0      858 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/deberta_v2/mixin_deberta_v2.py
+-rw-rw-rw-   0        0        0     7388 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/deberta_v2/modeling_deberta_v2.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.939031 adapters-0.2.1/src/adapters/models/distilbert/
+-rw-rw-rw-   0        0        0     1150 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/distilbert/__init__.py
+-rw-rw-rw-   0        0        0     4876 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/distilbert/adapter_model.py
+-rw-rw-rw-   0        0        0     2455 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/distilbert/mixin_distilbert.py
+-rw-rw-rw-   0        0        0     6356 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/distilbert/modeling_distilbert.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.943031 adapters-0.2.1/src/adapters/models/electra/
+-rw-rw-rw-   0        0        0     1144 2023-11-14 20:50:28.000000 adapters-0.2.1/src/adapters/models/electra/__init__.py
+-rw-rw-rw-   0        0        0     4429 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/electra/adapter_model.py
+-rw-rw-rw-   0        0        0     7523 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/electra/modeling_electra.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.950029 adapters-0.2.1/src/adapters/models/gpt2/
+-rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.2.1/src/adapters/models/gpt2/__init__.py
+-rw-rw-rw-   0        0        0     5832 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/gpt2/adapter_model.py
+-rw-rw-rw-   0        0        0     2597 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/gpt2/mixin_gpt2.py
+-rw-rw-rw-   0        0        0     6480 2023-11-14 20:50:28.000000 adapters-0.2.1/src/adapters/models/gpt2/modeling_gpt2.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.978030 adapters-0.2.1/src/adapters/models/gptj/
+-rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/gptj/__init__.py
+-rw-rw-rw-   0        0        0     5645 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/gptj/adapter_model.py
+-rw-rw-rw-   0        0        0     2394 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/gptj/mixin_gptj.py
+-rw-rw-rw-   0        0        0     6291 2023-11-19 13:40:10.000000 adapters-0.2.1/src/adapters/models/gptj/modeling_gptj.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.027029 adapters-0.2.1/src/adapters/models/llama/
+-rw-rw-rw-   0        0        0     1140 2023-08-25 14:37:02.000000 adapters-0.2.1/src/adapters/models/llama/__init__.py
+-rw-rw-rw-   0        0        0     5922 2024-04-20 14:48:45.000000 adapters-0.2.1/src/adapters/models/llama/adapter_model.py
+-rw-rw-rw-   0        0        0     2493 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/llama/mixin_llama.py
+-rw-rw-rw-   0        0        0    18419 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/llama/modeling_llama.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.052029 adapters-0.2.1/src/adapters/models/mbart/
+-rw-rw-rw-   0        0        0     1140 2023-08-28 09:38:56.000000 adapters-0.2.1/src/adapters/models/mbart/__init__.py
+-rw-rw-rw-   0        0        0     6319 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/mbart/adapter_model.py
+-rw-rw-rw-   0        0        0    15256 2023-11-19 13:40:10.000000 adapters-0.2.1/src/adapters/models/mbart/modeling_mbart.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.061030 adapters-0.2.1/src/adapters/models/mt5/
+-rw-rw-rw-   0        0        0     1136 2024-02-04 15:11:48.000000 adapters-0.2.1/src/adapters/models/mt5/__init__.py
+-rw-rw-rw-   0        0        0     7911 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/mt5/adapter_model.py
+-rw-rw-rw-   0        0        0    21626 2024-02-04 15:11:48.000000 adapters-0.2.1/src/adapters/models/mt5/modeling_mt5.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.126030 adapters-0.2.1/src/adapters/models/roberta/
+-rw-rw-rw-   0        0        0     1144 2023-08-28 09:38:56.000000 adapters-0.2.1/src/adapters/models/roberta/__init__.py
+-rw-rw-rw-   0        0        0     4710 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/roberta/adapter_model.py
+-rw-rw-rw-   0        0        0     8512 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/roberta/modeling_roberta.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.155030 adapters-0.2.1/src/adapters/models/t5/
+-rw-rw-rw-   0        0        0     1134 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/t5/__init__.py
+-rw-rw-rw-   0        0        0     7872 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/t5/adapter_model.py
+-rw-rw-rw-   0        0        0     5158 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/t5/mixin_t5.py
+-rw-rw-rw-   0        0        0    22273 2024-04-20 14:48:45.000000 adapters-0.2.1/src/adapters/models/t5/modeling_t5.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.188031 adapters-0.2.1/src/adapters/models/vit/
+-rw-rw-rw-   0        0        0     1136 2023-08-25 14:37:00.000000 adapters-0.2.1/src/adapters/models/vit/__init__.py
+-rw-rw-rw-   0        0        0     2984 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/vit/adapter_model.py
+-rw-rw-rw-   0        0        0     2347 2024-04-25 13:45:33.000000 adapters-0.2.1/src/adapters/models/vit/mixin_vit.py
+-rw-rw-rw-   0        0        0     4697 2023-11-19 13:40:10.000000 adapters-0.2.1/src/adapters/models/vit/modeling_vit.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.200031 adapters-0.2.1/src/adapters/models/xlm_roberta/
+-rw-rw-rw-   0        0        0     1150 2023-08-28 09:38:56.000000 adapters-0.2.1/src/adapters/models/xlm_roberta/__init__.py
+-rw-rw-rw-   0        0        0     4760 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/xlm_roberta/adapter_model.py
+-rw-rw-rw-   0        0        0     8644 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/xlm_roberta/modeling_xlm_roberta.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.210030 adapters-0.2.1/src/adapters/models/xmod/
+-rw-rw-rw-   0        0        0     1138 2023-11-14 20:50:28.000000 adapters-0.2.1/src/adapters/models/xmod/__init__.py
+-rw-rw-rw-   0        0        0     5218 2024-02-17 10:34:53.000000 adapters-0.2.1/src/adapters/models/xmod/adapter_model.py
+-rw-rw-rw-   0        0        0     2687 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/xmod/mixin_xmod.py
+-rw-rw-rw-   0        0        0     8460 2023-11-20 14:39:51.000000 adapters-0.2.1/src/adapters/models/xmod/modeling_xmod.py
+-rw-rw-rw-   0        0        0    12091 2024-05-11 21:07:29.000000 adapters-0.2.1/src/adapters/trainer.py
+-rw-rw-rw-   0        0        0     4193 2023-11-19 13:39:55.000000 adapters-0.2.1/src/adapters/training.py
+-rw-rw-rw-   0        0        0    35509 2024-05-11 21:07:29.000000 adapters-0.2.1/src/adapters/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.217031 adapters-0.2.1/src/adapters/wrappers/
+-rw-rw-rw-   0        0        0     1212 2023-08-25 14:37:02.000000 adapters-0.2.1/src/adapters/wrappers/__init__.py
+-rw-rw-rw-   0        0        0     3962 2024-01-05 22:29:03.000000 adapters-0.2.1/src/adapters/wrappers/configuration.py
+-rw-rw-rw-   0        0        0     5279 2023-09-09 08:42:47.000000 adapters-0.2.1/src/adapters/wrappers/model.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:26.805029 adapters-0.2.1/src/adapters.egg-info/
+-rw-rw-rw-   0        0        0    11450 2024-05-21 19:15:25.000000 adapters-0.2.1/src/adapters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5412 2024-05-21 19:15:26.000000 adapters-0.2.1/src/adapters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:15:25.000000 adapters-0.2.1/src/adapters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-04 20:36:09.000000 adapters-0.2.1/src/adapters.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     1534 2024-05-21 19:15:25.000000 adapters-0.2.1/src/adapters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 19:15:25.000000 adapters-0.2.1/src/adapters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 19:15:27.318030 adapters-0.2.1/tests/
+-rw-rw-rw-   0        0        0     4871 2024-04-20 14:48:45.000000 adapters-0.2.1/tests/test_adapter.py
+-rw-rw-rw-   0        0        0     1847 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_adapter_backward_compability.py
+-rw-rw-rw-   0        0        0     5523 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_adapter_config.py
+-rw-rw-rw-   0        0        0    10792 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_adapter_conversion.py
+-rw-rw-rw-   0        0        0     3425 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_adapter_custom_head.py
+-rw-rw-rw-   0        0        0     6882 2024-04-06 16:40:46.000000 adapters-0.2.1/tests/test_adapter_embeddings.py
+-rw-rw-rw-   0        0        0     9165 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_adapter_fusion_common.py
+-rw-rw-rw-   0        0        0     1249 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_adapter_fusion_config.py
+-rw-rw-rw-   0        0        0    19179 2024-02-17 10:34:53.000000 adapters-0.2.1/tests/test_adapter_heads.py
+-rw-rw-rw-   0        0        0     7249 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_adapter_hub.py
+-rw-rw-rw-   0        0        0     4133 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_adapter_save_id2label.py
+-rw-rw-rw-   0        0        0    21978 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_adapter_trainer.py
+-rw-rw-rw-   0        0        0     2012 2023-12-02 11:06:43.000000 adapters-0.2.1/tests/test_albert.py
+-rw-rw-rw-   0        0        0     1774 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_bart.py
+-rw-rw-rw-   0        0        0     1472 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_beit.py
+-rw-rw-rw-   0        0        0     1745 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_bert.py
+-rw-rw-rw-   0        0        0     3535 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_bert_generation.py
+-rw-rw-rw-   0        0        0     6026 2024-04-20 14:48:45.000000 adapters-0.2.1/tests/test_clip.py
+-rw-rw-rw-   0        0        0     1866 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_deberta.py
+-rw-rw-rw-   0        0        0     1885 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_debertaV2.py
+-rw-rw-rw-   0        0        0     1763 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_distilbert.py
+-rw-rw-rw-   0        0        0     1806 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_electra.py
+-rw-rw-rw-   0        0        0     3216 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_encoder_decoder.py
+-rw-rw-rw-   0        0        0     1685 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_gpt2.py
+-rw-rw-rw-   0        0        0     1747 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_gptj.py
+-rw-rw-rw-   0        0        0     1816 2024-04-25 13:45:33.000000 adapters-0.2.1/tests/test_llama.py
+-rw-rw-rw-   0        0        0     1497 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_mbart.py
+-rw-rw-rw-   0        0        0     1687 2024-02-04 15:11:48.000000 adapters-0.2.1/tests/test_mt5.py
+-rw-rw-rw-   0        0        0     1660 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_roberta.py
+-rw-rw-rw-   0        0        0     1671 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_t5.py
+-rw-rw-rw-   0        0        0     1622 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_vit.py
+-rw-rw-rw-   0        0        0     1293 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_xlm_roberta.py
+-rw-rw-rw-   0        0        0     1617 2023-11-20 14:39:51.000000 adapters-0.2.1/tests/test_xmod.py
```

### Comparing `adapters-0.2.0/LICENSE` & `adapters-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/PKG-INFO` & `adapters-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapters
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Unified Library for Parameter-Efficient and Modular Transfer Learning
 Home-page: https://github.com/adapter-hub/adapters
 Author: The AdapterHub team and community contributors
 Author-email: calpt@mail.de
 License: Apache
 Keywords: NLP deep learning transformer pytorch BERT adapters
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adapters Version: 0.2.0 Summary: A Unified Library
+Metadata-Version: 2.1 Name: adapters Version: 0.2.1 Summary: A Unified Library
 for Parameter-Efficient and Modular Transfer Learning Home-page: https://
 github.com/adapter-hub/adapters Author: The AdapterHub team and community
 contributors Author-email: calpt@mail.de License: Apache Keywords: NLP deep
 learning transformer pytorch BERT adapters Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

### Comparing `adapters-0.2.0/README.md` & `adapters-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/setup.cfg` & `adapters-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/setup.py` & `adapters-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 # when modifying the following list, make sure to update src/transformers/dependency_versions_check.py
 install_requires = [
     deps["transformers"],
 ]
 
 setup(
     name="adapters",
-    version="0.2.0",
+    version="0.2.1",
     author="The AdapterHub team and community contributors",
     author_email="calpt@mail.de",
     description="A Unified Library for Parameter-Efficient and Modular Transfer Learning",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="NLP deep learning transformer pytorch BERT adapters",
     license="Apache",
```

### Comparing `adapters-0.2.0/src/adapters/__init__.py` & `adapters-0.2.1/src/adapters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 from typing import TYPE_CHECKING
 
 from transformers.utils import _LazyModule
 
 
 _import_structure = {
```

### Comparing `adapters-0.2.0/src/adapters/composition.py` & `adapters-0.2.1/src/adapters/composition.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/configuration/adapter_config.py` & `adapters-0.2.1/src/adapters/configuration/adapter_config.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/configuration/adapter_fusion_config.py` & `adapters-0.2.1/src/adapters/configuration/adapter_fusion_config.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/configuration/model_adapters_config.py` & `adapters-0.2.1/src/adapters/configuration/model_adapters_config.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/context.py` & `adapters-0.2.1/src/adapters/context.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/head_utils.py` & `adapters-0.2.1/src/adapters/head_utils.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/heads/base.py` & `adapters-0.2.1/src/adapters/heads/base.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/heads/dependency_parsing.py` & `adapters-0.2.1/src/adapters/heads/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/heads/language_modeling.py` & `adapters-0.2.1/src/adapters/heads/language_modeling.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/heads/model_mixin.py` & `adapters-0.2.1/src/adapters/heads/model_mixin.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/hub_mixin.py` & `adapters-0.2.1/src/adapters/hub_mixin.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/loading.py` & `adapters-0.2.1/src/adapters/loading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,60 @@
 import json
 import logging
 from abc import ABC, abstractmethod
 from os import mkdir
 from os.path import exists, isdir, isfile, join
-from typing import Callable, Mapping, Sequence, Tuple
+from typing import Callable, Mapping, Optional, Sequence, Tuple
 
 import torch
 
+
+try:
+    from safetensors.torch import load_file, save_file
+
+    safetensors_available = True
+except ImportError:
+    safetensors_available = False
+
 from .configuration import AdapterConfig, build_full_config
 from .head_utils import STATIC_TO_FLEX_HEAD_MAP, get_head_config_and_rename_list
 from .utils import (
     ACTIVATION_RENAME,
     ADAPTERFUSION_CONFIG_NAME,
     ADAPTERFUSION_WEIGHTS_NAME,
     CONFIG_NAME,
     HEAD_CONFIG_NAME,
     HEAD_WEIGHTS_NAME,
+    SAFE_ADAPTERFUSION_WEIGHTS_NAME,
+    SAFE_HEAD_WEIGHTS_NAME,
+    SAFE_WEIGHTS_NAME,
     WEIGHTS_NAME,
     AdapterType,
     resolve_adapter_path,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 class WeightsLoaderHelper:
     """
     A class providing helper methods for saving and loading module weights.
     """
 
-    def __init__(self, model, weights_name, config_name):
+    def __init__(
+        self, model, weights_name, config_name, use_safetensors: bool = False, safe_weights_name: Optional[str] = None
+    ):
         self.model = model
         self.weights_name = weights_name
         self.config_name = config_name
+        self.use_safetensors = use_safetensors
+        if use_safetensors and not safetensors_available:
+            raise ValueError("Safetensors package not available. Please install via `pip install safetensors`.")
+        self.safe_weights_name = safe_weights_name or weights_name
 
     def state_dict(self, filter_func):
         return {k: v for (k, v) in self.model.state_dict().items() if filter_func(k)}
 
     def rename_state_dict(self, state_dict, *rename_funcs):
         new_state_dict = {}
         for k, v in state_dict.items():
@@ -64,16 +81,20 @@
             mkdir(save_directory)
         else:
             assert isdir(save_directory), "Saving path should be a directory where the module weights can be saved."
 
         # Get the state of all adapter modules for this task
         state_dict = self.state_dict(filter_func)
         # Save the adapter weights
-        output_file = join(save_directory, self.weights_name)
-        torch.save(state_dict, output_file)
+        if self.use_safetensors:
+            output_file = join(save_directory, self.safe_weights_name)
+            save_file(state_dict, output_file)
+        else:
+            output_file = join(save_directory, self.weights_name)
+            torch.save(state_dict, output_file)
         logger.info("Module weights saved in {}".format(output_file))
 
     def load_weights_config(self, save_directory):
         config_file = join(save_directory, self.config_name)
         logger.info("Loading module configuration from {}".format(config_file))
         # Load the config
         with open(config_file, "r", encoding="utf-8") as f:
@@ -125,18 +146,27 @@
         self,
         save_directory,
         filter_func,
         rename_func=None,
         loading_info=None,
         in_base_model=False,
     ):
-        weights_file = join(save_directory, self.weights_name)
         # Load the weights of the adapter
         try:
-            state_dict = torch.load(weights_file, map_location="cpu")
+            if self.use_safetensors:
+                weights_file = join(save_directory, self.safe_weights_name)
+                if exists(weights_file):
+                    state_dict = load_file(weights_file, device="cpu")
+                else:
+                    logger.info(f"No safetensors file found in {save_directory}. Falling back to torch.load...")
+                    weights_file = join(save_directory, self.weights_name)
+                    state_dict = torch.load(weights_file, map_location="cpu")
+            else:
+                weights_file = join(save_directory, self.weights_name)
+                state_dict = torch.load(weights_file, map_location="cpu")
         except Exception:
             raise OSError("Unable to load weights from pytorch checkpoint file. ")
         logger.info("Loading module weights from {}".format(weights_file))
 
         return self.load_weights_from_state_dict(
             state_dict, filter_func, rename_func=rename_func, loading_info=loading_info, in_base_model=in_base_model
         )
@@ -189,17 +219,21 @@
 
 class WeightsLoader(ABC):
     """
     An abstract class providing basic methods for saving and loading weights of a model. Extend this class to build
     custom module weight loaders.
     """
 
-    def __init__(self, model, weights_name, config_name):
+    def __init__(
+        self, model, weights_name, config_name, use_safetensors: bool = False, safe_weights_name: Optional[str] = None
+    ):
         self.model = model
-        self.weights_helper = WeightsLoaderHelper(model, weights_name, config_name)
+        self.weights_helper = WeightsLoaderHelper(
+            model, weights_name, config_name, use_safetensors=use_safetensors, safe_weights_name=safe_weights_name
+        )
 
     @abstractmethod
     def filter_func(self, name: str) -> Callable[[str], bool]:
         """
         The callable returned by this method is used to extract the module weights to be saved or loaded based on their
         names.
 
@@ -295,16 +329,18 @@
 class AdapterLoader(WeightsLoader):
     """
     A class providing methods for saving and loading adapter modules from the Hub, the filesystem or a remote url.
 
     Model classes passed to this loader must implement the `ModelAdaptersMixin` class.
     """
 
-    def __init__(self, model, adapter_type=None):
-        super().__init__(model, WEIGHTS_NAME, CONFIG_NAME)
+    def __init__(self, model, adapter_type=None, use_safetensors: bool = False):
+        super().__init__(
+            model, WEIGHTS_NAME, CONFIG_NAME, use_safetensors=use_safetensors, safe_weights_name=SAFE_WEIGHTS_NAME
+        )
         self.adapter_type = adapter_type
         if adapter_type and not AdapterType.has(self.adapter_type):
             raise ValueError("Invalid adapter type {}".format(self.adapter_type))
 
     def filter_func(self, adapter_name):
         return (
             lambda x: "_adapters.{}.".format(adapter_name) in x
@@ -536,16 +572,22 @@
 
 class AdapterFusionLoader(WeightsLoader):
     """
     A class providing methods for saving and loading AdapterFusion modules from the file system.
 
     """
 
-    def __init__(self, model, error_on_missing=True):
-        super().__init__(model, ADAPTERFUSION_WEIGHTS_NAME, ADAPTERFUSION_CONFIG_NAME)
+    def __init__(self, model, error_on_missing=True, use_safetensors: bool = False):
+        super().__init__(
+            model,
+            ADAPTERFUSION_WEIGHTS_NAME,
+            ADAPTERFUSION_CONFIG_NAME,
+            use_safetensors=use_safetensors,
+            safe_weights_name=SAFE_ADAPTERFUSION_WEIGHTS_NAME,
+        )
         self.error_on_missing = error_on_missing
 
     def filter_func(self, adapter_fusion_name):
         return lambda x: "adapter_fusion_layer.{}".format(adapter_fusion_name) in x
 
     def rename_func(self, old_name, new_name):
         return lambda k: k.replace(
@@ -657,15 +699,17 @@
             save_directory (str): The directory from where to load the weights.
             load_as (str, optional): Load the weights with this name. Defaults to None.
 
         Returns:
             Tuple[str, str]: A tuple consisting of the local file system directory from which the weights where loaded
             and the name of the loaded weights.
         """
-        if not exists(join(save_directory, ADAPTERFUSION_WEIGHTS_NAME)):
+        if not exists(join(save_directory, ADAPTERFUSION_WEIGHTS_NAME)) and not exists(
+            join(save_directory, SAFE_ADAPTERFUSION_WEIGHTS_NAME)
+        ):
             if self.error_on_missing:
                 raise ValueError("Loading path should be a directory where AdapterFusion is saved.")
             else:
                 logger.debug("No matching adapter fusion found in '{}'".format(save_directory))
                 return None, None
 
         config = self.weights_helper.load_weights_config(save_directory)
@@ -695,16 +739,22 @@
     """
     A class providing methods for saving and loading prediction head modules from the file system.
 
     Model classes supporting configurable head modules via config files should provide a prediction head dict at
     `model.heads` and a method `add_prediction_head(head_name, config)`.
     """
 
-    def __init__(self, model, error_on_missing=True, convert_to_flex_head=False):
-        super().__init__(model, HEAD_WEIGHTS_NAME, HEAD_CONFIG_NAME)
+    def __init__(self, model, error_on_missing=True, convert_to_flex_head=False, use_safetensors: bool = False):
+        super().__init__(
+            model,
+            HEAD_WEIGHTS_NAME,
+            HEAD_CONFIG_NAME,
+            use_safetensors=use_safetensors,
+            safe_weights_name=SAFE_HEAD_WEIGHTS_NAME,
+        )
         self.error_on_missing = error_on_missing
         self.convert_to_flex_head = convert_to_flex_head
 
     def filter_func(self, head_name):
         # ToDo remove this workaround
         if self.model.config.model_type in ["t5", "mt5"]:
             if head_name:
@@ -791,15 +841,17 @@
             save_directory (str): The directory from where to load the weights.
             load_as (str, optional): Load the weights with this name. Defaults to None.
 
         Returns:
             Tuple[str, str]: A tuple consisting of the local file system directory from which the weights where loaded
             and the name of the loaded weights.
         """
-        if not exists(join(save_directory, HEAD_WEIGHTS_NAME)):
+        if not exists(join(save_directory, HEAD_WEIGHTS_NAME)) and not exists(
+            join(save_directory, SAFE_HEAD_WEIGHTS_NAME)
+        ):
             if self.error_on_missing:
                 raise ValueError("Loading path should be a directory where the head is saved.")
             else:
                 logger.info("No matching prediction head found in '{}'".format(save_directory))
                 return None, None
         # label2id map used to override default
         custom_id2label = kwargs.pop("id2label", None)
```

### Comparing `adapters-0.2.0/src/adapters/methods/adapter_layer_base.py` & `adapters-0.2.1/src/adapters/methods/adapter_layer_base.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/methods/bottleneck.py` & `adapters-0.2.1/src/adapters/methods/bottleneck.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,21 @@
 
     def get_adapter(self, adapter_name: str):
         if adapter_name in self.adapters:
             return self.adapters[adapter_name]
         else:
             return None
 
+    def get_adapter_fusion(self, adapter_names: Union[List, str]):
+        adapter_names = adapter_names if isinstance(adapter_names, str) else ",".join(adapter_names)
+        if adapter_names in self.adapter_fusion_layer:
+            return self.adapter_fusion_layer[adapter_names]
+        else:
+            return None
+
     def pre_block(self, adapter_setup: Union[AdapterCompositionBlock, str], state: BottleneckState) -> BottleneckState:
         if isinstance(adapter_setup, AdapterCompositionBlock):
             adapter_name = adapter_setup.first()
         else:
             adapter_name = adapter_setup
         first_adapter = self.adapters[adapter_name]
         hidden_states, _, residual = first_adapter.pre_forward(
```

### Comparing `adapters-0.2.0/src/adapters/methods/lora.py` & `adapters-0.2.1/src/adapters/methods/lora.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/methods/modeling.py` & `adapters-0.2.1/src/adapters/methods/modeling.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/methods/prefix_tuning.py` & `adapters-0.2.1/src/adapters/methods/prefix_tuning.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/methods/prompt_tuning.py` & `adapters-0.2.1/src/adapters/methods/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/methods/utils.py` & `adapters-0.2.1/src/adapters/methods/utils.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/model_mixin.py` & `adapters-0.2.1/src/adapters/model_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -701,61 +701,65 @@
 
     def save_adapter(
         self,
         save_directory: str,
         adapter_name: str,
         meta_dict: dict = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
+        use_safetensors: bool = False,
     ):
         """
         Saves an adapter and its configuration file to a directory so that it can be shared or reloaded using
         `load_adapter()`.
 
         Args:
             save_directory (str): Path to a directory where the adapter should be saved.
             adapter_name (str): Name of the adapter to be saved.
+            use_safetensors (bool, optional): If True, weights are saved via `safetensors`. Otherwise, the regular torch save method is used.
 
         Raises:
             ValueError: If the given adapter name is invalid.
         """
-        loader = AdapterLoader(self)
+        loader = AdapterLoader(self, use_safetensors=use_safetensors)
         loader.save(save_directory, adapter_name, meta_dict)
         # save additional custom weights
         if custom_weights_loaders:
             for weights_loader in custom_weights_loaders:
                 weights_loader.save(save_directory, adapter_name)
 
     def save_adapter_fusion(
         self,
         save_directory: str,
         adapter_names: Union[Fuse, list, str],
         meta_dict: dict = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
+        use_safetensors: bool = False,
     ):
         """
         Saves an AdapterFusion layer and its configuration file to a directory so that it can be shared or reloaded
         using `load_adapter_fusion()`.
 
         Args:
             save_directory (str): Path to a directory where the AdapterFusion should be saved.
             adapter_names (Union[Fuse, list, str]): AdapterFusion to be saved.
+            use_safetensors (bool, optional): If True, weights are saved via `safetensors`. Otherwise, the regular torch save method is used.
 
         Raises:
             ValueError: If the given AdapterFusion name is invalid.
         """
         if isinstance(adapter_names, Fuse):
             adapter_fusion_name = ",".join(adapter_names.children)
         elif isinstance(adapter_names, list):
             adapter_fusion_name = ",".join(adapter_names)
         elif isinstance(adapter_names, str):
             adapter_fusion_name = adapter_names
         else:
             raise ValueError("Invalid AdapterFusion definition: {}".format(adapter_names))
 
-        loader = AdapterFusionLoader(self)
+        loader = AdapterFusionLoader(self, use_safetensors=use_safetensors)
         loader.save(save_directory, adapter_fusion_name, meta_dict)
         # save additional custom weights
         if custom_weights_loaders:
             for weights_loader in custom_weights_loaders:
                 weights_loader.save(save_directory, adapter_fusion_name)
 
     def load_adapter(
@@ -766,14 +770,15 @@
         model_name: str = None,
         load_as: str = None,
         source: str = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
         leave_out: Optional[List[int]] = None,
         id2label=None,
         set_active: bool = False,
+        use_safetensors: bool = False,
         **kwargs
     ) -> str:
         """
         Loads a pre-trained pytorch adapter module from the local file system or a remote location.
 
         Args:
             adapter_name_or_path (str): can be either:
@@ -793,19 +798,20 @@
                 - "ah" (default): search on AdapterHub.
                 - "hf": search on HuggingFace model hub.
                 - None: search on all sources
             leave_out: Dynamically drop adapter modules in the specified Transformer layers when loading the adapter.
             set_active (bool, optional):
                 Set the loaded adapter to be the active one. By default (False), the adapter is loaded but not
                 activated.
+            use_safetensors (bool, optional): If True, weights are loaded via `safetensors` if safetensors checkpoint is available. Otherwise, the regular torch save method is used.
 
         Returns:
             str: The name with which the adapter was added to the model.
         """
-        loader = AdapterLoader(self)
+        loader = AdapterLoader(self, use_safetensors=use_safetensors)
         load_dir, load_name = loader.load(
             adapter_name_or_path,
             config,
             version,
             model_name,
             load_as,
             source=source,
@@ -828,32 +834,34 @@
 
     def load_adapter_fusion(
         self,
         adapter_fusion_name_or_path: str,
         load_as: str = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
         set_active: bool = False,
+        use_safetensors: bool = False,
         **kwargs
     ) -> str:
         """
         Loads a pre-trained AdapterFusion layer from the local file system.
 
         Args:
             adapter_fusion_name_or_path (str):
                 a path to a directory containing AdapterFusion weights saved using `model.save_adapter_fusion()`.
             load_as (str, optional): Load the AdapterFusion using this name.
                     By default, the name with which the AdapterFusion layer was saved will be used.
             set_active (bool, optional):
                 Activate the loaded AdapterFusion. By default (False), the AdapterFusion is loaded but not activated.
+            use_safetensors (bool, optional): If True, weights are loaded via `safetensors` if safetensors checkpoint is available. Otherwise, the regular torch save method is used.
 
         Returns:
             str: The name with which the AdapterFusion was added to the model.
         """
 
-        loader = AdapterFusionLoader(self)
+        loader = AdapterFusionLoader(self, use_safetensors=use_safetensors)
         load_dir, load_name = loader.load(adapter_fusion_name_or_path, load_as, set_active=set_active)
         # load additional custom weights
         if custom_weights_loaders:
             for weights_loader in custom_weights_loaders:
                 weights_loader.load(
                     load_dir,
                     load_as=load_as,
@@ -864,56 +872,70 @@
         return load_name
 
     def save_all_adapters(
         self,
         save_directory: str,
         meta_dict: dict = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
+        use_safetensors: bool = False,
     ):
         """
         Saves all adapters of this model together with their configuration to subfolders of the given location.
 
         Args:
             save_directory (str): Path to a directory where the adapters should be saved.
+            use_safetensors (bool, optional): If True, weights are saved via `safetensors`. Otherwise, the regular torch save method is used.
         """
         os.makedirs(save_directory, exist_ok=True)
         for name in self.adapters_config:
             adapter_config = self.adapters_config.get(name)
             h = get_adapter_config_hash(adapter_config)
             save_path = join(save_directory, name)
             if meta_dict:
                 meta_dict.update({"config_id": h})
             else:
                 meta_dict = {"config_id": h}
-            self.save_adapter(save_path, name, meta_dict=meta_dict, custom_weights_loaders=custom_weights_loaders)
+            self.save_adapter(
+                save_path,
+                name,
+                meta_dict=meta_dict,
+                custom_weights_loaders=custom_weights_loaders,
+                use_safetensors=use_safetensors,
+            )
 
     def save_all_adapter_fusions(
         self,
         save_directory: str,
         meta_dict: dict = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
+        use_safetensors: bool = False,
     ):
         """
         Saves all AdapterFusion layers of this model together with their configuration to subfolders of the given
         location.
 
         Args:
             save_directory (str): Path to a directory where the AdapterFusion layers should be saved.
+            use_safetensors (bool, optional): If True, weights are saved via `safetensors`. Otherwise, the regular torch save method is used.
         """
         os.makedirs(save_directory, exist_ok=True)
         for name in self.adapters_config.fusions:
             adapter_fusion_config = self.adapters_config.get_fusion(name)
             h = get_adapter_config_hash(adapter_fusion_config)
             save_path = join(save_directory, name)
             if meta_dict:
                 meta_dict.update({"config_id": h})
             else:
                 meta_dict = {"config_id": h}
             self.save_adapter_fusion(
-                save_path, name, meta_dict=meta_dict, custom_weights_loaders=custom_weights_loaders
+                save_path,
+                name,
+                meta_dict=meta_dict,
+                custom_weights_loaders=custom_weights_loaders,
+                use_safetensors=use_safetensors,
             )
 
     def freeze_model(self, freeze=True):
         """Freezes all weights of the model."""
         # first freeze/ unfreeze all model weights
         for param in self.base_model.parameters():
             param.requires_grad = not freeze
@@ -1009,14 +1031,50 @@
                             else:
                                 destination[i][module.location_key] = nn.ModuleList([old_module, adapter_module])
                         else:
                             destination[i][module.location_key] = adapter_module
 
         return dict(destination)
 
+    def adapter_to(
+        self, name: str, device: Optional[Union[torch.device, str]] = None, dtype: Optional[torch.dtype] = None
+    ):
+        """
+        Moves the adapter with the given name to the specified device and data type.
+
+        Args:
+            name (str): The name of the adapter to be moved.
+            device (torch.device or str, optional): The device on which the adapter should be moved.
+            dtype (torch.dtype, optional): The data type to which the adapter should be cast.
+        """
+        for _, v in self.get_adapter(name).items():
+            for _, module in v.items():
+                module.to(device=device, dtype=dtype)
+
+    def adapter_fusion_to(
+        self,
+        adapter_names: Union[Fuse, list, str],
+        device: Optional[Union[torch.device, str]] = None,
+        dtype: Optional[torch.dtype] = None,
+    ):
+        """
+        Moves the adapter fusion layer with the given name to the specified device and data type.
+
+        Args:
+            adapter_names (Union[Fuse, list, str]): The name of the adapter fusion layer to be moved.
+            device (torch.device or str, optional): The device on which the adapter fusion layer should be moved.
+            dtype (torch.dtype, optional): The data type to which the adapter fusion layer should be cast.
+        """
+        for _, layer in self.iter_layers():
+            for module in layer.modules():
+                if isinstance(module, BottleneckLayer):
+                    fusion = module.get_adapter_fusion(adapter_names)
+                    if fusion is not None:
+                        fusion.to(device=device, dtype=dtype)
+
     def adapter_summary(self, as_dict=False) -> Union[str, dict]:
         """
         Returns a string summary of all adapters currently added to the model. Each entry in the summary table has the
         following attributes:
 
             - name: the name of the adapter
             - architecture: the architectural base of the adapter
@@ -1375,39 +1433,71 @@
         """
         if self.base_model is self:
             super().train_adapter_fusion(adapter_setup, unfreeze_adapters=unfreeze_adapters)
         else:
             self.base_model.train_adapter_fusion(adapter_setup, unfreeze_adapters=unfreeze_adapters)
         self.freeze_embeddings()
 
-    def save_head(self, save_directory: str, head_name: str = None):
-        loader = PredictionHeadLoader(self)
+    def save_head(self, save_directory: str, head_name: str = None, use_safetensors: bool = False) -> None:
+        """Saves a model prediction head to a directory such that it can be reloaded using `load_head()`.
+
+        Args:
+            save_directory (str): Path to the directory where the prediction head should be saved.
+            head_name (str, optional): Name of the head to save. Set to None if model only has one head. Defaults to None.
+            use_safetensors (bool, optional): If True, weights are saved via `safetensors`. Otherwise, the regular torch save method is used.
+        """
+        loader = PredictionHeadLoader(self, use_safetensors=use_safetensors)
         loader.save(save_directory, name=head_name)
 
-    def load_head(self, save_directory, load_as=None, id2label=None, **kwargs):
-        loader = PredictionHeadLoader(self, convert_to_flex_head=self._convert_to_flex_head)
+    def load_head(
+        self,
+        save_directory: str,
+        load_as: str = None,
+        id2label: Dict[int, str] = None,
+        use_safetensors: bool = False,
+        **kwargs
+    ) -> str:
+        """Loads a model prediction head from a directory where it was saved using `save_head()`.
+
+        Args:
+            save_directory (str): Path to the directory where the prediction head is saved.
+            load_as (str, optional): Load the AdapterFusion using this name.
+                    By default, the name with which the AdapterFusion layer was saved will be used.
+            id2label (Dict[int, str], optional): Provide a custom mapping from class ids to class labels. Defaults to None.
+            use_safetensors (bool, optional): If True, weights are loaded via `safetensors` if safetensors checkpoint is available. Otherwise, the regular torch save method is used.
+
+        Returns:
+            str: The name with which the prediction head was added to the model.
+        """
+        loader = PredictionHeadLoader(
+            self, convert_to_flex_head=self._convert_to_flex_head, use_safetensors=use_safetensors
+        )
         return loader.load(save_directory, load_as=load_as, id2label=id2label, **kwargs)
 
     def save_adapter(
         self,
         save_directory: str,
         adapter_name: str,
         with_head: bool = True,
         meta_dict: dict = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
+        use_safetensors: bool = False,
     ):
         if with_head:
             if custom_weights_loaders is None:
                 custom_weights_loaders = []
-            custom_weights_loaders.append(PredictionHeadLoader(self, error_on_missing=False))
+            custom_weights_loaders.append(
+                PredictionHeadLoader(self, error_on_missing=False, use_safetensors=use_safetensors)
+            )
         super().save_adapter(
             save_directory,
             adapter_name,
             meta_dict=meta_dict,
             custom_weights_loaders=custom_weights_loaders,
+            use_safetensors=use_safetensors,
         )
 
     def load_adapter(
         self,
         adapter_name_or_path: str,
         config: Union[dict, str] = None,
         version: str = None,
@@ -1415,24 +1505,26 @@
         load_as: str = None,
         source: str = None,
         with_head: bool = True,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
         leave_out: Optional[List[int]] = None,
         id2label=None,
         set_active: bool = False,
+        use_safetensors: bool = False,
         **kwargs
     ) -> str:
         if with_head:
             if custom_weights_loaders is None:
                 custom_weights_loaders = []
             custom_weights_loaders.append(
                 PredictionHeadLoader(
                     self,
                     error_on_missing=False,
                     convert_to_flex_head=self._convert_to_flex_head,
+                    use_safetensors=use_safetensors,
                 )
             )
         # Support passing a num_labels for compatibility reasons. Convert to label map here.
         num_labels = kwargs.pop("num_labels", None)
         if num_labels is not None:
             id2label = {i: "LABEL_" + str(i) for i in range(num_labels)}
         return super().load_adapter(
@@ -1442,23 +1534,25 @@
             model_name=model_name,
             load_as=load_as,
             source=source,
             custom_weights_loaders=custom_weights_loaders,
             leave_out=leave_out,
             id2label=id2label,
             set_active=set_active,
+            use_safetensors=use_safetensors,
             **kwargs,
         )
 
     def save_all_adapters(
         self,
         save_directory: str,
         with_head: bool = True,
         meta_dict: dict = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
+        use_safetensors: bool = False,
     ):
         os.makedirs(save_directory, exist_ok=True)
         for name in self.adapters_config:
             adapter_config = self.adapters_config.get(name)
             h = get_adapter_config_hash(adapter_config)
             save_path = join(save_directory, name)
             if meta_dict:
@@ -1467,75 +1561,96 @@
                 meta_dict = {"config_id": h}
             self.save_adapter(
                 save_path,
                 name,
                 meta_dict=meta_dict,
                 with_head=with_head,
                 custom_weights_loaders=custom_weights_loaders,
+                use_safetensors=use_safetensors,
             )
 
     def save_adapter_fusion(
         self,
         save_directory: str,
         adapter_names: Union[Fuse, list, str],
         meta_dict: dict = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
         with_head: Union[bool, str] = False,
+        use_safetensors: bool = False,
     ):
         """
         Saves an AdapterFusion layer and its configuration file to a directory so that it can be shared or reloaded
         using `load_adapter_fusion()`.
 
         Args:
             save_directory (str): Path to a directory where the AdapterFusion should be saved.
             adapter_names (Union[Fuse, list, str]): AdapterFusion to be saved.
             with_head (Union[bool, str]):
                 If True, will save a head with the same name as the AdapterFusionLayer. If a string, this will be used
                 as the name of the head to be saved.
+            use_safetensors (bool, optional): If True, weights are saved via `safetensors`. Otherwise, the regular torch save method is used.
 
         Raises:
             ValueError: If the given AdapterFusion name is invalid.
         """
-        super().save_adapter_fusion(save_directory, adapter_names, meta_dict, custom_weights_loaders)
+        super().save_adapter_fusion(
+            save_directory, adapter_names, meta_dict, custom_weights_loaders, use_safetensors=use_safetensors
+        )
 
         if with_head:
             # Make sure to cover the different options for adapter_names
             if isinstance(with_head, str):
                 head_name = with_head
             elif isinstance(adapter_names, Fuse):
                 head_name = adapter_names.name
             elif isinstance(adapter_names, list):
                 head_name = ",".join(adapter_names)
             else:
                 head_name = adapter_names
             if head_name not in self.heads:
                 raise ValueError("No head with name {} found".format(head_name))
-            loader = PredictionHeadLoader(self)
+            loader = PredictionHeadLoader(self, use_safetensors=use_safetensors)
             loader.save(save_directory, head_name)
 
     def load_adapter_fusion(
         self,
         adapter_fusion_name_or_path: str,
         load_as: str = None,
         custom_weights_loaders: Optional[List[WeightsLoader]] = None,
         set_active: bool = False,
         with_head: bool = True,
+        use_safetensors: bool = False,
         **kwargs
     ) -> str:
         if with_head:
             if custom_weights_loaders is None:
                 custom_weights_loaders = []
-            custom_weights_loaders.append(PredictionHeadLoader(self, error_on_missing=False))
-        super().load_adapter_fusion(adapter_fusion_name_or_path, load_as, custom_weights_loaders, set_active)
+            custom_weights_loaders.append(
+                PredictionHeadLoader(self, error_on_missing=False, use_safetensors=use_safetensors)
+            )
+        super().load_adapter_fusion(
+            adapter_fusion_name_or_path,
+            load_as,
+            custom_weights_loaders,
+            set_active,
+            use_safetensors=use_safetensors,
+            **kwargs,
+        )
 
-    def save_all_heads(self, save_directory):
+    def save_all_heads(self, save_directory: str, use_safetensors: bool = False):
+        """Saves all prediction heads of this model to subfolders of the given location.
+
+        Args:
+            save_directory (str): Path to the base directory where prediction heads should be saved.
+            use_safetensors (bool, optional): If True, weights are saved via `safetensors`. Otherwise, the regular torch save method is used.
+        """
         os.makedirs(save_directory, exist_ok=True)
         for head_name in self.heads:
             save_path = join(save_directory, head_name)
-            self.save_head(save_path, head_name)
+            self.save_head(save_path, head_name, use_safetensors=use_safetensors)
 
     def get_labels(self):
         return list(self.config.id2label.values())
 
     def get_labels_dict(self):
         return self.config.id2label
```

### Comparing `adapters-0.2.0/src/adapters/models/__init__.py` & `adapters-0.2.1/src/adapters/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/albert/__init__.py` & `adapters-0.2.1/src/adapters/models/albert/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/albert/adapter_model.py` & `adapters-0.2.1/src/adapters/models/albert/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/albert/mixin_albert.py` & `adapters-0.2.1/src/adapters/models/albert/mixin_albert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/albert/modeling_albert.py` & `adapters-0.2.1/src/adapters/models/albert/modeling_albert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/auto/__init__.py` & `adapters-0.2.1/src/adapters/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/auto/adapter_model.py` & `adapters-0.2.1/src/adapters/models/auto/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/auto/auto_factory.py` & `adapters-0.2.1/src/adapters/models/auto/auto_factory.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bart/__init__.py` & `adapters-0.2.1/src/adapters/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bart/adapter_model.py` & `adapters-0.2.1/src/adapters/models/bart/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bart/mixin_bart.py` & `adapters-0.2.1/src/adapters/models/bart/mixin_bart.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bart/modeling_bart.py` & `adapters-0.2.1/src/adapters/models/bart/modeling_bart.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/beit/__init__.py` & `adapters-0.2.1/src/adapters/models/beit/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/beit/adapter_model.py` & `adapters-0.2.1/src/adapters/models/beit/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/beit/mixin_beit.py` & `adapters-0.2.1/src/adapters/models/beit/mixin_beit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/beit/modeling_beit.py` & `adapters-0.2.1/src/adapters/models/beit/modeling_beit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bert/__init__.py` & `adapters-0.2.1/src/adapters/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bert/adapter_model.py` & `adapters-0.2.1/src/adapters/models/bert/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bert/mixin_bert.py` & `adapters-0.2.1/src/adapters/models/bert/mixin_bert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bert/modeling_bert.py` & `adapters-0.2.1/src/adapters/models/bert/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bert_generation/__init__.py` & `adapters-0.2.1/src/adapters/models/bert_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bert_generation/adapter_model.py` & `adapters-0.2.1/src/adapters/models/bert_generation/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/bert_generation/modeling_bert_generation.py` & `adapters-0.2.1/src/adapters/models/bert_generation/modeling_bert_generation.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/clip/__init__.py` & `adapters-0.2.1/src/adapters/models/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/clip/adapter_model.py` & `adapters-0.2.1/src/adapters/models/clip/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/clip/mixin_clip.py` & `adapters-0.2.1/src/adapters/models/clip/mixin_clip.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/clip/modeling_clip.py` & `adapters-0.2.1/src/adapters/models/clip/modeling_clip.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/deberta/__init__.py` & `adapters-0.2.1/src/adapters/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/deberta/adapter_model.py` & `adapters-0.2.1/src/adapters/models/deberta/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/deberta/mixin_deberta.py` & `adapters-0.2.1/src/adapters/models/deberta/mixin_deberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/deberta/modeling_deberta.py` & `adapters-0.2.1/src/adapters/models/deberta/modeling_deberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/deberta_v2/__init__.py` & `adapters-0.2.1/src/adapters/models/deberta_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/deberta_v2/adapter_model.py` & `adapters-0.2.1/src/adapters/models/deberta_v2/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/deberta_v2/mixin_deberta_v2.py` & `adapters-0.2.1/src/adapters/models/deberta_v2/mixin_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/deberta_v2/modeling_deberta_v2.py` & `adapters-0.2.1/src/adapters/models/deberta_v2/modeling_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/distilbert/__init__.py` & `adapters-0.2.1/src/adapters/models/distilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/distilbert/adapter_model.py` & `adapters-0.2.1/src/adapters/models/distilbert/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/distilbert/mixin_distilbert.py` & `adapters-0.2.1/src/adapters/models/distilbert/mixin_distilbert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/distilbert/modeling_distilbert.py` & `adapters-0.2.1/src/adapters/models/distilbert/modeling_distilbert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/electra/__init__.py` & `adapters-0.2.1/src/adapters/models/electra/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/electra/adapter_model.py` & `adapters-0.2.1/src/adapters/models/electra/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/electra/modeling_electra.py` & `adapters-0.2.1/src/adapters/models/electra/modeling_electra.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/gpt2/__init__.py` & `adapters-0.2.1/src/adapters/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/gpt2/adapter_model.py` & `adapters-0.2.1/src/adapters/models/gpt2/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/gpt2/mixin_gpt2.py` & `adapters-0.2.1/src/adapters/models/gpt2/mixin_gpt2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/gpt2/modeling_gpt2.py` & `adapters-0.2.1/src/adapters/models/gpt2/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/gptj/__init__.py` & `adapters-0.2.1/src/adapters/models/gptj/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/gptj/adapter_model.py` & `adapters-0.2.1/src/adapters/models/gptj/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/gptj/mixin_gptj.py` & `adapters-0.2.1/src/adapters/models/gptj/mixin_gptj.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/gptj/modeling_gptj.py` & `adapters-0.2.1/src/adapters/models/gptj/modeling_gptj.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/llama/__init__.py` & `adapters-0.2.1/src/adapters/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/llama/adapter_model.py` & `adapters-0.2.1/src/adapters/models/llama/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/llama/mixin_llama.py` & `adapters-0.2.1/src/adapters/models/llama/mixin_llama.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/llama/modeling_llama.py` & `adapters-0.2.1/src/adapters/models/llama/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/mbart/__init__.py` & `adapters-0.2.1/src/adapters/models/mbart/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/mbart/adapter_model.py` & `adapters-0.2.1/src/adapters/models/mbart/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/mbart/modeling_mbart.py` & `adapters-0.2.1/src/adapters/models/mbart/modeling_mbart.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/mt5/__init__.py` & `adapters-0.2.1/src/adapters/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/mt5/adapter_model.py` & `adapters-0.2.1/src/adapters/models/mt5/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/mt5/modeling_mt5.py` & `adapters-0.2.1/src/adapters/models/mt5/modeling_mt5.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/roberta/__init__.py` & `adapters-0.2.1/src/adapters/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/roberta/adapter_model.py` & `adapters-0.2.1/src/adapters/models/roberta/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/roberta/modeling_roberta.py` & `adapters-0.2.1/src/adapters/models/roberta/modeling_roberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/t5/__init__.py` & `adapters-0.2.1/src/adapters/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/t5/adapter_model.py` & `adapters-0.2.1/src/adapters/models/t5/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/t5/mixin_t5.py` & `adapters-0.2.1/src/adapters/models/t5/mixin_t5.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/t5/modeling_t5.py` & `adapters-0.2.1/src/adapters/models/t5/modeling_t5.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/vit/__init__.py` & `adapters-0.2.1/src/adapters/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/vit/adapter_model.py` & `adapters-0.2.1/src/adapters/models/vit/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/vit/mixin_vit.py` & `adapters-0.2.1/src/adapters/models/vit/mixin_vit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/vit/modeling_vit.py` & `adapters-0.2.1/src/adapters/models/vit/modeling_vit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/xlm_roberta/__init__.py` & `adapters-0.2.1/src/adapters/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/xlm_roberta/adapter_model.py` & `adapters-0.2.1/src/adapters/models/xlm_roberta/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/xlm_roberta/modeling_xlm_roberta.py` & `adapters-0.2.1/src/adapters/models/xlm_roberta/modeling_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/xmod/__init__.py` & `adapters-0.2.1/src/adapters/models/xmod/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/xmod/adapter_model.py` & `adapters-0.2.1/src/adapters/models/xmod/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/xmod/mixin_xmod.py` & `adapters-0.2.1/src/adapters/models/xmod/mixin_xmod.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/models/xmod/modeling_xmod.py` & `adapters-0.2.1/src/adapters/models/xmod/modeling_xmod.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/trainer.py` & `adapters-0.2.1/src/adapters/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,25 +208,26 @@
             f"Loading best adapter(s) from {self.state.best_model_checkpoint} (score: {self.state.best_metric})."
         )
         # attempt to re-load all adapters from checkpoint
         for adapter in model.adapters_config.adapters:
             adapter_dir = os.path.join(self.state.best_model_checkpoint, adapter)
             if os.path.exists(adapter_dir):
                 model.load_adapter(adapter_dir)
+                model.adapter_to(adapter, device=self.args.device)
         if self.train_adapter_fusion:
             logger.info(
                 f"Loading best adapter fusion(s) from {self.state.best_model_checkpoint} (score:"
                 f" {self.state.best_metric})."
             )
             # attempt to re-load all adapter fusions from checkpoint
             for fusion in model.adapters_config.fusions:
                 fusion_dir = os.path.join(self.state.best_model_checkpoint, fusion)
                 if os.path.exists(fusion_dir):
                     model.load_adapter_fusion(fusion_dir)
-        model.to(self.args.device)
+                    model.adapter_fusion_to(fusion, device=self.args.device)
 
 
 class AdapterTrainerCallback(TrainerCallback):
     def __init__(self, trainer):
         super().__init__()
         self.trainer = trainer
```

### Comparing `adapters-0.2.0/src/adapters/training.py` & `adapters-0.2.1/src/adapters/training.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/utils.py` & `adapters-0.2.1/src/adapters/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,21 @@
 from .context import ForwardContext
 
 
 logger = logging.getLogger(__name__)
 
 CONFIG_NAME = "adapter_config.json"
 WEIGHTS_NAME = "pytorch_adapter.bin"
+SAFE_WEIGHTS_NAME = "adapter.safetensors"
 HEAD_CONFIG_NAME = "head_config.json"
 HEAD_WEIGHTS_NAME = "pytorch_model_head.bin"
+SAFE_HEAD_WEIGHTS_NAME = "model_head.safetensors"
 ADAPTERFUSION_CONFIG_NAME = "adapter_fusion_config.json"
 ADAPTERFUSION_WEIGHTS_NAME = "pytorch_model_adapter_fusion.bin"
+SAFE_ADAPTERFUSION_WEIGHTS_NAME = "model_adapter_fusion.safetensors"
 EMBEDDING_FILE = "embedding.pt"
 TOKENIZER_PATH = "tokenizer"
 
 ADAPTER_HUB_URL = "https://raw.githubusercontent.com/Adapter-Hub/Hub/master/dist/v2/"
 ADAPTER_HUB_INDEX_FILE = ADAPTER_HUB_URL + "index/{}.json"
 ADAPTER_HUB_CONFIG_FILE = ADAPTER_HUB_URL + "architectures.json"
 ADAPTER_HUB_ALL_FILE = ADAPTER_HUB_URL + "all.json"
@@ -699,15 +702,17 @@
         if not resolved_folder:
             raise EnvironmentError(
                 "Unable to load file from {}. The file might be unavailable.".format(resolved_folder)
             )
         return resolved_folder
     # path to a local folder saved using save()
     elif isdir(adapter_name_or_path):
-        if isfile(join(adapter_name_or_path, WEIGHTS_NAME)) and isfile(join(adapter_name_or_path, CONFIG_NAME)):
+        if (
+            isfile(join(adapter_name_or_path, WEIGHTS_NAME)) or isfile(join(adapter_name_or_path, SAFE_WEIGHTS_NAME))
+        ) and isfile(join(adapter_name_or_path, CONFIG_NAME)):
             return adapter_name_or_path
         else:
             raise EnvironmentError(
                 "No file {} or no file {} found in directory {}".format(
                     WEIGHTS_NAME, CONFIG_NAME, adapter_name_or_path
                 )
             )
@@ -811,15 +816,17 @@
             return None
     elif source == "hf":
         try:
             model_info = HfApi().model_info(adapter_id)
             return AdapterInfo(
                 source="hf",
                 adapter_id=model_info.modelId,
-                model_name=model_info.config.get("adapters", {}).get("model_name") if model_info.config else None,
+                model_name=model_info.config.get("adapter_transformers", {}).get("model_name")
+                if model_info.config
+                else None,
                 username=model_info.modelId.split("/")[0],
                 sha1_checksum=model_info.sha,
             )
         except requests.exceptions.HTTPError:
             return None
     else:
         raise ValueError("Please specify either 'ah' or 'hf' as source.")
```

### Comparing `adapters-0.2.0/src/adapters/wrappers/__init__.py` & `adapters-0.2.1/src/adapters/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/wrappers/configuration.py` & `adapters-0.2.1/src/adapters/wrappers/configuration.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters/wrappers/model.py` & `adapters-0.2.1/src/adapters/wrappers/model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters.egg-info/PKG-INFO` & `adapters-0.2.1/src/adapters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapters
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Unified Library for Parameter-Efficient and Modular Transfer Learning
 Home-page: https://github.com/adapter-hub/adapters
 Author: The AdapterHub team and community contributors
 Author-email: calpt@mail.de
 License: Apache
 Keywords: NLP deep learning transformer pytorch BERT adapters
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adapters Version: 0.2.0 Summary: A Unified Library
+Metadata-Version: 2.1 Name: adapters Version: 0.2.1 Summary: A Unified Library
 for Parameter-Efficient and Modular Transfer Learning Home-page: https://
 github.com/adapter-hub/adapters Author: The AdapterHub team and community
 contributors Author-email: calpt@mail.de License: Apache Keywords: NLP deep
 learning transformer pytorch BERT adapters Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

### Comparing `adapters-0.2.0/src/adapters.egg-info/SOURCES.txt` & `adapters-0.2.1/src/adapters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/src/adapters.egg-info/requires.txt` & `adapters-0.2.1/src/adapters.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter.py` & `adapters-0.2.1/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_backward_compability.py` & `adapters-0.2.1/tests/test_adapter_backward_compability.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_config.py` & `adapters-0.2.1/tests/test_adapter_config.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_conversion.py` & `adapters-0.2.1/tests/test_adapter_conversion.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_custom_head.py` & `adapters-0.2.1/tests/test_adapter_custom_head.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_embeddings.py` & `adapters-0.2.1/tests/test_adapter_embeddings.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_fusion_common.py` & `adapters-0.2.1/tests/test_adapter_fusion_common.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_fusion_config.py` & `adapters-0.2.1/tests/test_adapter_fusion_config.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_heads.py` & `adapters-0.2.1/tests/test_adapter_heads.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_hub.py` & `adapters-0.2.1/tests/test_adapter_hub.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_save_id2label.py` & `adapters-0.2.1/tests/test_adapter_save_id2label.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_adapter_trainer.py` & `adapters-0.2.1/tests/test_adapter_trainer.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_albert.py` & `adapters-0.2.1/tests/test_albert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_bart.py` & `adapters-0.2.1/tests/test_bart.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_beit.py` & `adapters-0.2.1/tests/test_beit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_bert.py` & `adapters-0.2.1/tests/test_bert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_bert_generation.py` & `adapters-0.2.1/tests/test_bert_generation.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_clip.py` & `adapters-0.2.1/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_deberta.py` & `adapters-0.2.1/tests/test_deberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_debertaV2.py` & `adapters-0.2.1/tests/test_debertaV2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_distilbert.py` & `adapters-0.2.1/tests/test_distilbert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_electra.py` & `adapters-0.2.1/tests/test_electra.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_encoder_decoder.py` & `adapters-0.2.1/tests/test_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_gpt2.py` & `adapters-0.2.1/tests/test_gpt2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_gptj.py` & `adapters-0.2.1/tests/test_gptj.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_llama.py` & `adapters-0.2.1/tests/test_llama.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_mbart.py` & `adapters-0.2.1/tests/test_mbart.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_mt5.py` & `adapters-0.2.1/tests/test_mt5.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_roberta.py` & `adapters-0.2.1/tests/test_roberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_t5.py` & `adapters-0.2.1/tests/test_t5.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_vit.py` & `adapters-0.2.1/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_xlm_roberta.py` & `adapters-0.2.1/tests/test_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.2.0/tests/test_xmod.py` & `adapters-0.2.1/tests/test_xmod.py`

 * *Files identical despite different names*

