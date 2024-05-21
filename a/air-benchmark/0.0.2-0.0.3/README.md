# Comparing `tmp/air_benchmark-0.0.2.tar.gz` & `tmp/air_benchmark-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air_benchmark-0.0.2.tar", last modified: Tue May 14 15:26:23 2024, max compression
+gzip compressed data, was "air_benchmark-0.0.3.tar", last modified: Tue May 21 06:32:49 2024, max compression
```

## Comparing `air_benchmark-0.0.2.tar` & `air_benchmark-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,53 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-14 15:26:23.088621 air_benchmark-0.0.2/
--rw-r--r--   0 bo         (501) staff       (20)     1066 2024-05-13 06:34:57.000000 air_benchmark-0.0.2/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     7466 2024-05-14 15:26:23.087840 air_benchmark-0.0.2/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)     5035 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-14 15:26:23.071139 air_benchmark-0.0.2/air_benchmark/
--rw-r--r--   0 bo         (501) staff       (20)        0 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     6341 2024-05-14 15:26:01.000000 air_benchmark-0.0.2/air_benchmark/air_benchmark.py
--rw-r--r--   0 bo         (501) staff       (20)      108 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/console.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-14 15:26:23.078692 air_benchmark-0.0.2/air_benchmark/evaluation_utils/
--rw-r--r--   0 bo         (501) staff       (20)        0 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/evaluation_utils/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     1096 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/evaluation_utils/data_loader.py
--rw-r--r--   0 bo         (501) staff       (20)     1291 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/evaluation_utils/evaluation_arguments.py
--rw-r--r--   0 bo         (501) staff       (20)     6700 2024-05-14 15:26:01.000000 air_benchmark-0.0.2/air_benchmark/evaluation_utils/evaluator.py
--rw-r--r--   0 bo         (501) staff       (20)     6131 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/evaluation_utils/searcher.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-14 15:26:23.081089 air_benchmark-0.0.2/air_benchmark/model_utils/
--rw-r--r--   0 bo         (501) staff       (20)      143 2024-05-14 15:11:52.000000 air_benchmark-0.0.2/air_benchmark/model_utils/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)    12125 2024-05-14 15:26:01.000000 air_benchmark-0.0.2/air_benchmark/model_utils/flag_dres_model.py
--rw-r--r--   0 bo         (501) staff       (20)     1646 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/model_utils/model_arguments.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-14 15:26:23.084289 air_benchmark-0.0.2/air_benchmark/tasks/
--rw-r--r--   0 bo         (501) staff       (20)        0 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/tasks/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2434 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/tasks/long_doc_tasks.py
--rw-r--r--   0 bo         (501) staff       (20)     2391 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/air_benchmark/tasks/qa_tasks.py
--rw-r--r--   0 bo         (501) staff       (20)     4498 2024-05-14 15:26:01.000000 air_benchmark-0.0.2/air_benchmark/tasks/tasks.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-14 15:26:23.086604 air_benchmark-0.0.2/air_benchmark.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     7466 2024-05-14 15:26:23.000000 air_benchmark-0.0.2/air_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      876 2024-05-14 15:26:23.000000 air_benchmark-0.0.2/air_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2024-05-14 15:26:23.000000 air_benchmark-0.0.2/air_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       52 2024-05-14 15:26:23.000000 air_benchmark-0.0.2/air_benchmark.egg-info/entry_points.txt
--rw-r--r--   0 bo         (501) staff       (20)      103 2024-05-14 15:26:23.000000 air_benchmark-0.0.2/air_benchmark.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)       58 2024-05-14 15:26:23.000000 air_benchmark-0.0.2/air_benchmark.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)     1349 2024-05-14 15:26:01.000000 air_benchmark-0.0.2/pyproject.toml
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-14 15:26:23.085824 air_benchmark-0.0.2/scripts/
--rw-r--r--   0 bo         (501) staff       (20)     5532 2024-05-14 15:11:52.000000 air_benchmark-0.0.2/scripts/run_air_bench.py
--rw-r--r--   0 bo         (501) staff       (20)     3740 2024-05-14 15:00:34.000000 air_benchmark-0.0.2/scripts/zip_results.py
--rw-r--r--   0 bo         (501) staff       (20)       38 2024-05-14 15:26:23.088851 air_benchmark-0.0.2/setup.cfg
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.792834 air_benchmark-0.0.3/
+-rw-r--r--   0 bo         (501) staff       (20)     1066 2024-05-13 06:34:57.000000 air_benchmark-0.0.3/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     8698 2024-05-21 06:32:49.792033 air_benchmark-0.0.3/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     6359 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.773059 air_benchmark-0.0.3/air_benchmark/
+-rw-r--r--   0 bo         (501) staff       (20)      274 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/air_benchmark/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     5989 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/air_benchmark/air_benchmark.py
+-rw-r--r--   0 bo         (501) staff       (20)      108 2024-05-14 15:00:34.000000 air_benchmark-0.0.3/air_benchmark/console.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.780172 air_benchmark-0.0.3/air_benchmark/evaluation_utils/
+-rw-r--r--   0 bo         (501) staff       (20)        0 2024-05-14 15:00:34.000000 air_benchmark-0.0.3/air_benchmark/evaluation_utils/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     1096 2024-05-14 15:00:34.000000 air_benchmark-0.0.3/air_benchmark/evaluation_utils/data_loader.py
+-rw-r--r--   0 bo         (501) staff       (20)     1037 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/air_benchmark/evaluation_utils/evaluation_arguments.py
+-rw-r--r--   0 bo         (501) staff       (20)     6232 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/air_benchmark/evaluation_utils/evaluator.py
+-rw-r--r--   0 bo         (501) staff       (20)     3062 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/air_benchmark/evaluation_utils/searcher.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.782580 air_benchmark-0.0.3/air_benchmark/tasks/
+-rw-r--r--   0 bo         (501) staff       (20)        0 2024-05-14 15:00:34.000000 air_benchmark-0.0.3/air_benchmark/tasks/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2434 2024-05-14 15:00:34.000000 air_benchmark-0.0.3/air_benchmark/tasks/long_doc_tasks.py
+-rw-r--r--   0 bo         (501) staff       (20)     2196 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/air_benchmark/tasks/qa_tasks.py
+-rw-r--r--   0 bo         (501) staff       (20)     4312 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/air_benchmark/tasks/tasks.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.790709 air_benchmark-0.0.3/air_benchmark.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     8698 2024-05-21 06:32:49.000000 air_benchmark-0.0.3/air_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     1347 2024-05-21 06:32:49.000000 air_benchmark-0.0.3/air_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2024-05-21 06:32:49.000000 air_benchmark-0.0.3/air_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       52 2024-05-21 06:32:49.000000 air_benchmark-0.0.3/air_benchmark.egg-info/entry_points.txt
+-rw-r--r--   0 bo         (501) staff       (20)       56 2024-05-21 06:32:49.000000 air_benchmark-0.0.3/air_benchmark.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)       58 2024-05-21 06:32:49.000000 air_benchmark-0.0.3/air_benchmark.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)     1282 2024-05-21 06:29:02.000000 air_benchmark-0.0.3/pyproject.toml
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.782935 air_benchmark-0.0.3/scripts/
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.783475 air_benchmark-0.0.3/scripts/bm25/
+-rw-r--r--   0 bo         (501) staff       (20)     1378 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/bm25/evaluate_bm25.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.784722 air_benchmark-0.0.3/scripts/bm25/utils/
+-rw-r--r--   0 bo         (501) staff       (20)        0 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/bm25/utils/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)      324 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/bm25/utils/arguments.py
+-rw-r--r--   0 bo         (501) staff       (20)     4296 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/bm25/utils/searcher.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.785070 air_benchmark-0.0.3/scripts/hf-transformers/
+-rw-r--r--   0 bo         (501) staff       (20)     3910 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/hf-transformers/evaluate_hf_transformers.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.787878 air_benchmark-0.0.3/scripts/hf-transformers/utils/
+-rw-r--r--   0 bo         (501) staff       (20)        0 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/hf-transformers/utils/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2266 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/hf-transformers/utils/arguments.py
+-rw-r--r--   0 bo         (501) staff       (20)    12383 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/hf-transformers/utils/models.py
+-rw-r--r--   0 bo         (501) staff       (20)     2499 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/hf-transformers/utils/searcher.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.788424 air_benchmark-0.0.3/scripts/sentence-transformers/
+-rw-r--r--   0 bo         (501) staff       (20)     3115 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/sentence-transformers/evaluate_sentence_transformers.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.789761 air_benchmark-0.0.3/scripts/sentence-transformers/utils/
+-rw-r--r--   0 bo         (501) staff       (20)        0 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/sentence-transformers/utils/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     1413 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/sentence-transformers/utils/arguments.py
+-rw-r--r--   0 bo         (501) staff       (20)     2805 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/sentence-transformers/utils/models.py
+-rw-r--r--   0 bo         (501) staff       (20)     2563 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/sentence-transformers/utils/searcher.py
+-rw-r--r--   0 bo         (501) staff       (20)     3813 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/scripts/zip_results.py
+-rw-r--r--   0 bo         (501) staff       (20)       38 2024-05-21 06:32:49.793095 air_benchmark-0.0.3/setup.cfg
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.770309 air_benchmark-0.0.3/tests/
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-05-21 06:32:49.790113 air_benchmark-0.0.3/tests/tasks/
+-rw-r--r--   0 bo         (501) staff       (20)      300 2024-05-21 06:27:28.000000 air_benchmark-0.0.3/tests/tasks/test_tasks.py
```

### Comparing `air_benchmark-0.0.2/LICENSE` & `air_benchmark-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `air_benchmark-0.0.2/air_benchmark/air_benchmark.py` & `air_benchmark-0.0.3/air_benchmark/air_benchmark.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import logging
 from typing import List, Optional
 
 from air_benchmark.console import console, style_head, style_row
 from air_benchmark.evaluation_utils.data_loader import DataLoader
 from air_benchmark.evaluation_utils.evaluator import Evaluator
-from air_benchmark.evaluation_utils.searcher import Searcher
-from air_benchmark.model_utils.flag_dres_model import (FlagDRESModel,
-                                                       FlagDRESReranker)
-from air_benchmark.tasks.tasks import (BenchmarkTable, check_benchmark_version,
-                                       check_domains, check_languages,
-                                       check_task_types, get_task_name_list)
+from air_benchmark.evaluation_utils.searcher import Retriever, Reranker
+from air_benchmark.tasks.tasks import (
+    BenchmarkTable,
+    check_benchmark_version,
+    check_domains,
+    check_languages,
+    check_task_types,
+    get_task_name_list,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class AIRBench:
     def __init__(
         self,
@@ -30,79 +33,76 @@
         self.cache_dir = cache_dir
 
         self.data_loader = DataLoader(self.benchmark_version, cache_dir=self.cache_dir)
 
     @staticmethod
     def print_benchmark_table():
         for benchmark_version in BenchmarkTable:
-            print(
-                f"==================== Benchmark Version: {benchmark_version} ===================="
+
+            console.print(
+                f"Benchmark Dataset Version: {benchmark_version}",
+                style=style_head,
+                justify="center",
             )
+
             for task_type in BenchmarkTable[benchmark_version]:
-                print(
-                    f"  ******************* Task Type: {task_type} *******************"
+                console.print(
+                    f"Task Type: {task_type}", style=style_head, justify="center"
                 )
                 for domain in BenchmarkTable[benchmark_version][task_type]:
-                    print(
-                        f"    +++++++++++++++++++ Domain: {domain} +++++++++++++++++++"
+                    console.print(
+                        f"Domain: {domain}", style=style_head, justify="center"
                     )
                     for language in BenchmarkTable[benchmark_version][task_type][
                         domain
                     ]:
-                        print(
-                            f"      ------------------- Language: {language} -------------------"
+                        console.print(
+                            f"Language: {language}", style=style_head, justify="center"
                         )
                         for task_name in BenchmarkTable[benchmark_version][task_type][
                             domain
                         ][language]:
-                            print(f"        Task Name: {task_name}")
-                            print(
-                                f"        Source: {BenchmarkTable[benchmark_version][task_type][domain][language][task_name]['source']}"
+                            console.print(
+                                f"Task Name: {task_name}",
+                                style=style_row,
+                                justify="center",
+                            )
+                            console.print(
+                                f"Source: \
+                                {BenchmarkTable[benchmark_version][task_type][domain][language][task_name]['source']}",
+                                style=style_row,
+                                justify="center",
                             )
 
     @staticmethod
-    def check_encoder(encoder):
-        for method in ["__str__", "encode_queries", "encode_corpus"]:
-            if not hasattr(encoder, method) or not callable(
-                getattr(encoder, method, None)
+    def check_retriever(retriever):
+        for method in ["__str__", "__call__"]:
+            if not hasattr(retriever, method) or not callable(
+                getattr(retriever, method, None)
             ):
-                raise ValueError(f"Encoder should have `{method}` method.")
+                raise ValueError(f"Retriever should have `{method}` method.")
 
     @staticmethod
     def check_reranker(reranker):
-        for method in ["__str__", "compute_score"]:
+        for method in ["__str__", "__call__"]:
             if not hasattr(reranker, method) or not callable(
                 getattr(reranker, method, None)
             ):
                 raise ValueError(f"Reranker should have `{method}` method.")
 
     def run(
         self,
-        encoder: FlagDRESModel,
-        output_dir: str = "search_results",
-        search_top_k: int = 1000,
-        reranker_list: Optional[List[FlagDRESReranker]] = None,
-        rerank_top_k: int = 100,
+        retriever: Retriever,
+        reranker: Optional[Reranker] = None,
+        output_dir: str = "./search_results",
         overwrite: bool = False,
         **kwargs,
     ):
-        self.check_encoder(encoder)
-        if reranker_list is not None:
-            for reranker in reranker_list:
-                self.check_reranker(reranker)
-
-        searcher = Searcher(search_top_k)
-        evaluator = Evaluator(
-            self.data_loader,
-            searcher,
-            rerank_top_k=rerank_top_k,
-            k_values=[search_top_k],
-            overwrite=overwrite,
-        )
-
+        evaluator = Evaluator(self.data_loader, overwrite=overwrite)
+        
         for task_type in self.task_types:
             console.print(f"Task Type: {task_type}", style=style_head, justify="center")
             for domain in self.domains:
                 console.print(f"Domain: {domain}", style=style_head, justify="center")
                 for language in self.languages:
                     success, task_name_list = get_task_name_list(
                         self.benchmark_version, task_type, domain, language
@@ -120,33 +120,30 @@
 
                     for task_name in task_name_list:
                         console.print(
                             f"Task Name: {task_name}",
                             style=style_head,
                             justify="center",
                         )
-
-                        evaluator.generate_search_results(
-                            model=encoder,
-                            reranker_list=reranker_list,
-                            search_results_save_dir=output_dir,
+                        
+                        evaluator(
                             task_type=task_type,
                             domain=domain,
                             language=language,
                             task_name=task_name,
+                            search_results_save_dir=output_dir,
+                            retriever=retriever,
+                            reranker=reranker,
                             **kwargs,
                         )
         console.rule("[bold red]Evaluation Summary")
-        console.print(f"Encoder: {encoder}", style=style_row, justify="center")
-        reranker_names = [item.name for item in reranker_list]
-        console.print(
-            f"Rerankers: {*reranker_names,}", style=style_row, justify="center"
-        )
+        console.print(f"Retriever: {retriever}", style=style_row, justify="center")
+        console.print(f"Reranker: {reranker}", style=style_row, justify="center")
         console.print(
             f"Output directory: {output_dir}", style=style_row, justify="center"
         )
         console.print(
-            f"Search Top K: {search_top_k}", style=style_row, justify="center"
+            f"Search Top K: {retriever.search_top_k}", style=style_row, justify="center"
         )
         console.print(
-            f"Rerank Top K: {rerank_top_k}", style=style_row, justify="center"
+            f"Rerank Top K: {reranker.rerank_top_k}", style=style_row, justify="center"
         )
```

### Comparing `air_benchmark-0.0.2/air_benchmark/evaluation_utils/data_loader.py` & `air_benchmark-0.0.3/air_benchmark/evaluation_utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `air_benchmark-0.0.2/air_benchmark/evaluation_utils/evaluation_arguments.py` & `air_benchmark-0.0.3/air_benchmark/evaluation_utils/evaluation_arguments.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,17 +21,10 @@
     search_top_k: int = field(
         default=1000, metadata={"help": "Top k values for evaluation."}
     )
     rerank_top_k: int = field(default=100, metadata={"help": "Top k for reranking."})
     cache_dir: str = field(
         default=None, metadata={"help": "Cache directory for datasets."}
     )
-    bm25_tmp_dir: str = field(
-        default="./bm25_tmp_dir",
-        metadata={"help": "Cache directory for evaluating BM25."},
-    )
-    remove_bm25_tmp_dir: bool = field(
-        default=True, metadata={"help": "Remove BM25 tmp dir or not."}
-    )
     overwrite: bool = field(
         default=False, metadata={"help": "whether to overwrite evaluation results"}
     )
```

### Comparing `air_benchmark-0.0.2/air_benchmark/evaluation_utils/evaluator.py` & `air_benchmark-0.0.3/air_benchmark/evaluation_utils/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 import json
 import logging
 import os
-from typing import Dict, List, Optional
+from typing import Dict, Optional
 
 from air_benchmark.evaluation_utils.data_loader import DataLoader
-from air_benchmark.evaluation_utils.searcher import Searcher
+from air_benchmark.evaluation_utils.searcher import Retriever, Reranker
 
 logger = logging.getLogger(__name__)
 
 
 class Evaluator:
     def __init__(
         self,
         data_loader: DataLoader,
-        searcher: Optional[Searcher] = None,
-        rerank_top_k: int = 100,
-        k_values: List[int] = [1, 3, 5, 10, 100, 1000],
         overwrite: bool = False,
     ):
         self.data_loader = data_loader
-        self.searcher = searcher if searcher is not None else Searcher(max(k_values))
-        self.rerank_top_k = rerank_top_k
-        self.k_values = k_values
         self.overwrite = overwrite
         self.benchmark_version = data_loader.benchmark_version
 
     def check_data_info(
         self,
         data_info: Dict[str, str],
         model_name: str,
@@ -49,115 +43,110 @@
             data_info["domain"] != domain
             or data_info["language"] != language
             or data_info["task_name"] != task_name
         ):
             raise ValueError(
                 f'domain or language or task_name mismatch: {data_info["domain"]} vs {domain} or {data_info["language"]} vs {language} or {data_info["task_name"]} vs {task_name}'
             )
-
-    def generate_search_results(
+    
+    def __call__(
         self,
-        model,
-        reranker_list,
-        search_results_save_dir: str,
         task_type: str,
         domain: str,
         language: str,
         task_name: str,
+        search_results_save_dir: str,
+        retriever: Retriever,
+        reranker: Optional[Reranker] = None,
         **kwargs,
     ):
+        # Retrieval Stage
         no_reranker_search_results_save_dir = os.path.join(
-            search_results_save_dir, str(model), "NoReranker", task_type
+            search_results_save_dir, str(retriever), "NoReranker", task_type
         )
         os.makedirs(no_reranker_search_results_save_dir, exist_ok=True)
-
+        
         no_reranker_search_results_save_path = os.path.join(
             no_reranker_search_results_save_dir, domain, f"{language}_{task_name}.json"
         )
 
         if os.path.exists(no_reranker_search_results_save_path) and not self.overwrite:
             data_info, no_reranker_search_results = self.load_search_results(
                 no_reranker_search_results_save_path
             )
 
             self.check_data_info(
-                data_info, str(model), "NoReranker", domain, language, task_name
+                data_info, str(retriever), "NoReranker", domain, language, task_name
             )
         else:
             corpus, queries = self.data_loader.load_data(
                 task_type=task_type,
                 domain=domain,
                 language=language,
                 task_name=task_name,
             )
 
-            if str(model) == "BM25":
-                no_reranker_search_results = self.searcher.bm25_search(
-                    bm25_tmp_dir=kwargs.pop("bm25_tmp_dir", "./bm25_tmp_dir"),
-                    corpus=corpus,
-                    queries=queries,
-                    language=language,
-                    **kwargs,
-                )
-            else:
-                no_reranker_search_results = self.searcher.dense_search(
-                    model=model, corpus=corpus, queries=queries, **kwargs
-                )
+            no_reranker_search_results = retriever(
+                corpus=corpus,
+                queries=queries,
+                language=language,  # for language-specific retrievers, such as BM25Retriever
+                **kwargs,
+            )
             self.save_search_results(
-                model_name=str(model),
+                model_name=str(retriever),
                 reranker_name="NoReranker",
                 search_results=no_reranker_search_results,
                 output_path=no_reranker_search_results_save_path,
                 task_type=task_type,
                 domain=domain,
                 language=language,
                 task_name=task_name,
                 benchmark_version=self.benchmark_version,
             )
-
-        for reranker in reranker_list:
+        
+        # Reranking Stage
+        if reranker is not None:
             reranker_search_results_save_dir = os.path.join(
-                search_results_save_dir, str(model), str(reranker), task_type
+                search_results_save_dir, str(retriever), str(reranker), task_type
             )
             os.makedirs(reranker_search_results_save_dir, exist_ok=True)
-
+            
             rerank_search_results_save_path = os.path.join(
                 reranker_search_results_save_dir, domain, f"{language}_{task_name}.json"
             )
-
+            
             if os.path.exists(rerank_search_results_save_path) and not self.overwrite:
-                continue
-
+                return
+            
             corpus, queries = self.data_loader.load_data(
                 task_type=task_type,
                 domain=domain,
                 language=language,
                 task_name=task_name,
             )
-
-            rerank_search_results = self.searcher.rerank(
-                reranker=reranker,
-                search_results=no_reranker_search_results,
+            
+            rerank_search_results = reranker(
                 corpus=corpus,
                 queries=queries,
-                rerank_top_k=self.rerank_top_k,
+                search_results=no_reranker_search_results,
+                **kwargs,
             )
-
+            
             self.save_search_results(
-                model_name=str(model),
+                model_name=str(retriever),
                 reranker_name=str(reranker),
                 search_results=rerank_search_results,
                 output_path=rerank_search_results_save_path,
                 task_type=task_type,
                 domain=domain,
                 language=language,
                 task_name=task_name,
                 benchmark_version=self.benchmark_version,
             )
-
+    
     @staticmethod
     def save_search_results(
         model_name: str,
         reranker_name: str,
         search_results: Dict[str, Dict[str, float]],
         output_path: str,
         task_type: str,
```

### Comparing `air_benchmark-0.0.2/air_benchmark/model_utils/flag_dres_model.py` & `air_benchmark-0.0.3/scripts/hf-transformers/utils/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 from typing import Dict, List, Optional, Tuple, Union, cast
 
 import datasets
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 from tqdm import tqdm
-from transformers import (AutoModel, AutoModelForSequenceClassification,
-                          AutoTokenizer, BatchEncoding,
-                          DataCollatorWithPadding, PreTrainedTokenizerFast,
-                          is_torch_npu_available)
+from transformers import (
+    AutoModel,
+    AutoModelForSequenceClassification,
+    AutoTokenizer,
+    BatchEncoding,
+    DataCollatorWithPadding,
+    PreTrainedTokenizerFast,
+    is_torch_npu_available,
+)
 
 
 def _transform_func(
     examples: Dict[str, List], tokenizer: PreTrainedTokenizerFast, max_length: int
 ) -> BatchEncoding:
     return tokenizer(
         examples["text"],
@@ -28,14 +33,18 @@
 
 def _transform_func_for_last_pooling(
     examples: Dict[str, List],
     tokenizer: PreTrainedTokenizerFast,
     max_length: int = 8192,
 ) -> BatchEncoding:
 
+    if tokenizer.eos_token_id is None:
+        raise ValueError(
+            f"tokenizer.eos_token_id should not be `None`. tokenizer.eos_token_id={tokenizer.eos_token_id}"
+        )
     inputs = tokenizer(
         examples["text"],
         max_length=max_length - 1,
         padding=False,
         return_attention_mask=False,
         truncation=True,
     )
@@ -44,15 +53,19 @@
     ]
     inputs = tokenizer.pad(
         inputs, padding=True, return_attention_mask=True, return_tensors="pt"
     )
     return inputs
 
 
-class FlagDRESModel:
+class DRESModel:
+    """
+    Dense Retrieval Exact Search Models
+    """
+
     def __init__(
         self,
         model_name_or_path: str,
         pooling_method: str = "cls",
         normalize_embeddings: bool = True,
         use_fp16: bool = True,
         query_instruction_for_retrieval: Optional[str] = None,
@@ -62,20 +75,15 @@
         batch_size: int = 256,
         corpus_batch_size: int = 0,
         **kwargs,
     ) -> None:
         self.name = os.path.basename(model_name_or_path)
 
         self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
-        if "jina" in model_name_or_path:
-            self.model = AutoModel.from_pretrained(
-                model_name_or_path, trust_remote_code=True
-            )
-        else:
-            self.model = AutoModel.from_pretrained(model_name_or_path)
+        self.model = AutoModel.from_pretrained(model_name_or_path)
         self.query_instruction_for_retrieval = query_instruction_for_retrieval
         self.passage_instruction_for_retrieval = passage_instruction_for_retrieval
         self.normalize_embeddings = normalize_embeddings
         self.pooling_method = pooling_method
         self.batch_size = batch_size
         self.corpus_batch_size = (
             corpus_batch_size if corpus_batch_size > 0 else batch_size
@@ -96,15 +104,17 @@
         self.num_gpus = torch.cuda.device_count()
         if self.num_gpus > 1:
             self.model = torch.nn.DataParallel(self.model)
 
     def __str__(self) -> str:
         return self.name
 
-    def encode_queries(self, queries: List[str], **kwargs) -> np.ndarray:
+    def encode_queries(
+        self, queries: List[Union[Dict[str, str], str]], **kwargs
+    ) -> np.ndarray:
         """
         This function will be used for retrieval task
         if there is a instruction for queries, we will add it to the query text
         """
         if isinstance(queries[0], dict):
             if self.query_instruction_for_retrieval is not None:
                 input_texts = [
@@ -173,14 +183,17 @@
         input_was_string = False
         if isinstance(sentences, str):
             sentences = [sentences]
             input_was_string = True
 
         dataset = datasets.Dataset.from_dict({"text": sentences})
         if self.pooling_method == "last":
+            assert (
+                self.tokenizer.eos_token_id != None
+            ), "Setting `pooling_method='last'` require tokenizer.eos_token_id != None"
             dataset.set_transform(
                 partial(
                     _transform_func_for_last_pooling,
                     tokenizer=self.tokenizer,
                     max_length=max_length,
                 )
             )
@@ -242,21 +255,25 @@
                 batch_size = last_hidden_state.shape[0]
                 return last_hidden_state[
                     torch.arange(batch_size, device=last_hidden_state.device),
                     sequence_lengths,
                 ]
 
 
-class FlagDRESReranker:
+class DRESReranker:
+    """
+    Dense Retrieval Exact Search Reranker
+    """
+
     def __init__(
         self,
         model_name_or_path: str,
         use_fp16: bool = True,
-        query_instruction_for_retrieval: Optional[str] = None,
-        passage_instruction_for_retrieval: Optional[str] = None,
+        query_instruction_for_reranking: Optional[str] = None,
+        passage_instruction_for_reranking: Optional[str] = None,
         max_length: int = 512,
         batch_size: int = 256,
         **kwargs,
     ):
         self.name = os.path.basename(model_name_or_path)
 
         self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
@@ -266,16 +283,16 @@
                 model_name_or_path, num_labels=1, trust_remote_code=True
             )
         else:
             self.model = AutoModelForSequenceClassification.from_pretrained(
                 model_name_or_path
             )
 
-        self.query_instruction_for_retrieval = query_instruction_for_retrieval
-        self.passage_instruction_for_retrieval = passage_instruction_for_retrieval
+        self.query_instruction_for_reranking = query_instruction_for_reranking
+        self.passage_instruction_for_reranking = passage_instruction_for_reranking
         self.max_length = max_length
         self.batch_size = batch_size
 
         if use_fp16:
             self.model.half()
         if torch.cuda.is_available():
             self.device = torch.device("cuda")
@@ -290,22 +307,22 @@
         if self.num_gpus > 1:
             self.model = torch.nn.DataParallel(self.model)
 
     def __str__(self) -> str:
         return self.name
 
     def add_instruction(self, sentence_pairs: List[Tuple[str, str]]):
-        if self.query_instruction_for_retrieval is not None:
+        if self.query_instruction_for_reranking is not None:
             sentence_pairs = [
-                (f"{self.query_instruction_for_retrieval}{query}", passage)
+                (f"{self.query_instruction_for_reranking}{query}", passage)
                 for query, passage in sentence_pairs
             ]
-        if self.passage_instruction_for_retrieval is not None:
+        if self.passage_instruction_for_reranking is not None:
             sentence_pairs = [
-                (query, f"{self.passage_instruction_for_retrieval}{passage}")
+                (query, f"{self.passage_instruction_for_reranking}{passage}")
                 for query, passage in sentence_pairs
             ]
         return sentence_pairs
 
     @torch.no_grad()
     def compute_score(
         self, sentence_pairs: Union[List[Tuple[str, str]], Tuple[str, str]], **kwargs
```

### Comparing `air_benchmark-0.0.2/air_benchmark/model_utils/model_arguments.py` & `air_benchmark-0.0.3/scripts/hf-transformers/utils/arguments.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,40 +5,50 @@
 class ModelArgs:
     encoder: str = field(
         metadata={
             "help": 'Encoder name or path. For example, "BAAI/bge-m3" or "path/to/encoder".',
             "required": True,
         }
     )
-    reranker: str = field(
-        default=None,
-        metadata={
-            "help": 'One or more reranker name or path. For example, "BAAI/bge-reranker-v2-m3" or "path/to/reranker".',
-            "nargs": "+",
-        },
-    )
     pooling_method: str = field(
         default="cls",
-        metadata={"help": "Pooling method. Avaliable methods: 'cls', 'mean', 'last'"},
+        metadata={"help": "Pooling method. Available methods: 'cls', 'mean', 'last'"},
     )
     normalize_embeddings: bool = field(
         default=True, metadata={"help": "Normalize embeddings or not"}
     )
-    use_fp16: bool = field(default=True, metadata={"help": "Use fp16 for inference."})
-    add_instruction: bool = field(default=False, metadata={"help": "Add instruction?"})
-    query_instruction_for_retrieval: str = field(
+    add_instruction: bool = field(default=False, metadata={"help": "Add instruction for retrieval?"})
+    query_instruction: str = field(
         default=None, metadata={"help": "query instruction for retrieval"}
     )
-    passage_instruction_for_retrieval: str = field(
+    passage_instruction: str = field(
         default=None, metadata={"help": "passage instruction for retrieval"}
     )
-    max_query_length: int = field(default=512, metadata={"help": "Max query length."})
+    max_query_length: int = field(default=512, metadata={"help": "Max query length for retrieval."})
     max_passage_length: int = field(
-        default=512, metadata={"help": "Max passage length."}
+        default=512, metadata={"help": "Max passage length for retrieval."}
     )
-    batch_size: int = field(default=256, metadata={"help": "Inference batch size."})
+    batch_size: int = field(default=256, metadata={"help": "Inference batch size for retrieval."})
     corpus_batch_size: int = field(
         default=0,
         metadata={
             "help": "Inference batch size for corpus. If 0, then use `batch_size`."
         },
     )
+    
+    reranker: str = field(
+        default=None,
+        metadata={
+            "help": 'One or more reranker name or path. For example, "BAAI/bge-reranker-v2-m3" or "path/to/reranker".',
+        },
+    )
+    add_instruction_for_reranking: bool = field(default=False, metadata={"help": "Add instruction for reranking?"})
+    query_instruction_for_reranking: str = field(
+        default=None, metadata={"help": "query instruction for reranking"}
+    )
+    passage_instruction_for_reranking: str = field(
+        default=None, metadata={"help": "passage instruction for reranking"}
+    )
+    max_length_for_reranking: int = field(default=512, metadata={"help": "Max length for reranking."})
+    batch_size_for_reranking: int = field(default=256, metadata={"help": "Inference batch size for reranking."})
+
+    use_fp16: bool = field(default=True, metadata={"help": "Use fp16 for retrieval and reranking."})
```

### Comparing `air_benchmark-0.0.2/air_benchmark/tasks/long_doc_tasks.py` & `air_benchmark-0.0.3/air_benchmark/tasks/long_doc_tasks.py`

 * *Files identical despite different names*

### Comparing `air_benchmark-0.0.2/air_benchmark/tasks/qa_tasks.py` & `air_benchmark-0.0.3/air_benchmark/tasks/qa_tasks.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,20 +36,14 @@
 QALawTask = {
     "en": {
         "default": {
             "name": "Pile of Law (EUR-Lex)",
             "source": "https://huggingface.co/datasets/pile-of-law/pile-of-law",
         }
     },
-    "zh": {
-        "default": {
-            "name": "Law and Regulations Database of the People's Republic of China",
-            "source": "https://flk.npc.gov.cn/index.html",
-        }
-    },
 }
 
 QAArxivTask = {
     "en": {
         "default": {
             "name": "ArXiv (abstracts)",
             "source": "https://github.com/armancohan/long-summarization",
```

### Comparing `air_benchmark-0.0.2/air_benchmark/tasks/tasks.py` & `air_benchmark-0.0.3/air_benchmark/tasks/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+from itertools import chain
 from typing import List, Optional, Tuple
 
-from air_benchmark.tasks.long_doc_tasks import (LongDocArxivTask,
-                                                LongDocBookTask,
-                                                LongDocHealthcareTask,
-                                                LongDocLawTask)
-from air_benchmark.tasks.qa_tasks import (QAArxivTask, QAFinanceTask,
-                                          QAHealthcareTask, QALawTask,
-                                          QAMSMARCOTask, QANewsTask, QAWebTask,
-                                          QAWikiTask)
+from air_benchmark.tasks.long_doc_tasks import (
+    LongDocArxivTask,
+    LongDocBookTask,
+    LongDocHealthcareTask,
+    LongDocLawTask,
+)
+from air_benchmark.tasks.qa_tasks import (
+    QAArxivTask,
+    QAFinanceTask,
+    QAHealthcareTask,
+    QALawTask,
+    QAMSMARCOTask,
+    QANewsTask,
+    QAWebTask,
+    QAWikiTask,
+)
 
 LATEST_BENCHMARK_VERSION = "AIR-Bench_24.04"
 
 
 QATaskTable = {
     "wiki": QAWikiTask,
     "web": QAWebTask,
@@ -39,27 +48,27 @@
 
 
 BenchmarkTable = {
     "AIR-Bench_24.04": TaskTable,
 }
 
 
-def get_avaliable_benchmark_versions() -> List[str]:
+def get_available_benchmark_versions() -> List[str]:
     return sorted(list(BenchmarkTable.keys()))
 
 
-def get_avaliable_task_types() -> List[str]:
+def get_available_task_types() -> List[str]:
     return sorted(list(TaskTable.keys()))
 
 
 def get_available_domains() -> List[str]:
-    return sorted(list(QATaskTable.keys() or LongDocTaskTable.keys()))
+    return sorted(list(frozenset(chain(QATaskTable, LongDocTaskTable))))
 
 
-def get_avaliable_languages() -> List[str]:
+def get_available_languages() -> List[str]:
     languages = set()
     for task in QATaskTable.values():
         for lang in task.keys():
             languages.add(lang)
     for task in LongDocTaskTable.values():
         for lang in task.keys():
             languages.add(lang)
@@ -67,65 +76,65 @@
     return sorted(list(languages))
 
 
 def check_benchmark_version(benchmark_version: Optional[str]) -> str:
     if benchmark_version is None:
         benchmark_version = LATEST_BENCHMARK_VERSION
     else:
-        avaliable_benchmark_versions = get_avaliable_benchmark_versions()
+        available_benchmark_versions = get_available_benchmark_versions()
 
-        if benchmark_version not in avaliable_benchmark_versions:
+        if benchmark_version not in available_benchmark_versions:
             raise ValueError(
-                f"Invalid benchmark version: {benchmark_version}. Avaliable versions: {', '.join(avaliable_benchmark_versions)}"
+                f"Invalid benchmark version: {benchmark_version}. Available versions: {', '.join(available_benchmark_versions)}"
             )
 
     return benchmark_version
 
 
 def check_task_types(task_types: Optional[List[str]]) -> List[str]:
-    avaliable_task_types = get_avaliable_task_types()
+    available_task_types = get_available_task_types()
     if task_types is None:
-        task_types = avaliable_task_types
+        task_types = available_task_types
     else:
         task_types = list(set(task_types))
         task_types = [task_type.lower() for task_type in task_types]
         for task_type in task_types:
-            if task_type not in avaliable_task_types:
+            if task_type not in available_task_types:
                 raise ValueError(
-                    f"Invalid task type: {task_type}. Avaliable task types: {', '.join(avaliable_task_types)}"
+                    f"Invalid task type: {task_type}. Available task types: {', '.join(available_task_types)}"
                 )
     return task_types
 
 
 def check_domains(domains: Optional[List[str]]) -> List[str]:
-    avaliable_domains = get_available_domains()
+    available_domains = get_available_domains()
     if domains is None:
-        domains = avaliable_domains
+        domains = available_domains
     else:
         domains = list(set(domains))
         domains = [domain.lower() for domain in domains]
         for domain in domains:
-            if domain not in avaliable_domains:
+            if domain not in available_domains:
                 raise ValueError(
-                    f"Invalid domain: {domain}. Avaliable domains: {', '.join(avaliable_domains)}"
+                    f"Invalid domain: {domain}. Available domains: {', '.join(available_domains)}"
                 )
     return domains
 
 
 def check_languages(languages: Optional[List[str]]) -> List[str]:
-    avaliable_languages = get_avaliable_languages()
+    available_languages = get_available_languages()
     if languages is None:
-        languages = avaliable_languages
+        languages = available_languages
     else:
         languages = list(set(languages))
         languages = [language.lower() for language in languages]
         for language in languages:
-            if language not in avaliable_languages:
+            if language not in available_languages:
                 raise ValueError(
-                    f"Invalid language: {language}. Avaliable languages: {', '.join(avaliable_languages)}"
+                    f"Invalid language: {language}. Available languages: {', '.join(available_languages)}"
                 )
     return languages
 
 
 def get_task_name_list(
     benchmark_version: str, task_type: str, domain: str, language: str
 ) -> Tuple[bool, str]:
```

### Comparing `air_benchmark-0.0.2/pyproject.toml` & `air_benchmark-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "air-benchmark"
-version = "0.0.2"
+version = "0.0.3"
 description = "AIR-Bench: Automated Heterogeneous Information Retrieval Benchmark"
 readme = "README.md"
 authors = [{ name = "BAAI", email = "zhengliu1026@gmail.com" }, { name = "Jina AI", email = "research@jina.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -17,17 +17,14 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 keywords = ["embedding", "benchmark", "air-bench", "reranker", "information retrieval"]
 dependencies = [
     "datasets>=2.18.0",
-    "mteb>=1.7.17",
-    "torch>=1.6.0",
-    "transformers>=4.33.0",
     "rich>=13.7.1",
 ]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pytest"]
 
@@ -36,8 +33,8 @@
 "Huggingface Organization" = "https://huggingface.co/AIR-Bench"
 "Leaderboard" = "https://huggingface.co/spaces/AIR-Bench/leaderboard"
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "results"]
 
 [project.scripts]
-realpython = "reader.__main__:main"
+realpython = "reader.__main__:main"
```

### Comparing `air_benchmark-0.0.2/scripts/run_air_bench.py` & `air_benchmark-0.0.3/scripts/hf-transformers/evaluate_hf_transformers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,184 +1,133 @@
 """
-# Run all tasks
-python run_air_bench.py \
---output_dir ./search_results \
---encoder BAAI/bge-m3 \
---reranker BAAI/bge-reranker-v2-m3 \
---search_top_k 1000 \
---rerank_top_k 100 \
---max_query_length 512 \
---max_passage_length 512 \
---batch_size 512 \
---pooling_method cls \
---normalize_embeddings True \
---use_fp16 True \
---add_instruction False \
---overwrite False
+Requirements:
+    mteb>=1.7.17
+    torch>=1.6.0
+    transformers>=4.33.0
 
-# Run the tasks in the specified task type
-python run_air_bench.py \
---task_types long-doc \
---output_dir ./search_results \
---encoder BAAI/bge-m3 \
---reranker BAAI/bge-reranker-v2-m3 \
---search_top_k 1000 \
---rerank_top_k 100 \
---max_query_length 512 \
---max_passage_length 512 \
---batch_size 512 \
---pooling_method cls \
---normalize_embeddings True \
---use_fp16 True \
---add_instruction False \
---overwrite False
-
-# Run the tasks in the specified task type and domains
-python run_air_bench.py \
---task_types long-doc \
---domains arxiv book \
+# Run all tasks
+python evaluate_hf_transformers.py \
 --output_dir ./search_results \
 --encoder BAAI/bge-m3 \
---reranker BAAI/bge-reranker-v2-m3 \
 --search_top_k 1000 \
---rerank_top_k 100 \
 --max_query_length 512 \
 --max_passage_length 512 \
 --batch_size 512 \
 --pooling_method cls \
 --normalize_embeddings True \
---use_fp16 True \
---add_instruction False \
---overwrite False
-
-# Run the tasks in the specified languages
-python run_air_bench.py \
---languages en \
---output_dir ./search_results \
---encoder BAAI/bge-m3 \
 --reranker BAAI/bge-reranker-v2-m3 \
---search_top_k 1000 \
 --rerank_top_k 100 \
---max_query_length 512 \
---max_passage_length 512 \
---batch_size 512 \
---pooling_method cls \
---normalize_embeddings True \
+--max_length_for_reranking 512 \
+--batch_size_for_reranking 512 \
 --use_fp16 True \
---add_instruction False \
 --overwrite False
 
 # Run the tasks in the specified task type, domains, and languages
-python run_air_bench.py \
+python evaluate_hf_transformers.py \
 --task_types qa \
---domains wiki web \
+--domains finance law \
 --languages en \
 --output_dir ./search_results \
 --encoder BAAI/bge-m3 \
---reranker BAAI/bge-reranker-v2-m3 \
 --search_top_k 1000 \
---rerank_top_k 100 \
 --max_query_length 512 \
 --max_passage_length 512 \
 --batch_size 512 \
 --pooling_method cls \
 --normalize_embeddings True \
+--reranker BAAI/bge-reranker-v2-m3 \
+--rerank_top_k 100 \
+--batch_size_for_reranking 512 \
 --use_fp16 True \
---add_instruction False \
 --overwrite False
 """
-
-import logging
-
 from transformers import HfArgumentParser
 
-from air_benchmark.air_benchmark import AIRBench
-from air_benchmark.evaluation_utils.evaluation_arguments import EvalArgs
-from air_benchmark.model_utils.flag_dres_model import (FlagDRESModel,
-                                                       FlagDRESReranker)
-from air_benchmark.model_utils.model_arguments import ModelArgs
+from air_benchmark import EvalArgs, AIRBench
 
-logger = logging.getLogger(__name__)
+from utils.arguments import ModelArgs
+from utils.models import DRESModel, DRESReranker
+from utils.searcher import EmbeddingModelRetriever, CrossEncoderReranker
 
 
 def get_models(model_args: ModelArgs):
-    if model_args.encoder.lower() == "bm25":
-        return "BM25", []
-    encoder = FlagDRESModel(
-        model_name_or_path=model_args.encoder,
+    embedding_model = DRESModel(
+        model_args.encoder,
         pooling_method=model_args.pooling_method,
         normalize_embeddings=model_args.normalize_embeddings,
         use_fp16=model_args.use_fp16,
         query_instruction_for_retrieval=(
-            model_args.query_instruction_for_retrieval
+            model_args.query_instruction
             if model_args.add_instruction
             else None
         ),
         passage_instruction_for_retrieval=(
-            model_args.passage_instruction_for_retrieval
+            model_args.passage_instruction
             if model_args.add_instruction
             else None
         ),
         max_query_length=model_args.max_query_length,
         max_passage_length=model_args.max_passage_length,
         batch_size=model_args.batch_size,
         corpus_batch_size=model_args.corpus_batch_size,
     )
-    reranker_list = []
+    cross_encoder = None
     if model_args.reranker is not None:
-        for i in range(len(model_args.reranker)):
-            reranker = model_args.reranker[i]
-        for reranker in model_args.reranker:
-            if reranker is None or reranker.lower() == "none" or reranker == "":
-                continue
-            reranker_list.append(
-                FlagDRESReranker(
-                    model_name_or_path=reranker,
-                    use_fp16=model_args.use_fp16,
-                    query_instruction_for_retrieval=(
-                        model_args.query_instruction_for_retrieval
-                        if model_args.add_instruction
-                        else None
-                    ),
-                    passage_instruction_for_retrieval=(
-                        model_args.passage_instruction_for_retrieval
-                        if model_args.add_instruction
-                        else None
-                    ),
-                    max_length=max(
-                        model_args.max_query_length, model_args.max_passage_length
-                    ),
-                    batch_size=model_args.batch_size,
-                )
-            )
-    return encoder, reranker_list
+        cross_encoder = DRESReranker(
+            model_args.reranker,
+            use_fp16=model_args.use_fp16,
+            query_instruction_for_reranking=(
+                model_args.query_instruction_for_reranking
+                if model_args.add_instruction_for_reranking
+                else None
+            ),
+            passage_instruction_for_reranking=(
+                model_args.passage_instruction_for_reranking
+                if model_args.add_instruction_for_reranking
+                else None
+            ),
+            max_length=model_args.max_length_for_reranking,
+            batch_size=model_args.batch_size_for_reranking,
+        )
+    return embedding_model, cross_encoder
 
 
 def main():
     parser = HfArgumentParser([ModelArgs, EvalArgs])
     model_args, eval_args = parser.parse_args_into_dataclasses()
     model_args: ModelArgs
     eval_args: EvalArgs
 
-    encoder, reranker_list = get_models(model_args)
-
+    embedding_model, cross_encoder = get_models(model_args)
+    
     evaluation = AIRBench(
         benchmark_version=eval_args.benchmark_version,
         task_types=eval_args.task_types,
         domains=eval_args.domains,
         languages=eval_args.languages,
         cache_dir=eval_args.cache_dir,
     )
-
+    
+    retriever = EmbeddingModelRetriever(
+        embedding_model, 
+        search_top_k=eval_args.search_top_k,
+        corpus_chunk_size=10000000,  # 10M chunk size when encoding the corpus to avoid multiple tqdm bars
+    )
+    
+    if cross_encoder is not None:
+        reranker = CrossEncoderReranker(
+            cross_encoder,
+            rerank_top_k=eval_args.rerank_top_k,
+        )
+    else:
+        reranker = None
+    
     evaluation.run(
-        encoder,
+        retriever,
+        reranker=reranker,
         output_dir=eval_args.output_dir,
-        search_top_k=eval_args.search_top_k,
-        reranker_list=reranker_list,
-        rerank_top_k=eval_args.rerank_top_k,
         overwrite=eval_args.overwrite,
-        corpus_chunk_size=10000000,  # 10M chunk size when encoding the corpus to avoid multiple tqdm bars
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `air_benchmark-0.0.2/scripts/zip_results.py` & `air_benchmark-0.0.3/scripts/zip_results.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """
-# Zip "Embedding Model + NoReranker" search results in <search_results>/<model_name>/NoReranker to <save_dir>/<model_name>_NoReranker.zip.
+# Zip "Retrieval Model + NoReranker" search results in <search_results>/<retriever_name>/NoReranker to <save_dir>/<retriever_name>_NoReranker.zip.
 python zip_results.py \
 --results_dir search_results \
---model_name bge-m3 \
+--retriever_name bge-m3 \
 --save_dir search_results/zipped_results
 
-# Zip "Embedding Model + Reranker" search results in <search_results>/<model_name>/<reranker_name> to <save_dir>/<model_name>_<reranker_name>.zip.
+# Zip "Retrieval Model + Reranker" search results in <search_results>/<retriever_name>/<reranker_name> to <save_dir>/<retriever_name>_<reranker_name>.zip.
 python zip_results.py \
 --results_dir search_results \
---model_name bge-m3 \
+--retriever_name bge-m3 \
 --reranker_name bge-reranker-v2-m3 \
 --save_dir search_results/zipped_results
 """
 
 import argparse
 import os
 import zipfile
 
-from AIR_Bench.tasks import check_domains, check_task_types
+from air_benchmark.tasks.tasks import check_domains, check_task_types
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--results_dir",
         type=str,
         required=True,
         help="Path to the search results directory",
     )
     parser.add_argument(
-        "--model_name", type=str, required=True, help="Model name used for the search"
+        "--retriever_name", type=str, required=True, help="Model name used for the search"
     )
     parser.add_argument(
         "--reranker_name",
         type=str,
         default="NoReranker",
         help="Reranker name used for the search. Default: NoReranker",
     )
@@ -60,27 +60,27 @@
         for domain in os.listdir(task_type_dir):
             check_domains([domain])
 
 
 def zip_results(
     results_dir: str,
     save_dir: str,
-    model_name: str,
-    reranker_name: str = "NoReanker",
+    retriever_name: str,
+    reranker_name: str = "NoReranker",
     overwrite: bool = False,
 ):
-    results_path = os.path.join(results_dir, model_name, reranker_name)
+    results_path = os.path.join(results_dir, retriever_name, reranker_name)
     try:
         check_results_path(results_path)
     except Exception as e:
         print(f"Invalid file structure in {results_path}: {e}\n")
         return False
 
     os.makedirs(save_dir, exist_ok=True)
-    zip_filename = os.path.join(save_dir, f"{model_name}_{reranker_name}.zip")
+    zip_filename = os.path.join(save_dir, f"{retriever_name}_{reranker_name}.zip")
     if os.path.exists(zip_filename) and not overwrite:
         print(f"Zipped file {zip_filename} already exists.\n")
         return False
 
     try:
         print("Zipping search results...")
         with zipfile.ZipFile(zip_filename, "w", zipfile.ZIP_DEFLATED) as zipf:
@@ -99,22 +99,22 @@
 def main():
     args = get_args()
 
     print("=========================================")
     success = zip_results(
         args.results_dir,
         args.save_dir,
-        args.model_name,
+        args.retriever_name,
         reranker_name=args.reranker_name,
         overwrite=args.overwrite,
     )
     print("=========================================")
     if success:
         print(
-            "Success! Now you can upload the zipped search results to the 🤗  Hugging Face Leaderboard!"
+            "Success! Now you can upload the zipped search results to https://huggingface.co/spaces/AIR-Bench/leaderboard !"
         )
     else:
         print("Failed! Please check the error message and try again!")
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

