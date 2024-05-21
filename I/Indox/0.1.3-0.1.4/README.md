# Comparing `tmp/indox-0.1.3.tar.gz` & `tmp/indox-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indox-0.1.3.tar", last modified: Mon May 20 10:10:44 2024, max compression
+gzip compressed data, was "indox-0.1.4.tar", last modified: Tue May 21 15:54:06 2024, max compression
```

## Comparing `indox-0.1.3.tar` & `indox-0.1.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.672964 indox-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.643278 indox-0.1.3/Indox/
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.656961 indox-0.1.3/Indox/DataLoaderSplitter/
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.660961 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/
--rw-rw-rw-   0        0        0     6348 2024-05-11 13:44:58.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py
--rw-rw-rw-   0        0        0     2074 2024-05-13 06:41:26.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py
--rw-rw-rw-   0        0        0     4781 2024-05-13 08:12:00.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/EmbedClusterSummarize.py
--rw-rw-rw-   0        0        0     2856 2024-05-13 06:27:35.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py
--rw-rw-rw-   0        0        0       35 2024-05-14 14:02:48.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/__init__.py
--rw-rw-rw-   0        0        0     4078 2024-05-14 14:21:32.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/split.py
--rw-rw-rw-   0        0        0     6425 2024-05-13 08:09:25.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.661961 indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/
--rw-rw-rw-   0        0        0       45 2024-05-14 14:02:48.000000 indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/__init__.py
--rw-rw-rw-   0        0        0     2453 2024-05-15 14:05:13.000000 indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/loader.py
--rw-rw-rw-   0        0        0     3596 2024-05-15 08:19:59.000000 indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/split.py
--rw-rw-rw-   0        0        0      108 2024-05-14 14:18:27.000000 indox-0.1.3/Indox/DataLoaderSplitter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.662961 indox-0.1.3/Indox/Embeddings/
--rw-rw-rw-   0        0        0       67 2024-05-12 16:34:51.000000 indox-0.1.3/Indox/Embeddings/__init__.py
--rw-rw-rw-   0        0        0      495 2024-05-12 16:34:51.000000 indox-0.1.3/Indox/Embeddings/embedding_models.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.665960 indox-0.1.3/Indox/Evaluation/
--rw-rw-rw-   0        0        0       28 2024-05-13 12:54:42.000000 indox-0.1.3/Indox/Evaluation/__init__.py
--rw-rw-rw-   0        0        0     7715 2024-05-19 08:29:16.000000 indox-0.1.3/Indox/Evaluation/eval.py
--rw-rw-rw-   0        0        0     2906 2024-05-13 12:39:30.000000 indox-0.1.3/Indox/Evaluation/metrics.py
--rw-rw-rw-   0        0        0     4719 2024-05-19 08:29:16.000000 indox-0.1.3/Indox/Evaluation/similarity.py
--rw-rw-rw-   0        0        0    10059 2024-05-13 12:39:30.000000 indox-0.1.3/Indox/Evaluation/unieval.py
--rw-rw-rw-   0        0        0     2453 2024-05-11 13:44:58.000000 indox-0.1.3/Indox/Graph.py
--rw-rw-rw-   0        0        0     8869 2024-05-16 15:16:32.000000 indox-0.1.3/Indox/Indox.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.665960 indox-0.1.3/Indox/QaModels/
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.666962 indox-0.1.3/Indox/QaModels/Dspy_Cot/
--rw-rw-rw-   0        0        0       27 2024-05-12 15:50:15.000000 indox-0.1.3/Indox/QaModels/Dspy_Cot/__init__.py
--rw-rw-rw-   0        0        0     2654 2024-05-13 14:07:14.000000 indox-0.1.3/Indox/QaModels/Dspy_Cot/dspy.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.667963 indox-0.1.3/Indox/QaModels/Mistral/
--rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.3/Indox/QaModels/Mistral/__init__.py
--rw-rw-rw-   0        0        0     2756 2024-05-12 15:50:15.000000 indox-0.1.3/Indox/QaModels/Mistral/mistral.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.668963 indox-0.1.3/Indox/QaModels/OpenAi/
--rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.3/Indox/QaModels/OpenAi/__init__.py
--rw-rw-rw-   0        0        0     2232 2024-05-15 14:01:50.000000 indox-0.1.3/Indox/QaModels/OpenAi/openai.py
--rw-rw-rw-   0        0        0       95 2024-05-14 13:59:17.000000 indox-0.1.3/Indox/QaModels/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.669963 indox-0.1.3/Indox/Splitter/
--rw-rw-rw-   0        0        0       60 2024-05-15 04:55:56.000000 indox-0.1.3/Indox/Splitter/__init__.py
--rw-rw-rw-   0        0        0      377 2024-05-14 14:16:18.000000 indox-0.1.3/Indox/Splitter/semantic_text_splitter.py
--rw-rw-rw-   0        0        0       66 2024-05-12 15:34:14.000000 indox-0.1.3/Indox/__init__.py
--rw-rw-rw-   0        0        0      960 2024-05-14 11:18:39.000000 indox-0.1.3/Indox/config.yaml
--rw-rw-rw-   0        0        0     2738 2024-05-15 06:17:01.000000 indox-0.1.3/Indox/utils.py
--rw-rw-rw-   0        0        0     8896 2024-05-13 14:07:14.000000 indox-0.1.3/Indox/vectorstore.py
--rw-rw-rw-   0        0        0     2562 2024-05-16 15:16:32.000000 indox-0.1.3/Indox/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.670963 indox-0.1.3/Indox.egg-info/
--rw-rw-rw-   0        0        0     8261 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1391 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-05-11 13:44:58.000000 indox-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8261 2024-05-20 10:10:44.671964 indox-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6916 2024-05-20 09:59:26.000000 indox-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-20 10:10:44.672964 indox-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1307 2024-05-20 10:10:06.000000 indox-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.145660 indox-0.1.4/
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.113031 indox-0.1.4/Indox/
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.129691 indox-0.1.4/Indox/DataLoaderSplitter/
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.133662 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/
+-rw-rw-rw-   0        0        0     6348 2024-05-11 13:44:58.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py
+-rw-rw-rw-   0        0        0     2074 2024-05-13 06:41:26.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py
+-rw-rw-rw-   0        0        0     4781 2024-05-13 08:12:00.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/EmbedClusterSummarize.py
+-rw-rw-rw-   0        0        0     2856 2024-05-13 06:27:35.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py
+-rw-rw-rw-   0        0        0       35 2024-05-14 14:02:48.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/__init__.py
+-rw-rw-rw-   0        0        0     4078 2024-05-14 14:21:32.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/split.py
+-rw-rw-rw-   0        0        0     6425 2024-05-13 08:09:25.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.135662 indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/
+-rw-rw-rw-   0        0        0       45 2024-05-14 14:02:48.000000 indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/__init__.py
+-rw-rw-rw-   0        0        0     2453 2024-05-15 14:05:13.000000 indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/loader.py
+-rw-rw-rw-   0        0        0     3596 2024-05-15 08:19:59.000000 indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/split.py
+-rw-rw-rw-   0        0        0      108 2024-05-14 14:18:27.000000 indox-0.1.4/Indox/DataLoaderSplitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.136662 indox-0.1.4/Indox/Embeddings/
+-rw-rw-rw-   0        0        0       67 2024-05-12 16:34:51.000000 indox-0.1.4/Indox/Embeddings/__init__.py
+-rw-rw-rw-   0        0        0      441 2024-05-21 05:20:09.000000 indox-0.1.4/Indox/Embeddings/embedding_models.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.139661 indox-0.1.4/Indox/Evaluation/
+-rw-rw-rw-   0        0        0       28 2024-05-13 12:54:42.000000 indox-0.1.4/Indox/Evaluation/__init__.py
+-rw-rw-rw-   0        0        0     8003 2024-05-21 05:20:09.000000 indox-0.1.4/Indox/Evaluation/eval.py
+-rw-rw-rw-   0        0        0     2906 2024-05-13 12:39:30.000000 indox-0.1.4/Indox/Evaluation/metrics.py
+-rw-rw-rw-   0        0        0     4719 2024-05-19 08:29:16.000000 indox-0.1.4/Indox/Evaluation/similarity.py
+-rw-rw-rw-   0        0        0    10059 2024-05-13 12:39:30.000000 indox-0.1.4/Indox/Evaluation/unieval.py
+-rw-rw-rw-   0        0        0     2453 2024-05-11 13:44:58.000000 indox-0.1.4/Indox/Graph.py
+-rw-rw-rw-   0        0        0     8869 2024-05-16 15:16:32.000000 indox-0.1.4/Indox/Indox.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.140662 indox-0.1.4/Indox/QaModels/
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.141661 indox-0.1.4/Indox/QaModels/Dspy_Cot/
+-rw-rw-rw-   0        0        0       27 2024-05-12 15:50:15.000000 indox-0.1.4/Indox/QaModels/Dspy_Cot/__init__.py
+-rw-rw-rw-   0        0        0     2604 2024-05-20 11:24:22.000000 indox-0.1.4/Indox/QaModels/Dspy_Cot/dspy.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.142662 indox-0.1.4/Indox/QaModels/Mistral/
+-rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.4/Indox/QaModels/Mistral/__init__.py
+-rw-rw-rw-   0        0        0     2684 2024-05-20 11:34:09.000000 indox-0.1.4/Indox/QaModels/Mistral/mistral.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.143664 indox-0.1.4/Indox/QaModels/OpenAi/
+-rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.4/Indox/QaModels/OpenAi/__init__.py
+-rw-rw-rw-   0        0        0     2185 2024-05-20 11:23:53.000000 indox-0.1.4/Indox/QaModels/OpenAi/openai.py
+-rw-rw-rw-   0        0        0       95 2024-05-14 13:59:17.000000 indox-0.1.4/Indox/QaModels/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.143664 indox-0.1.4/Indox/Splitter/
+-rw-rw-rw-   0        0        0       60 2024-05-15 04:55:56.000000 indox-0.1.4/Indox/Splitter/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-05-14 14:16:18.000000 indox-0.1.4/Indox/Splitter/semantic_text_splitter.py
+-rw-rw-rw-   0        0        0       66 2024-05-12 15:34:14.000000 indox-0.1.4/Indox/__init__.py
+-rw-rw-rw-   0        0        0      960 2024-05-14 11:18:39.000000 indox-0.1.4/Indox/config.yaml
+-rw-rw-rw-   0        0        0     2738 2024-05-15 06:17:01.000000 indox-0.1.4/Indox/utils.py
+-rw-rw-rw-   0        0        0     8896 2024-05-13 14:07:14.000000 indox-0.1.4/Indox/vectorstore.py
+-rw-rw-rw-   0        0        0     2562 2024-05-16 15:16:32.000000 indox-0.1.4/Indox/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.144661 indox-0.1.4/Indox.egg-info/
+-rw-rw-rw-   0        0        0     8261 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1391 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-05-11 13:44:58.000000 indox-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     8261 2024-05-21 15:54:06.145660 indox-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6916 2024-05-20 09:59:26.000000 indox-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:54:06.146660 indox-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2024-05-21 14:19:39.000000 indox-0.1.4/setup.py
```

### Comparing `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py` & `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py` & `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/EmbedClusterSummarize.py` & `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/EmbedClusterSummarize.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py` & `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/split.py` & `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/split.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/utils.py` & `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/utils.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/loader.py` & `indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/loader.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/split.py` & `indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/split.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/Evaluation/eval.py` & `indox-0.1.4/Indox/Evaluation/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 from typing import Dict, Any
 
 import pandas as pd
 import textstat
 import torch
 from bert_score import BERTScorer
+from pandas import DataFrame
 from sentence_transformers import CrossEncoder
 from transformers import BertTokenizer, BertForSequenceClassification, GPT2LMHeadModel, GPT2Tokenizer
 from transformers import pipeline
 from .similarity import Similarity
-
+import numpy as np
 cfg = {"bert_toxic_tokenizer": "unitary/toxic-bert",
        "bert_toxic_model": "unitary/toxic-bert",
        "semantic_similarity": "sentence-transformers/bert-base-nli-mean-tokens",
        "bert_score_model": "bert-base-uncased",
        "reliability": 'vectara/hallucination_evaluation_model',
        "fairness": "wu981526092/Sentence-Level-Stereotype-Detector",
 
        }
 
 ALL_DIMANSIONS = ["BertScore", "Toxicity", "Similarity", "Reliability", "Fairness" , "Readibility"]
 
 
+def to_float(x):
+    if isinstance(x, np.ndarray):
+        return x.item()  # Convert numpy array to a single float
+    return float(x)  # Convert other types to float
+
+
 class Evaluation:
     def __init__(self, dimensions=None, config=cfg):
         if dimensions is None:
             dimensions = ALL_DIMANSIONS
 
         self.config = config
         if not isinstance(dimensions, list):
             dimensions = [dimensions]
 
         self.metrics = [eval(dim)(self.config) for dim in dimensions]
         self.result = pd.DataFrame()
 
-    def __call__(self, inputs=None) -> Dict[str, Any]:
+    def __call__(self, inputs=None) -> DataFrame:
         scores = {}
         [scores.update(score(inputs)) for score in self.metrics]
+        scores = pd.DataFrame(scores)
+        scores = scores.applymap(to_float).T
         return scores
 
     def update(self, inputs: Any) -> pd.DataFrame:
         result = self.__call__(inputs)
-        self.result = pd.concat([self.result, pd.DataFrame([result])], ignore_index=True)
+        self.result = pd.concat([self.result, result], ignore_index=True)
         return self.result
 
     def reset(self) -> None:
         self.result = pd.DataFrame()
 
 
 class BertScore(BERTScorer):
```

### Comparing `indox-0.1.3/Indox/Evaluation/metrics.py` & `indox-0.1.4/Indox/Evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/Evaluation/similarity.py` & `indox-0.1.4/Indox/Evaluation/similarity.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/Evaluation/unieval.py` & `indox-0.1.4/Indox/Evaluation/unieval.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/Graph.py` & `indox-0.1.4/Indox/Graph.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/Indox.py` & `indox-0.1.4/Indox/Indox.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/QaModels/Dspy_Cot/dspy.py` & `indox-0.1.4/Indox/QaModels/Dspy_Cot/dspy.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     Module class for DspyCotQA.
 
     Attributes:
         model (str): The model to be used.
         client (OpenAI): The OpenAI client.
     """
 
-    def __init__(self, model="gpt-3.5-turbo-0125", api_key=os.environ["OPENAI_API_KEY"]):
+    def __init__(self, model, api_key):
         super().__init__()
         self.model = model
         self.client = OpenAI(model=self.model, api_key=api_key)
         settings.configure(lm=self.client)
 
     def answer_question(self, context, question):
         """
```

### Comparing `indox-0.1.3/Indox/QaModels/Mistral/mistral.py` & `indox-0.1.4/Indox/QaModels/Mistral/mistral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import requests
-import os
 
 
 class MistralQA:
-    def __init__(self, model="mistralai/Mistral-7B-Instruct-v0.2", api_key=os.getenv("HF_API_KEY")):
+    def __init__(self, api_key, model):
         """
         Initializes the Mistral 7B Instruct model via the Hugging Face Inference API.
 
         Args:
             model (str, optional): The Mistral model version to use. Defaults to "mistralai/Mistral-7B-Instruct-v0.2".
         """
         self.model = model
```

### Comparing `indox-0.1.3/Indox/QaModels/OpenAi/openai.py` & `indox-0.1.4/Indox/QaModels/OpenAi/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 from openai import OpenAI
 import os
 
+
 class OpenAiQA:
-    def __init__(self, model="gpt-3.5-turbo-0125",api_key=os.environ["OPENAI_API_KEY"]):
+    def __init__(self, api_key, model):
         """
         Initializes the GPT-3 model with the specified model version.
 
         Args:
             model (str, optional): The GPT-3 model version to use for generating summaries. Defaults to "text-davinci-003".
         """
         self.model = model
```

### Comparing `indox-0.1.3/Indox/config.yaml` & `indox-0.1.4/Indox/config.yaml`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/utils.py` & `indox-0.1.4/Indox/utils.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/vectorstore.py` & `indox-0.1.4/Indox/vectorstore.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox/visualization.py` & `indox-0.1.4/Indox/visualization.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/Indox.egg-info/PKG-INFO` & `indox-0.1.4/Indox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Indox
-Version: 0.1.3
+Version: 0.1.4
 Summary: Indox Retrieval Augmentation
 Home-page: https://github.com/osllmai/inDox
 Author: nerdstudio
 Author-email: ashkan@nematifamilyfundation.onmicrosoft.com
 License: MIT
 Keywords: RAG,LLM
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `indox-0.1.3/Indox.egg-info/SOURCES.txt` & `indox-0.1.4/Indox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/PKG-INFO` & `indox-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Indox
-Version: 0.1.3
+Version: 0.1.4
 Summary: Indox Retrieval Augmentation
 Home-page: https://github.com/osllmai/inDox
 Author: nerdstudio
 Author-email: ashkan@nematifamilyfundation.onmicrosoft.com
 License: MIT
 Keywords: RAG,LLM
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `indox-0.1.3/README.md` & `indox-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `indox-0.1.3/setup.py` & `indox-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Read the README file for the long description
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='Indox',
-    version='0.1.3',
+    version='0.1.4',
     license='MIT',
     packages=find_packages(),
     package_data={'Indox': ['config.yaml']},
     include_package_data=True,
     description='Indox Retrieval Augmentation',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

