# Comparing `tmp/developergpt-0.7.2.tar.gz` & `tmp/developergpt-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.7.2.tar", last modified: Tue Apr 30 00:30:13 2024, max compression
+gzip compressed data, was "developergpt-0.7.3.tar", last modified: Tue May 21 02:13:56 2024, max compression
```

## Comparing `developergpt-0.7.2.tar` & `developergpt-0.7.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:13.267089 developergpt-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-30 00:30:05.000000 developergpt-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 00:30:05.000000 developergpt-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-04-30 00:30:13.267089 developergpt-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-30 00:30:05.000000 developergpt-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:13.267089 developergpt-0.7.2/developergpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/anthropic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/few_shot_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/gemini_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:13.267089 developergpt-0.7.2/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:30:13.267089 developergpt-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-30 00:30:05.000000 developergpt-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:13.267089 developergpt-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:05.000000 developergpt-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 00:30:05.000000 developergpt-0.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 00:30:05.000000 developergpt-0.7.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:13:56.909608 developergpt-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 02:13:49.000000 developergpt-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 02:13:49.000000 developergpt-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-21 02:13:56.909608 developergpt-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-21 02:13:49.000000 developergpt-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:13:56.905608 developergpt-0.7.3/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/anthropic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/few_shot_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/gemini_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-21 02:13:49.000000 developergpt-0.7.3/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:13:56.909608 developergpt-0.7.3/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-21 02:13:56.000000 developergpt-0.7.3/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-21 02:13:56.000000 developergpt-0.7.3/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 02:13:56.000000 developergpt-0.7.3/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 02:13:56.000000 developergpt-0.7.3/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-21 02:13:56.000000 developergpt-0.7.3/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 02:13:56.000000 developergpt-0.7.3/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 02:13:56.909608 developergpt-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-21 02:13:49.000000 developergpt-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:13:56.905608 developergpt-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:13:49.000000 developergpt-0.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-21 02:13:49.000000 developergpt-0.7.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 02:13:49.000000 developergpt-0.7.3/tests/test_cli.py
```

### Comparing `developergpt-0.7.2/LICENSE` & `developergpt-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.2/PKG-INFO` & `developergpt-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.7.2
+Version: 0.7.3
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -36,31 +36,31 @@
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini 1.0 Pro by default but also supports OpenAI GPT LLMs, Anthropic Claude 3 LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
-As of May 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
+As of May 2024, DeveloperGPT is completely free to use when using Google Gemini 1.0 Pro (used by default) or Google Gemini 1.0 Flash at up to 15 requests per minute.
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [llm_name] [cmd, chat]`
-| Model(s)                   | Source                                                                                                                       | Details                                                  |
-| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
-| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Haiku, Sonnet**          | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
-| **Zephyr**                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
-| **Gemma, Gemma-Base**      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
-| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
-| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
+| Model(s)                        | Source                                                                                                                       | Details                                                  |
+| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default), **Flash** | [Google Gemini 1.0 Pro, Gemini 1.0 Flash](https://deepmind.google/technologies/gemini/)                                      | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**                 | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Haiku, Sonnet**               | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
+| **Zephyr**                      | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
+| **Gemma, Gemma-Base**           | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
+| **Mistral-Q6, Mistral-Q4**      | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
+| **Mistral**                     | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
@@ -101,15 +101,15 @@
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chat_demo.gif)
 
 Use `developergpt --offline chat` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
 
 Use `developergpt --model [model_name] chat` to use a different LLM instead of Gemini. 
 ```bash
 # Example
-$ developergpt --model gemma chat
+$ developergpt --model mistral chat
 ```
 
 Chat moderation is **NOT** implemented - all your chat messages should follow the terms of use of the LLM used. 
 
 ## Usage
 DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used. Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
@@ -122,15 +122,15 @@
 ```bash
 # see available commands
 $ developergpt 
 ```
 
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini Pro 1.0. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
+By default, DeveloperGPT uses Google Gemini 1.0 Pro. To use Gemini 1.0 Pro or Gemini 1.5 Flash, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
 2. Set your Google API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -166,43 +166,43 @@
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 #### Using Anthropic LLMs
-To use Anthropic Claude LLMs, you will need an Anthropic API key.
+To use Anthropic Claude 3 Sonnet or Haiku, you will need an Anthropic API key.
 
 1. Get your own Anthropic API Key: https://www.anthropic.com/api
 2. Set your Anthropic API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Anthropic API Key (using zsh for example)
 $ echo 'export ANTHROPIC_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 
 ### Usage and Cost 
-#### Google Gemini
-As of May 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
+#### Google Gemini LLMs
+As of May 2024, Google Gemini 1.0 Pro and Gemini 1.5 Flash is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### Hugging Face Hosted Open LLMs 
 As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### OpenAI GPT
-You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
+You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. The average cost per query using GPT-3.5 is < 0.0001 cents. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Anthropic Claude LLMs
-You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. Based on preliminary testing, using DeveloperGPT with Claude Haiku should cost less than 10 cents per day with regular usage. See https://www.anthropic.com/api for pricing details. 
+You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. The average cost per query using Claude 3 Haiku is < 0.0001 cents. See https://www.anthropic.com/api for pricing details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
 - Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
-- Thanks to Google for the generous Gemini Pro API free tier. 
+- Thanks to Google for the generous Gemini API free tier. 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.7.2/README.md` & `developergpt-0.7.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini 1.0 Pro by default but also supports OpenAI GPT LLMs, Anthropic Claude 3 LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
-As of May 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
+As of May 2024, DeveloperGPT is completely free to use when using Google Gemini 1.0 Pro (used by default) or Google Gemini 1.0 Flash at up to 15 requests per minute.
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [llm_name] [cmd, chat]`
-| Model(s)                   | Source                                                                                                                       | Details                                                  |
-| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
-| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Haiku, Sonnet**          | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
-| **Zephyr**                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
-| **Gemma, Gemma-Base**      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
-| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
-| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
+| Model(s)                        | Source                                                                                                                       | Details                                                  |
+| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default), **Flash** | [Google Gemini 1.0 Pro, Gemini 1.0 Flash](https://deepmind.google/technologies/gemini/)                                      | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**                 | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Haiku, Sonnet**               | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
+| **Zephyr**                      | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
+| **Gemma, Gemma-Base**           | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
+| **Mistral-Q6, Mistral-Q4**      | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
+| **Mistral**                     | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
@@ -64,15 +64,15 @@
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chat_demo.gif)
 
 Use `developergpt --offline chat` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
 
 Use `developergpt --model [model_name] chat` to use a different LLM instead of Gemini. 
 ```bash
 # Example
-$ developergpt --model gemma chat
+$ developergpt --model mistral chat
 ```
 
 Chat moderation is **NOT** implemented - all your chat messages should follow the terms of use of the LLM used. 
 
 ## Usage
 DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used. Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
@@ -85,15 +85,15 @@
 ```bash
 # see available commands
 $ developergpt 
 ```
 
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini Pro 1.0. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
+By default, DeveloperGPT uses Google Gemini 1.0 Pro. To use Gemini 1.0 Pro or Gemini 1.5 Flash, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
 2. Set your Google API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -129,43 +129,43 @@
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 #### Using Anthropic LLMs
-To use Anthropic Claude LLMs, you will need an Anthropic API key.
+To use Anthropic Claude 3 Sonnet or Haiku, you will need an Anthropic API key.
 
 1. Get your own Anthropic API Key: https://www.anthropic.com/api
 2. Set your Anthropic API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Anthropic API Key (using zsh for example)
 $ echo 'export ANTHROPIC_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 
 ### Usage and Cost 
-#### Google Gemini
-As of May 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
+#### Google Gemini LLMs
+As of May 2024, Google Gemini 1.0 Pro and Gemini 1.5 Flash is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### Hugging Face Hosted Open LLMs 
 As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### OpenAI GPT
-You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
+You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. The average cost per query using GPT-3.5 is < 0.0001 cents. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Anthropic Claude LLMs
-You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. Based on preliminary testing, using DeveloperGPT with Claude Haiku should cost less than 10 cents per day with regular usage. See https://www.anthropic.com/api for pricing details. 
+You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. The average cost per query using Claude 3 Haiku is < 0.0001 cents. See https://www.anthropic.com/api for pricing details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
 - Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
-- Thanks to Google for the generous Gemini Pro API free tier. 
+- Thanks to Google for the generous Gemini API free tier. 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.7.2/developergpt/anthropic_adapter.py` & `developergpt-0.7.3/developergpt/anthropic_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.2/developergpt/cli.py` & `developergpt-0.7.3/developergpt/cli.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.2/developergpt/config.py` & `developergpt-0.7.3/developergpt/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,25 +25,27 @@
 ### Supported LLMs and Configuration ###
 GPT35 = "gpt35"
 GPT4 = "gpt4"
 ZEPHYR = "zephyr"
 GEMMA = "gemma"
 GEMMA_BASE = "gemma-base"
 GEMINI = "gemini"
+FLASH = "flash"
 MISTRAL_Q6 = "mistral-q6"
 MISTRAL_Q4 = "mistral-q4"
 MISTRAL_HF = "mistral"
 SONNET = "sonnet"
 HAIKU = "haiku"
 BLOOM = "bloom"  # not supported due to poor performance
 SUPPORTED_MODELS = set(
     [
         GPT35,
         GPT4,
         GEMINI,
+        FLASH,
         ZEPHYR,
         MISTRAL_Q6,
         MISTRAL_Q4,
         MISTRAL_HF,
         GEMMA,
         GEMMA_BASE,
         SONNET,
@@ -87,15 +89,16 @@
 
 HF_INSTRUCT_MODELS = set([GEMMA, ZEPHYR, MISTRAL_HF])
 
 # set of models that support the new chat completion endpoint
 HF_CHAT_COMPLETION_MODELS = set([ZEPHYR])
 
 GOOGLE_MODEL_MAP = {
-    GEMINI: "gemini-1.0-pro",
+    GEMINI: "models/gemini-1.0-pro-latest",
+    FLASH: "models/gemini-1.5-flash-latest",
 }
 
 ### API Key Constants ###
 
 GOOGLE_API_KEY = "GOOGLE_API_KEY"
 OPEN_AI_API_KEY = "OPENAI_API_KEY"
 HUGGING_FACE_API_KEY = "HUGGING_FACE_API_KEY"
```

### Comparing `developergpt-0.7.2/developergpt/few_shot_prompts.py` & `developergpt-0.7.3/developergpt/few_shot_prompts.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.2/developergpt/gemini_adapter.py` & `developergpt-0.7.3/developergpt/gemini_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.2/developergpt/huggingface_adapter.py` & `developergpt-0.7.3/developergpt/huggingface_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.2/developergpt/openai_adapter.py` & `developergpt-0.7.3/developergpt/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.2/developergpt/utils.py` & `developergpt-0.7.3/developergpt/utils.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.2/developergpt.egg-info/PKG-INFO` & `developergpt-0.7.3/developergpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.7.2
+Version: 0.7.3
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -36,31 +36,31 @@
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini 1.0 Pro by default but also supports OpenAI GPT LLMs, Anthropic Claude 3 LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
-As of May 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
+As of May 2024, DeveloperGPT is completely free to use when using Google Gemini 1.0 Pro (used by default) or Google Gemini 1.0 Flash at up to 15 requests per minute.
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [llm_name] [cmd, chat]`
-| Model(s)                   | Source                                                                                                                       | Details                                                  |
-| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
-| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Haiku, Sonnet**          | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
-| **Zephyr**                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
-| **Gemma, Gemma-Base**      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
-| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
-| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
+| Model(s)                        | Source                                                                                                                       | Details                                                  |
+| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default), **Flash** | [Google Gemini 1.0 Pro, Gemini 1.0 Flash](https://deepmind.google/technologies/gemini/)                                      | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**                 | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Haiku, Sonnet**               | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
+| **Zephyr**                      | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
+| **Gemma, Gemma-Base**           | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
+| **Mistral-Q6, Mistral-Q4**      | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
+| **Mistral**                     | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
@@ -101,15 +101,15 @@
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chat_demo.gif)
 
 Use `developergpt --offline chat` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
 
 Use `developergpt --model [model_name] chat` to use a different LLM instead of Gemini. 
 ```bash
 # Example
-$ developergpt --model gemma chat
+$ developergpt --model mistral chat
 ```
 
 Chat moderation is **NOT** implemented - all your chat messages should follow the terms of use of the LLM used. 
 
 ## Usage
 DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used. Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
@@ -122,15 +122,15 @@
 ```bash
 # see available commands
 $ developergpt 
 ```
 
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini Pro 1.0. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
+By default, DeveloperGPT uses Google Gemini 1.0 Pro. To use Gemini 1.0 Pro or Gemini 1.5 Flash, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
 2. Set your Google API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -166,43 +166,43 @@
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 #### Using Anthropic LLMs
-To use Anthropic Claude LLMs, you will need an Anthropic API key.
+To use Anthropic Claude 3 Sonnet or Haiku, you will need an Anthropic API key.
 
 1. Get your own Anthropic API Key: https://www.anthropic.com/api
 2. Set your Anthropic API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Anthropic API Key (using zsh for example)
 $ echo 'export ANTHROPIC_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 
 ### Usage and Cost 
-#### Google Gemini
-As of May 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
+#### Google Gemini LLMs
+As of May 2024, Google Gemini 1.0 Pro and Gemini 1.5 Flash is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### Hugging Face Hosted Open LLMs 
 As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### OpenAI GPT
-You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
+You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. The average cost per query using GPT-3.5 is < 0.0001 cents. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Anthropic Claude LLMs
-You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. Based on preliminary testing, using DeveloperGPT with Claude Haiku should cost less than 10 cents per day with regular usage. See https://www.anthropic.com/api for pricing details. 
+You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. The average cost per query using Claude 3 Haiku is < 0.0001 cents. See https://www.anthropic.com/api for pricing details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
 - Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
-- Thanks to Google for the generous Gemini Pro API free tier. 
+- Thanks to Google for the generous Gemini API free tier. 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.7.2/developergpt.egg-info/SOURCES.txt` & `developergpt-0.7.3/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.2/setup.py` & `developergpt-0.7.3/setup.py`

 * *Files identical despite different names*

